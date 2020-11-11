---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/09/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 02a7cf83bbd3de7dba69a75eeff0d6676d1e0952
ms.sourcegitcommit: 133d53a85073e3ce526a3de8de668e7bca79f48e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/11/2020
ms.locfileid: "94484008"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="f6f7d-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="f6f7d-104">Aktuelle Versionshinweise</span><span class="sxs-lookup"><span data-stu-id="f6f7d-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="november-09-2020"></a><span data-ttu-id="f6f7d-105">9\. November 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-105">November 09, 2020</span></span>

<span data-ttu-id="f6f7d-106">Version 2.14.2</span><span class="sxs-lookup"><span data-stu-id="f6f7d-106">Version 2.14.2</span></span>

### <a name="app-service"></a><span data-ttu-id="f6f7d-107">App Service</span><span class="sxs-lookup"><span data-stu-id="f6f7d-107">App Service</span></span>

* <span data-ttu-id="f6f7d-108">Fehlerbehebung Nr. 15604 und 15605: Dotnet5-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-108">Fix #15604, #15605: Add Dotnet5 support</span></span>

## <a name="november-06-2020"></a><span data-ttu-id="f6f7d-109">6\. November 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-109">November 06, 2020</span></span>

<span data-ttu-id="f6f7d-110">Version 2.14.1</span><span class="sxs-lookup"><span data-stu-id="f6f7d-110">Version 2.14.1</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-111">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-111">ARM</span></span>

* <span data-ttu-id="f6f7d-112">Hotfix: Unterstützung für mehrzeilige TS-Zeichenfolgen für Vorlageneingaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-112">Hotfix: Add TS multiline string support for template inputs</span></span>

## <a name="october-27-2020"></a><span data-ttu-id="f6f7d-113">27. Oktober 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-113">October 27, 2020</span></span>

<span data-ttu-id="f6f7d-114">Version 2.14.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-114">Version 2.14.0</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-115">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-115">AKS</span></span>

* <span data-ttu-id="f6f7d-116">PPG-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-116">Add PPG support</span></span>
* <span data-ttu-id="f6f7d-117">Maximales Timeout für den Lastenausgleich auf 100 Minuten aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-117">Update max standard load balancer timeout to 100 minutes</span></span>

### <a name="apim"></a><span data-ttu-id="f6f7d-118">APIM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-118">APIM</span></span>

* <span data-ttu-id="f6f7d-119">Problem beim Erstellen der Tarifinstanz „Consumption“ behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-119">Fix issue with creating consumption tier instance</span></span>

### <a name="app-config"></a><span data-ttu-id="f6f7d-120">App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="f6f7d-120">App Config</span></span>

* <span data-ttu-id="f6f7d-121">Abfrage von Schlüsselwerten anhand von kommagetrennten Bezeichnungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-121">Fix querying key-values by comma separated labels</span></span>

### <a name="app-service"></a><span data-ttu-id="f6f7d-122">App Service</span><span class="sxs-lookup"><span data-stu-id="f6f7d-122">App Service</span></span>

* <span data-ttu-id="f6f7d-123">Fehlerbehebung: Fehler bei „az webapp up“, wenn der Benutzer nicht über Schreibberechtigungen für das übergeordnete Verzeichnis des Projekts verfügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-123">Bugfix: az webapp up fails when user doesn't have write permissions to project's parent directory</span></span>
* <span data-ttu-id="f6f7d-124">Fehlerbehebung Nr. 13777: Fehlerbehebung zum Entfernen von Escapezeichen aus XML</span><span class="sxs-lookup"><span data-stu-id="f6f7d-124">Fix #13777: Fix to remove escape chars from XML</span></span>
* <span data-ttu-id="f6f7d-125">Fehlerbehebung Nr. 15441: Fehler „AttributeError“ bei „az webapp create-remote-connection“: Das Objekt „Thread“ besitzt kein Attribut vom Typ „isAlive“.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-125">Fix #15441: az webapp create-remote-connection fails with AttributeError: 'Thread' object has no attribute 'isAlive'</span></span>
* <span data-ttu-id="f6f7d-126">[BREAKING CHANGE] az webapp up: Optionale Parameter hinzugefügt (Betriebssystem und Runtime) und Runtimes aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-126">[BREAKING CHANGE] az webapp up: add optional params (os & runtime) and updated runtimes</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-127">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-127">ARM</span></span>

* <span data-ttu-id="f6f7d-128">Was-wäre-wenn-Befehle für Vorlagenbereitstellung nun allgemein verfügbar</span><span class="sxs-lookup"><span data-stu-id="f6f7d-128">Make template deployment What-If commands GA</span></span>
* <span data-ttu-id="f6f7d-129">[BREAKING CHANGE] Benutzerbestätigung für „az ts create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-129">[BREAKING CHANGE] Add user confirmation for az ts create</span></span>
* <span data-ttu-id="f6f7d-130">Zurückgegebene Daten beim Markieren mehrerer Ressourcen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-130">Fix the returned data when tagging multiple resources</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-131">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-131">Backup</span></span>

* <span data-ttu-id="f6f7d-132">`az backup policy create`: Unterstützung für die Erstellung von IaaSVM-Sicherungsrichtlinien über die CLI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-132">`az backup policy create`: Add support for IaaSVM backup policy creation from CLI</span></span>
* <span data-ttu-id="f6f7d-133">Grenzwert für den VM-Schutz von 100 auf 1.000 erhöht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-133">Increasing VM protection limit from 100 to 1000</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-134">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-134">Compute</span></span>

* <span data-ttu-id="f6f7d-135">sig image-definition create: „--features“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-135">sig image-definition create: add --features</span></span>
* <span data-ttu-id="f6f7d-136">Neue API-Version von gallery_images 2020-09-30</span><span class="sxs-lookup"><span data-stu-id="f6f7d-136">New API version of gallery_images 2020-09-30</span></span>
* <span data-ttu-id="f6f7d-137">`az vm update / az sig image-version update`: Unterstützung der Aktualisierung der VM-/Imageversion (auch bei Verwendung eines mandantenübergreifenden Images)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-137">`az vm update / az sig image-version update`: Support update vm/image-version even it uses a cross tenant image</span></span>
* <span data-ttu-id="f6f7d-138">Überprüfung von VM-Host-SKUs entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-138">Remove validation of vm host SKUs</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f6f7d-139">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-139">Cosmos DB</span></span>

* <span data-ttu-id="f6f7d-140">`az cosmosdb create/update`: Fehlermeldung für falsche Eingabe für „--locations“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-140">`az cosmosdb create/update`: Improve error message from incorrect --locations input</span></span>
* <span data-ttu-id="f6f7d-141">`az cosmosdb sql container create/update`: Parameter „--analytical-storage-ttl“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-141">`az cosmosdb sql container create/update`: Add --analytical-storage-ttl parameter</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-142">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-142">HDInsight</span></span>

* <span data-ttu-id="f6f7d-143">[BREAKING CHANGE] az hdinsight create: Zwei Parameter entfernt: --public-network-access-type und --outbound-public-network-access-type</span><span class="sxs-lookup"><span data-stu-id="f6f7d-143">[BREAKING CHANGE] az hdinsight create: remove two parameters: --public-network-access-type and  --outbound-public-network-access-type</span></span>

### <a name="iot-central"></a><span data-ttu-id="f6f7d-144">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f6f7d-144">IoT Central</span></span>

* <span data-ttu-id="f6f7d-145">Vorschauwarnung entfernt, da die Version bereits allgemein verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-145">Remove preview warning since it is already GAed</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6f7d-146">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-146">Key Vault</span></span>

* <span data-ttu-id="f6f7d-147">`--enable-soft-delete false` beim Erstellen oder Aktualisieren von Tresoren als ungültig erklärt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-147">Invalidate `--enable-soft-delete false` while creating or updating vaults</span></span>
* <span data-ttu-id="f6f7d-148">`--bypass` und `--default-action` funktionieren nun gemeinsam mit Netzwerk-ACL-Parametern bei der Erstellung von Tresoren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-148">Make `--bypass` and `--default-action` work together with network acl parameters while creating vaults</span></span>

### <a name="misc"></a><span data-ttu-id="f6f7d-149">Verschiedenes:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-149">Misc.</span></span>

* <span data-ttu-id="f6f7d-150">„bash-completion“ zu Dockerfile hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-150">Add bash-completion to Dockerfile</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-151">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-151">RDBMS</span></span>

* <span data-ttu-id="f6f7d-152">Befehl „List-SKUS“, Tabellentransformer, lokaler Kontext für Postgres, MySQL, MariaDB (Einzelserver) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-152">Add List-SKUS Command, Table Transformers, Local Context for Postgres, MySQL, Mariadb Single Server</span></span>
* <span data-ttu-id="f6f7d-153">[BREAKING CHANGE] Aktualisierungen von Parameternamen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-153">[BREAKING CHANGE] Parameter name updates.</span></span> <span data-ttu-id="f6f7d-154">Verbesserungen der Verwaltungsebene für MySQL und PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-154">Improvements to Management Plane for MySQL and PostgreSQL</span></span>
* <span data-ttu-id="f6f7d-155">`az postgres|mariadb|mysql server create`: Erstellungsumgebung für Postgres, MySQL und MariaDB aktualisiert: Neue Felder in der Ausgabe, neue Werte für Parameter `--public` im create-Befehl eingeführt (all,<IP>,<IPRange>,0.0.0.0)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-155">`az postgres|mariadb|mysql server create` : Update create experience for Postgres, MySQL and MariaDB - new fields in the output , Introduce new values for `--public` parameter in create command (all,<IP>,<IPRange>,0.0.0.0)</span></span>

### <a name="signalr"></a><span data-ttu-id="f6f7d-156">SignalR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-156">SignalR</span></span>

* <span data-ttu-id="f6f7d-157">`az signalr create`: Neue Option `--enable-messaging-logs` hinzugefügt, um zu steuern, ob der Dienst Messagingprotokolle generiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-157">`az signalr create`: Add new option `--enable-messaging-logs` for controling service generate messaging logs or not</span></span>
* <span data-ttu-id="f6f7d-158">`az signalr update`: Neue Option `--enable-messaging-logs` hinzugefügt, um zu steuern, ob der Dienst Messagingprotokolle generiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-158">`az signalr update`: Add new option `--enable-messaging-logs` for controling service generate messaging logs or not</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-159">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-159">SQL</span></span>

* <span data-ttu-id="f6f7d-160">[BREAKING CHANGE] Antwort für den Parameternamen der Sicherungsspeicherredundanz und Wert für MI korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-160">[BREAKING CHANGE] Fix response for backup storage redundancy param name and value for MI</span></span>
* <span data-ttu-id="f6f7d-161">`az sql db audit-policy show`: Erweitert, um die Überwachungsrichtlinie der Datenbank (einschließlich LA- und EH-Daten) anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-161">`az sql db audit-policy show`: extend to show database's audit policy including LA and EH data</span></span>
* <span data-ttu-id="f6f7d-162">`az sql db audit-policy update`: Erweitert, um das LA- und EH-Update zusammen mit der Überwachungsrichtlinie der Datenbank zuzulassen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-162">`az sql db audit-policy update`: extend to allow LA and EH update along with database's audit policy</span></span>
* <span data-ttu-id="f6f7d-163">`az sql db audit-policy wait`: CLI im Wartezustand platziert, bis eine Bedingung der Überwachungsrichtlinie der Datenbank erfüllt ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-163">`az sql db audit-policy wait`: place the CLI in a waiting state until a condition of the database's audit policy is met.</span></span>
* <span data-ttu-id="f6f7d-164">`az sql server audit-policy show`: Erweitert, um die Überwachungsrichtlinie des Servers (einschließlich LA- und EH-Daten) anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-164">`az sql server audit-policy show`: extend to show servers's audit policy including LA and EH data</span></span>
* <span data-ttu-id="f6f7d-165">`az sql server audit-policy update`: Erweitert, um das LA- und EH-Update zusammen mit der Überwachungsrichtlinie des Servers zuzulassen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-165">`az sql server audit-policy update`: extend to allow LA and EH update along with server's audit policy</span></span>
* <span data-ttu-id="f6f7d-166">`az sql server audit-policy wait`: CLI im Wartezustand platziert, bis eine Bedingung der Überwachungsrichtlinie des Servers erfüllt ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-166">`az sql server audit-policy wait`: place the CLI in a waiting state until a condition of the server's audit policy is met.</span></span>
* <span data-ttu-id="f6f7d-167">Reine AAD-Unterstützung für SQL Managed Instance und Server hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-167">Add AAD-only Support for SQL Managed Instances and Servers</span></span>
* <span data-ttu-id="f6f7d-168">`az sql db replica create`: Argument „--partner-database“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-168">`az sql db replica create`: Add --partner-database argument</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-169">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-169">Storage</span></span>

* <span data-ttu-id="f6f7d-170">Fehlerbehebung Nr. 15111: Fehler bei `az storage logging update` ohne optionales Argument</span><span class="sxs-lookup"><span data-stu-id="f6f7d-170">Fix #15111: `az storage logging update` fails without optional argument</span></span>
* <span data-ttu-id="f6f7d-171">Problem behoben, das auftrat, wenn der Befehl „set-tier“ mit Dienstprinzipalanmeldung verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-171">Fix bug when using set-tier command with service principal login</span></span>
* <span data-ttu-id="f6f7d-172">Version für Data Lake für Dateien auf 2020-02-10 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-172">Upgrade version for file datalake to 2020-02-10</span></span>
* <span data-ttu-id="f6f7d-173">`az storage queue list`: Unterstützung für Track2</span><span class="sxs-lookup"><span data-stu-id="f6f7d-173">`az storage queue list`: Track2 supported</span></span>
* <span data-ttu-id="f6f7d-174">`az storage fs access`: Unterstützung der rekursiven Verwaltung von ACLs</span><span class="sxs-lookup"><span data-stu-id="f6f7d-174">`az storage fs access`: Support managing ACLs recursively</span></span>

### <a name="synapse"></a><span data-ttu-id="f6f7d-175">Synapse</span><span class="sxs-lookup"><span data-stu-id="f6f7d-175">Synapse</span></span>

* <span data-ttu-id="f6f7d-176">Cmdlets für Pipeline, verknüpften Dienst, Trigger, Notebook, Datenfluss und Dataset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-176">Add pipeline, linked service, trigger, notebook, data flow and dataset related cmdlets</span></span>

## <a name="october-13-2020"></a><span data-ttu-id="f6f7d-177">13. Oktober 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-177">October 13, 2020</span></span>

<span data-ttu-id="f6f7d-178">Version 2.13.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-178">Version 2.13.0</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-179">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-179">ACR</span></span>

* <span data-ttu-id="f6f7d-180">`az acr helm`: URL zur eingestellten Unterstützung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-180">`az acr helm`: Update deprecation url</span></span>
* <span data-ttu-id="f6f7d-181">logtemplate- und systemtask-Änderungen für ACR Tasks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-181">Add logtemplate and systemtask changes for ACR Tasks</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-182">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-182">AKS</span></span>

* <span data-ttu-id="f6f7d-183">Unterstützung von „virtual-node“ bei „aks create“: `az aks create --enable-addons virtual-node`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-183">Support virtual-node with aks create: `az aks create --enable-addons virtual-node`</span></span>
* <span data-ttu-id="f6f7d-184">Option nur für Knotenimages für CLI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-184">Add node image only option for CLI</span></span>
* <span data-ttu-id="f6f7d-185">Es wird erwartet, dass das Add-On „kube-dashboard“ standardmäßig deaktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-185">Expect kube-dashboard addon be disabled by default</span></span>
* <span data-ttu-id="f6f7d-186">`az aks create/update`: LicenseType-Unterstützung für Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-186">`az aks create/update`: Add LicenseType support for Windows</span></span>
* <span data-ttu-id="f6f7d-187">Unterstützung für das Hinzufügen eines Spot-Knotenpools</span><span class="sxs-lookup"><span data-stu-id="f6f7d-187">Support add Spot node pool</span></span>
* <span data-ttu-id="f6f7d-188">Beachten der in der Azure CLI definierten Add-On-Namen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-188">Honor addon names defined in Azure CLI</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-189">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-189">AMS</span></span>

* <span data-ttu-id="f6f7d-190">Fehlerbehebung Nr. 14687: Gemischte Ressourcengruppen- und Kontonamen im Befehl „az ams streaming-endpoint show“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-190">Fix #14687: Mixed resource group and account name in command "az ams streaming-endpoint show"</span></span>

### <a name="app-config"></a><span data-ttu-id="f6f7d-191">App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="f6f7d-191">App Config</span></span>

* <span data-ttu-id="f6f7d-192">Testfehler behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-192">Fix test bug</span></span>
* <span data-ttu-id="f6f7d-193">Unterstützung der AAD-Authentifizierung für Datenvorgänge</span><span class="sxs-lookup"><span data-stu-id="f6f7d-193">Support AAD auth for data operations</span></span>

### <a name="app-service"></a><span data-ttu-id="f6f7d-194">App Service</span><span class="sxs-lookup"><span data-stu-id="f6f7d-194">App Service</span></span>

* <span data-ttu-id="f6f7d-195">`az functionapp deployment source config-zip`: Es wurde ein Problem behoben, das dazu führte, dass „config-zip“ bei Erfolg unter Linux ggf. eine Ausnahme auslöste.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-195">`az functionapp deployment source config-zip`: Fixed an issue where config-zip could throw an exception on success on linux consumption</span></span>
* <span data-ttu-id="f6f7d-196">Fehlerbehebung: Bessere Fehlermeldungen für Befehle vom Typ „webapp“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-196">Bugfix: Better error messages for webapp commands</span></span>
* <span data-ttu-id="f6f7d-197">`az appservice domain create, show-terms`: Option zum Erstellen einer App Service-Domäne hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-197">`az appservice domain create, show-terms`: Add ability to create app service domain</span></span>
* <span data-ttu-id="f6f7d-198">`az functionapp create`: Vorschauflag aus Java 11 beim Erstellen einer neuen Funktions-App entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-198">`az functionapp create`: Removed the preview flag from Java 11 when creating a new function app</span></span>
* <span data-ttu-id="f6f7d-199">[BREAKING CHANGE:] az webapp create, az webapp up – verfügbare webapp-Runtimes aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-199">[BREAKING CHANGE] az webapp create, az webapp up - Update available webapp runtimes</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-200">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-200">ARM</span></span>

* <span data-ttu-id="f6f7d-201">`az ts`: Neue Befehle für Vorlagenspezifikationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-201">`az ts`: Add new commands for template specs</span></span>
* <span data-ttu-id="f6f7d-202">`az deployment` : Unterstützung für „--template-spec -s“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-202">`az deployment` : Add support for --template-spec -s</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-203">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-203">Compute</span></span>

* <span data-ttu-id="f6f7d-204">Beschränkung der FD-Anzahl bei der Hostgruppenerstellung korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-204">Fix host group creation FD count limitation</span></span>
* <span data-ttu-id="f6f7d-205">Neuer Befehl hinzugefügt, um das Upgrade von Erweiterungen für VMSS zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-205">Add new command to support upgrading extensions for VMSS</span></span>
* <span data-ttu-id="f6f7d-206">Problem des fehlenden Imageverweises behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-206">Fix the image reference is missing issue</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-207">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-207">HDInsight</span></span>

* <span data-ttu-id="f6f7d-208">`az hdinsight create`: Informationen zur Einstellung für Argument „--public-networrk-access-type“ und „--outbound-public-network-access-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-208">`az hdinsight create`: add deprecate information for argument --public-networrk-access-type and --outbound-public-network-access-type</span></span>
* <span data-ttu-id="f6f7d-209">`az hdinsight create`: Informationen zur Einstellung für Argument `--public-networrk-access-type` und `--outbound-public-network-access-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-209">`az hdinsight create`: add deprecate information for argument `--public-networrk-access-type` and `--outbound-public-network-access-type`</span></span>
* <span data-ttu-id="f6f7d-210">`az hdinsight create`: Parameter `--idbroker` hinzugefügt, um die Erstellung von ESP-Clustern mit HDInsight-Identitätsbroker für Kunden zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-210">`az hdinsight create`:  add parameter `--idbroker` to support customer to create ESP cluster with HDInsight Id Broker</span></span>

### <a name="iot-central"></a><span data-ttu-id="f6f7d-211">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f6f7d-211">IoT Central</span></span>

* <span data-ttu-id="f6f7d-212">Veraltetes Befehlsmodul „az iotcentral“ entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-212">Remove deprecated 'az iotcentral' command module</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6f7d-213">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-213">Key Vault</span></span>

* <span data-ttu-id="f6f7d-214">Unterstützung von `--hsm-name` für `az keyvault key encrypt/decrypt`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-214">Support `--hsm-name` for `az keyvault key encrypt/decrypt`</span></span>

### <a name="lab"></a><span data-ttu-id="f6f7d-215">Labor</span><span class="sxs-lookup"><span data-stu-id="f6f7d-215">Lab</span></span>

* <span data-ttu-id="f6f7d-216">Fehlerbehebung Nr. 14127: `__init__()` akzeptiert ein positionelles Argument, angegeben wurden jedoch zwei.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-216">Fix #14127: `__init__()` takes 1 positional argument but 2 were given</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-217">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-217">Network</span></span>

* <span data-ttu-id="f6f7d-218">`az network application-gateway ssl-cert show`: Beispiel zur Veranschaulichung des Zertifikatformats und der Abrufinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-218">`az network application-gateway ssl-cert show`: Add example to demonstrate certificate format and fetch information</span></span>
* <span data-ttu-id="f6f7d-219">`az network application-gateway rule`: Unterstützung für die Option „--priority“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-219">`az network application-gateway rule`: Support --priority option</span></span>
* <span data-ttu-id="f6f7d-220">`az network application-gateway create`: Fehler behoben, dass die Erstellung ohne Angabe der öffentlichen IP-Adresse nicht möglich ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-220">`az network application-gateway create`: Fix bug that cannot create without public IP sepcified</span></span>
* <span data-ttu-id="f6f7d-221">`az network application-gateway waf-policy managed-rule rule-set add`: Verfügbarmachen des Serverfehlers für den Benutzer, um eine intuitivere Hinweismeldung zu ermöglich</span><span class="sxs-lookup"><span data-stu-id="f6f7d-221">`az network application-gateway waf-policy managed-rule rule-set add`: Expose server error to user to give more intuitive hint message.</span></span>
* <span data-ttu-id="f6f7d-222">`az network application-gateway waf-policy managed-rule rule-set update`: Unterstützung zur Änderung der Typversion des Regelsatzes</span><span class="sxs-lookup"><span data-stu-id="f6f7d-222">`az network application-gateway waf-policy managed-rule rule-set update`: Support to change rule set type version.</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-223">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-223">RDBMS</span></span>

* <span data-ttu-id="f6f7d-224">Fehlerbehebung: az postgres flexible-server create – hartcodierte API-Version aus Netzwerkclient entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-224">Bugfix: az postgres flexible-server create Remove hardcoded API version from network client.</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-225">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-225">Role</span></span>

* <span data-ttu-id="f6f7d-226">Fehlerbehebung Nr. 15278: `az role assignment list/delete`: Leere Zeichenfolgenargumente verboten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-226">Fix #15278: `az role assignment list/delete`: Forbid empty string arguments</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-227">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-227">SQL</span></span>

* <span data-ttu-id="f6f7d-228">`az sql midb log-replay`: Unterstützung für den Protokollwiedergabedienst in der verwalteten Datenbank</span><span class="sxs-lookup"><span data-stu-id="f6f7d-228">`az sql midb log-replay`: Support for log replay service on managed database</span></span>
* <span data-ttu-id="f6f7d-229">Ignorieren der Groß-/Kleinschreibung im Parameterwert für die Sicherungsspeicherredundanz für verwaltete Instanzen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-229">Ignore character casing for backup storage redundancy param value for managed instance</span></span>
* <span data-ttu-id="f6f7d-230">[BREAKING CHANGE:] az sql db create: Parameter „--backup-storage-redundancy“ hinzugefügt. Warnung, wenn folgende Angabe fehlt: bsr/bsr == Geo</span><span class="sxs-lookup"><span data-stu-id="f6f7d-230">[BREAKING CHANGE] az sql db create: Add --backup-storage-redundancy parameter; add warning for unspecified bsr/bsr == Geo.</span></span>

### <a name="sql-vm"></a><span data-ttu-id="f6f7d-231">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-231">SQL VM</span></span>

* <span data-ttu-id="f6f7d-232">`az sql vm show`: Konfigurationsoptionen für das Flag „--expand“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-232">`az sql vm show`: Add configuration options to --expand flag</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-233">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-233">Storage</span></span>

* <span data-ttu-id="f6f7d-234">[BREAKING CHANGE] `az storage blob copy start`: Formatproblem für `--destination-if-modified-since` und `--destination-if-unmodified-since` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-234">[BREAKING CHANGE] `az storage blob copy start`: Fix format issue for `--destination-if-modified-since` and `--destination-if-unmodified-since`</span></span>
* <span data-ttu-id="f6f7d-235">[BREAKING CHANGE] `az storage blob incremental-copy start`: Formatproblem für `--destination-if-modified-since` und `--destination-if-unmodified-since` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-235">[BREAKING CHANGE] `az storage blob incremental-copy start`: Fix format issue for `--destination-if-modified-since` and `--destination-if-unmodified-since`</span></span>
* <span data-ttu-id="f6f7d-236">`az storage fs`: Problem mit Verbindungszeichenfolge behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-236">`az storage fs`: Fix connection string issue</span></span>
* <span data-ttu-id="f6f7d-237">`az storage share-rm`: Zugriffsebene der GA-Version</span><span class="sxs-lookup"><span data-stu-id="f6f7d-237">`az storage share-rm`: GA release access tier</span></span>
* <span data-ttu-id="f6f7d-238">`az storage container-rm`: Neue Befehlsgruppe hinzugefügt, um den Ressourcenanbieter „Microsoft.Storage“ für Verwaltungsvorgänge für Container zu verwenden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-238">`az storage container-rm`: Add a new command group to use the Microsoft.Storage resource provider for container management operations.</span></span>

## <a name="september-29-2020"></a><span data-ttu-id="f6f7d-239">29. September 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-239">September 29, 2020</span></span>

<span data-ttu-id="f6f7d-240">Version 2.12.1</span><span class="sxs-lookup"><span data-stu-id="f6f7d-240">Version 2.12.1</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-241">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-241">RDBMS</span></span>

* <span data-ttu-id="f6f7d-242">Hotfix: `az postgres flexible-server create`: VnetName zum Ausschließen des Servernamens aktualisiert und Standardregion für MySQL aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-242">Hotfix: `az postgres flexible-server create` : Update VnetName to exclude servername and update default region for MySQL</span></span>

## <a name="september-22-2020"></a><span data-ttu-id="f6f7d-243">22. September 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-243">September 22, 2020</span></span>

<span data-ttu-id="f6f7d-244">Version 2.12.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-244">Version 2.12.0</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-245">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-245">ACR</span></span>

* <span data-ttu-id="f6f7d-246">Fehlerbehebung Nr. 14811: Hinzufügen von Unterstützung für die Außerkraftsetzung von „dockerignore“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-246">Fix #14811 Add support for dockerignore override</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-247">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-247">AKS</span></span>

* <span data-ttu-id="f6f7d-248">Die CLI sollte eine leere kubeconfig-Datei tolerieren.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-248">CLI should tolerate empty kubeconfig</span></span>
* <span data-ttu-id="f6f7d-249">Fehlerbehebung Nr. 12871: az aks enable-addons: Das automatisch generierte Hilfebeispiel ist für die Option „virtual-node“ falsch.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-249">FIX #12871: az aks enable-addons: Autogenerated help example is wrong for vitual-node option</span></span>
* <span data-ttu-id="f6f7d-250">Legacyaktionen für ACI-Connectors entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-250">Remove legacy aci connector actions</span></span>
* <span data-ttu-id="f6f7d-251">Unterstützung für Richtlinien-Add-On in der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-251">Support azure policy addon in azure-cli</span></span>
* <span data-ttu-id="f6f7d-252">Problem mit Groß-/Kleinbuchstaben für AKS-Dashboard-Add-On behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-252">Fix case sensitive issue for AKS dashboard addon</span></span>
* <span data-ttu-id="f6f7d-253">„mgmt-containerservice“ auf 9.4.0 aktualisiert und 09-01-API aktiviert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-253">Update mgmt-containerservice to 9.4.0 and enable 09-01 API</span></span>

### <a name="apim"></a><span data-ttu-id="f6f7d-254">APIM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-254">APIM</span></span>

* <span data-ttu-id="f6f7d-255">Unterstützung der Befehle für die Entitäten „product“/„productapi“/„namedValue“ und SDK-Version aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-255">Support product / productapi / namedValue entity commands && bump sdk version</span></span>

### <a name="app-config"></a><span data-ttu-id="f6f7d-256">App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="f6f7d-256">App Config</span></span>

* <span data-ttu-id="f6f7d-257">Unterstützung für die Aktivierung/Deaktivierung von PublicNetworkAccess für vorhandene Speicher</span><span class="sxs-lookup"><span data-stu-id="f6f7d-257">Support enabling/disabling PublicNetworkAccess for existing stores</span></span>

### <a name="app-service"></a><span data-ttu-id="f6f7d-258">App Service</span><span class="sxs-lookup"><span data-stu-id="f6f7d-258">App Service</span></span>

* <span data-ttu-id="f6f7d-259">Unterstützung für den Tarif „Premium V3“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-259">Add support for Premium V3 pricing tier</span></span>
* <span data-ttu-id="f6f7d-260">Fehlerbehebung Nr. 12653: az webapp log config --application-logging: keine Deaktivierung, wenn „false“ festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-260">Fix #12653: az webapp log config --application-logging false doesn't turn it off</span></span>
* <span data-ttu-id="f6f7d-261">Fehlerbehebung Nr. 14684: Entfernen von „access-restriction“ nach IP-Adresse funktioniert nicht. Fehlerbehebung Nr. 13837: -az webapp create – Beispiel für verschiedene RSgroups für Plan und WebApp</span><span class="sxs-lookup"><span data-stu-id="f6f7d-261">Fix #14684: access-restriction remove by ip address does not work; #13837-az webapp create - Example for different RSgroups for Plan and WebApp</span></span>
* <span data-ttu-id="f6f7d-262">functionapp: Unterstützung für benutzerdefinierte Handler hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-262">functionapp: Add support for custom handlers.</span></span> <span data-ttu-id="f6f7d-263">Powershell 6.2 wurde als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-263">Deprecated Powershell 6.2.</span></span>
* <span data-ttu-id="f6f7d-264">functionapp: Problem behoben, das dazu führte, dass die App-Einstellung für benutzerdefinierte Linux-Images falsch festgelegt wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-264">functionapp: Fix issue where app setting was being incorrectly set for linux custom images</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-265">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-265">ARM</span></span>

* <span data-ttu-id="f6f7d-266">`az deployment group/sub/mg/tenant what-if`: Ignorierte Ressourcenänderungen als letztes anzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-266">`az deployment group/sub/mg/tenant what-if`: Show "Ignore" resource changes last</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-267">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-267">Compute</span></span>

* <span data-ttu-id="f6f7d-268">Neuer Lizenztyp bei VM-Erstellung/-Aktualisierung hinzugefügt: RHEL_BYOS, SLES_BYOS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-268">Add new license_type in vm create/update: RHEL_BYOS, SLES_BYOS</span></span>
* <span data-ttu-id="f6f7d-269">Upgrade der Datenträger-API-Version auf 2020-06-30 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-269">Upgrade disk API version to 2020-06-30</span></span>
* <span data-ttu-id="f6f7d-270">Datenträgererstellung: „--logical-sector-size“ und „--tier“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-270">disk create: add --logical-sector-size, --tier</span></span>
* <span data-ttu-id="f6f7d-271">Datenträgeraktualisierung: Unterstützung für „--disk-iops-read-only“, „--disk-mbps-read-only“, „--max-shares“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-271">disk update: Support --disk-iops-read-only, --disk-mbps-read-only, --max-shares</span></span>
* <span data-ttu-id="f6f7d-272">Neuer Befehl: disk-encryption-set list-associated-resources</span><span class="sxs-lookup"><span data-stu-id="f6f7d-272">New command disk-encryption-set list-associated-resources</span></span>
* <span data-ttu-id="f6f7d-273">vm boot-diagnostics enable: „--storage“ wird optional.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-273">vm boot-diagnostics enable: --storage becomes optional</span></span>
* <span data-ttu-id="f6f7d-274">Neuer Befehl: vm boot-diagnostics get-boot-log-uris</span><span class="sxs-lookup"><span data-stu-id="f6f7d-274">New command: vm boot-diagnostics get-boot-log-uris</span></span>
* <span data-ttu-id="f6f7d-275">vm boot-diagnostics get-boot-log: Unterstützung für verwalteten Speicher</span><span class="sxs-lookup"><span data-stu-id="f6f7d-275">vm boot-diagnostics get-boot-log: support managed storage</span></span>

### <a name="config"></a><span data-ttu-id="f6f7d-276">Konfigurationen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-276">Config</span></span>

* <span data-ttu-id="f6f7d-277">„local-context“ in „config param-persist“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-277">Rename local-context to config param-persist</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f6f7d-278">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-278">Cosmos DB</span></span>

* <span data-ttu-id="f6f7d-279">Unterstützung für Migrations-APIs für Durchsatzressource für das Autoskalierungsfeature in CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-279">Support for Migration APIs for Throughput resource for Autoscale feature in CosmosDB</span></span>

### <a name="eventhub"></a><span data-ttu-id="f6f7d-280">Eventhub</span><span class="sxs-lookup"><span data-stu-id="f6f7d-280">Eventhub</span></span>

<span data-ttu-id="f6f7d-281">Clusterbefehle und Parameter „trusted_service_access_enabled“ für Networkruleset hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-281">Added Cluster commands and trusted_service_access_enabled parameter for Networkruleset</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-282">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-282">Extension</span></span>

* <span data-ttu-id="f6f7d-283">`az extension add`: Option `--upgrade` hinzugefügt, um die Erweiterung zu aktualisieren, sofern sie bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-283">`az extension add`: Add `--upgrade` option to update the extension if already installed</span></span>
* <span data-ttu-id="f6f7d-284">Dynamische Installation standardmäßig aktivieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-284">Turn on dynamic install by default</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-285">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-285">IoT</span></span>

* <span data-ttu-id="f6f7d-286">Minimale TLS-Version bei IoT Hub-Erstellung zulässig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-286">Enabled minimum TLS version on IoT Hub Create</span></span>

### <a name="iot-central"></a><span data-ttu-id="f6f7d-287">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f6f7d-287">IoT Central</span></span>

* <span data-ttu-id="f6f7d-288">Der Vorgang zum Löschen der App ist jetzt ein zeitintensiver Vorgang.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-288">App delete operation is now long running operation</span></span>

### <a name="iot-hub"></a><span data-ttu-id="f6f7d-289">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="f6f7d-289">Iot Hub</span></span>

* <span data-ttu-id="f6f7d-290">Befehl „show-connection-string“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-290">Deprecated 'show-connection-string' command</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6f7d-291">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-291">Key Vault</span></span>

* <span data-ttu-id="f6f7d-292">Public Preview von verwaltetem HSM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-292">Managed HSM public preview</span></span>
* <span data-ttu-id="f6f7d-293">Problem behoben, dass `--maxresults` beim Auflisten von Ressourcen oder Ressourcenversionen nicht wirksam wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-293">Fix the issue that `--maxresults` does not take effect while listing resources or resource versions</span></span>

### <a name="kusto"></a><span data-ttu-id="f6f7d-294">Kusto</span><span class="sxs-lookup"><span data-stu-id="f6f7d-294">Kusto</span></span>

* <span data-ttu-id="f6f7d-295">Nachricht zur Einstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-295">Add deprecating message</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-296">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-296">Monitor</span></span>

* <span data-ttu-id="f6f7d-297">`az monitor log-analytics workspace linked-storage`: detaillierte Fehlermeldung für Kunden verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-297">`az monitor log-analytics workspace linked-storage`: expose detailed error message to customers</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-298">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-298">Network</span></span>

* <span data-ttu-id="f6f7d-299">`az network vnet subnet`: Unterstützung für „--disable-private-endpoint-network-policies“ und „--disable-private-link-service-network-policies“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-299">`az network vnet subnet`: Support --disable-private-endpoint-network-policies and --disable-private-link-service-network-policies</span></span>
* <span data-ttu-id="f6f7d-300">Problem behoben, das beim Aktualisieren von „flow-log“ auftrat, wenn die untergeordnete Eigenschaft „network_watcher_flow_analytics_configuration“ auf „None“ festgelegt war</span><span class="sxs-lookup"><span data-stu-id="f6f7d-300">Fix bug while updateing flow-log when its subproperty network_watcher_flow_analytics_configuration is None</span></span>
* <span data-ttu-id="f6f7d-301">Aktualisierung der API-Version auf 2020-06-01</span><span class="sxs-lookup"><span data-stu-id="f6f7d-301">API version bump to 2020-06-01</span></span>
* <span data-ttu-id="f6f7d-302">Unterstützung für „--tcp-port-behavior“ beim Konfigurieren einer TCP-Konfiguration von Verbindungsmonitor V2</span><span class="sxs-lookup"><span data-stu-id="f6f7d-302">Support --tcp-port-behavior while configuring a TCP configuration of a Connection Monitor V2</span></span>
* <span data-ttu-id="f6f7d-303">Unterstützung für mehr Typen und Abdeckungsebenen beim Erstellen eines Endpunkts von Verbindungsmonitor V2</span><span class="sxs-lookup"><span data-stu-id="f6f7d-303">Support more types and coverage level while creating Endpoint of Connection Monitor V2</span></span>
* <span data-ttu-id="f6f7d-304">Unterstützung für „--host-subnet“, um VirtualHub unter VirtualRouter zu erstellen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-304">Support --host-subnet to create VirtualHub underneath as VirtualRouter</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-305">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-305">RDBMS</span></span>

* <span data-ttu-id="f6f7d-306">Aktualisierungen der Verwaltungsebene für PostgreSQL und MySQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-306">Management Plane updates for PostgreSQL and MySQL</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-307">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-307">Role</span></span>

* <span data-ttu-id="f6f7d-308">`az role assignment create/update`: Unterstützung für `--description`, `--condition` und `--condition-version`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-308">`az role assignment create/update`: Support `--description`, `--condition` and `--condition-version`</span></span>
* <span data-ttu-id="f6f7d-309">`az ad app permission delete`: Unterstützung für `--api-permissions` zum Löschen spezifischer `ResourceAccess`-Elemente</span><span class="sxs-lookup"><span data-stu-id="f6f7d-309">`az ad app permission delete`: Support `--api-permissions` to delete specific `ResourceAccess`</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f6f7d-310">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6f7d-310">Service Fabric</span></span>

* <span data-ttu-id="f6f7d-311">Befehle für verwaltete Cluster und Knotentypen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-311">Add managed cluster and node type commands</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-312">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-312">SQL</span></span>

* <span data-ttu-id="f6f7d-313">„azure-mgmt-sql“ auf 0.20.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-313">Upgrade azure-mgmt-sql to 0.20.0</span></span>
* <span data-ttu-id="f6f7d-314">Optionaler Parameter für Redundanz des Sicherungsspeichers zum Cmdlet „mi create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-314">Add backup storage redundancy optional parameter to MI create cmdlet</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-315">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-315">Storage</span></span>

* <span data-ttu-id="f6f7d-316">`az storage share-rm stats`: Abrufen der Nutzung (in Bytes) der auf der Freigabe gespeicherten Daten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-316">`az storage share-rm stats`: Get the usage bytes of the data stored on the share.</span></span>
* <span data-ttu-id="f6f7d-317">Allgemein verfügbares Release für Zeitpunktwiederherstellung von Speicherblobs</span><span class="sxs-lookup"><span data-stu-id="f6f7d-317">GA release storage blob PITR</span></span>
* <span data-ttu-id="f6f7d-318">`az storage blob query`: Unterstützung für Azure Storage-Abfragebeschleunigung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-318">`az storage blob query`: Support Azure Storage Query Acceleration</span></span>
* <span data-ttu-id="f6f7d-319">Unterstützung des vorläufigen Löschens für Dateifreigaben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-319">Support Soft Delete for file share</span></span>
* <span data-ttu-id="f6f7d-320">`az storage copy`: Unterstützung für Kontoanmeldeinformationen hinzugefügt und `--source-local-path`, `--destination-local-path` und `--destination-account-name` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-320">`az storage copy`: Add account credentials support and deprecate `--source-local-path`, `--destination-local-path`, `--destination-account-name`</span></span>
* <span data-ttu-id="f6f7d-321">`az storage account blob-service-properties update`: Unterstützung der Aufbewahrungsrichtlinie für Containerlöschungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-321">`az storage account blob-service-properties update`: Add container delete retention policy support</span></span>

### <a name="synapse"></a><span data-ttu-id="f6f7d-322">Synapse</span><span class="sxs-lookup"><span data-stu-id="f6f7d-322">Synapse</span></span>

* <span data-ttu-id="f6f7d-323">Tippfehler im Beispiel für „az synapse role assignment create“ und „az synapse role assignment delete“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-323">Fixed typo in example of az synapse role assignment create and delete</span></span>

## <a name="august-28-2020"></a><span data-ttu-id="f6f7d-324">28. August 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-324">August 28, 2020</span></span>

<span data-ttu-id="f6f7d-325">Version 2.11.1</span><span class="sxs-lookup"><span data-stu-id="f6f7d-325">Version 2.11.1</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-326">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-326">ACR</span></span>

* <span data-ttu-id="f6f7d-327">Dienstebene „Isoliert“ zum Agentpool hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-327">Add Isolated Tier to Agent Pool</span></span>
* <span data-ttu-id="f6f7d-328">Quellkontext des OCI-Artefakts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-328">Add OCI Artifact Source Context</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-329">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-329">AKS</span></span>

* <span data-ttu-id="f6f7d-330">Problem bei der Erstellung des AKS-Clusters behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-330">Fix aks cluster create issue</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6f7d-331">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6f7d-331">Cognitive Services</span></span>

* <span data-ttu-id="f6f7d-332">[BREAKING CHANGE] Anzeigen zusätzlicher rechtlicher Bedingungen für bestimmte APIs</span><span class="sxs-lookup"><span data-stu-id="f6f7d-332">[BREAKING CHANGE] Show additional legal term for certain APIs</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-333">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-333">Network</span></span>

* <span data-ttu-id="f6f7d-334">[BREAKING CHANGE] Erstellung öffentlicher und privater IP-Adressen beim Erstellen einer Application Gateway-Instanz zulässig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-334">[BREAKING CHANGE] Allow to create both public and private IP while creating an Application Gateway</span></span>
* <span data-ttu-id="f6f7d-335">`az network list-service-tags`: Details zur Verwendung des Standortparameters zur Hilfemeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-335">`az network list-service-tags`: add details on location parameter use to the help message</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-336">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-336">Storage</span></span>

* <span data-ttu-id="f6f7d-337">`az storage blob list`: Unterstützung der OR-Eigenschaften mit neuer API-Version</span><span class="sxs-lookup"><span data-stu-id="f6f7d-337">`az storage blob list`: Support OR properties with new api version</span></span>

## <a name="august-25-2020"></a><span data-ttu-id="f6f7d-338">25. August 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-338">August 25, 2020</span></span>

<span data-ttu-id="f6f7d-339">Version 2.11.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-339">Version 2.11.0</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-340">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-340">AKS</span></span>

* <span data-ttu-id="f6f7d-341">Vorschautag aus dem Add-On für virtuelle Knoten entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-341">Remove preview tag from Virtual Node add-on</span></span>
* <span data-ttu-id="f6f7d-342">AKS-CMK-Argument bei Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-342">Add AKS CMK argument in cluster creation</span></span>
* <span data-ttu-id="f6f7d-343">Netzwerkprofil bei Verwendung des Lastenausgleichs im Basic-Tarif festgelegt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-343">Set network profile when using basic load balancer.</span></span>
* <span data-ttu-id="f6f7d-344">Überprüfung der maximalen Pods aus CLI entfernt, wird nun durch Preflight verarbeitet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-344">Remove max pods validation from CLI and let preflight handle it</span></span>
* <span data-ttu-id="f6f7d-345">Add-Ons korrigiert, die in der Hilfemeldung in `az aks create` verfügbar sind</span><span class="sxs-lookup"><span data-stu-id="f6f7d-345">Fixing add-ons available in the help message in `az aks create`</span></span>
* <span data-ttu-id="f6f7d-346">Unterstützung für das Autoskalierungsprofil für Cluster in Core-CLI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-346">Bring in support for cluster autoscaler profile in core CLI</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-347">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-347">AppService</span></span>

* <span data-ttu-id="f6f7d-348">`az webapp`: Befehl „list-instances“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-348">`az webapp`: Add list-instances command</span></span>
* <span data-ttu-id="f6f7d-349">`az webapp ssh`: Parameter „--instance“ für die Verbindungsherstellung mit einer bestimmten Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-349">`az webapp ssh`: Add --instance parameter to connect to a specific instance</span></span>
* <span data-ttu-id="f6f7d-350">`az webapp create-remote-connection`: Parameter „--instance“ für die Verbindungsherstellung mit einer bestimmten Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-350">`az webapp create-remote-connection`: Add --instance parameter to connect to a specific instance</span></span>
* <span data-ttu-id="f6f7d-351">Fehlerbehebung Nr. 14758: Fehler bei „az webapp create“ beim Erstellen von Windows-Apps mit „--runtime dotnetcore“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-351">Fix #14758: az webapp create errors when creating windows app with --runtime dotnetcore</span></span>
* <span data-ttu-id="f6f7d-352">Fehlerbehebung Nr. 14701: „functionapp create --assign-identity“ implementiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-352">Fix #14701: Implement functionapp create --assign-identity</span></span>
* <span data-ttu-id="f6f7d-353">Fehlerbehebung Nr. 11244: `az webapp auth update`: Optionaler Parameter zum Aktualisieren von „client-secret-certificate-thumbprint“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-353">Fix #11244: `az webapp auth update`: Add optional parameter to update client-secret-certificate-thumbprint</span></span>
* <span data-ttu-id="f6f7d-354">`az functionapp keys`: Befehle hinzugefügt, mit denen Benutzer die Funktions-App-Schlüssel verwalten können</span><span class="sxs-lookup"><span data-stu-id="f6f7d-354">`az functionapp keys`: Added commands that allow users to manage their function app keys</span></span>
* <span data-ttu-id="f6f7d-355">`az functionapp function`: Befehle hinzugefügt, mit denen Benutzer die einzelnen Funktionen verwalten können</span><span class="sxs-lookup"><span data-stu-id="f6f7d-355">`az functionapp function`: Added commands that allow users to manage their individual functions</span></span>
* <span data-ttu-id="f6f7d-356">`az functionapp function keys`: Befehle hinzugefügt, mit denen Benutzer die Funktionsschlüssel verwalten können</span><span class="sxs-lookup"><span data-stu-id="f6f7d-356">`az functionapp function keys`: Added commands that allow users to manage their function keys</span></span>
* <span data-ttu-id="f6f7d-357">Fehlerbehebung Nr. 14788: Mit „az webapp create“ kann nicht die richtige Web-App abgerufen werden, wenn es sich bei den Namen um Teilzeichenfolgen handelt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-357">Fix #14788: az webapp create not getting correct webapp when names are substrings</span></span>
* <span data-ttu-id="f6f7d-358">`az functionapp create`: Möglichkeit zum Erstellen von 2.x-Funktionen in Regionen entfernt, in denen sie nicht unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-358">`az functionapp create`: Removed ability to create 2.x Functions in regions that don't support it</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-359">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-359">ARM</span></span>

* <span data-ttu-id="f6f7d-360">`az resource list`: Rückgabedaten von `createdTime`, `changedTime` und `provisioningState` erweitert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-360">`az resource list`: Extend the return data of `createdTime`, `changedTime` and `provisioningState`</span></span>
* <span data-ttu-id="f6f7d-361">`az resource`: Parameter `--latest-include-preview` hinzugefügt, um die Verwendung der neuesten API-Version zu unterstützen, unabhängig davon, ob es sich dabei um eine Vorschauversion handelt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-361">`az resource`: Add parameter `--latest-include-preview` to support using the latest api-version whether this version is preview</span></span>

### <a name="aro"></a><span data-ttu-id="f6f7d-362">ARO</span><span class="sxs-lookup"><span data-stu-id="f6f7d-362">ARO</span></span>

* <span data-ttu-id="f6f7d-363">CLI-Erweiterungen, einschließlich Berechtigungen für die Überprüfung von Routingtabellen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-363">CLI enhancements, including route table checking permissions</span></span>

### <a name="cloud"></a><span data-ttu-id="f6f7d-364">Cloud</span><span class="sxs-lookup"><span data-stu-id="f6f7d-364">Cloud</span></span>

* <span data-ttu-id="f6f7d-365">`az cloud register`: Registrierung von Clouds mit einer Konfigurationsdatei korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-365">`az cloud register`: Fix registering clouds with a config file</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-366">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-366">Compute</span></span>

* <span data-ttu-id="f6f7d-367">VM-SKUs aktualisiert, die den beschleunigten Netzwerkbetrieb unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-367">Update VM SKUs that support accelerated networking</span></span>
* <span data-ttu-id="f6f7d-368">`az vm create`: Automatische Patches auf Gastsystemen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-368">`az vm create`: Automatic in-guest patching</span></span>
* <span data-ttu-id="f6f7d-369">`az image builder create`: „--vm-size“, „--os-disk-size“, „--vnet“ und „--subnet“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-369">`az image builder create`: Add --vm-size, --os-disk-size, --vnet, --subnet</span></span>
* <span data-ttu-id="f6f7d-370">Neuer Befehl „az vm assess-patches“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-370">New command az vm assess-patches</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-371">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-371">Container</span></span>

* <span data-ttu-id="f6f7d-372">Fehlerbehebung Nr. 6235: Hilfetext für ports-Parameter bei der Containererstellung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-372">Fix #6235: Update help text for ports parameter in container create</span></span>

### <a name="datalake-store"></a><span data-ttu-id="f6f7d-373">Data Lake-Speicher</span><span class="sxs-lookup"><span data-stu-id="f6f7d-373">Datalake Store</span></span>

* <span data-ttu-id="f6f7d-374">Fehlerbehebung Nr. 14545 für Data Lake-Verknüpfungsvorgang</span><span class="sxs-lookup"><span data-stu-id="f6f7d-374">Fix issue #14545 for data lake join operation</span></span>

### <a name="eventhub"></a><span data-ttu-id="f6f7d-375">EventHub</span><span class="sxs-lookup"><span data-stu-id="f6f7d-375">EventHub</span></span>

* <span data-ttu-id="f6f7d-376">`az eventhubs eventhub create/update`: Dokumentation zu „destination_name“ geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-376">`az eventhubs eventhub create/update`: Change documentation of destination_name</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-377">Erweiterung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-377">Extension</span></span>

* <span data-ttu-id="f6f7d-378">Befehl `az extension list-versions` hinzugefügt, um alle verfügbaren Versionen einer Erweiterung aufzulisten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-378">Add `az extension list-versions` command to list all available versions of an extension</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-379">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-379">HDInsight</span></span>

* <span data-ttu-id="f6f7d-380">Unterstützung für das Erstellen von Clustern mit Autoskalierungskonfiguration und Unterstützung für die Verwaltung der Autoskalierungskonfiguration</span><span class="sxs-lookup"><span data-stu-id="f6f7d-380">Support creating cluster with autoscale configuration and Support managing autoscale configuration</span></span>
* <span data-ttu-id="f6f7d-381">Unterstützung für das Erstellen eines Clusters mit Verschlüsselung auf dem Host</span><span class="sxs-lookup"><span data-stu-id="f6f7d-381">Support creating cluster with encryption at host</span></span>

### <a name="iotcentral"></a><span data-ttu-id="f6f7d-382">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="f6f7d-382">IoTCentral</span></span>

* <span data-ttu-id="f6f7d-383">Verbesserungen bei der CLI-Dokumentation</span><span class="sxs-lookup"><span data-stu-id="f6f7d-383">CLI documentation improvements</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-384">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-384">Monitor</span></span>

* <span data-ttu-id="f6f7d-385">`az monitor metrics alert create`: Unterstützung von „RG“ und „Sub“ als Bereichswerte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-385">`az monitor metrics alert create`: support RG and Sub as the scope values</span></span>

### <a name="netappfiles"></a><span data-ttu-id="f6f7d-386">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="f6f7d-386">NetAppFiles</span></span>

* <span data-ttu-id="f6f7d-387">[BREAKING CHANGE] az netappfiles snapshot create: „file-system-id“ aus Parametern entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-387">[BREAKING CHANGE] az netappfiles snapshot create: Removed file-system-id from parameters</span></span>
* <span data-ttu-id="f6f7d-388">[BREAKING CHANGE] az netappfiles snapshot show: Die Momentaufnahme enthält nicht länger den Parameter „file-system-id“.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-388">[BREAKING CHANGE] az netappfiles snapshot show: Snapshot no longer has parameter file-system-id</span></span>
* <span data-ttu-id="f6f7d-389">`az netappfiles account`: Das Modell „ActiveDirectory“ verfügt nun über den neuen Parameter „backup_operators“.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-389">`az netappfiles account`: Model ActiveDirectory has a new parameter backup_operators</span></span>
* <span data-ttu-id="f6f7d-390">`az netappfiles volume show`: Das Modell „dataProtection“ verfügt nun über den neuen Parameter „snapshot“.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-390">`az netappfiles volume show`: Model dataProtection has a new parameter snapshot</span></span>
* <span data-ttu-id="f6f7d-391">`az netappfiles volume show`: Das Modell „Volume“ verfügt nun über den neuen Parameter „snapshot_directory_visible“.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-391">`az netappfiles volume show`: Model Volume has a new parameter snapshot_directory_visible</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-392">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-392">Network</span></span>

* <span data-ttu-id="f6f7d-393">`az network dns export`: Für MX, PTR, NS und SRV wird nun der FQDN anstelle des relativen Pfads exportiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-393">`az network dns export`: export FQDN for MX, PTR, NS and SRV type instead of relative path</span></span>
* <span data-ttu-id="f6f7d-394">Unterstützung privater Links für verwaltete Datenträger</span><span class="sxs-lookup"><span data-stu-id="f6f7d-394">Support private link for managed disks</span></span>
* <span data-ttu-id="f6f7d-395">`az network application-gateway auth-cert show`: Beispiel zur Veranschaulichung des Zertifikatformats hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-395">`az network application-gateway auth-cert show`: Add example to demonstrate certificate format</span></span>
* <span data-ttu-id="f6f7d-396">`az network private-endpoint-connection`: Unterstützung der App-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="f6f7d-396">`az network private-endpoint-connection`: support app configuration</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-397">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-397">RBAC</span></span>

* <span data-ttu-id="f6f7d-398">`az ad group create`: Unterstützung der Angabe einer Beschreibung beim Erstellen einer Gruppe</span><span class="sxs-lookup"><span data-stu-id="f6f7d-398">`az ad group create`: support specify description when creating a group</span></span>
* <span data-ttu-id="f6f7d-399">`az role definition create`: Ausgabe einer lesbaren Nachricht anstelle einer Ausnahme, wenn „assignableScope“ ein leeres Array ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-399">`az role definition create`: print human readable message instead of exception when assignableScope is an empty array</span></span>
* <span data-ttu-id="f6f7d-400">[BREAKING CHANGE] `az ad sp create-for-rbac`: Standardberechtigung des erstellten Zertifikats geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-400">[BREAKING CHANGE] `az ad sp create-for-rbac`: change default permission of created certificate</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-401">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-401">SQL</span></span>

* <span data-ttu-id="f6f7d-402">`az sql server audit-policy`: Unterstützung für SQL Server-Überwachung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-402">`az sql server audit-policy`: Add sql server auditing support</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-403">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-403">Storage</span></span>

* <span data-ttu-id="f6f7d-404">`az storage blob copy start-batch`: Fehlerbehebung Nr. 6018 für „--source-sas“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-404">`az storage blob copy start-batch`: Fix #6018 for --source-sas</span></span>
* <span data-ttu-id="f6f7d-405">`az storage account or-policy`: Unterstützung für die Objektreplikationsrichtlinie für Speicherkonten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-405">`az storage account or-policy`: Support storage account object replication policy</span></span>
* <span data-ttu-id="f6f7d-406">Fehlerbehebung Nr. 14083, um die Version des Pakets „azure-multiapi-storage“ aufgrund eines Paketproblems zu aktualisieren und neue API-Versionen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-406">Fix issue #14083 to upgrade azure-multiapi-storage package version for package issue and new api version support</span></span>
* <span data-ttu-id="f6f7d-407">`az storage blob generate-sas`: Beispiele für „--ip“ hinzugefügt und Fehlermeldung optimiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-407">`az storage blob generate-sas`: add examples for --ip  and refine error message</span></span>
* <span data-ttu-id="f6f7d-408">`az storage blob list`: Problem bei „next_marker“ behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-408">`az storage blob list`: Fix next_marker issue</span></span>

### <a name="synapse"></a><span data-ttu-id="f6f7d-409">Synapse</span><span class="sxs-lookup"><span data-stu-id="f6f7d-409">Synapse</span></span>

* <span data-ttu-id="f6f7d-410">Cmdlets für Arbeitsbereich, Spark-Pool und SQL-Pool hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-410">Add workspace, sparkpool, sqlpool related cmdlets</span></span>
* <span data-ttu-id="f6f7d-411">Befehle im Zusammenhang mit Spark-Aufträgen basierend auf track2 SDK hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-411">Add spark job releated commands based on track2 sdk</span></span>
* <span data-ttu-id="f6f7d-412">Befehle im Zusammenhang mit accesscontrol-Feature basierend auf track2 SDK hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-412">Add accesscontrol feature related commands based on track2 sdk</span></span>

### <a name="upgrade"></a><span data-ttu-id="f6f7d-413">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-413">Upgrade</span></span>

* <span data-ttu-id="f6f7d-414">Befehl `az upgrade` zum Aktualisieren der Azure CLI und von Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-414">Add `az upgrade` command to upgrade azure cli and extensions</span></span>

## <a name="august-11-2020"></a><span data-ttu-id="f6f7d-415">11. August 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-415">August 11, 2020</span></span>

<span data-ttu-id="f6f7d-416">Version 2.10.1</span><span class="sxs-lookup"><span data-stu-id="f6f7d-416">Version 2.10.1</span></span>

### <a name="app-service"></a><span data-ttu-id="f6f7d-417">App Service</span><span class="sxs-lookup"><span data-stu-id="f6f7d-417">App Service</span></span>

* <span data-ttu-id="f6f7d-418">Behebung Nr. 9887: webapp und functionapp, Unterstützung für das Zuweisen/Entfernen einer benutzerseitig verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="f6f7d-418">Fix #9887 webapp and functionapp, support assigning/removing user managed identity</span></span>
* <span data-ttu-id="f6f7d-419">Behebung Nr. 1382, Nr. 14055: Fehlermeldungen für „az webapp create“ und „az webapp config container set“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-419">Fix #1382, #14055: Update error messages for az webapp create and az webapp config container set</span></span>
* <span data-ttu-id="f6f7d-420">`az webapp up`: Standardmäßige ASP-Auswahllogik korrigiert, wenn der Parameter „--plan“ nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-420">`az webapp up`: Fix default ASP selection logic when --plan parameter is not provided</span></span>

### <a name="appconfig"></a><span data-ttu-id="f6f7d-421">AppConfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-421">AppConfig</span></span>

* <span data-ttu-id="f6f7d-422">Unterstützung für die Aktivierung/Deaktivierung von PublicNetworkAccess während der Speichererstellung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-422">Support enabling/disabling PublicNetworkAccess during store creation</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-423">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-423">Compute</span></span>

* <span data-ttu-id="f6f7d-424">Unterstützung für das Zuordnen einer Datenträgerzugriffsressource für Datenträger und Momentaufnahmen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-424">Support associating disk and snapshot with a disk-access resource</span></span>

### <a name="lab"></a><span data-ttu-id="f6f7d-425">Labor</span><span class="sxs-lookup"><span data-stu-id="f6f7d-425">Lab</span></span>

* <span data-ttu-id="f6f7d-426">Fehlerbehebung Nr. 7904: Fehler bei der Datumsüberprüfung bei der Lab-VM-Erstellung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-426">Fix for issue #7904 date validation bug in lab vm creation</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-427">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-427">Storage</span></span>

* <span data-ttu-id="f6f7d-428">`az storage blob upload-batch`: Problembehebung Nr. 14660 mit nicht positionellen Argumenten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-428">`az storage blob upload-batch`: Fix issue #14660 with unpositional arguments</span></span>

## <a name="august-04-2020"></a><span data-ttu-id="f6f7d-429">04. August 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-429">August 04, 2020</span></span>

<span data-ttu-id="f6f7d-430">Version 2.10.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-430">Version 2.10.0</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-431">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-431">AKS</span></span>

* <span data-ttu-id="f6f7d-432">`az aks update`: Argument „--enable-aad“ geändert, um einen RBAC-fähigen AAD-fremden Cluster zu einem von AKS-verwalteten AAD-Cluster zu migrieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-432">`az aks update`: Change --enable-aad argument to migrate a RBAC-enabled non-AAD cluster to a AKS-managed AAD cluster</span></span>
* <span data-ttu-id="f6f7d-433">`az aks install-cli`: Argumente „--kubelogin-version“ und „--kubelogin-install-location“ zum Installieren von kubelogin hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-433">`az aks install-cli`: Add --kubelogin-version and --kubelogin-install-location arguments to install kubelogin</span></span>
* <span data-ttu-id="f6f7d-434">Befehl „az aks nodepool get-upgrades“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-434">Add az aks nodepool get-upgrades command</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-435">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-435">AMS</span></span>

* <span data-ttu-id="f6f7d-436">Korrektur 14021: „az ams account sp“ ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-436">Fix #14021: az ams account sp is not idempotent</span></span>

### <a name="apim"></a><span data-ttu-id="f6f7d-437">APIM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-437">APIM</span></span>

* <span data-ttu-id="f6f7d-438">APIM-API-Import: API-Importunterstützung und Erweiterung anderer CLI-Befehle auf der API-Ebene</span><span class="sxs-lookup"><span data-stu-id="f6f7d-438">apim api import: support API import and enchance other api level cli commands</span></span>

### <a name="app-service"></a><span data-ttu-id="f6f7d-439">App Service</span><span class="sxs-lookup"><span data-stu-id="f6f7d-439">App Service</span></span>

* <span data-ttu-id="f6f7d-440">Korrektur 13035: Zugriffsbeschränkungsüberprüfung für „az webapp config“ hinzugefügt, um Duplikate zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-440">Fix #13035: Add validation for az webapp config access-restriction to avoid adding duplicates</span></span>

### <a name="appconfig"></a><span data-ttu-id="f6f7d-441">AppConfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-441">AppConfig</span></span>

* <span data-ttu-id="f6f7d-442">Bei fehlender Angabe wird die Standard-SKU verwendet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-442">Default to standard sku if not specified</span></span>
* <span data-ttu-id="f6f7d-443">[BREAKING CHANGE] Einstellungen mit JSON-Inhaltstyp werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-443">[BREAKING CHANGE] Support settings with JSON content type</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-444">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-444">ARM</span></span>

* <span data-ttu-id="f6f7d-445">`az resource tag`: Fehler im Zusammenhang mit managedApp-Kennzeichnung sowie einige damit zusammenhängende Testprobleme behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-445">`az resource tag`: Fix the bug of managedApp tagging and some related test issues</span></span>
* <span data-ttu-id="f6f7d-446">`az deployment mg/tenant what-if`: Unterstützung für die Bereitstellung auf Verwaltungsgruppen- und Mandantenebene hinzugefügt (Was-wäre-wenn)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-446">`az deployment mg/tenant what-if`: Add support to management group and tenant level deployment What-If</span></span>
* <span data-ttu-id="f6f7d-447">`az deployment mg/tenant create`: Parameter „--confirm-with-what-if/-c“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-447">`az deployment mg/tenant create`: Add --confirm-with-what-if/-c parameter.</span></span>
* <span data-ttu-id="f6f7d-448">`az deployment mg/tenant create`: Parameter „--what-if-result-format/-r“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-448">`az deployment mg/tenant create`: Add --what-if-result-format/-r parameter.</span></span>
* <span data-ttu-id="f6f7d-449">`az deployment mg/tenant create`: Parameter „--what-if-exclude-change-types/-x“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-449">`az deployment mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="f6f7d-450">`az tag`: Unterstützung von „az tag“ für Ressourcen-ID-Parameter</span><span class="sxs-lookup"><span data-stu-id="f6f7d-450">`az tag`: az tag support for resource id parameter</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-451">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-451">Backup</span></span>

* <span data-ttu-id="f6f7d-452">Auslösung von AFS-Container-/Elementerkennung nur bei Bedarf</span><span class="sxs-lookup"><span data-stu-id="f6f7d-452">Trigger AFS container/item discovery only when needed</span></span>

### <a name="cdn"></a><span data-ttu-id="f6f7d-453">CDN</span><span class="sxs-lookup"><span data-stu-id="f6f7d-453">CDN</span></span>

* <span data-ttu-id="f6f7d-454">Private Link-Felder zu Ursprung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-454">Add private link fields to origin</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-455">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-455">Compute</span></span>

* <span data-ttu-id="f6f7d-456">`az vm/vmss create`: Wahl eines gültigen Benutzernamens für den Benutzer bei ungültigem Standardbenutzernamen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-456">`az vm/vmss create`: Select a valid username for user if the default username is invalid</span></span>
* <span data-ttu-id="f6f7d-457">`az vm update`: Unterstützung mandantenübergreifender Images</span><span class="sxs-lookup"><span data-stu-id="f6f7d-457">`az vm update`: support cross tenant image</span></span>
* <span data-ttu-id="f6f7d-458">`az disk-access`: Neue Befehlsgruppe für die Verwendung der Datenträgerzugriffsressource hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-458">`az disk-access`: Add new command group to operate disk access resource</span></span>
* <span data-ttu-id="f6f7d-459">Unterstützung der automatischen Platzierung dedizierter Hostgruppen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-459">Support dedicated host group automatic placement</span></span>
* <span data-ttu-id="f6f7d-460">Unterstützung von PPG und SPG im VMSS-Orchestrierungsmodus</span><span class="sxs-lookup"><span data-stu-id="f6f7d-460">Support ppg and spg in VMSS orchestration mode</span></span>

### <a name="config"></a><span data-ttu-id="f6f7d-461">Config</span><span class="sxs-lookup"><span data-stu-id="f6f7d-461">Config</span></span>

* <span data-ttu-id="f6f7d-462">`az config`: Neuer Befehl (`config`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-462">`az config`: Add new `config` command module</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-463">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-463">Extension</span></span>

* <span data-ttu-id="f6f7d-464">Unterstützung der automatischen Installation einer Erweiterung, wenn die Erweiterung eines Befehls nicht installiert ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-464">Support automatically installing an extension if the extension of a command is not installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-465">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-465">HDInsight</span></span>

* <span data-ttu-id="f6f7d-466">Drei Parameter zum Befehl `az hdinsight create` hinzugefügt, um Private Link und Verschlüsselung während der Übertragung zu unterstützen:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-466">Add 3 parameters to the command `az hdinsight create` to support private link and encryption in transit feature:</span></span>

### <a name="iot-hub"></a><span data-ttu-id="f6f7d-467">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="f6f7d-467">Iot Hub</span></span>

* <span data-ttu-id="f6f7d-468">Korrektur 7792: „iot hub create“ ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-468">Fix #7792: IoT Hub Create is not idempotent</span></span>

### <a name="iot-central"></a><span data-ttu-id="f6f7d-469">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f6f7d-469">IoT Central</span></span>

* <span data-ttu-id="f6f7d-470">Parameteroptionenliste für IoT Central hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-470">Add paramater option list for iot central</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-471">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-471">KeyVault</span></span>

* <span data-ttu-id="f6f7d-472">`az keyvault key encrypt/decrypt`: Parameter `--data-type` zum expliziten Angeben der Art von Originaldaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-472">`az keyvault key encrypt/decrypt`: add parameter `--data-type` for explicitly specifing the type of original data</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-473">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-473">Monitor</span></span>

* <span data-ttu-id="f6f7d-474">`az monitor log-analytics workspace data-export`: Unterstützung des Event Hub-Namespace als Ziel</span><span class="sxs-lookup"><span data-stu-id="f6f7d-474">`az monitor log-analytics workspace data-export`: support event hub namespace as the destination.</span></span>
* <span data-ttu-id="f6f7d-475">`az monitor autoscale`: Unterstützung von Namespace und Dimensionen für „--condition“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-475">`az monitor autoscale`: support namespace and dimensions for --condition</span></span>

### <a name="netappfiles"></a><span data-ttu-id="f6f7d-476">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="f6f7d-476">NetAppFiles</span></span>

* <span data-ttu-id="f6f7d-477">`az volume revert`:  Volumewiederherstellung hinzugefügt, um ein Volume auf eine der zugehörigen Momentaufnahmen zurückzusetzen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-477">`az volume revert`:  Add Volume Revert to revert a volume to one of its snapshots.</span></span>
* <span data-ttu-id="f6f7d-478">[BREAKING CHANGE] `az netappfiles mount-target` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-478">[BREAKING CHANGE] Remove `az netappfiles mount-target`.</span></span>
* <span data-ttu-id="f6f7d-479">`az volume show`: Standort zu Active Directory-Eigenschaften hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-479">`az volume show`: Add site to Active Directory Properties</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-480">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-480">Network</span></span>

* <span data-ttu-id="f6f7d-481">`az application-gateway private-link add`: Unterstützung der Angabe eines vorhandenen Subnetzes nach ID</span><span class="sxs-lookup"><span data-stu-id="f6f7d-481">`az application-gateway private-link add`: support to specify an existing subnet by ID</span></span>
* <span data-ttu-id="f6f7d-482">`az network application-gateway waf-policy create`: Unterstützung von Version und Typ</span><span class="sxs-lookup"><span data-stu-id="f6f7d-482">`az network application-gateway waf-policy create`: support version and type</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-483">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-483">Storage</span></span>

* <span data-ttu-id="f6f7d-484">Korrektur 10302: Unterstützung der Ermittlung des wahrscheinlichen Inhaltstyps beim Synchronisieren von Dateien</span><span class="sxs-lookup"><span data-stu-id="f6f7d-484">Fix #10302: Support guess content-type when synchronizing files</span></span>
* <span data-ttu-id="f6f7d-485">`az storage blob lease`: Neue API-Version für Blobleasevorgänge angewendet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-485">`az storage blob lease`: Apply new api version for blob lease operations</span></span>
* <span data-ttu-id="f6f7d-486">`az storage fs access`: Unterstützung von AAD-Anmeldeinformationen bei der Verwaltung der Zugriffssteuerung für das ADLS Gen2-Konto</span><span class="sxs-lookup"><span data-stu-id="f6f7d-486">`az storage fs access`: Support AAD credential in managing access control for ADLS Gen2 account</span></span>
* <span data-ttu-id="f6f7d-487">`az storage share-rm create/update`: „--access-tier“ hinzugefügt, um die Zugriffsebene zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-487">`az storage share-rm create/update`: add --access-tier to support access tier</span></span>

## <a name="july-16-2020"></a><span data-ttu-id="f6f7d-488">16. Juli 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-488">July 16, 2020</span></span>

<span data-ttu-id="f6f7d-489">Version 2.9.1</span><span class="sxs-lookup"><span data-stu-id="f6f7d-489">Version 2.9.1</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-490">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-490">AKS</span></span>

* <span data-ttu-id="f6f7d-491">Explizite Einstellung von VMSS im Windows-Beispielbefehl entfernt, da dies jetzt die Standardeinstellung ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-491">Remove explicit setting of VMSS in Windows example command since it is now default</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-492">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-492">IoT</span></span>

* <span data-ttu-id="f6f7d-493">[BREAKING CHANGE] `az iot pnp`: IoT-PNP-Vorschaubefehle aus Core-CLI entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-493">[BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI</span></span>

### <a name="rest"></a><span data-ttu-id="f6f7d-494">REST</span><span class="sxs-lookup"><span data-stu-id="f6f7d-494">REST</span></span>

* <span data-ttu-id="f6f7d-495">Behebung Nr. 14152: `az rest`: ARM-URLs ohne Abonnement-ID werden nun akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-495">Fix #14152: `az rest`: Accept ARM URLs without subscription ID</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-496">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-496">Storage</span></span>

* <span data-ttu-id="f6f7d-497">Behebung Nr. 14138: Einige Berechtigungen sind nun optional.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-497">Fix #14138: Make some permissions optional</span></span>

## <a name="july-14-2020"></a><span data-ttu-id="f6f7d-498">14. Juli 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-498">July 14, 2020</span></span>

<span data-ttu-id="f6f7d-499">Version 2.9.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-499">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-500">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-500">ACR</span></span>

* <span data-ttu-id="f6f7d-501">Verarbeiten des Protokollartefaktlinks aus der Registrierung zum Streamen von Protokollen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-501">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="f6f7d-502">Helm2-Befehle als veraltet kennzeichnen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-502">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-503">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-503">AKS</span></span>

* <span data-ttu-id="f6f7d-504">`az aks create`: Argument „--enable-aad“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-504">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="f6f7d-505">`az aks update`: Argument „--enable-aad“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-505">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="f6f7d-506">APIM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-506">APIM</span></span>

* <span data-ttu-id="f6f7d-507">Allgemeine Befehle vom Typ „az apim api“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-507">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="f6f7d-508">AppConfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-508">AppConfig</span></span>

* <span data-ttu-id="f6f7d-509">Beispiel für die Verwendung von „--fields“ in AppConfig-Revision hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-509">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-510">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-510">AppService</span></span>

* <span data-ttu-id="f6f7d-511">`az functionapp create`: Unterstützung für Java 11 und PowerShell 7 hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-511">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="f6f7d-512">Unterstützung für Stapel-API hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-512">Added Stacks API Support.</span></span>
* <span data-ttu-id="f6f7d-513">Behebung von Nr. 14208: Erstellen einer App mit mehreren Containern erzeugt einen Fehler</span><span class="sxs-lookup"><span data-stu-id="f6f7d-513">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="f6f7d-514">Korrektur von „az webapp create“ – hartcodierte Laufzeitstapel verwenden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-514">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-515">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-515">ARM</span></span>

* <span data-ttu-id="f6f7d-516">`az resource tag`: Behebung des Problems beim Taggen von Ressourcen mit dem Ressourcentyp `Microsoft.ContainerInstance/containerGroups`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-516">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-517">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-517">Compute</span></span>

* <span data-ttu-id="f6f7d-518">Datenträgerversion aktualisieren 2020-05-01, Compute 2020-06-01</span><span class="sxs-lookup"><span data-stu-id="f6f7d-518">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="f6f7d-519">Doppelte Verschlüsselung des Datenträgerverschlüsselungssatzes</span><span class="sxs-lookup"><span data-stu-id="f6f7d-519">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="f6f7d-520">`az vmss update`: Unterstützung für das Angeben eines mandantenübergreifendes Image.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-520">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="f6f7d-521">`az sig image-version create`: Unterstützung für das Angeben eines mandantenübergreifendes Image.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-521">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="f6f7d-522">vm/vmss create: Verschlüsselung von Cache und Daten während der Übertragung für (Betriebssystem-)Datenträger und temporäre Datenträger für VM und VMSS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-522">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="f6f7d-523">Vorgang „simulate-eviction“ für VM und VMSS hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-523">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6f7d-524">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-524">CosmosDB</span></span>

* <span data-ttu-id="f6f7d-525">Aktuelle Features: Autoscale, IpRules, EnableFreeTier und EnableAnalyticalStorage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-525">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f6f7d-526">EventGrid</span><span class="sxs-lookup"><span data-stu-id="f6f7d-526">EventGrid</span></span>

* <span data-ttu-id="f6f7d-527">CLI-Unterstützung für 2020-04-01-preview hinzufügen und Previewfunktionen mit „is_Preview=True“ kennzeichnen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-527">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="f6f7d-528">Suchen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-528">Find</span></span>

* <span data-ttu-id="f6f7d-529">Behebung von Nr. 14094 „az find“: Abfragen schlagen fehl, wenn nicht angemeldet und Telemetrie deaktiviert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-529">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-530">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-530">HDInsight</span></span>

* <span data-ttu-id="f6f7d-531">Zwei Befehle zur Unterstützung der Neustartfunktion für HDInsight-Knoten hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-531">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-532">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-532">Monitor</span></span>

* <span data-ttu-id="f6f7d-533">Vorschaukennzeichnung für Befehle unter Log Analytics-Arbeitsbereich entfernen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-533">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="f6f7d-534">`az monitor diagnostic-settings subscription`: Diagnoseeinstellungen für Abonnement unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-534">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="f6f7d-535">`az monitor metrics`: „,“ und „|“ in Metrikname unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-535">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="f6f7d-536">`az monitor log-analytics workspace data-export`: Log Analytics-Datenexport unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-536">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-537">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-537">Network</span></span>

* <span data-ttu-id="f6f7d-538">`az network application-gateway frontend-ip update`: Parameter „--public-ip-address“ als veraltet markieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-538">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="f6f7d-539">„azure-mgmt-network“ auf 11.0.0 aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-539">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="f6f7d-540">`az network express-route gateway connection`: Routingkonfiguration unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-540">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="f6f7d-541">`az network virtual-appliance`: Virtuelle Azure-Netzwerkgerät unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-541">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="f6f7d-542">Application Gateway-Unterstützung der Funktion für private Links</span><span class="sxs-lookup"><span data-stu-id="f6f7d-542">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="f6f7d-543">PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="f6f7d-543">PolicyInsights</span></span>

* <span data-ttu-id="f6f7d-544">`az policy state`: Befehl „trigger-scan“ zu Auswertungen der Compliance von Auslöserrichtinien hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-544">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="f6f7d-545">`az policy state list`: Versionen von Richtlinienentitäten in jedem Compliancedatensatz verfügbar machen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-545">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-546">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-546">Profile</span></span>

* <span data-ttu-id="f6f7d-547">`az account get-access-token`: „expiresOn“ für verwaltete Identität anzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-547">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-548">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-548">RDBMS</span></span>

* <span data-ttu-id="f6f7d-549">TLS-Mindestversion unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-549">Support Minimum TLS version</span></span>
* <span data-ttu-id="f6f7d-550">Infrastrukturverschlüsselung für Azure Postgres und MySQL hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-550">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="f6f7d-551">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="f6f7d-551">Security</span></span>

* <span data-ttu-id="f6f7d-552">Befehl „allowed_connections“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-552">Add allowed_connections commands</span></span>
* <span data-ttu-id="f6f7d-553">Befehle für adaptive Netzwerkhärtung hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-553">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="f6f7d-554">Befehle vom Typ „adaptive_application_controls“ hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-554">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="f6f7d-555">Hinzufügen von „az security iot-solution“/„iot-alerts“/„iot-recommendations“/„iot-analytics“ REST zu Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-555">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="f6f7d-556">CLI für Einhaltung gesetzlicher Bestimmungen hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-556">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="f6f7d-557">SignalR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-557">SignalR</span></span>

* <span data-ttu-id="f6f7d-558">Features einschließlich der Verwaltung privater Endpunktverbindungen, Netzwerkregeln und Upstream hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-558">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-559">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-559">SQL</span></span>

* <span data-ttu-id="f6f7d-560">`az sql mi create`, `az sql mi update`: Parameter `--tags` zur Unterstützung von Ressourcenkennzeichnung hinzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-560">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="f6f7d-561">`az sql mi failover`: Failover vom primären oder sekundären Punkt unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-561">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-562">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-562">Storage</span></span>

* <span data-ttu-id="f6f7d-563">`az storage account create/update`: „--allow-blob-public-access“ hinzufügen, um den öffentlichen Zugriff für Blob und Container zuzulassen oder zu unterbinden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-563">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="f6f7d-564">`az storage account create/update`: `--min-tls-version` hinzufügen, um das Festlegen der TLS-Mindestversion für Anforderungen an den Speicher zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-564">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="f6f7d-565">Token-Anmeldeinformationen zum Einchecken entfernen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-565">Remove check in token credential</span></span>
* <span data-ttu-id="f6f7d-566">Namen des Speicherkontos in Beispielen korrigieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-566">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="f6f7d-567">Webapp</span><span class="sxs-lookup"><span data-stu-id="f6f7d-567">Webapp</span></span>

* <span data-ttu-id="f6f7d-568">Fehlerbehebung: „az webapp log deployment show -“ gibt Bereitstellungsprotokolle anstatt von Protokollmetadaten zurück</span><span class="sxs-lookup"><span data-stu-id="f6f7d-568">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="f6f7d-569">Fehlerbehebung: „az webapp vnet-integration“ hinzufügen – Fehlerbehandlung korrigieren bei ungültigem VNET-Namen, VNET-Ressourcen-ID unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-569">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="f6f7d-570">23. Juni 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-570">June 23, 2020</span></span>

<span data-ttu-id="f6f7d-571">Version 2.8.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-571">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-572">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-572">ACR</span></span>

* <span data-ttu-id="f6f7d-573">Unterstützung für Deaktivierung des Regionsendpunkts/Routings hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-573">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="f6f7d-574">[BREAKING CHANGE] `az acr login --expose-token` akzeptiert Benutzername und Kennwort nicht.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-574">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-575">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-575">ACS</span></span>

* <span data-ttu-id="f6f7d-576">Privater Cluster und API „2019-10-27-preview“ entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-576">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-577">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-577">AKS</span></span>

* <span data-ttu-id="f6f7d-578">Unterstützung: Ja, für „az aks upgrade“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-578">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="f6f7d-579">„Änderung der Standard-VM-SKU in Standard_D2s_v3 (Nr. 13541)“ wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-579">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="f6f7d-580">„az aks update --uptime-sla“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-580">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="f6f7d-581">Tippfehler im Befehl „az aks update“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-581">Fix typo in az aks update command</span></span>
* <span data-ttu-id="f6f7d-582">Änderung, um einen Agentpool mit 0 Knoten zu unterstützen und die manuelle Skalierung für einen Pool mit CAS-Aktivierung zu blockieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-582">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="f6f7d-583">Tippfehler in VirtualMachineScaleSets korrigiert und Verweise auf Kubernetes-Versionen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-583">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-584">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-584">AMS</span></span>

* <span data-ttu-id="f6f7d-585">ÄNDERUNG: Hilfetext für Parameter „--expiry“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-585">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-586">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-586">AppService</span></span>

* <span data-ttu-id="f6f7d-587">`az webapp log deployment show`: Anzeigen des aktuellen Bereitstellungsprotokolls oder der Bereitstellungsprotokolle einer bestimmten Bereitstellung, wenn die Bereitstellungs-ID angegeben ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-587">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="f6f7d-588">`az webapp log deployment list`: Liste der verfügbaren Bereitstellungsprotokolle</span><span class="sxs-lookup"><span data-stu-id="f6f7d-588">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="f6f7d-589">Behebung: Oberflächenfehler bei Angabe eines ungültigen Web-App-Namens</span><span class="sxs-lookup"><span data-stu-id="f6f7d-589">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="f6f7d-590">Nr. 13261 korrigiert: „az webapp list-runtimes“ nutzt eine statische Liste, bis die neue API für verfügbare Stapel zur Verfügung steht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-590">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="f6f7d-591">`az appservice ase create`: Erstellungsproblem behoben (Nr. 13361)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-591">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="f6f7d-592">`az appservice ase list-addresses`: SDK-Änderung korrigiert (Nr. 13140)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-592">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="f6f7d-593">Web-App-/Sloterstellung für Windows-Container korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-593">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="f6f7d-594">`az webapp auth update`: Optionaler Parameter zum Aktualisieren der Laufzeitversion hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-594">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="f6f7d-595">Unterstützung für das Auflisten, Löschen, Genehmigen und Ablehnen der Verbindung mit privatem Endpunkt für eine Web-App in der CLI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-595">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="f6f7d-596">Behebung Nr. 13888: Unterstützung für Static Web Apps hinzugefügt: Befehle zum Abrufen, Auflisten und Erstellen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-596">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="f6f7d-597">Fehlermeldungen für die SSH-Tunnelverbindung verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-597">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-598">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-598">ARM</span></span>

* <span data-ttu-id="f6f7d-599">`az tag`: Beispiele für „-h“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-599">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="f6f7d-600">`az deployment group/sub what-if`: Parameter „--exclude-change-types/-x“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-600">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="f6f7d-601">`az deployment group/sub/mg/tenant create`: Parameter „--what-if-exclude-change-types/-x“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-601">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="f6f7d-602">`az deployment group/sub/mg/tenant validate`: Anzeigen von Fehlermeldungen in einem besseren Format</span><span class="sxs-lookup"><span data-stu-id="f6f7d-602">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="f6f7d-603">`az group export`: Neue Parameter `--skip-resource-name-params` und `--skip-all-params` hinzugefügt, um das Überspringen der Parametrisierung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-603">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="f6f7d-604">API „az feature unregister“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-604">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="f6f7d-605">ARO</span><span class="sxs-lookup"><span data-stu-id="f6f7d-605">ARO</span></span>

* <span data-ttu-id="f6f7d-606">„Public“/„Private“ zu Parametern zur Unterstützung bei Eingangs-/APIServer-Sichtbarkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-606">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-607">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-607">Batch</span></span>

* <span data-ttu-id="f6f7d-608">`az batch account create`: Neuer Parameter `--public-network-access` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-608">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="f6f7d-609">`az batch account create`: Neuer Parameter `--identity-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-609">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="f6f7d-610">`az batch account set`: Neuer Parameter `--identity-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-610">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="f6f7d-611">[BREAKING CHANGE] az batch pool create: Bei der Erstellung eines Pools mithilfe eines benutzerdefinierten Images kann die Eigenschaft „--image“ nun ausschließlich auf ein Shared Image Gallery-Image verweisen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-611">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="f6f7d-612">[BREAKING CHANGE] az batch pool create: Bei der Erstellung eines Pools mit der Option „--json-file“ und Angabe einer Netzwerkkonfiguration (networkConfiguration) wurde die Eigenschaft „publicIPs“ in die neue Eigenschaft „publicIPAddressConfiguration“ verschoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-612">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="f6f7d-613">Diese neue Eigenschaft unterstützt außerdem die neue Eigenschaft „ipAddressProvisioningType“. Diese gibt an, wie der Pool IP-Adressen und die Eigenschaft „publicIPs“ zuordnen muss, um die Konfiguration einer Liste mit PublicIP-Ressourcen zu ermöglichen, die bei der Festlegung von „ipAddressProvisioningType“ auf „UserManaged“ verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-613">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="f6f7d-614">`az network private-link-resource`: Unterstützung für die Microsoft.Batch-Ressource „batchAccount“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-614">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="f6f7d-615">`az network private-endpoint-connection`: Unterstützung für die Microsoft.Batch-Ressource „batchAccount“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-615">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="f6f7d-616">CDN</span><span class="sxs-lookup"><span data-stu-id="f6f7d-616">CDN</span></span>

* <span data-ttu-id="f6f7d-617">`az cdn custom-domain enable-https`: Unterstützung für BYOC hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-617">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="f6f7d-618">`az cdn custom-domain enable-https`: Aktivierung von benutzerdefiniertem HTTPS mit CDN-verwalteten Zertifikaten für die SKUs Standard_Verizon und Standard_Microsoft korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-618">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6f7d-619">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6f7d-619">Cognitive Services</span></span>

* <span data-ttu-id="f6f7d-620">[BREAKING CHANGE] `az cognitiveservices account` besitzt nun eine einheitliche Struktur für alle Befehle.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-620">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="f6f7d-621">`az cognitiveservices account identity`: Identitätsverwaltung für Cognitive Services hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-621">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-622">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-622">Compute</span></span>

* <span data-ttu-id="f6f7d-623">`az image builder`: API-Version auf 2020-02-14 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-623">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="f6f7d-624">`az image builder create`: `--identity` zur Unterstützung der Identitätskonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-624">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="f6f7d-625">`az image builder customizer add`: Unterstützung für Windows Update-Anpassung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-625">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="f6f7d-626">Neuer Befehl `az image builder cancel`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-626">New command `az image builder cancel`</span></span>
* <span data-ttu-id="f6f7d-627">Anzeigen einer Warnung, wenn ein Benutzer eine VMSS bereitstellt, die an eine bestimmte (und nicht an die neueste) Imageversion angeheftet ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-627">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f6f7d-628">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-628">Cosmos DB</span></span>

* <span data-ttu-id="f6f7d-629">`az cosmosdb`: Befehl „exists“ zu Datenbank- und Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-629">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="f6f7d-630">Zulassen der Erstellung fester Sammlungen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-630">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="f6f7d-631">EventHub</span><span class="sxs-lookup"><span data-stu-id="f6f7d-631">EventHub</span></span>

* <span data-ttu-id="f6f7d-632">`az eventhubs namespace create` : Parameter für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-632">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-633">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-633">Extension</span></span>

* <span data-ttu-id="f6f7d-634">„--version“ hinzugefügt, um die Installation über eine bestimmte Version zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-634">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="f6f7d-635">CLI-Erweiterungen dürfen nun Pakete im Namespace „azure“ enthalten.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-635">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="f6f7d-636">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="f6f7d-636">Iot Hub</span></span>

* <span data-ttu-id="f6f7d-637">[BREAKING CHANGE] az iot hub job: Veraltete job-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-637">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-638">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-638">KeyVault</span></span>

* <span data-ttu-id="f6f7d-639">`az keyvault key import`: Unterstützt das Importieren aus Zeichenfolgen über zwei neue Parameter.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-639">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="f6f7d-640">Unterstützung der Ver- und Entschlüsselung von Zeichenfolgen/Bytes mit gespeicherten Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="f6f7d-640">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-641">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-641">Monitor</span></span>

* <span data-ttu-id="f6f7d-642">Unterstützung für „no wait“ bei der Clustererstellung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-642">Support no wait for cluster creation</span></span>
* <span data-ttu-id="f6f7d-643">`az monitor log-analytics workspace saved-search`: Unterstützung neuer Befehle für gespeicherte Suche</span><span class="sxs-lookup"><span data-stu-id="f6f7d-643">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-644">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-644">Network</span></span>

* <span data-ttu-id="f6f7d-645">`az network application-gateway address-pool update`: Hilfenachricht optimiert und Beispiele hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-645">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="f6f7d-646">`az network vnet create`: Unterstützung für das Argument „--nsg“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-646">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="f6f7d-647">`az network lb address-pool`: Unterstützung für das Erstellen eines Back-End-Pools des Lastenausgleichs mit Back-End-Adresse</span><span class="sxs-lookup"><span data-stu-id="f6f7d-647">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="f6f7d-648">`az network application-gateway address-pool`: Korrektur für das Argument „--add“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-648">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-649">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-649">RBAC</span></span>

* <span data-ttu-id="f6f7d-650">`az ad sp create-for-rabc`: Unterstützung von Namen mit Leerzeichen, Schrägstrich und umgekehrtem Schrägstrich</span><span class="sxs-lookup"><span data-stu-id="f6f7d-650">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="f6f7d-651">`az ad sp create-for-rbac`: Fehlermeldung optimiert, die angezeigt wird, wenn Benutzer einen ungültigen Bereich angeben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-651">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="f6f7d-652">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="f6f7d-652">Security</span></span>

* <span data-ttu-id="f6f7d-653">Befehle für Sicherheitsbewertungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-653">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-654">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-654">SQL</span></span>

* <span data-ttu-id="f6f7d-655">`az sql db ltr-policy/ltr-backup`: Aktualisieren/Anzeigen der Richtlinie zur langfristigen Aufbewahrung, Anzeigen/Löschen von Sicherungen zur langfristigen Aufbewahrung, Wiederherstellen von Sicherungen zur langfristigen Aufbewahrung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-655">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-656">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-656">Storage</span></span>

* <span data-ttu-id="f6f7d-657">Authentifizierungsproblem behoben, um das Abrufen eines Tokens für „--subscription“ zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-657">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="f6f7d-658">`az storage remove`: Problem Nr. 13459 behoben, um eine Ausnahme bei einem Vorgangsfehler auszulösen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-658">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="f6f7d-659">Probleme Nr. 13012, 13632 und 13657 behoben, um nicht verwendete Argumente für Befehle im Zusammenhang mit „generate-sas“ zu entfernen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-659">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="f6f7d-660">`az storage logging update`: Überprüfung für Protokollierungsversion hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-660">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="f6f7d-661">`az storage blob show`: Weitere Eigenschaften für Blob mit Track 2 SDK hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-661">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="f6f7d-662">Behebung Nr. 13708: Warnmeldung für Anmeldeinformationen optimiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-662">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="f6f7d-663">`az storage share-rm create/update`: Unterstützung für NFS-Protokoll und Root-Squash hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-663">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="f6f7d-664">`az storage account create`: Unterstützung für doppelte Verschlüsselung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-664">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="f6f7d-665">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: „--expiry“ und „--permissions“ als erforderlich festgelegt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-665">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="f6f7d-666">`az storage blob set-tier`: Migration zu Track 2, um das Festlegen der Aktivierungspriorität zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-666">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="f6f7d-667">2\. Juni 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-667">June 02, 2020</span></span>

<span data-ttu-id="f6f7d-668">Version 2.7.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-668">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-669">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-669">ACR</span></span>

* <span data-ttu-id="f6f7d-670">Tippfehler in einer Fehlermeldung der Tokenerstellung korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-670">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-671">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-671">AKS</span></span>

* <span data-ttu-id="f6f7d-672">Standard-VM-SKU in „Standard_D2s_v3“ geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-672">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="f6f7d-673">Erstellung der Rollenzuweisung für MSI-Cluster plus benutzerdefiniertes Subnetz korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-673">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-674">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-674">AppService</span></span>

* <span data-ttu-id="f6f7d-675">Fehlerbehebung Nr. 12739: Von „az appservice list-locations“ werden einige ungültige Standorte zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-675">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-676">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-676">ARM</span></span>

* <span data-ttu-id="f6f7d-677">`az deployment`: Fehlerbehebung Nr. 13159 der fehlerhaften JSON-Meldung nach dem Entfernen von Kommentaren und nach dem Komprimieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-677">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="f6f7d-678">`az resource tag`: Fehlerbehebung Nr. 13255 für das Markieren von Ressourcen mit dem Ressourcentyp `Microsoft.ContainerRegistry/registries/webhooks`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-678">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="f6f7d-679">Beispiele für das Ressourcenmodul verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-679">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="f6f7d-680">ARO</span><span class="sxs-lookup"><span data-stu-id="f6f7d-680">ARO</span></span>

* <span data-ttu-id="f6f7d-681">CLIError in das richtige Flag für „--worker-vm-disk-size-gb“ geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-681">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="f6f7d-682">EventHub</span><span class="sxs-lookup"><span data-stu-id="f6f7d-682">EventHub</span></span>

* <span data-ttu-id="f6f7d-683">Fehlerbehebung Nr. 12406: „intervalInSeconds“ wird von Argument „--capture-interval“ nicht aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-683">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-684">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-684">HDInsight</span></span>

* <span data-ttu-id="f6f7d-685">„get_json_object“ in „shell_safe_json_parse“ geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-685">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-686">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-686">Monitor</span></span>

* <span data-ttu-id="f6f7d-687">`az monitor metrics alert`: Verschiedene Hilfemeldungen optimiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-687">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="f6f7d-688">`az monitor diagnostic-settings create`: Unterstützung für das Argument „--export-to-resource-specific“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-688">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="f6f7d-689">Unterstützung für die Wiederherstellung von LA-Arbeitsbereichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-689">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-690">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-690">Network</span></span>

* <span data-ttu-id="f6f7d-691">`az network dns zone`: Unterstützung des Bindestrichs (-)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-691">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="f6f7d-692">`az network vpn-connection ipsec-policy`: „--sa-lifetime“ und „--sa-max-size“ im Beispiel in höhere Werte geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-692">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="f6f7d-693">Netzwerk auf 2020-04-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-693">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="f6f7d-694">`az network private-endpoint-connection`: Unterstützung von Event Grid</span><span class="sxs-lookup"><span data-stu-id="f6f7d-694">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="f6f7d-695">`az network express-route list-route-tables`: Fehler behoben, der dazu führte, dass Routen nicht als Tabelle aufgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-695">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="f6f7d-696">Verpackung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-696">Packaging</span></span>

* <span data-ttu-id="f6f7d-697">Ubuntu-Paket (Focal) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-697">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-698">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-698">RBAC</span></span>

* <span data-ttu-id="f6f7d-699">`az ad sp credential reset`: Erstellung von Anmeldeinformationen geändert, um problematische Sonderzeichen zu vermeiden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-699">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="f6f7d-700">Redis</span><span class="sxs-lookup"><span data-stu-id="f6f7d-700">Redis</span></span>

* <span data-ttu-id="f6f7d-701">Fehlerbehebung Nr. 13529: Dokumentation des Parameters „enable_non_ssl_port“ geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-701">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-702">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-702">Storage</span></span>

* <span data-ttu-id="f6f7d-703">`az storage copy`: Parameter `--follow-symlinks` zur Unterstützung von symbolischen Verknüpfungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-703">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="f6f7d-704">Lokaler Kontext für Speicherkonto aktiviert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-704">Enable local context for storage account</span></span>
* <span data-ttu-id="f6f7d-705">`az storage logging`: Fehlerbehebung Nr. 11969: Fehlermeldung optimiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-705">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="f6f7d-706">19. Mai 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-706">May 19, 2020</span></span>

<span data-ttu-id="f6f7d-707">Version 2.6.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-707">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-708">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-708">ACR</span></span>

* <span data-ttu-id="f6f7d-709">Standardtimeout von fünf Minuten für jede an ACR gesendete Anforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-709">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="f6f7d-710">Unterstützung für das Deaktivieren des Zugriffs auf das öffentliche Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-710">Support disable public network access</span></span>
* <span data-ttu-id="f6f7d-711">`az acr token create`: Argument „--days“ verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-711">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="f6f7d-712">`az acr import`: Akzeptiert Werte für das Argument „--source“, bei denen der Servername einen Anmeldenamen enthält (mittels clientseitiger Korrektur)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-712">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-713">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-713">ACS</span></span>

* <span data-ttu-id="f6f7d-714">Fehlerbehebung: Felderbereinigung für Felder entfernt, die nicht mehr vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="f6f7d-714">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-715">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-715">AKS</span></span>

* <span data-ttu-id="f6f7d-716">Hilfekontext des Befehls „uptime-sla“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-716">Update uptime-sla command help context</span></span>
* <span data-ttu-id="f6f7d-717">Bereichsüberprüfung für die Aktualisierung der Mindestanzahl für die Autoskalierung entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-717">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="f6f7d-718">Hotfix, der bewirkt, dass bei der CLI kein Fehler auftritt, wenn der Benutzer nur das Windows-Kennwort angibt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-718">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-719">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-719">AMS</span></span>

* <span data-ttu-id="f6f7d-720">`az ams transform create`: Funktion zum Erstellen einer Transformation mit einer FaceDetector-Voreinstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-720">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="f6f7d-721">`az ams content-key-policy create` : Funktion zum Erstellen einer FairPlay-Inhaltsschlüsselrichtlinie mit einer Konfiguration für die Offlinemiete hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-721">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="f6f7d-722">AppConfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-722">AppConfig</span></span>

* <span data-ttu-id="f6f7d-723">Fehlerbehebung für die Schlüsselauflistungswerte mit Feldern</span><span class="sxs-lookup"><span data-stu-id="f6f7d-723">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-724">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-724">AppService</span></span>

* <span data-ttu-id="f6f7d-725">`az functionapp create`: AzureWebJobsDashboard wird nur festgelegt, wenn AppInsights deaktiviert ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-725">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="f6f7d-726">Fehlerbehebung Nr. 10664: VNET-Integration – Standortüberprüfungsfehler und Fehlerbehebung Nr. 13257: Fehler bei „az webapp up“, wenn eine Ressourcengruppe erstellt werden muss</span><span class="sxs-lookup"><span data-stu-id="f6f7d-726">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="f6f7d-727">`az webapp|functionapp config ssl import`: Ressourcengruppenübergreifende Suche des Schlüsseltresors im Abonnement und verbesserte Hilfe und Beispiele</span><span class="sxs-lookup"><span data-stu-id="f6f7d-727">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="f6f7d-728">Lokaler Kontext für App Service integriert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-728">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-729">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-729">ARM</span></span>

* <span data-ttu-id="f6f7d-730">`az deployment`: Problem behoben, das dazu führte, dass templateLink beim Bereitstellen oder Überprüfen von „template-uri“ nicht zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-730">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="f6f7d-731">`az deployment`: Problem behoben, das dazu führte, dass speziell codierte Zeichen von der Bereitstellung/Überprüfung nicht unterstützt wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-731">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="f6f7d-732">`az deployment sub/group what-if`: Arrayausrichtung und Fehlerbehandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-732">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="f6f7d-733">`az deployment operation`: Veraltete Informationen angepasst</span><span class="sxs-lookup"><span data-stu-id="f6f7d-733">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="f6f7d-734">ARO</span><span class="sxs-lookup"><span data-stu-id="f6f7d-734">ARO</span></span>

* <span data-ttu-id="f6f7d-735">Beispiele zu folgenden Befehlen hinzugefügt: az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="f6f7d-735">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="f6f7d-736">Funktion „generate_random_id“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-736">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-737">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-737">Backup</span></span>

* <span data-ttu-id="f6f7d-738">FriendlyName im Befehl zum Aktivieren des Schutzes für AzureFileShare zulässig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-738">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="f6f7d-739">Korrektur im IaasVM-Befehl „restore-disks“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-739">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="f6f7d-740">BackupManagementType „MAB“ zum Befehl zum Auflisten der Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-740">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="f6f7d-741">Unterstützung für die Wiederholung des Richtlinienupdates für fehlerhafte Elemente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-741">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="f6f7d-742">Funktion zum Fortsetzen des Schutzes für virtuelle Azure-Computer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-742">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="f6f7d-743">Unterstützung zum Angeben der Ressourcengruppe zum Speichern von instantRP beim Erstellen oder Ändern der Richtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-743">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="f6f7d-744">CI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-744">CI</span></span>

* <span data-ttu-id="f6f7d-745">Unterstützung für flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-745">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-746">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-746">Compute</span></span>

* <span data-ttu-id="f6f7d-747">Neuer Befehl: az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="f6f7d-747">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="f6f7d-748">`az vm list-skus`: Verhalten von „--zone“aktualisiert. Jetzt werden alle SKU-Typen zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-748">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-749">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-749">Core</span></span>

* <span data-ttu-id="f6f7d-750">Aktivierungsstatus aus dem lokalen Kontext für globale Benutzerebene aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-750">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-751">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-751">Extension</span></span>

* <span data-ttu-id="f6f7d-752">`az extension add`: „--system“ hinzugefügt, um die Installation von Erweiterungen in einem Systempfad zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-752">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="f6f7d-753">Unterstützung für „.egg-info“ zum Speichern der Metadaten für die Radtyperweiterung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-753">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-754">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-754">IoT</span></span>

* <span data-ttu-id="f6f7d-755">`az iot`: Nachricht des IoT-Befehlsmoduls mit dem Hinweis auf die Erweiterung für die erste Ausführung aktualisiert, sodass sie anstelle der veralteten ID die korrekte moderne ID (`azure-iot`) enthält</span><span class="sxs-lookup"><span data-stu-id="f6f7d-755">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="f6f7d-756">IoT Hub</span><span class="sxs-lookup"><span data-stu-id="f6f7d-756">IoT Hub</span></span>

* <span data-ttu-id="f6f7d-757">Unterstützung für API- und Netzwerkisolationsbefehle für 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="f6f7d-757">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="f6f7d-758">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="f6f7d-758">NetAppFiles</span></span>

* <span data-ttu-id="f6f7d-759">`az volume create`: „snapshot-id“ als Parameter zum Erstellen eines Volumes hinzugefügt. Ermöglicht Benutzern das Erstellen eines Volumes auf der Grundlage einer vorhandenen Momentaufnahme.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-759">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-760">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-760">Network</span></span>

* <span data-ttu-id="f6f7d-761">TTL-Wert korrigiert, der für „dns add-record“ unbeabsichtigt geändert wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-761">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="f6f7d-762">`az network public-ip create`: Kunden über einen bevorstehenden Breaking Change informiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-762">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="f6f7d-763">Unterstützung von generischen Befehlen für Private Link-Szenario</span><span class="sxs-lookup"><span data-stu-id="f6f7d-763">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="f6f7d-764">`az network private-endpoint-connection`: Unterstützung für MySQL-, Postgres- und MariaDB-Typen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-764">`az network private-endpoint-connection`: Support mysql, postgres and mariadb types</span></span>
* <span data-ttu-id="f6f7d-765">`az network private-endpoint-connection`: Unterstützung von CosmosDB-Typen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-765">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="f6f7d-766">`az network private-endpoint`: „--group-ids“ und Umleitung an „--group-id“ als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-766">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="f6f7d-767">Output</span><span class="sxs-lookup"><span data-stu-id="f6f7d-767">Output</span></span>

* <span data-ttu-id="f6f7d-768">Anzeigen der Updateanweisung bei der Suche, beim Feedback und in „--help“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-768">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="f6f7d-769">Verpackung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-769">Packaging</span></span>

* <span data-ttu-id="f6f7d-770">Erstellen von MSI-/Homebrew-Paketen mit Abhängigkeiten, die aus „requirements.txt“ aufgelöst werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-770">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-771">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-771">RBAC</span></span>

* <span data-ttu-id="f6f7d-772">`az ad sp credential reset`: Erstellung unsicherer Anmeldeinformationen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-772">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-773">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-773">Storage</span></span>

* <span data-ttu-id="f6f7d-774">`az storage account file-service-properties update/show`: Unterstützung für Dateieigenschaften für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-774">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="f6f7d-775">`az storage container create`: Fehlerbehebung Nr. 13373 durch Hinzufügen eines Validierungssteuerelements für öffentlichen Zugriff</span><span class="sxs-lookup"><span data-stu-id="f6f7d-775">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="f6f7d-776">Unterstützung für ADLS Gen2 (track2) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-776">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="f6f7d-777">`az storage blob sync`: Unterstützung für `--connection-string`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-777">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="f6f7d-778">`az storage blob sync`: Falsche Fehlermeldung korrigiert, die angezeigt wird, wenn der Installationsspeicherort von „azcopy“ nicht gefunden wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-778">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="f6f7d-779">30. April 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-779">April 30, 2020</span></span>

<span data-ttu-id="f6f7d-780">Version 2.5.1</span><span class="sxs-lookup"><span data-stu-id="f6f7d-780">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-781">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-781">ACR</span></span>

* <span data-ttu-id="f6f7d-782">`az acr check-health`: „DOCKER_PULL_ERROR“ unter Windows behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-782">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-783">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-783">Compute</span></span>

* <span data-ttu-id="f6f7d-784">`az vm list-ip-addresses`: Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-784">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="f6f7d-785">Fehler behoben, der bei der VM-Erstellung auftrat, wenn „endpoint_vm_image_alias_doc“ im Cloudprofil nicht festgelegt war</span><span class="sxs-lookup"><span data-stu-id="f6f7d-785">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="f6f7d-786">`az vmss create`: „--os-disk-size-gb“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-786">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f6f7d-787">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-787">Cosmos DB</span></span>

* <span data-ttu-id="f6f7d-788">`az cosmosdb create/update`: Unterstützung für „--enable-public-network“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-788">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-789">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-789">Extension</span></span>

* <span data-ttu-id="f6f7d-790">Laden der falschen Metadaten für die Radtyperweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-790">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="f6f7d-791">Verpackung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-791">Packaging</span></span>

* <span data-ttu-id="f6f7d-792">Az-Skript für Git Bash/Cygwin unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-792">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-793">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-793">SQL</span></span>

* <span data-ttu-id="f6f7d-794">`az sql instance-pool`: Befehlsgruppe für Instanzpools hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-794">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-795">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-795">Storage</span></span>

* <span data-ttu-id="f6f7d-796">Paket „azure-multiapi-storage“ auf 0.3.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-796">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="f6f7d-797">Unterstützung von GZRS für Speicherkontoerstellung und -aktualisierung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-797">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="f6f7d-798">`az storage account failover`: Unterstützung für das Failover von GRS/GZRS-Speicherkonten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-798">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="f6f7d-799">`az storage blob upload`: Parameter „--encryption-scope“ hinzugefügt, um die Angabe von Informationen zum Verschlüsselungsbereich zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-799">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="f6f7d-800">28. April 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-800">April 28, 2020</span></span>

<span data-ttu-id="f6f7d-801">Version 2.5.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-801">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-802">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-802">ACS</span></span>

* <span data-ttu-id="f6f7d-803">[BREAKING CHANGE] az openshift create: Parameter „--vnet-peer“ entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-803">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="f6f7d-804">`az openshift create`: Flags zur Unterstützung des privaten Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-804">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="f6f7d-805">`az openshift`: Upgrade auf API-Version `2019-10-27-preview`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-805">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="f6f7d-806">`az openshift`: Befehl `update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-806">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-807">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-807">AKS</span></span>

* <span data-ttu-id="f6f7d-808">`az aks create`: Unterstützung für Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-808">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-809">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-809">AppService</span></span>

* <span data-ttu-id="f6f7d-810">`az webapp deployment source config-zip`: Energiesparmodus nach „request.get()“ entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-810">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-811">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-811">ARM</span></span>

* <span data-ttu-id="f6f7d-812">Was-wäre-wenn-Befehle für Vorlagenbereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-812">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="f6f7d-813">ARO</span><span class="sxs-lookup"><span data-stu-id="f6f7d-813">ARO</span></span>

* <span data-ttu-id="f6f7d-814">`az aro`: Tabellenausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-814">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="f6f7d-815">CI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-815">CI</span></span>

* <span data-ttu-id="f6f7d-816">pytest integriert und nose für Automatisierungstest als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-816">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-817">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-817">Compute</span></span>

* <span data-ttu-id="f6f7d-818">`az vmss disk detach`: Datenträgerfehler „NoneType“ behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-818">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="f6f7d-819">`az vm availability-set list`: Unterstützung zum Anzeigen der VM-Liste</span><span class="sxs-lookup"><span data-stu-id="f6f7d-819">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="f6f7d-820">`az vm list-skus`: Anzeigeproblem des Tabellenformats behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-820">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-821">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-821">KeyVault</span></span>

* <span data-ttu-id="f6f7d-822">Neuer Parameter `--enable-rbac-authorization` bei Erstellung oder Aktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-822">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-823">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-823">Monitor</span></span>

* <span data-ttu-id="f6f7d-824">Unterstützung der CMK-Features für LA-Cluster</span><span class="sxs-lookup"><span data-stu-id="f6f7d-824">Support LA cluster CMK features</span></span>
* <span data-ttu-id="f6f7d-825">`az monitor log-analytics workspace linked-storage`: Unterstützung für BYOS-Features</span><span class="sxs-lookup"><span data-stu-id="f6f7d-825">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-826">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-826">Network</span></span>

* <span data-ttu-id="f6f7d-827">`az network security-partner`: Unterstützung des Sicherheitspartneranbieters</span><span class="sxs-lookup"><span data-stu-id="f6f7d-827">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="f6f7d-828">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-828">Privatedns</span></span>

* <span data-ttu-id="f6f7d-829">Funktion in privater DNS-Zone zum Importieren der Exportzonendatei hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-829">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="f6f7d-830">21. April 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-830">April 21, 2020</span></span>

<span data-ttu-id="f6f7d-831">Version 2.4.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-831">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-832">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-832">ACR</span></span>

* <span data-ttu-id="f6f7d-833">`az acr run --cmd`: Deaktivieren der Arbeitsverzeichnisaußerkraftsetzung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-833">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="f6f7d-834">Unterstützung dedizierter Datenendpunkte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-834">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-835">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-835">AKS</span></span>

* <span data-ttu-id="f6f7d-836">`az aks list -o table` sollte „privateFqdn“ als FQDN für private Cluster anzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-836">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="f6f7d-837">„--uptime-sla“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-837">Add --uptime-sla</span></span>
* <span data-ttu-id="f6f7d-838">containerservice-Paket aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-838">Update containerservice package</span></span>
* <span data-ttu-id="f6f7d-839">Unterstützung für öffentliche IP-Adressen für Knoten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-839">Add node public IP support</span></span>
* <span data-ttu-id="f6f7d-840">Tippfehler im help-Befehl korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-840">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="f6f7d-841">AppConfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-841">AppConfig</span></span>

* <span data-ttu-id="f6f7d-842">Schlüsseltresorverweis für die Befehle „kv list“ und „kv export“ aufgelöst</span><span class="sxs-lookup"><span data-stu-id="f6f7d-842">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="f6f7d-843">Fehlerbehebung für die Werte für das Auflisten von Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="f6f7d-843">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-844">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-844">AppService</span></span>

* <span data-ttu-id="f6f7d-845">`az functionapp create`: Vorgehensweise zum Festlegen von „linuxFxVersion“ für Linux-Funktions-Apps (.NET) geändert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-845">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="f6f7d-846">Dadurch sollte der Fehler behoben sein, der die Erstellung von Linux-Verbrauchs-Apps (.NET) verhindert hat.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-846">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="f6f7d-847">[BREAKING CHANGE] `az webapp create`: Korrektur vorgenommen, um vorhandene App-Einstellungen (AppSettings) für „az webapp create“ beizubehalten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-847">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="f6f7d-848">[BREAKING CHANGE] `az webapp up`: Korrektur vorgenommen, um bei Verwendung des Flags „-g“ eine RG für den Befehl „az webapp up“ zu erstellen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-848">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="f6f7d-849">[BREAKING CHANGE] `az webapp config`: Korrektur vorgenommen, um Werte für Nicht-JSON-Ausgaben mit „az webapp config connection-string list“ anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-849">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-850">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-850">ARM</span></span>

* <span data-ttu-id="f6f7d-851">`az deployment create/validate`: Parameter `--no-prompt` hinzugefügt, um das Überspringen der Eingabeaufforderung für fehlende Parameter für die ARM-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-851">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="f6f7d-852">`az deployment group/mg/sub/tenant validate`: Unterstützung von Kommentaren in der Bereitstellungsparameterdatei</span><span class="sxs-lookup"><span data-stu-id="f6f7d-852">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="f6f7d-853">`az deployment`: `is_preview` für Parameter `--handle-extended-json-format` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-853">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="f6f7d-854">`az deployment group/mg/sub/tenant cancel`: Unterstützung für den Abbruch der Bereitstellung für ARM-Vorlagen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-854">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="f6f7d-855">`az deployment group/mg/sub/tenant validate`: Fehlermeldung bei einem Fehler der Bereitstellungsüberprüfung verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-855">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="f6f7d-856">`az deployment-scripts`: Neue Befehle für DeploymentScripts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-856">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="f6f7d-857">`az resource tag`: Parameter `--is-incremental` hinzugefügt, um das inkrementelle Hinzufügen von Tags zur Ressource zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-857">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="f6f7d-858">ARO</span><span class="sxs-lookup"><span data-stu-id="f6f7d-858">ARO</span></span>

* <span data-ttu-id="f6f7d-859">`az aro`:  ARO-Befehlsmodul von Azure RedHat OpenShift V4 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-859">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-860">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-860">Batch</span></span>

* <span data-ttu-id="f6f7d-861">Batch-API aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-861">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-862">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-862">Compute</span></span>

* <span data-ttu-id="f6f7d-863">`az sig image-version create`: Speicherkontotyp „Premium_LRS“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-863">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="f6f7d-864">`az vmss update`: Problem behoben, das beim Aktualisieren der Beendigungsbenachrichtigung auftrat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-864">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="f6f7d-865">`az vm/vmss create`: Unterstützung für spezialisierte Imageversion hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-865">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="f6f7d-866">SIG-API-Version 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="f6f7d-866">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="f6f7d-867">`az sig image-version create`: „--target-region-encryption“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-867">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="f6f7d-868">Fehler bei Serientestausführung behoben, der auf die Duplizierung des Schlüsseltresornamens im globalen In-Memory-Cache zurückzuführen war.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-868">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6f7d-869">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-869">CosmosDB</span></span>

* <span data-ttu-id="f6f7d-870">Unterstützung für `az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-870">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="f6f7d-871">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f6f7d-871">IoT Central</span></span>

* <span data-ttu-id="f6f7d-872">`az iotcentral` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-872">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="f6f7d-873">Befehlsmodul `az iot central` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-873">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-874">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-874">Monitor</span></span>

* <span data-ttu-id="f6f7d-875">Unterstützung eines Private Link-Szenarios für die Überwachung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-875">Support private link scenario for monitor</span></span>
* <span data-ttu-id="f6f7d-876">Falsche Simulationsmethode in „test_monitor_general_operations.py“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-876">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-877">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-877">Network</span></span>

* <span data-ttu-id="f6f7d-878">SKU für den Befehl zur Aktualisierung der öffentlichen IP-Adresse als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-878">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="f6f7d-879">`az network private-endpoint`: Unterstützung für private DNS-Zonengruppe</span><span class="sxs-lookup"><span data-stu-id="f6f7d-879">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="f6f7d-880">Feature für lokalen Kontext für VNET-/Subnetzparameter aktiviert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-880">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="f6f7d-881">Falsches Verwendungsbeispiel in „test_nw_flow_log_delete“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-881">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="f6f7d-882">Verpackung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-882">Packaging</span></span>

* <span data-ttu-id="f6f7d-883">Unterstützung für Ubuntu-/Disco-Paket eingestellt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-883">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-884">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-884">RBAC</span></span>

* <span data-ttu-id="f6f7d-885">`az ad app create/update`: Unterstützung von „--optional-claims“ als Parameter</span><span class="sxs-lookup"><span data-stu-id="f6f7d-885">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-886">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-886">RDBMS</span></span>

* <span data-ttu-id="f6f7d-887">Azure Active Directory-Administratorbefehle für PostgreSQL und MySQL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-887">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f6f7d-888">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6f7d-888">Service Fabric</span></span>

* <span data-ttu-id="f6f7d-889">Fehlerbehebung Nr. 12891: `az sf application update --application-parameters` entfernt alte Parameter, die nicht in der Anforderung enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-889">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="f6f7d-890">Fehlerbehebung Nr. 12470: az sf create cluster: Fehler im Zusammenhang mit der Dauerhaftigkeit und Zuverlässigkeit von Updates sowie im Zusammenhang mit der codebasierten Suche der VMSS unter Angabe eines bestimmten Knotentypnamens behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-890">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-891">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-891">SQL</span></span>

* <span data-ttu-id="f6f7d-892">`az sql mi op list`, `az sql mi op get`, `az sql mi op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-892">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="f6f7d-893">`az sql midb`: Aktualisieren/Anzeigen der Richtlinie zur langfristigen Aufbewahrung, Anzeigen/Löschen von Sicherungen zur langfristigen Aufbewahrung, Wiederherstellen von Sicherungen zur langfristigen Aufbewahrung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-893">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-894">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-894">Storage</span></span>

* <span data-ttu-id="f6f7d-895">„azure-mgmt-storage“ auf 9.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-895">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="f6f7d-896">`az storage logging off`: Unterstützung für das Ausschalten der Protokollierung für ein Speicherkonto</span><span class="sxs-lookup"><span data-stu-id="f6f7d-896">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="f6f7d-897">`az storage account update`: Automatische Rotation von Schlüsseln für CMK aktiviert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-897">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="f6f7d-898">`az storage account encryption-scope create/update/list/show`: Unterstützung zum Anpassen des Verschlüsselungsbereichs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-898">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="f6f7d-899">`az storage container create`: „--default-encryption-scope“ und „--deny-encryption-scope-override“ hinzugefügt, um den Verschlüsselungsbereich für die Containerebene festzulegen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-899">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="f6f7d-900">Umfrage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-900">Survey</span></span>

* <span data-ttu-id="f6f7d-901">Switch zum Deaktivieren des Umfragelinks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-901">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="f6f7d-902">01. April 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-902">April 01, 2020</span></span>

<span data-ttu-id="f6f7d-903">Version 2.3.1</span><span class="sxs-lookup"><span data-stu-id="f6f7d-903">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-904">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-904">ACR</span></span>

* <span data-ttu-id="f6f7d-905">Falsche Version von „azure-mgmt-containerregistry“ für Linux korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-905">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-906">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-906">Profile</span></span>

* <span data-ttu-id="f6f7d-907">az login: Anmeldefehler behoben, der auftrat, wenn nicht das Cloudprofil `latest` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-907">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="f6f7d-908">31. März 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-908">March 31, 2020</span></span>

<span data-ttu-id="f6f7d-909">Version 2.3.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-909">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-910">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-910">ACR</span></span>

* <span data-ttu-id="f6f7d-911">„az acr task update“: NULL-Zeiger-Ausnahme</span><span class="sxs-lookup"><span data-stu-id="f6f7d-911">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="f6f7d-912">`az acr import`: Hilfe und Fehlermeldung geändert, um die Verwendung von „--source“ und „--registry“ zu verdeutlichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-912">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="f6f7d-913">Überprüfung für das Argument „registry_name“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-913">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="f6f7d-914">`az acr login`: Vorschauflag für „--expose-token“ entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-914">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="f6f7d-915">[BREAKING CHANGE] Branch-Parameter „az acr task create/update“ entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-915">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="f6f7d-916">„az acr task update“: Kunde kann nun Kontext, Git-Token und/oder Trigger einzeln aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-916">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="f6f7d-917">„az acr agentpool“: Neues Feature</span><span class="sxs-lookup"><span data-stu-id="f6f7d-917">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-918">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-918">AKS</span></span>

* <span data-ttu-id="f6f7d-919">„apiServerAccessProfile“ bei der Aktualisierung von „--api-server-authorized-ip-ranges“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-919">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="f6f7d-920">aks update: Überschreibung ausgehender IP-Adressen mit Eingabewerten bei der Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-920">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="f6f7d-921">Keine SPN-Erstellung für MSI-Cluster sowie Unterstützung der Anfügung von ACR an MSI-Cluster</span><span class="sxs-lookup"><span data-stu-id="f6f7d-921">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-922">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-922">AMS</span></span>

* <span data-ttu-id="f6f7d-923">Fix 12469: Hinzufügen von „content-key-policy“ für Fairplay aufgrund von Problemen mit dem Parameter „ask“ nicht erfolgreich</span><span class="sxs-lookup"><span data-stu-id="f6f7d-923">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="f6f7d-924">AppConfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-924">AppConfig</span></span>

* <span data-ttu-id="f6f7d-925">„--skip-keyvault“ für „kv export“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-925">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-926">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-926">AppService</span></span>

* <span data-ttu-id="f6f7d-927">Fix 12509: Tag für „az webapp up“ standardmäßig entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-927">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="f6f7d-928">az functionapp create: Hilfemenü für „--runtime-version“ aktualisiert und Warnung hinzugefügt, wenn der Benutzer „--runtime-version“ für .NET angibt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-928">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="f6f7d-929">az functionapp create: Methode zum Festlegen von „javaVersion“ für Windows-Funktions-Apps aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-929">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-930">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-930">ARM</span></span>

* <span data-ttu-id="f6f7d-931">az deployment create/validate: Standardmäßige Verwendung von „--handle-extended-json-format“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-931">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="f6f7d-932">az lock create: Beispiele für die Erstellung einer Unterressource in der Hilfedokumentation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-932">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="f6f7d-933">az deployment {group/mg/sub/tenant} list: Unterstützung der provisioningState-Filterung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-933">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="f6f7d-934">az deployment: Analysefehler für Kommentar unter letztem Argument behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-934">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-935">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-935">Backup</span></span>

* <span data-ttu-id="f6f7d-936">Mehrere Dateiwiederherstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-936">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="f6f7d-937">Unterstützung der ausschließlichen Sicherung von Betriebssystemdatenträgern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-937">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="f6f7d-938">Parameter „restore-as-unmanaged-disk“ für die Angabe einer nicht verwalteten Wiederherstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-938">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-939">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-939">Compute</span></span>

* <span data-ttu-id="f6f7d-940">az vm create: Option „NONE“ von „--nsg-rule“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-940">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="f6f7d-941">az vmss create/update: Vorschautag für automatische VMSS-Reparaturen entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-941">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="f6f7d-942">az vm update: Unterstützung von „--workspace“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-942">az vm update: Support --workspace</span></span>
* <span data-ttu-id="f6f7d-943">Fehler im VirtualMachineScaleSetExtension-Initialisierungscode behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-943">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="f6f7d-944">Upgrade der VMAccessAgent-Version auf 2.4 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-944">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="f6f7d-945">az vmss set-orchestration-service-state: Unterstützung zum Festlegen des Orchestrierungdienstzustands für VMSS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-945">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="f6f7d-946">Upgrade der Datenträger-API-Version auf 2019-11-01 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-946">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="f6f7d-947">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="f6f7d-947">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f6f7d-948">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-948">Cosmos DB</span></span>

* <span data-ttu-id="f6f7d-949">Fehlende Option „--type“ für Veraltungsumleitungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-949">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="f6f7d-950">Docker</span><span class="sxs-lookup"><span data-stu-id="f6f7d-950">Docker</span></span>

* <span data-ttu-id="f6f7d-951">Update auf Alpine 3.11 und Python 3.6.10 durchgeführt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-951">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-952">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-952">Extension</span></span>

* <span data-ttu-id="f6f7d-953">Laden von Erweiterungen im Systempfad mittels Paketen ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-953">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-954">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-954">HDInsight</span></span>

* <span data-ttu-id="f6f7d-955">(az hdinsight create:) Unterstützung der Angabe der unterstützten TLS-Mindestversion durch Kunden unter Verwendung des Parameters `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-955">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="f6f7d-956">Zulässiger Wert: 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="f6f7d-956">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-957">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-957">IoT</span></span>

* <span data-ttu-id="f6f7d-958">Codebesitzer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-958">Add codeowner</span></span>
* <span data-ttu-id="f6f7d-959">az iot hub create: Standard-SKU von F1 in S1 geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-959">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="f6f7d-960">iot hub: Unterstützung von „IotHub“ im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-960">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="f6f7d-961">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="f6f7d-961">IoTCentral</span></span>

* <span data-ttu-id="f6f7d-962">Fehlerdetails sowie Standardanwendungsvorlage und Aufforderungsmeldung aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-962">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-963">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-963">KeyVault</span></span>

* <span data-ttu-id="f6f7d-964">Unterstützung von Zertifikatsicherung/-wiederherstellung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-964">Support certificate backup/restore</span></span>
* <span data-ttu-id="f6f7d-965">keyvault create/update: Unterstützung von „--retention-days“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-965">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="f6f7d-966">Keine Anzeige von verwalteten Schlüsseln/Geheimnissen bei der Auflistung mehr</span><span class="sxs-lookup"><span data-stu-id="f6f7d-966">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="f6f7d-967">az keyvault create: Unterstützung von `--network-acls`, `--network-acls-ips` und `--network-acls-vnets` zur Angabe von Netzwerkregeln bei der Tresorerstellung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-967">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="f6f7d-968">Sperre</span><span class="sxs-lookup"><span data-stu-id="f6f7d-968">Lock</span></span>

* <span data-ttu-id="f6f7d-969">Fehlerbehebung für „az lock delete“: „az lock delete“ funktioniert für „Microsoft.DocumentDB“ nicht.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-969">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-970">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-970">Monitor</span></span>

* <span data-ttu-id="f6f7d-971">az monitor clone: Unterstützung des Klonens von Metrikregeln zwischen Ressourcen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-971">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="f6f7d-972">Fix IcM179210086: Erstellung einer benutzerdefinierten Metrikwarnung für die Application Insights-Metrik nicht möglich</span><span class="sxs-lookup"><span data-stu-id="f6f7d-972">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="f6f7d-973">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="f6f7d-973">NetAppFiles</span></span>

* <span data-ttu-id="f6f7d-974">az volume create: Datenschutzvolumes zum Hinzufügen von Replikationsvorgängen zugelassen: Genehmigen, Aussetzen, Fortsetzen, Status, Entfernen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-974">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-975">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-975">Network</span></span>

* <span data-ttu-id="f6f7d-976">az network application-gateway waf-policy managed-rule rule-set add: Unterstützung von „ Microsoft_BotManagerRuleSet“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-976">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="f6f7d-977">network watcher flow-log show: Falsche Veraltungsinformationen behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-977">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="f6f7d-978">Unterstützung von Hostnamen im Application Gateway-Listener</span><span class="sxs-lookup"><span data-stu-id="f6f7d-978">support host names in application gateway listener</span></span>
* <span data-ttu-id="f6f7d-979">az network nat gateway: Unterstützung der Erstellung einer leeren Ressource ohne öffentliche IP-Adresse oder Präfix für öffentliche IP-Adressen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-979">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="f6f7d-980">Unterstützung der VPN-Gateway-Generierung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-980">Support vpn gateway generation</span></span>
* <span data-ttu-id="f6f7d-981">Unterstützung von `--if-none-match` in `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-981">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="f6f7d-982">Verpackung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-982">Packaging</span></span>

* <span data-ttu-id="f6f7d-983">Unterstützung von Python 3.5 eingestellt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-983">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-984">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-984">Profile</span></span>

* <span data-ttu-id="f6f7d-985">az login: Warnung für MFA-Fehler</span><span class="sxs-lookup"><span data-stu-id="f6f7d-985">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-986">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-986">RDBMS</span></span>

* <span data-ttu-id="f6f7d-987">Befehle zur Verwaltung von Verschlüsselungsschlüsseln für Serverdaten für PostgreSQL und MySQL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-987">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="f6f7d-988">10. März 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-988">March 10, 2020</span></span>

<span data-ttu-id="f6f7d-989">Version 2.2.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-989">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-990">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-990">ACR</span></span>

* <span data-ttu-id="f6f7d-991">Fix: `az acr login` löst fälschlicherweise Fehler aus</span><span class="sxs-lookup"><span data-stu-id="f6f7d-991">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="f6f7d-992">Neuer Befehl `az acr helm install-cli` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-992">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="f6f7d-993">Privater Link und CMK-Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-993">Add private link and CMK support</span></span>
* <span data-ttu-id="f6f7d-994">Befehl „private-link-resource list“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-994">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-995">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-995">AKS</span></span>

* <span data-ttu-id="f6f7d-996">Durchsuchen von AKS in Cloud-Shell korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-996">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="f6f7d-997">az aks: NoneType-Fehler beim Überwachen von „addon“ und „agentpool“ behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-997">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="f6f7d-998">„--nodepool-tags“ zum Knotenpool beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-998">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="f6f7d-999">„--tags“ beim Hinzufügen oder Aktualisieren eines Knotenpool in einem Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-999">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="f6f7d-1000">aks create: `--enable-private-cluster` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1000">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="f6f7d-1001">„--nodepool-labels“ beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1001">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="f6f7d-1002">„--labels“ beim Hinzufügen eines neuen Knotenpools zu einem Azure-Kubernetes-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1002">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="f6f7d-1003">Fehlender Schrägstrich (/) in der Dashboard-URL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1003">add missing / in the dashboard url</span></span>
* <span data-ttu-id="f6f7d-1004">Unterstützung der Erstellung von AKS-Clustern, sodass verwaltete Identitäten möglich sind</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1004">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="f6f7d-1005">az aks: Überprüfen, ob das Netzwerk-Plug-In entweder „azure“ oder „kubenet“ ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1005">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="f6f7d-1006">az aks: Unterstützung für AAD-Sitzungsschlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1006">az aks: Add aad session key support</span></span>
* <span data-ttu-id="f6f7d-1007">[BREAKING CHANGE] az aks: Unterstützung von MSI-Änderungen für GF und BF für omsagent (Containerüberwachung)(#1)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1007">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="f6f7d-1008">az aks use-dev-spaces: Endpunkt-Typoption zum Befehl „use-dev-spaces“, hinzugefügt, um den auf einem Azure Dev Spaces-Controller erstellten Endpunkt anzupassen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1008">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="f6f7d-1009">AppConfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1009">AppConfig</span></span>

* <span data-ttu-id="f6f7d-1010">Verwendung von „kv set“ entsperrt, um Schlüsseltresorverweis und -funktion hinzuzufügen …</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1010">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1011">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1011">AppService</span></span>

* <span data-ttu-id="f6f7d-1012">az webapp create : Beheben eines Problems beim Ausführen des Befehls mit „--runtime“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1012">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="f6f7d-1013">az functionapp deployment source config-zip: Fehlermeldung hinzugefügt, wenn der Ressourcengruppen- oder Funktionsname ungültig oder nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1013">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="f6f7d-1014">functionapp create: Warnmeldung korrigiert, die derzeit mit `functionapp create` angezeigt wird und ein `--functions_version`-Flag angibt, aber irrtümlich ein `_` anstelle eines `-` im Flagnamen verwendet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1014">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="f6f7d-1015">az functionapp create: Es wurde aktualisiert, wie linuxFxVersion und der Containerimagename für Linux-Funktions-Apps festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1015">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="f6f7d-1016">az functionapp deployment source config-zip: Problems behoben, das durch die Racebedingung für die Änderung von App-Einstellungen während der ZIP-Bereitstellung verursacht wird und während der Bereitstellung 5xx-Fehler ausgibt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1016">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="f6f7d-1017">Fix #5720946: „az webapp backup“ legt Namen nicht fest</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1017">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-1018">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1018">ARM</span></span>

* <span data-ttu-id="f6f7d-1019">az resource: Beispiele für das Ressourcenmodul verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1019">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="f6f7d-1020">az policy assignment list: Unterstützung für das Auflisten von Richtlinienzuweisungen im Verwaltungsgruppenbereich</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1020">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="f6f7d-1021">`az deployment group` und `az deployment operation group` für Vorlagenbereitstellung in Ressourcengruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1021">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="f6f7d-1022">Dies ist ein Duplikat von `az group deployment` und `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1022">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="f6f7d-1023">`az deployment sub` und `az deployment operation sub` für Vorlagenbereitstellung im Abonnementbereich hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1023">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="f6f7d-1024">Dies ist ein Duplikat von `az deployment` und `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1024">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="f6f7d-1025">`az deployment mg` und `az deployment operation mg` für Vorlagenbereitstellung in Verwaltungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1025">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="f6f7d-1026">`az deployment tenant` und `az deployment operation tenant` für Vorlagenbereitstellung im Mandantenbereich hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1026">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="f6f7d-1027">az policy assignment create: Beschreibung zu Parameter `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1027">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="f6f7d-1028">az group deployment create: Parameter `--aux-tenants` zur mandantenübergreifenden Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1028">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="f6f7d-1029">CDN</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1029">CDN</span></span>

* <span data-ttu-id="f6f7d-1030">CDN-WAF-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1030">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-1031">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1031">Compute</span></span>

* <span data-ttu-id="f6f7d-1032">az sig image-version: „--data-snapshot-luns“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1032">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="f6f7d-1033">az ppg show: „--colocation-status“ hinzugefügt, um das Abrufen des Zusammenstellungsstatus aller Ressourcen in der Näherungsplatzierungsgruppe zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1033">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="f6f7d-1034">az vmss create/update: Unterstützung automatischer Reparaturen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1034">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="f6f7d-1035">[BREAKING CHANGE] az image template: „template“ in „builder“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1035">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="f6f7d-1036">az image builder create: „--image-template“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1036">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f6f7d-1037">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1037">Cosmos DB</span></span>

* <span data-ttu-id="f6f7d-1038">Gespeicherte Prozedur „Add Sql“, udf- und trigger-Cmdlets hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1038">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="f6f7d-1039">az cosmosdb create: „--key-uri“ hinzugefügt, um das Hinzufügen von Schlüsseltresor-Verschlüsselungsinformationen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1039">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-1040">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1040">KeyVault</span></span>

* <span data-ttu-id="f6f7d-1041">keyvault create: „soft-delete“ standardmäßig aktiviert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1041">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-1042">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1042">Monitor</span></span>

* <span data-ttu-id="f6f7d-1043">az monitor metrics alert create: Unterstützung von `~` in `--condition`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1043">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1044">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1044">Network</span></span>

* <span data-ttu-id="f6f7d-1045">az network application-gateway rewrite-rule create: Unterstützung der URL-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1045">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="f6f7d-1046">az network dns zone import: Bei „--zone-name“ wird die Groß-/Kleinschreibung künftig nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1046">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="f6f7d-1047">az network private-endpoint/private-link-service: Vorschaubezeichnung entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1047">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="f6f7d-1048">az network bastion: Unterstützung von „bastion“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1048">az network bastion: support bastion</span></span>
* <span data-ttu-id="f6f7d-1049">az network vnet list-available-ips: Unterstützung für das Auflisten verfügbarer IPs in einem VNET</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1049">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="f6f7d-1050">az network watcher flow-log create/list/delete/update: neue Befehle hinzugefügt, um Watcher-Datenflussprotokolle zu verwalten und „--location“ zur expliziten Identifizierung von Watcher verfügbar zu machen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1050">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="f6f7d-1051">az network watcher flow-log configure: veraltet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1051">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="f6f7d-1052">az network watcher flow-log show: Unterstützung von „--location“ und „--name“, um ein ARM-formatiertes Ergebnis zu erhalten; alte formatierte Ausgabe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1052">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="f6f7d-1053">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1053">Policy</span></span>

* <span data-ttu-id="f6f7d-1054">az policy assignment create: Fehler behoben, dass automatisch generierter Name der Richtlinienzuweisung den Grenzwert überschreitet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1054">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-1055">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1055">RBAC</span></span>

* <span data-ttu-id="f6f7d-1056">az ad group show: Problem behoben, dass „--group“-Wert als regulärer Ausdruck behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1056">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-1057">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1057">RDBMS</span></span>

* <span data-ttu-id="f6f7d-1058">SDK-Version von „azure-mgmt-rdbms“ auf 2.0.0 festgelegt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1058">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="f6f7d-1059">az postgres private-endpoint-connection: Verwalten von Verbindungen mit privatem Postgres-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1059">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="f6f7d-1060">az postgres private-link-resource: Verwalten von privaten Postgres-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1060">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="f6f7d-1061">az mysql private-endpoint-connection: Verwalten von Verbindungen mit privatem MySQL-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1061">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="f6f7d-1062">az mysql private-link-resource: Verwalten von privaten MySQL-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1062">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="f6f7d-1063">az mariadb private-endpoint-connection: Verwalten von Verbindungen mit privatem MariaDB-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1063">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="f6f7d-1064">az mariadb private-link-resource: Verwalten von privaten MariaDB-Linkressourcen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1064">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="f6f7d-1065">Aktualisieren von Tests von privaten RDBMS-Endpunkten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1065">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-1066">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1066">SQL</span></span>

* <span data-ttu-id="f6f7d-1067">Sql midb: list-deleted, show-deleted, update-retention, show-retention hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1067">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="f6f7d-1068">(sql server create:) Optionales Flag „Enable“/„Disable“ für public-network-access zu „sql server create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1068">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="f6f7d-1069">(sql server update): kundenorientierte Änderung vorgenommen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1069">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="f6f7d-1070">Eigenschaft „minimal_tls_version“ für MI und SQL-Datenbank hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1070">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1071">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1071">Storage</span></span>

* <span data-ttu-id="f6f7d-1072">az storage blob delete-batch: Flag `--dryrun` mit Fehlverhalten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1072">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="f6f7d-1073">az storage account network-rule hinzugefügt (Fehlerbehebung): Hinzufügen von Vorgängen muss idempotent sein</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1073">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="f6f7d-1074">az storage account create/update: Unterstützung für Routingpräferenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1074">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="f6f7d-1075">„azure-mgmt-storage“ auf Version 8.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1075">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="f6f7d-1076">az storage container immutability create: Parameter „--allow-protected-append-write“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1076">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="f6f7d-1077">az storage account private-link-resource list: Unterstützung zum Auflisten privater Linkressourcen für Speicherkonto hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1077">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="f6f7d-1078">az storage account private-endpoint-connection approve/reject/show/delete: Unterstützung der Verwaltung von Verbindungen mit privaten Endpunkten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1078">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="f6f7d-1079">az storage account blob-service-properties update: „--enable-restore-policy“ und „--restore-days“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1079">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="f6f7d-1080">az storage blob restore: Unterstützung für die Wiederherstellung von Blobbereichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1080">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="f6f7d-1081">18. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1081">February 18, 2020</span></span>

<span data-ttu-id="f6f7d-1082">Version 2.1.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1082">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1083">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1083">ACR</span></span>

* <span data-ttu-id="f6f7d-1084">Neues Argument `--expose-token` für `az acr login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1084">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="f6f7d-1085">Falsche Ausgabe für `az acr task identity show -n Name -r Registry -o table` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1085">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="f6f7d-1086">az acr login: Auslösen von „CLIError“, wenn vom Docker-Befehl Fehler zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1086">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-1087">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1087">ACS</span></span>

* <span data-ttu-id="f6f7d-1088">aks create/update: Validierung für `--vnet-subnet-id` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1088">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="f6f7d-1089">Aladdin</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1089">Aladdin</span></span>

* <span data-ttu-id="f6f7d-1090">Analysieren der generierten Beispiele in „_help.py“ der Befehle</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1090">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-1091">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1091">AMS</span></span>

* <span data-ttu-id="f6f7d-1092">az ams ist jetzt allgemein verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1092">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="f6f7d-1093">AppConfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1093">AppConfig</span></span>

* <span data-ttu-id="f6f7d-1094">Hilfenachricht überarbeitet, um nicht unterstützte Schlüssel-/Bezeichnungsfilter auszuschließen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1094">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="f6f7d-1095">Vorschautag für die meisten Befehle entfernt (mit Ausnahme der Flags für verwaltete Identitäten und Features)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1095">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="f6f7d-1096">Kundenseitig verwalteter Schlüssel beim Aktualisieren der Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1096">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1097">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1097">AppService</span></span>

* <span data-ttu-id="f6f7d-1098">az webapp list-runtimes: Fehler bei „list-runtimes“ behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1098">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="f6f7d-1099">„az webapp|functionapp config ssl create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1099">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="f6f7d-1100">Unterstützung für v3-Funktions-Apps und Node 12</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1100">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-1101">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1101">ARM</span></span>

* <span data-ttu-id="f6f7d-1102">az policy assignment create: Fehlermeldung korrigiert, die angezeigt wird, wenn der Parameter `--policy` ungültig ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1102">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="f6f7d-1103">az group deployment create: Fehler „stat: path too long for Windows" korrigiert, der angezeigt wird, wenn eine zu große Datei vom Typ „parameters.json“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1103">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-1104">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1104">Backup</span></span>

* <span data-ttu-id="f6f7d-1105">Korrektur des Wiederherstellungsflows auf Elementebene am ursprünglichen Speicherort</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1105">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="f6f7d-1106">Unterstützung von „Als Dateien wiederherstellen“ für SQL- und SAP-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1106">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-1107">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1107">Compute</span></span>

* <span data-ttu-id="f6f7d-1108">vm/vmss/availability-set update: „--ppg“ hinzugefügt, um die Aktualisierung von „ProximityPlacementGroup“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1108">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="f6f7d-1109">vmss create: „--data-disk-iops“ und „--data-disk-mbps“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1109">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="f6f7d-1110">az vm host: Vorschautag für `vm host` und `vm host group` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1110">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="f6f7d-1111">[BREAKING CHANGE] Behebung Nr. 10728: `az vm create`: Automatisches Erstellen des Subnetzes, wenn das VNET angegeben wird und das Subnetz nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1111">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="f6f7d-1112">Erhöhen der Stabilität von „vm image list“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1112">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="f6f7d-1113">Eventhub</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1113">Eventhub</span></span>

* <span data-ttu-id="f6f7d-1114">Azure Stack-Unterstützung für Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1114">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-1115">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1115">KeyVault</span></span>

* <span data-ttu-id="f6f7d-1116">az keyvault key create: neuer Wert `import` für Parameter `--ops` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1116">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="f6f7d-1117">az keyvault key list-versions: Unterstützung des Parameters `--id` für die Angabe von Schlüsseln</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1117">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="f6f7d-1118">Unterstützung für Verbindungen mit privaten Endpunkten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1118">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1119">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1119">Network</span></span>

* <span data-ttu-id="f6f7d-1120">Geändert in „azure-mgmt-network 9.0.0“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1120">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="f6f7d-1121">az network private-link-service update/create: Unterstützung von „--enable-proxy-protocol“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1121">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="f6f7d-1122">Feature für Version 2 von Verbindungsmonitor hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1122">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="f6f7d-1123">Verpackung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1123">Packaging</span></span>

* <span data-ttu-id="f6f7d-1124">[BREAKING CHANGE] Unterstützung für Python 2.7 eingestellt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1124">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-1125">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1125">Profile</span></span>

* <span data-ttu-id="f6f7d-1126">Vorschau: Neue Attribute `homeTenantId` und `managedByTenants` zu Abonnementkonten hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1126">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="f6f7d-1127">Führen Sie `az login` erneut aus, damit die Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1127">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="f6f7d-1128">az login: Eine Warnung wird angezeigt, wenn ein Abonnement von mehren Mandanten aufgeführt wird und der erste als Standard festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1128">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="f6f7d-1129">Fügen Sie `--tenant` in `az login` ein, um beim Zugreifen auf dieses Abonnement einen bestimmten Mandanten auszuwählen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1129">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-1130">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1130">Role</span></span>

* <span data-ttu-id="f6f7d-1131">az role assignment create: Problem behoben, das beim Zuweisen einer Rolle zu einem Dienstprinzipal nach Anzeigename einen Fehler vom Typ „HTTP 400“ verursachte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1131">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-1132">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1132">SQL</span></span>

* <span data-ttu-id="f6f7d-1133">Cmdlet `az sql mi update` der verwalteten SQL-Instanz mit zwei neuen Parametern aktualisiert: tier und family</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1133">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1134">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1134">Storage</span></span>

* <span data-ttu-id="f6f7d-1135">[BREAKING CHANGE] `az storage account create`: Art des Standardspeicherkontos in StorageV2 geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1135">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="f6f7d-1136">04. Februar 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1136">February 04, 2020</span></span>

<span data-ttu-id="f6f7d-1137">Version 2.0.81</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1137">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-1138">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1138">ACS</span></span>

* <span data-ttu-id="f6f7d-1139">Unterstützung für das Festlegen zugeordneter Ausgangsports und Leerlauftimeouts für Load Balancer Standard hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1139">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="f6f7d-1140">Aktualisierung auf API-Version 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1140">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1141">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1141">ACR</span></span>

* <span data-ttu-id="f6f7d-1142">[BREAKING CHANGE] `az acr delete` löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1142">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="f6f7d-1143">[BREAKING CHANGE] „az acr task delete“ löst eine Eingabeaufforderung aus.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1143">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="f6f7d-1144">Neue Befehlsgruppe „az acr taskrun show/list/delete“ für die Aufgabenausführungsverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1144">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-1145">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1145">AKS</span></span>

* <span data-ttu-id="f6f7d-1146">Jeder Cluster erhält einen separaten Dienstprinzipal zur Verbesserung der Isolation.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1146">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="f6f7d-1147">AppConfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1147">AppConfig</span></span>

* <span data-ttu-id="f6f7d-1148">Unterstützung für den Import/Export von KeyVault-Verweisen in/aus AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1148">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="f6f7d-1149">Unterstützung für den Import/Export aller Bezeichnungen in appconfig und aus appconfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1149">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="f6f7d-1150">Überprüfen der Schlüssel- und Featurenamen vor dem Festlegen und Importieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1150">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="f6f7d-1151">Verfügbarmachen der SKU-Änderung für den Konfigurationsspeicher</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1151">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="f6f7d-1152">Befehlsgruppe für die verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1152">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1153">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1153">AppService</span></span>

* <span data-ttu-id="f6f7d-1154">Azure Stack: Oberflächenbefehle im Profil „2019-03-01-hybrid“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1154">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="f6f7d-1155">functionapp: Funktion zum Erstellen von Java-Funktions-Apps in Linux hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1155">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-1156">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1156">ARM</span></span>

* <span data-ttu-id="f6f7d-1157">Behebung von Problem Nr. 10246: `az resource tag` stürzt ab, wenn der übergebene Parameter `--ids` der Ressourcengruppen-ID entspricht.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1157">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="f6f7d-1158">Behebung von Problem Nr. 11658: Der Befehl `az group export` unterstützt die Parameter `--query` und `--output` nicht.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1158">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="f6f7d-1159">Behebung von Problem Nr. 10279: Der Exitcode von `az group deployment validate` ist 0, wenn bei der Überprüfung ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1159">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="f6f7d-1160">Behebung von Problem Nr. 9916: Fehlermeldung des Konflikts zwischen Tag und anderen Filterbedingungen für Befehl `az resource list` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1160">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="f6f7d-1161">Neuer Parameter `--managed-by` hinzugefügt, um das Hinzufügen der Informationen vom Typ „managedBy“ für Befehl `az group create` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1161">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="f6f7d-1162">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1162">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="f6f7d-1163">Untergruppe `monitor` hinzugefügt, um Log Analytics-Überwachung im Azure Red Hat OpenShift-Cluster zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1163">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="f6f7d-1164">BotService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1164">BotService</span></span>

* <span data-ttu-id="f6f7d-1165">Behebung von Problem Nr. 11697: `az bot create` ist nicht idempotent.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1165">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="f6f7d-1166">Tests zur Namenskorrektur geändert, sodass sie nur im Livemodus ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1166">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="f6f7d-1167">CDN</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1167">CDN</span></span>

* <span data-ttu-id="f6f7d-1168">Unterstützung für das rulesEngine-Feature hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1168">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="f6f7d-1169">Neue Befehlsgruppe „cdn endpoint rule“ zum Verwalten von Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1169">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="f6f7d-1170">azure-mgmt-cdn-Version auf 4.0.0 aktualisiert, um API-Version 2019-04-15 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1170">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="f6f7d-1171">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1171">Deployment Manager</span></span>

* <span data-ttu-id="f6f7d-1172">Auflistungsvorgang für alle Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1172">Add list operation for all resources.</span></span>
* <span data-ttu-id="f6f7d-1173">Schrittressource für neuen Schritttyp optimiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1173">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="f6f7d-1174">Paket „azure-mgmt-deploymentmanager“ zur Verwendung von Version 0.2.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1174">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-1175">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1175">IoT</span></span>

* <span data-ttu-id="f6f7d-1176">Befehle vom Typ „IoT hub Job“ als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1176">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="f6f7d-1177">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1177">IoT Central</span></span>

* <span data-ttu-id="f6f7d-1178">Unterstützung der App-Erstellung/-Aktualisierung mit neuem SKU-Namen ST0, ST1, ST2</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1178">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6f7d-1179">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1179">Key Vault</span></span>

* <span data-ttu-id="f6f7d-1180">Neuer Befehl `az keyvault key download` zum Herunterladen von Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1180">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="f6f7d-1181">Sonstiges</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1181">Misc</span></span>

* <span data-ttu-id="f6f7d-1182">Behebung Nr. 6371: Unterstützung für die Vervollständigung von Dateinamen und Umgebungsvariablen in Bash</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1182">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1183">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1183">Network</span></span>

* <span data-ttu-id="f6f7d-1184">Behebung Nr. 2092: az network dns record-set add/remove: Warnung hinzugefügt, wenn Datensatzgruppe nicht gefunden wurde.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1184">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="f6f7d-1185">In Zukunft wird ein zusätzliches Argument unterstützt, um diese automatische Erstellung zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1185">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="f6f7d-1186">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1186">Policy</span></span>

* <span data-ttu-id="f6f7d-1187">Neuer Befehl `az policy metadata` hinzugefügt, um umfangreiche Richtlinienmetadatenressourcen abzurufen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1187">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="f6f7d-1188">`az policy remediation create`: Geben Sie mit dem Parameter `--resource-discovery-mode` an, ob die Konformität vor der Wartung neu bewertet werden soll.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1188">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-1189">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1189">Profile</span></span>

* <span data-ttu-id="f6f7d-1190">`az account get-access-token`: Parameter `--tenant` hinzugefügt, um das Token für den Mandanten direkt abzurufen. Es muss kein Abonnement angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1190">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-1191">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1191">RBAC</span></span>

* <span data-ttu-id="f6f7d-1192">[BREAKING CHANGE] Behebung Nr. 11883: `az role assignment create`: Bei leerem Bereich wird ein Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1192">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="f6f7d-1193">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1193">Security</span></span>

* <span data-ttu-id="f6f7d-1194">Neue Befehle `az atp show` und `az atp update` hinzugefügt, um erweiterte Einstellungen für den Bedrohungsschutz für Speicherkonten anzuzeigen und zu verwalten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1194">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-1195">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1195">SQL</span></span>

* <span data-ttu-id="f6f7d-1196">`sql dw create`: Parameter `--zone-redundant` und `--read-replica-count` als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1196">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="f6f7d-1197">Diese Parameter gelten nicht für Datawarehouse.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1197">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="f6f7d-1198">[BREAKING CHANGE] `az sql db create`: „WideWorldImportersStd“ und „WideWorldImportersFull“ als dokumentierte zulässige Werte für „az sql db create --sample-name“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1198">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="f6f7d-1199">Diese Beispieldatenbanken führen immer zu einem Fehler bei der Erstellung.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1199">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="f6f7d-1200">Neue Befehle `sql db classification show/list/update/delete` und `sql db classification recommendation list/enable/disable` zur Verwaltung von Vertraulichkeitsklassifizierungen für SQL-Datenbanken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1200">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="f6f7d-1201">`az sql db audit-policy`: Behebung für leere Überwachungsaktionen und -gruppen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1201">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1202">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1202">Storage</span></span>

* <span data-ttu-id="f6f7d-1203">Neue Befehlsgruppe `az storage share-rm` hinzugefügt, um den Ressourcenanbieter „Microsoft.Storage“ für Verwaltungsvorgänge der Azure-Dateifreigabe zu verwenden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1203">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="f6f7d-1204">Behebung für Problem Nr. 11415: Berechtigungsfehler für `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1204">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="f6f7d-1205">Integration von Azcopy 10.3.3 und Unterstützung von Win32</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1205">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="f6f7d-1206">`az storage copy`: Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1206">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="f6f7d-1207">`az storage remove`: Parameter `--inlcude` und `--exclude` in Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1207">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="f6f7d-1208">`az storage sync`: Parameter `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1208">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="f6f7d-1209">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1209">ServiceFabric</span></span>

* <span data-ttu-id="f6f7d-1210">Neue Befehle zum Verwalten von Anwendung und Diensten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1210">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="f6f7d-1211">13. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1211">January 13, 2020</span></span>

<span data-ttu-id="f6f7d-1212">Version 2.0.80</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1212">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-1213">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1213">Compute</span></span>

* <span data-ttu-id="f6f7d-1214">Datenträgeraktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1214">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="f6f7d-1215">Momentaufnahmeerstellung/-aktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1215">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1216">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1216">Storage</span></span>

* <span data-ttu-id="f6f7d-1217">„azure-mgmt-storage“ auf Version 7.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1217">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="f6f7d-1218">`az storage account create`: `--encryption-key-type-for-table` und `--encryption-key-type-for-queue` zur Unterstützung des Tabellen- und Warteschlangenverschlüsselungsdiensts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1218">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="f6f7d-1219">7\. Januar 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1219">January 07, 2020</span></span>

<span data-ttu-id="f6f7d-1220">Version 2.0.79</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1220">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1221">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1221">ACR</span></span>

* <span data-ttu-id="f6f7d-1222">[BREAKING CHANGE] Parameter „--os“ für „acr build“, „acr task create/update“, „acr run“ und „acr pack“ wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1222">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="f6f7d-1223">Verwenden Sie stattdessen „--platform“.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1223">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="f6f7d-1224">AppConfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1224">AppConfig</span></span>

* <span data-ttu-id="f6f7d-1225">Unterstützung für das Importieren/Exportieren von Featureflags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1225">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="f6f7d-1226">Neuer Befehl „az appconfig kv set-keyvault“ für das Erstellen einer KeyVault-Referenz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1226">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="f6f7d-1227">Unterstützung verschiedener Benennungskonventionen beim Exportieren von Featureflags in eine Datei</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1227">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1228">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1228">AppService</span></span>

* <span data-ttu-id="f6f7d-1229">Behebung von Problem Nr. 7154: Aktualisierung der Dokumentation für Befehl „<>“, sodass Backticks anstelle von einfachen Anführungszeichen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1229">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="f6f7d-1230">Behebung von Problem Nr. 11287: „webapp up“: Für die mit „up“ erstellte App muss standardmäßig SSL aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1230">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="f6f7d-1231">Behebung von Problem Nr. 11592: Flag „az webapp up“ für statische HTML-Websites hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1231">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-1232">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1232">ARM</span></span>

* <span data-ttu-id="f6f7d-1233">Behebung `az resource tag`: Recovery Services-Tresor-Tags können nicht aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1233">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-1234">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1234">Backup</span></span>

* <span data-ttu-id="f6f7d-1235">Neuer Befehl „backup protection undelete“ hinzugefügt, um die Funktion zum vorläufigen Löschen für IaasVM-Workloads zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1235">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="f6f7d-1236">Neuer Parameter „--soft-delete-feature-state“ hinzugefügt, um den Befehl „backup-properties“ festzulegen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1236">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="f6f7d-1237">Unterstützung für den Ausschluss von Datenträgern für IaasVM-Workload hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1237">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-1238">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1238">Compute</span></span>

* <span data-ttu-id="f6f7d-1239">Fehler `vm create` in Azure Stack-Profil behoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1239">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="f6f7d-1240">vm monitor metrics tail/list-definitions: Unterstützung einer Abfragemetrik und von Listendefinitionen für eine VM.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1240">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="f6f7d-1241">Neue Aktion des Befehls zum erneuten Anwenden für „az vm“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1241">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-1242">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1242">HDInsight</span></span>

* <span data-ttu-id="f6f7d-1243">Unterstützung für das Erstellen eines Kafka-Clusters mit Kafka-REST-Proxy</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1243">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="f6f7d-1244">„azure-mgmt-hdinsight“ auf 1.3.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1244">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="f6f7d-1245">Verschiedenes:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1245">Misc.</span></span>

* <span data-ttu-id="f6f7d-1246">Vorschaubefehl `az version show` hinzugefügt, um die Versionen der Azure CLI-Module und Erweiterungen standardmäßig im JSON-Format oder im mit „--output“ konfigurierten Format anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1246">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="f6f7d-1247">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1247">Event Hubs</span></span>

* <span data-ttu-id="f6f7d-1248">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus „az eventhubs eventhub update“ und „az eventhubs eventhub create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1248">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="f6f7d-1249">Diese Option ist für Event Hub-Entitäten nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1249">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="f6f7d-1250">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1250">Service Bus</span></span>

* <span data-ttu-id="f6f7d-1251">[BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus Befehlen „az servicebus topic create“, „az servicebus topic update“, „az servicebus queue create“ und „az servicebus queue update“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1251">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="f6f7d-1252">Diese Option ist für Service Bus-Themen und -Warteschlangen nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1252">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-1253">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1253">RBAC</span></span>

* <span data-ttu-id="f6f7d-1254">Behebung Nr. 11712: `az ad app/sp show` gibt nicht den Exitcode 3 zurück, wenn die Anwendung oder der Dienstprinzipal nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1254">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1255">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1255">Storage</span></span>

* <span data-ttu-id="f6f7d-1256">`az storage account create`: Vorschaukennzeichnung für Parameter „--enable-hierarchical-namespace“ entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1256">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="f6f7d-1257">azure-mgmt-storage-Version auf 7.0.0 aktualisiert, um API-Version 2019-06-01 zu verwenden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1257">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="f6f7d-1258">Neue Parameter `--enable-delete-retention` und `--delete-retention-days` hinzugefügt, um die Verwaltung der Aufbewahrungsrichtlinie für Löschen für „blob-service-properties“ von Speicherkonten zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1258">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="f6f7d-1259">17. Dezember 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1259">December 17, 2019</span></span>

<span data-ttu-id="f6f7d-1260">2.0.78</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1260">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1261">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1261">ACR</span></span>

* <span data-ttu-id="f6f7d-1262">Unterstützung für lokalen Kontext in „acr task run“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1262">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-1263">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1263">ACS</span></span>

* <span data-ttu-id="f6f7d-1264">[BREAKING CHANGE] az openshift create: `--workspace-resource-id` in `--workspace-id` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1264">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-1265">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1265">AMS</span></span>

* <span data-ttu-id="f6f7d-1266">Befehle zum Anzeigen aktualisiert, sodass 3 zurückgegeben wird, wenn die Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1266">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="f6f7d-1267">AppConfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1267">AppConfig</span></span>

* <span data-ttu-id="f6f7d-1268">Fehler beim Anhängen der API-Version an die Anforderungs-URL korrigiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1268">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="f6f7d-1269">Die vorhandene Lösung funktioniert nicht mit Paginierung.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1269">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="f6f7d-1270">Unterstützung für die Anzeige von weiteren Sprachen neben Englisch hinzugefügt, da der Back-End-Dienst Unicode für die Globalisierung unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1270">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1271">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1271">AppService</span></span>

* <span data-ttu-id="f6f7d-1272">Problem Nr. 11217 behoben: Web-App: „az webapp config ssl upload“ muss Slot-Parameter unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1272">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="f6f7d-1273">Problem Nr. 10965 behoben: Error: Der Name darf nicht leer sein.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1273">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="f6f7d-1274">Entfernen anhand von „ip_address“ und „subnet“ zulassen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1274">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="f6f7d-1275">Unterstützung des Imports von Zertifikaten aus Key Vault hinzugefügt `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1275">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-1276">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1276">ARM</span></span>

* <span data-ttu-id="f6f7d-1277">Paket „azure-mgmt-resource“ auf die Verwendung von 6.0.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1277">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="f6f7d-1278">Mandantenübergreifende Unterstützung für Befehl `az group deployment create` durch Hinzufügen des neuen Parameters `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1278">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="f6f7d-1279">Neuer Parameter `--metadata` hinzugefügt, um das Hinzufügen von Metadateninformationen für Richtliniensatzdefinitionen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1279">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-1280">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1280">Backup</span></span>

* <span data-ttu-id="f6f7d-1281">Unterstützung der Sicherung für SQL- und SAP Hana-Workloads hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1281">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="f6f7d-1282">BotService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1282">BotService</span></span>

* <span data-ttu-id="f6f7d-1283">[Breaking Change] Flag „--version“ aus Vorschaubefehl „az bot create“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1283">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="f6f7d-1284">Nur v4-SDK-Bots werden unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1284">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="f6f7d-1285">Überprüfung der Namensverfügbarkeit für „az bot create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1285">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="f6f7d-1286">Unterstützung für das Aktualisieren der Symbol-URL für einen Bot über „az bot update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1286">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="f6f7d-1287">Unterstützung für das Aktualisieren eines Direct Line-Kanals über „az bot directline update“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1287">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="f6f7d-1288">Unterstützung für Flag „--enable-enhanced-auth“ zu „az bot directline create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1288">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="f6f7d-1289">Die folgenden Befehlsgruppen sind allgemein verfügbar und befinden sich nicht in der Vorschau: „az bot authsetting“.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1289">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="f6f7d-1290">Die folgenden Befehle in „az bot“ sind allgemein verfügbar und befinden sich nicht in der Vorschau: „create“, „prepare-deploy“, „show“, „delete“, „update“.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1290">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="f6f7d-1291">„az bot prepare-deploy“ korrigiert, indem der Wert voon „--proj-file-path“ in Kleinschreibung geändert wurde (z. B. „Test.csproj“ in „test.csproj“).</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1291">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-1292">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1292">Compute</span></span>

* <span data-ttu-id="f6f7d-1293">vmss create/update: „--scale-in-policy“ hinzugefügt, womit entschieden wird, welche virtuellen Computer beim horizontalen Herunterskalieren einer VM-Skalierungsgruppe zum Entfernen ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1293">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="f6f7d-1294">vm/vmss update: „--priority“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1294">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="f6f7d-1295">vm/vmss update: „--max-price“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1295">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="f6f7d-1296">Befehlsgruppe „disk-encryption-set“ hinzugefügt (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1296">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="f6f7d-1297">disk create: „--encryption-type“ und „--disk-encryption-set“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1297">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="f6f7d-1298">vm/vmss create: „--os-disk-encryption-set“ und „--data-disk-encryption-sets“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1298">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-1299">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1299">Core</span></span>

* <span data-ttu-id="f6f7d-1300">Unterstützung für Python 3.4 entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1300">Removed support for Python 3.4</span></span>
* <span data-ttu-id="f6f7d-1301">Plug-In für HaTS-Umfrage in mehreren Befehlen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1301">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="f6f7d-1302">DLS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1302">DLS</span></span>

* <span data-ttu-id="f6f7d-1303">ADLS-SDK-Version aktualisiert (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1303">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="f6f7d-1304">Installieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1304">Install</span></span>

* <span data-ttu-id="f6f7d-1305">Installationsskript unterstützt Python 3.8</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1305">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-1306">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1306">IOT</span></span>

* <span data-ttu-id="f6f7d-1307">[BREAKING CHANGE] Parameter „--failover-region“ aus „manual-failover“ entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1307">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="f6f7d-1308">Das Failover erfolgt jetzt in eine zugewiesene, geografisch gekoppelte sekundäre Region.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1308">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6f7d-1309">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1309">Key Vault</span></span>

* <span data-ttu-id="f6f7d-1310">Nr. 8095 behoben: `az keyvault storage remove`: Hilfemeldung verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1310">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="f6f7d-1311">Nr. 8921 behoben: `az keyvault key/secret/certificate list/list-deleted/list-versions`: Validierungsfehler in Parameter `--maxresults` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1311">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="f6f7d-1312">Nr. 10512 behoben: `az keyvault set-policy`: Fehlermeldung verbessert, wenn weder `--object-id`, `--spn` noch `--upn` angegeben ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1312">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="f6f7d-1313">Nr. 10846 behoben: `az keyvault secret show-deleted`: Wenn `--id` angegeben ist, ist `--name/-n` nicht erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1313">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="f6f7d-1314">Nr. 11084 behoben: `az keyvault secret download`: Hilfemeldung von Parameter `--encoding` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1314">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1315">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1315">Network</span></span>

* <span data-ttu-id="f6f7d-1316">az network application-gateway probe: Unterstützung für Option „--port“ hinzugefügt, um einen Port zum Prüfen von Back-End-Servern beim Erstellen und Aktualisieren anzugeben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1316">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="f6f7d-1317">az network application-gateway url-path-map create/update: Fehlerbehebung für `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1317">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="f6f7d-1318">az network application-gateway: Unterstützung für `--rewrite-rule-set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1318">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="f6f7d-1319">az network list-service-aliases: Unterstützung für Listendienstaliase hinzugefügt, die für Dienstendpunktrichtlinien verwendet werden können</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1319">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="f6f7d-1320">az network dns zone import: Unterstützung für „.@“ in Datensatzname hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1320">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="f6f7d-1321">Verpackung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1321">Packaging</span></span>

* <span data-ttu-id="f6f7d-1322">Back-Edge-Builds für PIP-Installation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1322">Added back edge builds for pip install</span></span>
* <span data-ttu-id="f6f7d-1323">Ubuntu-Eoan-Paket hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1323">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="f6f7d-1324">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1324">Policy</span></span>

* <span data-ttu-id="f6f7d-1325">Unterstützung für Version 2019-09-01 der Richtlinien-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1325">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="f6f7d-1326">az policy set-definition: Unterstützung der Gruppierung innerhalb von Richtliniensatzdefinitionen mit `--definition-groups`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1326">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="f6f7d-1327">Redis</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1327">Redis</span></span>

* <span data-ttu-id="f6f7d-1328">Vorschauparameter `--replicas-per-master` zu Befehl `az redis create`hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1328">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="f6f7d-1329">„azure-mgmt-redis“ von 6.0.0 auf 7.0.0rc1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1329">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="f6f7d-1330">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1330">ServiceFabric</span></span>

* <span data-ttu-id="f6f7d-1331">Hinzufügen von Logik in Knotentyp korrigiert, einschließlich Nr. 10963: Beim Hinzufügen eines neuen Knotentyps mit Dauerhaftigkeitsstufe „Gold“ wird immer ein CLI-Fehler ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1331">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="f6f7d-1332">ServiceFabricNodeVmExt-Version in Erstellungsvorlage auf 1.1 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1332">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-1333">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1333">SQL</span></span>

* <span data-ttu-id="f6f7d-1334">Parameter „--read-scale“ und „--read-replicas“ zu Befehlen „sql db create“ und „sql db update“ hinzugefügt, um Leseskalierungsverwaltung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1334">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1335">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1335">Storage</span></span>

* <span data-ttu-id="f6f7d-1336">Allgemein verfügbares Release – Eigenschaft „Large File Shares“ für Befehle „storage account create“ und „storage account update“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1336">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="f6f7d-1337">Allgemein verfügbares Release – Unterstützung von SAS-Token für die Benutzerdelegierung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1337">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="f6f7d-1338">Neue Befehle `az storage account blob-service-properties show` und `az storage account blob-service-properties update --enable-change-feed` hinzugefügt, um Blob-Diensteigenschaften für das Speicherkonto zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1338">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="f6f7d-1339">[BEVORSTEHENDER BREAKING CHANGE] `az storage copy`: Das Zeichen `*` wird nicht mehr als Platzhalter in der URL, es werden jedoch die neuen Parameter „--include-pattern“ und „--exclude-pattern“ mit Unterstützung des Platzhalters `*` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1339">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="f6f7d-1340">Problem Nr. 11043 behoben: Unterstützung für das Entfernen des gesamten Containers/der gesamten Freigabe in `az storage remove` Befehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1340">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="f6f7d-1341">26. November 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1341">November 26, 2019</span></span>

<span data-ttu-id="f6f7d-1342">Version 2.0.77</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1342">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1343">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1343">ACR</span></span>

* <span data-ttu-id="f6f7d-1344">Parameter `--branch` in „acr task create/update“ als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1344">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="f6f7d-1345">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1345">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="f6f7d-1346">`--workspace-resource-id`-Flag hinzugefügt, um die Erstellung eines Azure Red Hat OpenShift-Clusters mit Überwachung zuzulassen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1346">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="f6f7d-1347">`monitor_profile`-Flag hinzugefügt, um einen Azure Red Hat OpenShift-Clusters mit Überwachung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1347">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-1348">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1348">AKS</span></span>

* <span data-ttu-id="f6f7d-1349">Unterstützung des Rotationsvorgangs für Clusterzertifikate mithilfe von für Cluster Zertifikat Rotation mit „az aks rotate-certs“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1349">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="f6f7d-1350">AppConfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1350">AppConfig</span></span>

* <span data-ttu-id="f6f7d-1351">Unterstützung für die Verwendung von „:“ für `as az appconfig kv import`-Trennzeichen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1351">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="f6f7d-1352">Problem beim Auflisten von Schlüsselwerten mit mehreren Bezeichnungen, einschließlich NULL-Bezeichnung, behoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1352">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="f6f7d-1353">Verwaltungsebenen-SDK, „azure-mgmt-appconfiguration“, auf Version 0.3.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1353">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="f6f7d-1354">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1354">AppService</span></span>

* <span data-ttu-id="f6f7d-1355">Problem Nr. 11100 behoben AttributeError für „az webapp up“ beim Erstellen eines Dienstplans</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1355">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="f6f7d-1356">az webapp up: Erzwingen der Erstellung oder Bereitstellung auf einer Website für unterstützte Sprachen, es werden keine Standardeinstellungen verwendet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1356">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="f6f7d-1357">Unterstützung für App Service-Umgebung hinzugefügt: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1357">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-1358">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1358">Backup</span></span>

* <span data-ttu-id="f6f7d-1359">Problem in Az-Sicherungsrichtlinie „list-associated-items“ behoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1359">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="f6f7d-1360">Optionaler Parameter „BackupManagementType“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1360">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-1361">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1361">Compute</span></span>

* <span data-ttu-id="f6f7d-1362">API-Version von Compute, Datenträger, Momentaufnahmen auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1362">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="f6f7d-1363">vmss create: Verbesserung für – Orchestrierungsmodus</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1363">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="f6f7d-1364">sig image-definition create: „--os-state“ hinzugefügt, um die Angabe zu ermöglichen, ob die unter diesem Image erstellten virtuellen Computer „generalisiert“ oder „spezialisiert“ sind</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1364">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="f6f7d-1365">sig image-definition create: „--hyper-v-generation“ hinzugefügt, um die Angabe der Hypervisorgeneration zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1365">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="f6f7d-1366">sig image-version create: Unterstützung für „--os-snapshot“ und „--data-snapshots“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1366">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="f6f7d-1367">image create: „--data-disk-caching“ hinzugefügt, um die Angabe der Zwischenspeicherungseinstellung von Datenträger zu ermöflichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1367">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="f6f7d-1368">Upgrade des Python-Compute-SDK auf 10.0.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1368">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="f6f7d-1369">vm/vmss create: „Spot“ zu Aufzählungseigenschaft „Priority“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1369">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="f6f7d-1370">[Breaking Change] Parameter „--max-billing“ für sowohl VM als auch VMSS in „--max-price“ umbenannt, um die Konsistenz mit Swagger- und PowerShell-Cmdlets sicherzustellen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1370">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="f6f7d-1371">vm monitor log show: Unterstützung für das Abfragen von Protokollen über verknüpften Protokollanalyse-Arbeitsbereich hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1371">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-1372">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1372">IOT</span></span>

* <span data-ttu-id="f6f7d-1373">Behebung Nr. 2531: Argumente für Benutzerfreundlichkeit für Hub-Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1373">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="f6f7d-1374">Behebung Nr. 8323: Fehlende Parameter zum Erstellen eines benutzerdefinierten Speicherendpunkts hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1374">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="f6f7d-1375">Regressionsfehler behoben: Die Änderungen wurden rückgängig gemacht, sodass der standardmäßige Speicherendpunkt überschrieben wurde.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1375">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6f7d-1376">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1376">Key Vault</span></span>

* <span data-ttu-id="f6f7d-1377">Nr. 11121 behoben: Bei der Verwendung von `az keyvault certificate list` erfordert die Übergabe von `--include-pending` jetzt nicht mehr den Wert `true` oder `false`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1377">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="f6f7d-1378">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1378">NetAppFiles</span></span>

* <span data-ttu-id="f6f7d-1379">Upgrade von „azure-mgmt-netapp“ auf Version 0.7.0, die einige zusätzliche Volumeeigenschaften enthält, die bevorstehenden Replikationsvorgängen zugeordnet sind</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1379">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1380">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1380">Network</span></span>

* <span data-ttu-id="f6f7d-1381">application-gateway waf-config: veraltet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1381">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="f6f7d-1382">application-gateway waf-policy: Untergruppe „managed-rules“ zur Verwaltung von verwalteten Regelsätzen und Ausschlussregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1382">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="f6f7d-1383">application-gateway waf-policy: Untergruppe „policy-setting“ zur Verwaltung der globalen Konfiguration von „waf-policy“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1383">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="f6f7d-1384">[BREAKING CHANGE] application-gateway waf-policy: Untergruppenregel in „custom-rule“ umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1384">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="f6f7d-1385">application-gateway http-listener: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1385">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="f6f7d-1386">application-gateway url-path-map rule: „--firewall-policy“ beim Erstellen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1386">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="f6f7d-1387">Verpackung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1387">Packaging</span></span>

* <span data-ttu-id="f6f7d-1388">Az-Wrapper in Python neu geschrieben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1388">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="f6f7d-1389">Unterstützung für Python 3.8 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1389">Added support for Python 3.8</span></span>
* <span data-ttu-id="f6f7d-1390">Für RPM-Paket in Python 3 geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1390">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-1391">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1391">Profile</span></span>

* <span data-ttu-id="f6f7d-1392">Fehler beim Ausführen von `az login -u {} -p {}` mit Microsoft-Konto entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1392">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="f6f7d-1393">`SSLError` beim Ausführen von `az login` hinter einem Proxy mit einem selbstsignierten Stammzertifikat entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1393">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="f6f7d-1394">Nr. 10578 behoben: `az login` hängt, wenn mehrere Instanzen gleichzeitig unter Windows oder WSL gestartet werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1394">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="f6f7d-1395">Nr. 11059 behoben: `az login --allow-no-subscriptions` schlägt fehl, wenn Abonnements im Mandanten vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1395">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="f6f7d-1396">Nr. 11238 behoben: Nach dem Umbenennen eines Abonnements führt die Anmeldung mit MSI dazu, dass das gleiche Abonnement zweimal angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1396">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-1397">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1397">RBAC</span></span>

* <span data-ttu-id="f6f7d-1398">Nr. 10996 behoben: Fehler für `--force-change-password-next-login` in `az ad user update` entfernt, wenn `--password` nicht angegeben ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1398">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="f6f7d-1399">Redis</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1399">Redis</span></span>

* <span data-ttu-id="f6f7d-1400">Nr. 2902 behoben: Festlegen von Speicherkonfigurationen beim Aktualisieren des Basic-SKU-Cache vermeiden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1400">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="f6f7d-1401">Reservations</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1401">Reservations</span></span>

* <span data-ttu-id="f6f7d-1402">SDK-Version auf 0.6.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1402">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="f6f7d-1403">Abrechnungsplandetails nach dem Aufrufen von „Get-Gatalogs“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1403">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="f6f7d-1404">Neuer Befehl `az reservations reservation-order calculate` zum Berechnen des Preises für eine Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1404">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="f6f7d-1405">Neuer Befehl `az reservations reservation-order purchase` zum Erwerb einer neuen Reservierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1405">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="f6f7d-1406">REST</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1406">Rest</span></span>
* <span data-ttu-id="f6f7d-1407">`az rest` in allgemeine Verfügbarkeit geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1407">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-1408">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1408">SQL</span></span>

* <span data-ttu-id="f6f7d-1409">„azure-mgmt-sql“ auf Version 0.15.0 aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1409">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1410">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1410">Storage</span></span>

* <span data-ttu-id="f6f7d-1411">storage account create: „--enable-hierarchical-namespace“ hinzugefügt, um Dateisystemsemantik in Blobdienst zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1411">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="f6f7d-1412">Ausnahme ohne Zusammenhang aus Fehlermeldung entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1412">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="f6f7d-1413">Probleme mit falscher Fehlermeldung „Sie verfügen nicht über die erforderlichen Berechtigungen zum Ausführen dieses Vorgangs“ behoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1413">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="f6f7d-1414">bei Blockierung durch Netzwerkregeln oder bei „AuthenticationFailed“.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1414">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="f6f7d-1415">4\. November 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1415">November 4, 2019</span></span>

<span data-ttu-id="f6f7d-1416">Version 2.0.76</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1416">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1417">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1417">ACR</span></span>

* <span data-ttu-id="f6f7d-1418">Vorschauparameter `--pack-image-tag` wurde dem Befehl `az acr pack build` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1418">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="f6f7d-1419">Unterstützung der Aktivierung der Überwachung beim Erstellen einer Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1419">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="f6f7d-1420">Unterstützung von RBAC mit Repositoryumfang hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1420">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-1421">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1421">AKS</span></span>

* <span data-ttu-id="f6f7d-1422">`--enable-cluster-autoscaler`, `--min-count` und `--max-count` wurden dem Befehl `az aks create` hinzugefügt, sodass die automatische Clusterskalierung für den Knotenpool aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1422">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="f6f7d-1423">Die obigen Flags sowie `--update-cluster-autoscaler` und `--disable-cluster-autoscaler` wurden dem Befehl `az aks update` hinzugefügt, sodass Updates der automatischen Clusterskalierung zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1423">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="f6f7d-1424">AppConfig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1424">AppConfig</span></span>

* <span data-ttu-id="f6f7d-1425">Befehlsgruppe der AppConfig-Funktion zum Verwalten von in einer App Configuration-Instanz gespeicherten Featureflags wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1425">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="f6f7d-1426">Geringfügiger Programmfehler für Befehl „appconfig kv export to file“ wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1426">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="f6f7d-1427">Das Lesen der Zieldateiinhalte wird während des Exports angehalten.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1427">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1428">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1428">AppService</span></span>

* <span data-ttu-id="f6f7d-1429">`az appservice plan create`: Unterstützung für das Festlegen von „persitescalung“ beim Erstellen eines App-Serviceplans wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1429">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="f6f7d-1430">Ein Problem wurde behoben, aufgrund dessen der Vorgang „webapp config ssl bind“ vorhandene Tags aus der Ressource entfernt hat.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1430">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="f6f7d-1431">Flag `--build-remote` wurde für `az functionapp deployment source config-zip` hinzugefügt, um die Remotebuildaktion während der Funktions-App-Bereitstellung zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1431">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="f6f7d-1432">Die Standardknotenversion in Funktions-Apps wurde für Windows in ~ 10 geändert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1432">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="f6f7d-1433">`--runtime-version`-Eigenschaft zu `az functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1433">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-1434">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1434">ARM</span></span>

* <span data-ttu-id="f6f7d-1435">`az deployment/group deployment validate`: Parameter `--handle-extended-json-format` wurde hinzugefügt, um bei der Bereitstellung mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1435">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="f6f7d-1436">„azure-mgmt-resource“ auf „2019-07-01“ festgelegt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1436">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-1437">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1437">Backup</span></span>

* <span data-ttu-id="f6f7d-1438">Unterstützung für AzureFiles-Sicherung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1438">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-1439">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1439">Compute</span></span>

* <span data-ttu-id="f6f7d-1440">`az vm create`: Beim gleichzeitigen Festlegen von beschleunigtem Netzwerkbetrieb und einer vorhandenen NIC wurde eine Warnung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1440">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="f6f7d-1441">`az vm create`: `--vmss` hinzugefügt, um eine vorhandene VM-Skalierungsgruppe anzugeben, welcher der virtuelle Computer zugewiesen werden soll.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1441">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="f6f7d-1442">`az vm/vmss create`: Eine lokale Kopie der Imagealiasdatei wurde hinzugefügt, sodass in einer eingeschränkten Netzwerkumgebung darauf zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1442">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="f6f7d-1443">`az vmss create`: `--orchestration-mode` hinzugefügt, um anzugeben, wie virtuelle Computer von der Skalierungsgruppe verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1443">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="f6f7d-1444">`az vm/vmss update`: `--ultra-ssd-enabled` hinzugefügt, um das Aktualisieren der SSD-Einstellung zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1444">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="f6f7d-1445">[BREAKING CHANGE] `az vm extension set`: Ein Fehler wurde behoben, aufgrund dessen Benutzer mit `--ids` keine Erweiterung auf einem virtuellen Computer festlegen konnten.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1445">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="f6f7d-1446">Neue Befehle wurden zu `az vm image terms accept/cancel/show` hinzugefügt , um Azure Marketplace-Imagebedingungen zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1446">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="f6f7d-1447">VMAccessForLinux auf Version 1.5 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1447">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6f7d-1448">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1448">CosmosDB</span></span>

* <span data-ttu-id="f6f7d-1449">[BREAKING CHANGE] `az sql container create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1449">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="f6f7d-1450">[BREAKING CHANGE] `az gremlin graph create`: `--partition-key-path` in erforderlichen Parameter geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1450">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="f6f7d-1451">`az sql container create`: `--unique-key-policy` und `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1451">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="f6f7d-1452">`az sql container create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1452">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="f6f7d-1453">`gremlin graph create`: `--conflict-resolution-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1453">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="f6f7d-1454">`gremlin graph create/update`: Aktualisierung des `--idx`-Standardschemas</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1454">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="f6f7d-1455">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1455">Fixed typo in help message</span></span>
* <span data-ttu-id="f6f7d-1456">Datenbank: Informationen zur eingestellten Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1456">database: Added deprecation information</span></span>
* <span data-ttu-id="f6f7d-1457">Auflistung: Informationen zur eingestellten Unterstützung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1457">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-1458">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1458">IoT</span></span>

* <span data-ttu-id="f6f7d-1459">Neuer Routingquelltyp hinzugefügt: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1459">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="f6f7d-1460">Fehlende Features in `az iot hub create` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1460">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6f7d-1461">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1461">Key Vault</span></span>

* <span data-ttu-id="f6f7d-1462">Ein unerwarteter Fehler wurde behoben, bei dem keine Zertifikatdatei vorhanden war.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1462">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="f6f7d-1463">Funktionsunfähigkeit von `az keyvault recover/purge` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1463">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="f6f7d-1464">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1464">NetAppFiles</span></span>

* <span data-ttu-id="f6f7d-1465">„azure-mgmt-netapp“ wurde auf 0.6.0 aktualisiert, um API-Version 2019-07-01 zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1465">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="f6f7d-1466">Diese neue API-Version umfasst:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1466">This new API version includes:</span></span>

    - <span data-ttu-id="f6f7d-1467">Volumeerstellung `--protocol-types` akzeptiert jetzt „NFSv4.1“ anstelle von „NFSv4“.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1467">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="f6f7d-1468">Die Richtlinie der Volumeexportrichtlinie heißt jetzt „nfsv41“ anstelle von „nfsv4“.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1468">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="f6f7d-1469">Volume `--creation-token` wurde in `--file-path` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1469">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="f6f7d-1470">Das Erstellungsdatum einer Momentaufnahme heißt jetzt einfach „erstellt“.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1470">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1471">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1471">Network</span></span>

* <span data-ttu-id="f6f7d-1472">`az network private-dns link vnet create/update`: Unterstützung für mandantenübergreifende Verknüpfung virtueller Netzwerke.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1472">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="f6f7d-1473">[BREAKING CHANGE] `az network vnet subnet list`: `--resource-group` und `--vnet-name` wurden geändert und sind jetzt erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1473">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="f6f7d-1474">`az network public-ip prefix create`: Unterstützung der Angabe der IP-Adressversion (IPv4, IPv6) bei der Erstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1474">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="f6f7d-1475">„azure-mgmt-network“ auf 7.0.0 und „api-version“ auf 2019-09-01 festgelegt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1475">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="f6f7d-1476">`az network vrouter`: Unterstützung für neuen virtuellen Dienstrouter und virtuelles Routerpeering hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1476">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="f6f7d-1477">`az network express-route gateway connection`: Unterstützung für `--internet-security` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1477">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-1478">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1478">Profile</span></span>

* <span data-ttu-id="f6f7d-1479">Funktionsunfähigkeit von `az account get-access-token --resource-type ms-graph` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1479">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="f6f7d-1480">Warnung aus `az login` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1480">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-1481">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1481">RBAC</span></span>

* <span data-ttu-id="f6f7d-1482">Funktionsunfähigkeit von `az ad app update --id {} --display-name {}` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1482">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="f6f7d-1483">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1483">ServiceFabric</span></span>

* <span data-ttu-id="f6f7d-1484">`az sf cluster create`: Ein Problem wurde behoben, indem die Compute-VMSS von „template.json“ für Service Fabric unter Linux und Windows von Standarddatenträgern auf verwaltete Datenträger umgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1484">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-1485">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1485">SQL</span></span>

* <span data-ttu-id="f6f7d-1486">Die Parameter `--compute-model`, `--auto-pause-delay` und `--min-capacity` wurden hinzugefügt, um CRUD-Vorgänge für das neue SQL-Datenbank-Angebot zu unterstützen: Serverloses Computemodell.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1486">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1487">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1487">Storage</span></span>

* <span data-ttu-id="f6f7d-1488">`az storage account create/update`: Parameter „--enable-files-adds“ und Azure Active Directory-Eigenschaftenargumentgruppe hinzugefügt, um Active Directory Domain-Dienstauthentifizierung für Azure Files zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1488">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="f6f7d-1489">`az storage account keys list/renew` wurde erweitert, um die Auflistung oder erneute Generierung von Kerberos-Schlüsseln des Speicherkontos zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1489">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="f6f7d-1490">15. Oktober 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1490">October 15, 2019</span></span>

<span data-ttu-id="f6f7d-1491">Version 2.0.75</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1491">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-1492">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1492">AKS</span></span>

* <span data-ttu-id="f6f7d-1493">Standardwert `--load-balancer-sku` in `standard` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1493">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="f6f7d-1494">Standardwert `--vm-set-type` in `virtualmachinescalesets` geändert, sofern von der Kubernetes-Version unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1494">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-1495">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1495">AMS</span></span>

* <span data-ttu-id="f6f7d-1496">[BREAKING CHANGE] Name von `job start` in `job create` geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1496">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="f6f7d-1497">[BREAKING CHANGE] Parameter `--ask` von `content-key-policy create` geändert, sodass eine hexadezimale Zeichenfolge mit 32 Zeichen anstelle von UTF8 verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1497">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1498">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1498">AppService</span></span>

* <span data-ttu-id="f6f7d-1499">Befehle vom Typ `webapp config access-restriction show|set|add|remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1499">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="f6f7d-1500">Bessere Fehlerbehandlung zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1500">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="f6f7d-1501">Unterstützung für SKU `Isolated` zu `appservice plan update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1501">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-1502">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1502">ARM</span></span>

* <span data-ttu-id="f6f7d-1503">Parameter `--handle-extended-json-format` zu `deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1503">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-1504">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1504">Compute</span></span>

* <span data-ttu-id="f6f7d-1505">Parameter `--enable-agent` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1505">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="f6f7d-1506">`vm create` geändert, um bei der Verwendung von Zonen die SKU „Standard“ für die öffentliche IP-Adresse zu verwenden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1506">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="f6f7d-1507">`vm create` geändert, um automatisch einen gültigen Computernamen für eine VM zu erstellen, falls keiner angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1507">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="f6f7d-1508">Parameter `--computer-name-prefix` zu `vmss create` hinzugefügt, um das benutzerdefinierte Computernamenspräfix virtueller Computer in VMSS zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1508">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="f6f7d-1509">Parameter `--workspace` zu `vm create` hinzugefügt, um automatisch einen Log Analytics-Arbeitsbereich zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1509">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="f6f7d-1510">API-Version für Kataloge auf 2019-07-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1510">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-1511">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1511">Core</span></span>

* <span data-ttu-id="f6f7d-1512">Syntaxprüfung für Parameter `--set` im generischen Updatebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1512">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-1513">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1513">IoT</span></span>

* <span data-ttu-id="f6f7d-1514">Problem behoben, bei dem für `iot hub show` der Fehler „Ressource nicht gefunden.“ zurückgegeben wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1514">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-1515">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1515">Monitor</span></span>

* <span data-ttu-id="f6f7d-1516">Unterstützung für CRUD zu `monitor log-analytics workspace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1516">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1517">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1517">Network</span></span>

* <span data-ttu-id="f6f7d-1518">Unterstützung für mandantenübergreifende virtuelle Verbindung zu `network private-dns link vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1518">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="f6f7d-1519">[BREAKING CHANGE]`network vnet subnet list` geändert, um Parameter `--resource-group` und `--vnet-name` vorauszusetzen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1519">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-1520">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1520">SQL</span></span>

* <span data-ttu-id="f6f7d-1521">Befehle zu `sql mi ad-admin` hinzugefügt, die das Festlegen eines AAD-Administrators für verwaltete Instanzen unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1521">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1522">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1522">Storage</span></span>

* <span data-ttu-id="f6f7d-1523">Parameter `--preserve-s2s-access-tier` zu `storage copy` hinzugefügt, um die Zugriffsebene beim Kopieren von Dienst zu Dienst beizubehalten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1523">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="f6f7d-1524">Parameter `--enable-large-file-share` zu `storage account [create|update]` hinzugefügt, um große Dateifreigaben für ein Speicherkonto zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1524">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="f6f7d-1525">24. September 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1525">September 24, 2019</span></span>

<span data-ttu-id="f6f7d-1526">Version 2.0.74</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1526">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1527">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1527">ACR</span></span>

* <span data-ttu-id="f6f7d-1528">Erforderlicher Parameter `--type` zu `acr config retention update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1528">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="f6f7d-1529">[BREAKING CHANGE] Umbenannter Parameter `--name -n` in `--registry -r ` für Befehlsgruppe `acr config` geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1529">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-1530">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1530">AKS</span></span>

* <span data-ttu-id="f6f7d-1531">Parameter `--load-balancer-sku` zum Befehl `aks create` hinzugefügt, um die Erstellung von AKS-Clustern mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1531">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="f6f7d-1532">Parameter `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` und `--load-balancer-outbound-ip-prefixes` zu den Befehlen `aks [create|update]` hinzugefügt,um die Aktualisierung des Lastenausgleichsprofils eines AKS-Clusters mit SLB zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1532">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="f6f7d-1533">Parameter `--vm-set-type` zum Befehl `aks create` hinzugefügt, um die Angabe von VM-Typen eines AKS-Clusters (vmas oder vmss) zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1533">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-1534">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1534">ARM</span></span>

* <span data-ttu-id="f6f7d-1535">Parameter `--handle-extended-json-format` zum Befehl `group deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1535">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-1536">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1536">Compute</span></span>

* <span data-ttu-id="f6f7d-1537">Parameter `--terminate-notification-time` zu den Befehlen `vmss [create|update]` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1537">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="f6f7d-1538">Parameter `--enable-terminate-notification` zu den Befehlen `vmss update` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1538">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="f6f7d-1539">Parameter `--priority,` `--eviction-policy,` `--max-billing` zu `[vm|vmss] create`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1539">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="f6f7d-1540">`disk create` geändert, um die Angabe der genauen Größe des Datenträgeruploads zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1540">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="f6f7d-1541">Unterstützung für inkrementelle Momentaufnahmen für verwaltete Datenträger zu `snapshot create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1541">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f6f7d-1542">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1542">Cosmos DB</span></span>

* <span data-ttu-id="f6f7d-1543">Parameter `--type <key-type>` zum Befehl `cosmosdb keys list` hinzugefügt, um Schlüssel, schreibgeschützte Schlüssel oder Verbindungszeichenfolgen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1543">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="f6f7d-1544">Befehl `cosmosdb keys regenerate` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1544">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="f6f7d-1545">[VERALTET] Befehle `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` und `cosmosdb list-read-only-keys` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1545">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f6f7d-1546">EventGrid</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1546">EventGrid</span></span>

* <span data-ttu-id="f6f7d-1547">Endpunkthilfetext korrigiert, um auf den richtigen Parameter zu verweisen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1547">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6f7d-1548">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1548">Key Vault</span></span>

* <span data-ttu-id="f6f7d-1549">Problem behoben, aufgrund dessen die Anmeldung mit einem Mandanten (`login -t`) unter Umständen zu einem Fehler von `keyvault create` führte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1549">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-1550">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1550">Monitor</span></span>

* <span data-ttu-id="f6f7d-1551">Problem behoben, aufgrund dessen das Zeichen `:` in `--condition` für `monitor metrics alert create` nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1551">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="f6f7d-1552">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1552">Policy</span></span>

* <span data-ttu-id="f6f7d-1553">Unterstützung für Policy-API-Version 2019-06-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1553">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="f6f7d-1554">Parameter `--enforcement-mode` zum Befehl `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1554">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1555">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1555">Storage</span></span>

* <span data-ttu-id="f6f7d-1556">Parameter `--blob-type` zum Befehl `az storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1556">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="f6f7d-1557">10. September 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1557">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1558">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1558">ACR</span></span>

* <span data-ttu-id="f6f7d-1559">Befehlsgruppe `acr config retention` zum Konfigurieren der Aufbewahrungsrichtlinie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1559">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-1560">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1560">AKS</span></span>

* <span data-ttu-id="f6f7d-1561">Unterstützung für die ACR-Integration mit den folgenden Befehlen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1561">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="f6f7d-1562">Parameter `--attach-acr` zu `aks [create|update]` hinzugefügt, um einen ACR an einen AKS-Cluster anzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1562">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="f6f7d-1563">Parameter `--detach-acr` zu `aks update` hinzugefügt, um den ACR von einem AKS-Cluster zu trennen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1563">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-1564">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1564">ARM</span></span>

* <span data-ttu-id="f6f7d-1565">Zur Verwendung der API-Version 2019-05-10 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1565">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-1566">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1566">Batch</span></span>

* <span data-ttu-id="f6f7d-1567">Neue JSON-Konfigurationseinstellungen für `batch pool create` zu `--json-file` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1567">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="f6f7d-1568">`MountConfigurations` für Dateisystemeinbindungen hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1568">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="f6f7d-1569">Optionale Eigenschaft `publicIPs` in `NetworkConfiguration` für öffentliche IP-Adressen für Pools hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1569">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="f6f7d-1570">Unterstützung für Kataloge mit freigegebenen Images zu `--image` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1570">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="f6f7d-1571">[BREAKING CHANGE] Standardwert von `--start-task-wait-for-success` für `batch pool create` in `true` geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1571">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="f6f7d-1572">[BREAKING CHANGE] Standardwert von `Scope` für `AutoUserSpecification` geändert, damit immer „Pool“ verwendet wird (vormals `Task` für Windows-Knoten bzw. `Pool` für Linux-Knoten)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1572">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="f6f7d-1573">Dieses Argument kann nur über eine JSON-Konfiguration mit `--json-file` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1573">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-1574">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1574">HDInsight</span></span>

* <span data-ttu-id="f6f7d-1575">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1575">GA release</span></span>
* <span data-ttu-id="f6f7d-1576">[BREAKING CHANGE] Parameter `--workernode-count/-c` von `az hdinsight resize` in erforderlich geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1576">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6f7d-1577">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1577">Key Vault</span></span>

* <span data-ttu-id="f6f7d-1578">Problem behoben, aufgrund dessen Subnetze nicht aus Netzwerkregeln gelöscht werden konnten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1578">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="f6f7d-1579">Problem behoben, aufgrund dessen doppelte Subnetze und IP-Adressen zu Netzwerkregeln hinzugefügt werden konnten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1579">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1580">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1580">Network</span></span>

* <span data-ttu-id="f6f7d-1581">Parameter `--interval` zu `network watcher flow-log` hinzugefügt, um den Wert für das Intervall der Datenverkehrsanalyse festzulegen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1581">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="f6f7d-1582">`network application-gateway identity` zum Verwalten der Gatewayidentität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1582">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="f6f7d-1583">Unterstützung zum Festlegen der Key Vault-ID zu `network application-gateway ssl-cert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1583">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="f6f7d-1584">`network express-route peering peer-connection [show|list]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1584">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="f6f7d-1585">Richtlinie</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1585">Policy</span></span>

* <span data-ttu-id="f6f7d-1586">Zur Verwendung der API-Version 2019-01-01 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1586">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="f6f7d-1587">27. August 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1587">August 27, 2019</span></span>

<span data-ttu-id="f6f7d-1588">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1588">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1589">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1589">ACR</span></span>

* <span data-ttu-id="f6f7d-1590">[BREAKING CHANGE] Unterstützung für SKU `classic` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1590">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="f6f7d-1591">API Management</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1591">API Management</span></span>

* <span data-ttu-id="f6f7d-1592">[VORSCHAU] Befehlsgruppe `apim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1592">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1593">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1593">AppService</span></span>

* <span data-ttu-id="f6f7d-1594">Problem mit dem Befehl `webapp webjob continuous start` bei Angabe eines Slots behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1594">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="f6f7d-1595">`webapp up` geändert, um den Ordner `env` zu erkennen und aus der für die Bereitstellung verwendeten Datei zu entfernen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1595">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-1596">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1596">Keyvault</span></span>

* <span data-ttu-id="f6f7d-1597">Fehler in `keyvault secret set` behoben, aufgrund dessen das Argument `--expires` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1597">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1598">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1598">Network</span></span>

* <span data-ttu-id="f6f7d-1599">Unterstützung für IPv6-Adressen zu Argumenten vom Typ `--private-ip-address-version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1599">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="f6f7d-1600">Neue Befehle vom Typ `network private-endpoint [create|update|list-types]` für die Verwaltung privater Endpunkte hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1600">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="f6f7d-1601">Befehlsgruppe `network private-link-service` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1601">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="f6f7d-1602">Argumente `--private-endpoint-network-policies` und `--private-link-service-network-policies` zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1602">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-1603">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1603">RBAC</span></span>

* <span data-ttu-id="f6f7d-1604">Problem mit `ad app update --homepage` behoben, aufgrund dessen die Startseite nicht aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1604">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="f6f7d-1605">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1605">ServiceFabric</span></span>

* <span data-ttu-id="f6f7d-1606">Unterstützung für Key Vault-Namen mit Groß- und Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1606">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="f6f7d-1607">Problem bei der Verwendung von Zertifikaten in Key Vault behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1607">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="f6f7d-1608">Problem bei der Verwendung von PFX-Zertifikatdateien behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1608">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="f6f7d-1609">Problem mit `sf cluster certificate add` behoben, wenn keine Key Vault-Ressourcengruppe angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1609">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="f6f7d-1610">Problem behoben, aufgrund dessen `sf cluster set` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1610">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="f6f7d-1611">SignalR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1611">SignalR</span></span>

* <span data-ttu-id="f6f7d-1612">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1612">Added new commands:</span></span>
  * <span data-ttu-id="f6f7d-1613">`signalr cors`: Verwalten von CORS für SignalR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1613">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="f6f7d-1614">`signalr restart`: Starten eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1614">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="f6f7d-1615">`signalr update`: Aktualisieren eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1615">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="f6f7d-1616">Argument `--service-mode` zu `signalr create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1616">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1617">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1617">Storage</span></span>

* <span data-ttu-id="f6f7d-1618">Befehl `storage account revoke-delegation-keys` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1618">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="f6f7d-1619">13. August 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1619">August 13, 2019</span></span>

<span data-ttu-id="f6f7d-1620">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1620">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1621">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1621">AppService</span></span>

* <span data-ttu-id="f6f7d-1622">Problem behoben, aufgrund dessen bei Befehlen vom Typ `webapp webjob continuous` für Slots Fehler auftraten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1622">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="f6f7d-1623">BotService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1623">BotService</span></span>

* <span data-ttu-id="f6f7d-1624">[BREAKING CHANGE] Unterstützung für die Erstellung von Bots der Version 3 entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1624">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="f6f7d-1625">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1625">CognitiveServices</span></span>

* <span data-ttu-id="f6f7d-1626">Befehle vom Typ `cognitiveservices account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1626">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f6f7d-1627">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1627">Cosmos DB</span></span>

* <span data-ttu-id="f6f7d-1628">Beim Aktualisieren mehrerer Schreibstandorte wurde eine Warnung entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1628">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="f6f7d-1629">CRUD-Befehle für CosmosDB SQL-, MongoDB-, Cassandra-, Gremlin- und Tabellenressourcen sowie den Ressourcendurchsatz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1629">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-1630">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1630">HDInsight</span></span>

<span data-ttu-id="f6f7d-1631">Dieses Release enthält zahlreiche wichtige Änderungen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1631">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="f6f7d-1632">[BREAKING CHANGE] Parameter für `hdinsight create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1632">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="f6f7d-1633">`--storage-default-container` in `--storage-container` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1633">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="f6f7d-1634">`--storage-default-filesystem` in `--storage-filesystem` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1634">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="f6f7d-1635">[BREAKING CHANGE] Das Argument `--name` von `application create` wurde so geändert, dass es den Anwendungsnamen anstelle des Clusternamens darstellt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1635">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="f6f7d-1636">Argument `--cluster-name` zu `application create` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1636">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="f6f7d-1637">[BREAKING CHANGE] Parameter für `application create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1637">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="f6f7d-1638">`--application-type` in `--type` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1638">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="f6f7d-1639">`--marketplace-identifier` in `--marketplace-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1639">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="f6f7d-1640">`--https-endpoint-access-mode` in `--access-mode` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1640">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="f6f7d-1641">`--https-endpoint-destination-port` in `--destination-port` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1641">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="f6f7d-1642">[BREAKING CHANGE] Parameter für `application create` entfernt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1642">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="f6f7d-1643">[WICHTIGE ÄNDERUNG] `--target-instance-count` für `hdinsight resize` in `--workernode-count` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1643">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="f6f7d-1644">[BREAKING CHANGE] Alle Befehle in der Gruppe `hdinsight script-action` wurden so geändert, dass sie den Parameter `--name` als Namen der Skriptaktion verwenden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1644">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="f6f7d-1645">Argument `--cluster-name` zu allen Befehlen vom Typ `hdinsight script-action` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1645">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="f6f7d-1646">[BREAKING CHANGE]`--script-execution-id` für alle Befehle vom Typ `hdinsight script-action` in `--execution-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1646">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="f6f7d-1647">[BREAKING CHANGE]`hdinsight script-action show` in `hdinsight script-action show-execution-details` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1647">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="f6f7d-1648">[WICHTIGE ÄNDERUNG] Parameter in `hdinsight script-action execute --roles` geändert, sodass sie durch Leerzeichen anstelle von Kommas getrennt sind</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1648">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="f6f7d-1649">[BREAKING CHANGE] Parameter `--persisted` für `hdinsight script-action list` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1649">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="f6f7d-1650">Der Parameter `hdinsight create --cluster-configurations` wurde so geändert, dass er einen Pfad zu einer lokalen JSON-Datei oder JSON-Zeichenfolge akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1650">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="f6f7d-1651">Befehl `hdinsight script-action list-execution-history` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1651">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="f6f7d-1652">`hdinsight monitor enable --workspace` geändert, um die ID oder den Namen eines Log Analytics-Arbeitsbereichs zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1652">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="f6f7d-1653">Argument `hdinsight monitor enable --primary-key` hinzugefügt. Dieses Argument wird benötigt, wenn eine Arbeitsbereichs-ID als Parameter angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1653">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="f6f7d-1654">Weitere Beispiele und aktualisierte Beschreibungen für Hilfemeldungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1654">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-1655">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1655">Interactive</span></span>

* <span data-ttu-id="f6f7d-1656">Ladefehler behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1656">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="f6f7d-1657">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1657">Kubernetes</span></span>

* <span data-ttu-id="f6f7d-1658">Änderung, um `https` zu verwenden, wenn der Dashboardcontainerport `https` verwendet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1658">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1659">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1659">Network</span></span>

* <span data-ttu-id="f6f7d-1660">Argument `--yes` hinzugefügt zu `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1660">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-1661">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1661">Profile</span></span>

* <span data-ttu-id="f6f7d-1662">Argument `--resource-type` zu `account get-access-token` zum Abrufen von Ressourcenzugriffstoken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1662">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="f6f7d-1663">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1663">ServiceFabric</span></span>

* <span data-ttu-id="f6f7d-1664">Alle unterstützten Betriebssystemversionen für „sf cluster create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1664">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="f6f7d-1665">Fehler beim Überprüfen des primären Zertifikats behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1665">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1666">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1666">Storage</span></span>

* <span data-ttu-id="f6f7d-1667">Befehl `storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1667">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="f6f7d-1668">30. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1668">July 30, 2019</span></span>

<span data-ttu-id="f6f7d-1669">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1669">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1670">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1670">ACR</span></span>

* <span data-ttu-id="f6f7d-1671">Problem #9952 behoben (Regression im Befehl `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1671">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="f6f7d-1672">Standardname des Generatorimages in `acr pack build` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1672">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1673">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1673">Appservice</span></span>

* <span data-ttu-id="f6f7d-1674">`webapp config ssl` geändert, um eine Meldung anzuzeigen, wenn eine Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1674">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="f6f7d-1675">Problem behoben, aufgrund dessen `functionapp create` den Speicherkontotypen `Standard_RAGRS` nicht akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1675">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="f6f7d-1676">Problem behoben, aufgrund dessen für `webapp up` ein Fehler auftrat, wenn für die Ausführung ältere Python-Versionen verwendet wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1676">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1677">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1677">Network</span></span>

* <span data-ttu-id="f6f7d-1678">Ungültiger Parameter `--ids` aus `network nic ip-config add` entfernt (Fehlerbehebungen #9861)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1678">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="f6f7d-1679">Fehlerbehebungen #9604.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1679">Fixes #9604.</span></span> <span data-ttu-id="f6f7d-1680">Parameter `--root-certs` zu `network application-gateway http-settings [create|update]` hinzugefügt, um vom Benutzer zugewiesene vertrauenswürdige Stammzertifikate zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1680">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="f6f7d-1681">Argument `--subscription` für `network dns record-set ns create` korrigiert (#9965)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1681">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-1682">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1682">RBAC</span></span>

* <span data-ttu-id="f6f7d-1683">Befehl `user update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1683">Added `user update` command</span></span>
* <span data-ttu-id="f6f7d-1684">[VERALTET]`--upn-or-object-id` in benutzerbezogenen Befehlen als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1684">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="f6f7d-1685">Verwenden Sie das Ersatzargument `--id`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1685">Use replacement argument `--id`</span></span>
* <span data-ttu-id="f6f7d-1686">Argument `--id` zu benutzerbezogenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1686">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-1687">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1687">SQL</span></span>

* <span data-ttu-id="f6f7d-1688">Verwaltungsbefehle für Schlüssel verwalteter Instanzen und TDE-Schutzvorrichtung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1688">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1689">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1689">Storage</span></span>

* <span data-ttu-id="f6f7d-1690">Befehl `storage remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1690">Added `storage remove` command</span></span>
* <span data-ttu-id="f6f7d-1691">Problem mit `storage blob update` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1691">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-1692">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1692">VM</span></span>

* <span data-ttu-id="f6f7d-1693">`list-skus` wurde geändert, um eine neuere API-Version für die Ausgabe von Zonendetails zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1693">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="f6f7d-1694">Standardwert `--single-placement-group` für `vmss create` in `false` geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1694">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="f6f7d-1695">Möglichkeit zum Auswählen von ZRS-Speicher-SKUs für `[snapshot|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1695">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="f6f7d-1696">Neue Befehlsgruppe `vm host` zur Unterstützung dedizierter Hosts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1696">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="f6f7d-1697">Parameter `--host` und `--host-group` für `vm create` hinzugefügt, um den dedizierten VM-Host festzulegen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1697">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="f6f7d-1698">16. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1698">July 16, 2019</span></span>

<span data-ttu-id="f6f7d-1699">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1699">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1700">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1700">Appservice</span></span>

* <span data-ttu-id="f6f7d-1701">`webapp identity`-Befehle geändert, um eine korrekte Fehlermeldung zurückzugeben, wenn „ResourceGroupName“ oder der App-Name ungültig sind</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1701">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="f6f7d-1702">`webapp list` korrigiert, sodass der korrekte Wert für „numberOfSites“ zurückgegeben wird, wenn „ResourceGroup“ nicht angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1702">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="f6f7d-1703">Nebeneffekte von `appservice plan create` und `webapp create` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1703">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-1704">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1704">Core</span></span>

* <span data-ttu-id="f6f7d-1705">Problem behoben, aufgrund dessen `--subscription` angezeigt wurde, obwohl nicht anwendbar</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1705">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-1706">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1706">Batch</span></span>

* <span data-ttu-id="f6f7d-1707">[BREAKING CHANGE]`batch pool node-agent-skus list` durch `batch pool supported-images list` ersetzt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1707">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="f6f7d-1708">Unterstützung für Sicherheitsregeln hinzugefügt, die den Netzwerkzugriff auf einen Pool basierend auf dem Quellport des Datenverkehrs blockieren, wenn die Option `--json-file` von `batch pool create network` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1708">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="f6f7d-1709">Unterstützung für die Ausführung der Aufgabe im Arbeitsverzeichnis des Containers oder der Batch-Aufgabe hinzugefügt, wenn die Option `--json-file` von `batch task create` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1709">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="f6f7d-1710">Fehler in Option `--application-package-references` von `batch pool create` behoben, aufgrund dessen nur Standardeinstellungen möglich waren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1710">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f6f7d-1711">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1711">Eventhubs</span></span>

* <span data-ttu-id="f6f7d-1712">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1712">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-1713">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1713">RDBMS</span></span>

* <span data-ttu-id="f6f7d-1714">Optionaler Parameter zum Angeben der Replikat-SKU für den Befehl zum Erstellen von Replikaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1714">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="f6f7d-1715">Problem mit CI-Testfehler bei der Erstellung von MySQL-Replikaten behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1715">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="f6f7d-1716">Relay</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1716">Relay</span></span>

* <span data-ttu-id="f6f7d-1717">Problem mit Hybridverbindung behoben, wenn die Client-Autorisierung deaktiviert ist [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1717">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="f6f7d-1718">Parameter `--requires-transport-security` zu `relay wcfrelay create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1718">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="f6f7d-1719">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1719">Servicebus</span></span>

* <span data-ttu-id="f6f7d-1720">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1720">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1721">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1721">Storage</span></span>

* <span data-ttu-id="f6f7d-1722">AADDS für Files für Speicherkontoaktualisierung aktiviert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1722">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="f6f7d-1723">Problem `storage blob service-properties update --set` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1723">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="f6f7d-1724">2\. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1724">July 2, 2019</span></span>

<span data-ttu-id="f6f7d-1725">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1725">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-1726">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1726">Core</span></span>

* <span data-ttu-id="f6f7d-1727">Befehlsmodule sind jetzt in einer einzelnen verteilbaren Python-Komponente zusammengefasst.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1727">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="f6f7d-1728">Die direkte Verwendung zahlreicher Pakete vom Typ `azure-cli-` in PyPI ist daher veraltet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1728">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="f6f7d-1729">Dadurch sollte sich die Installationsgröße reduzieren. Darüber hinaus sollte es nur Benutzer betreffen, die eine direkte Installation über `pip` ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1729">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1730">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1730">ACR</span></span>

* <span data-ttu-id="f6f7d-1731">Unterstützung für Trigger mit Timer zu Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1731">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1732">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1732">Appservice</span></span>

* <span data-ttu-id="f6f7d-1733">`functionapp create` wurde so geändert, das Application Insights standardmäßig aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1733">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="f6f7d-1734">[BREAKING CHANGE] Veralteter Befehl `functionapp devops-build` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1734">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="f6f7d-1735">Verwenden Sie stattdessen den neuen Befehl `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1735">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="f6f7d-1736">Unterstützung des Funktions-App-Plans für Linux-Verbrauch zu `functionapp deployment config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1736">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f6f7d-1737">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1737">Cosmos DB</span></span>

* <span data-ttu-id="f6f7d-1738">Unterstützung für das Deaktivieren von TTL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1738">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="f6f7d-1739">DLS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1739">DLS</span></span>

* <span data-ttu-id="f6f7d-1740">Aktualisierte ADLS-Version (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1740">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="f6f7d-1741">Feedback</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1741">Feedback</span></span>

* <span data-ttu-id="f6f7d-1742">Wird ein fehlgeschlagener Erweiterungsbefehl gemeldet, versucht `az feedback` nun, über den Index die Projekt-/Repository-URL der Erweiterung im Browser zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1742">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-1743">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1743">HDInsight</span></span>

* <span data-ttu-id="f6f7d-1744">[BREAKING CHANGE] Der Befehlsgruppenname `oms` wurde in `monitor` geändert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1744">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="f6f7d-1745">[BREAKING CHANGE]`--http-password/-p` als erforderlicher Parameter festgelegt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1745">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="f6f7d-1746">Vervollständigungen für `--cluster-admin-account` und `cluster-users-group-dns` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1746">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="f6f7d-1747">Parameter `cluster-users-group-dns` so geändert, dass er erforderlich ist, wenn `—esp` vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1747">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="f6f7d-1748">Timeout für alle vorhandenen automatischen Argumentvervollständigungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1748">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="f6f7d-1749">Timeout für das Transformieren des Ressourcennamens in eine Ressourcen-ID hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1749">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="f6f7d-1750">Die automatischen Vervollständigungen wurden so geändert, dass Ressourcen aus einer beliebigen Ressourcengruppe ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1750">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="f6f7d-1751">Dabei kann es sich um eine andere Ressourcengruppe als die mit `-g` angegebene Gruppe handeln.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1751">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="f6f7d-1752">Unterstützung für die Parameter `--sub-domain-suffix` und `--disable_gateway_auth` im Befehl `hdinsight application create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1752">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="f6f7d-1753">Verwaltete Dienste</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1753">Managed Services</span></span>

* <span data-ttu-id="f6f7d-1754">Befehlsmodul für verwaltete Dienste als Vorschau eingeführt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1754">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-1755">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1755">Profile</span></span>
* <span data-ttu-id="f6f7d-1756">Argument `--subscription` für Abmeldebefehl unterdrückt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1756">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-1757">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1757">RBAC</span></span>

* <span data-ttu-id="f6f7d-1758">[BREAKING CHANGE] Argument `--password` für `create-for-rbac` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1758">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="f6f7d-1759">Parameter `--assignee-principal-type` zum Befehl `create` hinzugefügt, um zeitweilige Fehler zu vermeiden, die durch die Replikationswartezeit des AAD-Graph-Servers verursacht werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1759">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="f6f7d-1760">Absturz in `ad signed-in-user` beim Auflisten von in Besitz befindlichen Objekten behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1760">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="f6f7d-1761">Problem behoben, aufgrund dessen `ad sp` nicht die richtige Anwendung über einen Dienstprinzipal fand</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1761">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-1762">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1762">RDBMS</span></span>

* <span data-ttu-id="f6f7d-1763">Unterstützung für die Replikation für MariaDB hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1763">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-1764">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1764">SQL</span></span>

* <span data-ttu-id="f6f7d-1765">Zulässige Werte für `sql db create --sample-name` dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1765">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1766">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1766">Storage</span></span>

* <span data-ttu-id="f6f7d-1767">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage blob generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1767">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="f6f7d-1768">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage container generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1768">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="f6f7d-1769">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1769">VM</span></span>

* <span data-ttu-id="f6f7d-1770">Fehler behoben, aufgrund dessen `vmss create` bei der Ausführung mit `--no-wait` eine Fehlermeldung zurückgab</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1770">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="f6f7d-1771">Die clientseitige Validierung für `vmss create --single-placement-group` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1771">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="f6f7d-1772">Es tritt kein Fehler auf, wenn `--single-placement-group` auf `true` und für `--instance-count` ein größerer Wert als 100 festgelegt wird oder wenn Verfügbarkeitszonen angegeben werden. Diese Validierung wird jedoch dem Computedienst überlassen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1772">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="f6f7d-1773">Problem behoben, aufgrund dessen bei der Verwendung von `--latest` für `[vm|vmss] extension image list` ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1773">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="f6f7d-1774">18. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1774">June 18, 2019</span></span>

<span data-ttu-id="f6f7d-1775">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1775">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-1776">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1776">Core</span></span>

<span data-ttu-id="f6f7d-1777">In diesem Release wird das neue [Preview]-Tag eingeführt, um Kunden gegenüber deutlich zu machen, dass sich eine Befehlsgruppe, ein Befehl oder ein Argument in der Vorschauphase befindet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1777">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="f6f7d-1778">Diese Information war zuvor im Hilfetext oder implizit durch die Versionsnummer des Befehlsmoduls angegeben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1778">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="f6f7d-1779">Die Befehlszeilenschnittstelle wird künftig Versionsnummern für einzelne Pakete entfernen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1779">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="f6f7d-1780">Wenn sich ein Befehl in der Vorschauphase befindet, gilt dies auch für alle seine Argumente.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1780">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="f6f7d-1781">Wenn eine Befehlsgruppe als Vorschau gekennzeichnet ist, befinden sich auch alle Befehle und Argumente in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1781">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="f6f7d-1782">Infolge dieser Änderung befinden sich in diesem Release verschiedene Befehlsgruppen anscheinend „plötzlich“ in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1782">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="f6f7d-1783">Tatsächlich ist es jedoch so, dass sich die meisten Pakete in der Vorschauphase befanden, in diesem Release jedoch als allgemein verfügbar gelten.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1783">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1784">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1784">ACR</span></span>
* <span data-ttu-id="f6f7d-1785">Befehl „acr check-health“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1785">Added 'acr check-health' command</span></span>
* <span data-ttu-id="f6f7d-1786">Verbesserte Fehlerbehandlung für AAD-Token und für das Abrufen externer Befehle</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1786">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-1787">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1787">ACS</span></span>
* <span data-ttu-id="f6f7d-1788">Veraltete ACS-Befehle werden jetzt in der Hilfeansicht ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1788">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-1789">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1789">AMS</span></span>
* <span data-ttu-id="f6f7d-1790">[BREAKING CHANGE] Änderung, damit ISO 8601-Zeitzeichenfolgen für „archive-window-length“ und „key-frame-interval-duration“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1790">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1791">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1791">AppService</span></span>
* <span data-ttu-id="f6f7d-1792">Standortbasiertes Routing für `webapp deleted list` und `webapp deleted restore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1792">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="f6f7d-1793">Problem behoben, aufgrund dessen in Azure Cloud Shell nicht auf die von einer Web-App protokollierte Ziel-URL („Sie können die App starten unter...“) geklickt werden konnte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1793">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="f6f7d-1794">Problem behoben, aufgrund dessen beim Erstellen von Apps bei einigen SKUs ein AlwaysOn-Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1794">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="f6f7d-1795">Vorabüberprüfung zu `[appservice|webapp] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1795">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="f6f7d-1796">`[webapp|functionapp] traffic-routing` korrigiert, damit der richtige actionHostName-Wert verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1796">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="f6f7d-1797">Slotunterstützung zu `functionapp`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1797">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-1798">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1798">Batch</span></span>
* <span data-ttu-id="f6f7d-1799">AAD-Authentifizierungsregression korrigiert, die von übermäßiger Berichterstellung für Authentifizierung mit gemeinsam verwendetem Schlüssel verursacht wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1799">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="f6f7d-1800">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1800">BatchAI</span></span>
* <span data-ttu-id="f6f7d-1801">BatchAI-Befehle sind jetzt veraltet und ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1801">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="f6f7d-1802">BotService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1802">BotService</span></span>
* <span data-ttu-id="f6f7d-1803">Für Befehle, die Version 3 des SDK unterstützen, wurden die Warnmeldungen „Support eingestellt“/„Wartungsmodus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1803">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6f7d-1804">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1804">CosmosDB</span></span>
* <span data-ttu-id="f6f7d-1805">[VERALTET] Der Befehl `cosmosdb list-keys` wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1805">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="f6f7d-1806">Befehl `cosmosdb keys list` hinzugefügt, er ersetzt `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1806">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="f6f7d-1807">`cosmsodb create/update`: Neues Format für „--location“ hinzugefügt, um das Festlegen der Eigenschaft „isZoneRedundant“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1807">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="f6f7d-1808">Das alte Format wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1808">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f6f7d-1809">EventGrid</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1809">EventGrid</span></span>
* <span data-ttu-id="f6f7d-1810">`eventgrid domain`-Befehle für CRUD-Vorgänge für Domänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1810">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="f6f7d-1811">`eventgrid domain topic`-Befehle für CRUD-Vorgänge für Domänenthemen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1811">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="f6f7d-1812">Argument `--odata-query` zu `eventgrid [topic|event-subscription] list` zum Filtern der Ergebnisse mithilfe von OData-Syntax hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1812">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="f6f7d-1813">`event-subscription create/update`: „servicebusqueue“ als neue Werte für den Parameter `--endpoint-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1813">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="f6f7d-1814">[BREAKING CHANGE] Unterstützung für `--included-event-types All` mit `eventgrid event-subscription [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1814">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-1815">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1815">HDInsight</span></span>
* <span data-ttu-id="f6f7d-1816">Unterstützung für den Parameter `--ssh-public-key` im Befehl vom Typ `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1816">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-1817">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1817">IoT</span></span>
* <span data-ttu-id="f6f7d-1818">Unterstützung für das erneute Generieren von Autorisierungsrichtlinienschlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1818">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="f6f7d-1819">SDK und Unterstützung für den Bereitstellungsdienst des DigitalTwin-Repositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1819">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1820">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1820">Network</span></span>
* <span data-ttu-id="f6f7d-1821">Zonenunterstützung für NAT Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1821">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="f6f7d-1822">Befehl `network list-service-tags` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1822">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="f6f7d-1823">Problem mit `dns zone import` behoben, aufgrund dessen Benutzer keine A-Platzhaltereinträge importieren konnten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1823">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="f6f7d-1824">Problem mit `watcher flow-log configure` behoben, aufgrund dessen die Flowprotokollierung in bestimmten Regionen nicht aktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1824">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-1825">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1825">Resource</span></span>
* <span data-ttu-id="f6f7d-1826">Befehl `az rest` zum Ausführen von REST-Aufrufen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1826">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="f6f7d-1827">Fehler behoben, der bei Verwendung von `policy assignment list` mit `--scope` auf Ressourcengruppen- oder Abonnementebene auftrat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1827">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="f6f7d-1828">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1828">ServiceBus</span></span>
* <span data-ttu-id="f6f7d-1829">Problem mit `servicebus topic create --max-size` behoben [Nr. 9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1829">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-1830">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1830">SQL</span></span>
* <span data-ttu-id="f6f7d-1831">`--location` wurde geändert und ist nun für `sql [server|mi] create` optional. Ohne Angabe wird der Ressourcengruppenstandort verwendet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1831">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="f6f7d-1832">Der Fehler, dass das Objekt „NoneType“ nicht wiederholbar ist, wurde für `sql db list-editions --available` behoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1832">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="f6f7d-1833">SQLVm</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1833">SQLVm</span></span>
* <span data-ttu-id="f6f7d-1834">[WICHTIGE ÄNDERUNG] `sql vm create` wurde geändert und erfordert nun den Parameter `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1834">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="f6f7d-1835">Änderung, um beim Erstellen oder Aktualisieren einer SQL-VM das Festlegen der SQL-Image-SKU zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1835">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1836">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1836">Storage</span></span>
* <span data-ttu-id="f6f7d-1837">Problem mit fehlendem Kontoschlüssel für `storage container generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1837">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="f6f7d-1838">Problem mit `storage blob sync` unter Linux behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1838">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-1839">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1839">VM</span></span>
* <span data-ttu-id="f6f7d-1840">[VORSCHAU] Befehle vom Typ `vm image template` zum Erstellen von VM-Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1840">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="f6f7d-1841">4\. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1841">June 4, 2019</span></span>

<span data-ttu-id="f6f7d-1842">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1842">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-1843">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1843">Core</span></span>
* <span data-ttu-id="f6f7d-1844">Fehler behoben, aufgrund dessen bei Befehlen ein Fehler auftrat, wenn `--output yaml` mit `--query` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1844">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1845">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1845">ACR</span></span>
* <span data-ttu-id="f6f7d-1846">Befehlsgruppe „acr pack“ zum Erstellen von Aufgaben zur Schnellerstellung mit Buildpacks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1846">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-1847">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1847">ACS</span></span>
* <span data-ttu-id="f6f7d-1848">Zulassen der Aktivierung/Deaktivierung des AKS-Add-Ons für das Kube-Dashboard</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1848">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="f6f7d-1849">Ausgeben einer benutzerfreundlichen Nachricht, wenn das Abonnement nicht in der Whitelist zur Verwendung von Azure Red Hat OpenShift enthalten ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1849">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-1850">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1850">Batch</span></span>
* <span data-ttu-id="f6f7d-1851">Bessere Fehlerbehandlung, wenn der Benutzer nicht bei einem Konto angemeldet ist \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1851">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-1852">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1852">IoT</span></span>
* <span data-ttu-id="f6f7d-1853">Unterstützung für manuelles Failover hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1853">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1854">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1854">Network</span></span>
* <span data-ttu-id="f6f7d-1855">Befehle vom Typ `network application-gateway waf-policy` hinzugefügt, um benutzerdefinierte WAF-Regeln zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1855">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="f6f7d-1856">Argumente `--waf-policy` und `--max-capacity` zu `network application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1856">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="f6f7d-1857">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1857">Resource</span></span>
* <span data-ttu-id="f6f7d-1858">Verbesserte Fehlermeldungen aus `deployment create`, wenn TTY nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1858">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-1859">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1859">Role</span></span>
* <span data-ttu-id="f6f7d-1860">Hilfetext aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1860">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-1861">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1861">Compute</span></span>
* <span data-ttu-id="f6f7d-1862">Unterstützung zu `vm create` für virtuelle Computer aus einem verwalteten Image mit Datenträger-LUNs hinzugefügt, die nicht bei 0 beginnen oder die Nummern überspringen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1862">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="f6f7d-1863">21. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1863">May 21, 2019</span></span>

<span data-ttu-id="f6f7d-1864">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1864">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-1865">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1865">Core</span></span>
* <span data-ttu-id="f6f7d-1866">Besseres Feedback für Authentifizierungsfehler hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1866">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="f6f7d-1867">Problem behoben, aufgrund dessen die CLI Erweiterungen lädt, die nicht mit der Core-Version kompatibel waren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1867">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="f6f7d-1868">Problem beim Starten behoben, wenn `clouds.config` beschädigt ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1868">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-1869">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1869">ACR</span></span>
* <span data-ttu-id="f6f7d-1870">Unterstützung für verwaltete Identitäten zu Aufgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1870">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-1871">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1871">ACS</span></span>
* <span data-ttu-id="f6f7d-1872">`openshift create`-Befehl bei der Verwendung mit dem AAD-Kundenclient korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1872">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1873">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1873">AppService</span></span>
* <span data-ttu-id="f6f7d-1874">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet – wird in der nächsten Version entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1874">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="f6f7d-1875">`functionapp devops-pipeline` geändert, um das Buildprotokoll von Azure DevOps im ausführlichen Modus abzurufen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1875">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="f6f7d-1876">[BREAKING CHANGE] Flag `--use_local_settings` aus dem Befehl `functionapp devops-pipeline` entfernt – kein Vorgang wurde ausgeführt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1876">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="f6f7d-1877">`webapp up` geändert, sodass die JSON-Ausgabe zurückgegeben wird, wenn `--logs` nicht verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1877">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="f6f7d-1878">Unterstützung hinzugefügt zum Schreiben von Standardressourcen in die lokale Konfiguration für `webapp up`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1878">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="f6f7d-1879">Unterstützung zu `webapp up` hinzugefügt für die erneute Bereitstellung einer App ohne Verwendung des `--location`-Arguments</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1879">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="f6f7d-1880">Problem behoben, bei dem für die ASP-Erstellung der Linux-SKU „Free“ der SKU-Wert „Free“ nicht funktioniert hat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1880">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="f6f7d-1881">BotService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1881">BotService</span></span>
* <span data-ttu-id="f6f7d-1882">Geändert, sodass Groß-/Kleinschreibung für `--lang`-Parameter für Befehle zulässig ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1882">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="f6f7d-1883">Beschreibung für das Befehlsmodul aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1883">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="f6f7d-1884">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1884">Consumption</span></span>
* <span data-ttu-id="f6f7d-1885">Fehlende erforderliche Parameter bei der Ausführung von `consumption usage list --billing-period-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1885">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-1886">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1886">IoT</span></span>
* <span data-ttu-id="f6f7d-1887">Unterstützung für das Auflisten aller Schlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1887">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1888">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1888">Network</span></span>
* [BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="f6f7d-1890">`--nat-gateway`-Argument zu `network vnet subnet [create|update]` für das Anfügen an ein NAT-Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1890">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="f6f7d-1891">Problem mit `dns zone import` behoben, aufgrund dessen Eintragsnamen keinem Datensatztyp entsprochen haben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1891">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-1892">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1892">RDBMS</span></span>
* <span data-ttu-id="f6f7d-1893">Postgres- und MySLQ-Unterstützung für die Georeplikation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1893">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-1894">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1894">RBAC</span></span>
* <span data-ttu-id="f6f7d-1895">Unterstützung für den Verwaltungsgruppenumfang zu `role assignment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1895">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-1896">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1896">Storage</span></span>
* <span data-ttu-id="f6f7d-1897">`storage blob sync`: Synchronisierungsbefehl für Speicherblob hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1897">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="f6f7d-1898">Compute</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1898">Compute</span></span>
* <span data-ttu-id="f6f7d-1899">`--computer-name` zu `vm create` zum Festlegen des Computernamens eines virtuellen Computers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1899">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="f6f7d-1900">`--ssh-key-value` umbenannt in `--ssh-key-values` für `[vm|vmss] create`: Jetzt können mehrere öffentliche SSH-Schlüsselwerte oder -pfade akzeptiert werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1900">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="f6f7d-1901">__Hinweis__ : Dies ist **kein** Breaking Change: `--ssh-key-value` wird korrekt analysiert, da nur eine Übereinstimmung mit `--ssh-key-values` besteht.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1901">__Note__ : This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="f6f7d-1902">`--type`-Argument von `ppg create` in optionales Argument geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1902">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="f6f7d-1903">6\. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1903">May 6, 2019</span></span>

<span data-ttu-id="f6f7d-1904">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1904">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-1905">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1905">ACS</span></span>
* <span data-ttu-id="f6f7d-1906">[BREAKING CHANGE] Flag `--fqdn` aus den `openshift`-Befehlen entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1906">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="f6f7d-1907">Geändert, sodass die allgemein verfügbare Azure Red Hat Openshift-API-Version verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1907">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="f6f7d-1908">Flag `customer-admin-group-id` wurde zu `openshift create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1908">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="f6f7d-1909">[ALLGEMEIN VERFÜGBAR] `(PREVIEW)` aus der `aks create`-Option `--network-policy` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1909">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1910">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1910">Appservice</span></span>
* <span data-ttu-id="f6f7d-1911">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1911">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="f6f7d-1912">Umbenannt in `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1912">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="f6f7d-1913">Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1913">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="f6f7d-1914">Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1914">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="f6f7d-1915">Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1915">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="f6f7d-1916">Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1916">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="f6f7d-1917">Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1917">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="f6f7d-1918">`webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1918">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="f6f7d-1919">Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1919">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="f6f7d-1920">Befehl `create-remote-connection` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1920">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-1921">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1921">Batch</span></span>
* <span data-ttu-id="f6f7d-1922">Fehler im Validierungssteuerelement für `--application-package-references`-Optionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1922">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="f6f7d-1923">Botservice</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1923">Botservice</span></span>
* <span data-ttu-id="f6f7d-1924">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass standardmäßig eine leerer Web-App-Bot erstellt wird (d. h. kein Bot wird in App Service bereitgestellt)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1924">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="f6f7d-1925">`--echo`-Flag zu `bot create` hinzugefügt, sodass das alte Verhalten mit `-v v4` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1925">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="f6f7d-1926">[BREAKING CHANGE] Standardwert von `--version` in `v4` geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1926">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="f6f7d-1927">__HINWEIS:__ `bot prepare-publish` verwendet weiterhin den alten Standard.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1927">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="f6f7d-1928">[BREAKING CHANGE]`--lang` geändert, sodass der Standard nicht mehr `Csharp` ist.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1928">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="f6f7d-1929">Wenn der Befehl `--lang` erfordert und dies nicht angegeben ist, wird der Befehl nun mit Fehler beendet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1929">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="f6f7d-1930">[BREAKING CHANGE]`--appid`- und `--password`-Argumente für `bot create` in erforderlich geändert, sie können jetzt über `ad app create` erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1930">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="f6f7d-1931">`--appid`- und `--password`-Validierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1931">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="f6f7d-1932">[BREAKING CHANGE]`bot create -v v4` geändert, sodass kein Speicherkonto bzw. keine Application Insights-Instanz erstellt oder verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1932">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="f6f7d-1933">[BREAKING CHANGE]`bot create -v v3` geändert, sodass eine Region erforderlich ist, in der Application Insights verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1933">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="f6f7d-1934">[BREAKING CHANGE]`bot update` geändert, sodass es sich jetzt nur auf spezifische Eigenschaften eines Bots auswirkt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1934">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="f6f7d-1935">[BREAKING CHANGE]`--lang`-Flags geändert, sodass `Javascript` anstelle von `Node` akzeptiert wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1935">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="f6f7d-1936">[BREAKING CHANGE]`Node` als zulässiger `--lang`-Wert entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1936">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="f6f7d-1937">[BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass `SCM_DO_BUILD_DURING_DEPLOYMENT` nicht mehr auf TRUE festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1937">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="f6f7d-1938">Alle Bereitstellungen über Kudu fungieren ihrem Standardverhalten entsprechend.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1938">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="f6f7d-1939">`bot download` für Bots ohne `.bot`-Dateien geändert, sodass die sprachspezifische Konfigurationsdatei mit Werten aus den Anwendungseinstellungen für den Bot erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1939">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="f6f7d-1940">Unterstützung für `Typescript` zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1940">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="f6f7d-1941">Warnmeldung zu `bot prepare-deploy` für `Javascript`- und `Typescript`-Bots hinzugefügt, wenn `package.json` in `--code-dir` nicht enthalten ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1941">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="f6f7d-1942">`bot prepare-deploy` geändert, sodass bei Erfolg `true` zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1942">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="f6f7d-1943">Ausführliche Protokollierung zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1943">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="f6f7d-1944">Mehr verfügbare Application Insights-Regionen zu `az bot create -v v3` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1944">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="f6f7d-1945">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1945">Configure</span></span>
* <span data-ttu-id="f6f7d-1946">Unterstützung für die ordnerbasierte Argument-Standardwertkonfigurationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1946">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f6f7d-1947">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1947">Eventhubs</span></span>
* <span data-ttu-id="f6f7d-1948">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1948">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="f6f7d-1949">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1949">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1950">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1950">Network</span></span>
* <span data-ttu-id="f6f7d-1951">[BREAKING CHANGE]`--cache`-Argument mit `--defer` für `vnet [create|update]` ersetzt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1951">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="f6f7d-1952">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1952">Policy Insights</span></span>
* <span data-ttu-id="f6f7d-1953">Unterstützung für `--expand PolicyEvaluationDetails` hinzugefügt, sodass Richtlinienauswertungsdetails von der Ressource abgefragt werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1953">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-1954">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1954">Role</span></span>
* <span data-ttu-id="f6f7d-1955">[VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1955">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="f6f7d-1956">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1956">Service Bus</span></span>
* <span data-ttu-id="f6f7d-1957">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1957">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="f6f7d-1958">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1958">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="f6f7d-1959">`topic [create|update]` korrigiert, sodass `--max-size`-Unterstützung für 10-, 20-, 40- und 80-GB-Werte mit Premium-SKU zulässig ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1959">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-1960">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1960">SQL</span></span>
* <span data-ttu-id="f6f7d-1961">Befehle vom Typ `sql virtual-cluster [list|show|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1961">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-1962">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1962">VM</span></span>
* <span data-ttu-id="f6f7d-1963">`--protect-from-scale-in` und `--protect-from-scale-set-actions` zu `vmss update` hinzugefügt, sodass Aktualisierungen der Schutzrichtlinie von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1963">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="f6f7d-1964">`--instance-id` zu `vmss update` hinzugefügt, sodass allgemeine Aktualisierungen von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1964">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="f6f7d-1965">`--instance-id` zu `vmss wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1965">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="f6f7d-1966">Neue `ppg`-Befehlsgruppe für die Verwaltung von Näherungsplatzierungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1966">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="f6f7d-1967">`--ppg` zu `[vm|vmss] create` und `vm availability-set create` für die Verwaltung von PPGs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1967">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="f6f7d-1968">Parameter `--hyper-v-generation` zu `image create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1968">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="f6f7d-1969">23. April 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1969">April 23, 2019</span></span>

<span data-ttu-id="f6f7d-1970">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1970">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-1971">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1971">ACS</span></span>
* <span data-ttu-id="f6f7d-1972">`aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1972">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="f6f7d-1973">`(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1973">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-1974">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1974">AMS</span></span>
* <span data-ttu-id="f6f7d-1975">Fehler bei der Objekt- und Kontofilteraktualisierung behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1975">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-1976">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1976">AppService</span></span>
* <span data-ttu-id="f6f7d-1977">Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1977">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="f6f7d-1978">Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1978">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="f6f7d-1979">`--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1979">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="f6f7d-1980">`--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1980">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="f6f7d-1981">Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1981">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="f6f7d-1982">Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1982">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="f6f7d-1983">`webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1983">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="f6f7d-1984">`-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1984">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="f6f7d-1985">`webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1985">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="f6f7d-1986">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1986">Deployment Manager</span></span>
* <span data-ttu-id="f6f7d-1987">[VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1987">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="f6f7d-1988">Labor</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1988">Lab</span></span>
* <span data-ttu-id="f6f7d-1989">Fehler behoben, der zu einer vorzeitigen Beendigung führen würde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1989">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-1990">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1990">Network</span></span>
* <span data-ttu-id="f6f7d-1991">Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1991">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-1992">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1992">Resource</span></span>
* <span data-ttu-id="f6f7d-1993">[VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1993">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="f6f7d-1994">Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1994">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="f6f7d-1995">Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1995">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="f6f7d-1996">Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1996">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-1997">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1997">SQL</span></span>
* <span data-ttu-id="f6f7d-1998">Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1998">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="f6f7d-1999">Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-1999">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="f6f7d-2000">Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2000">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="f6f7d-2001">Befehl `sql server wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2001">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2002">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2002">Storage</span></span>
* <span data-ttu-id="f6f7d-2003">Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2003">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2004">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2004">VM</span></span>
* <span data-ttu-id="f6f7d-2005">`--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2005">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="f6f7d-2006">`--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2006">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="f6f7d-2007">`--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2007">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="f6f7d-2008">9\. April 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2008">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2009">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2009">Core</span></span>
* <span data-ttu-id="f6f7d-2010">Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2010">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2011">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2011">ACR</span></span>
* <span data-ttu-id="f6f7d-2012">Unterstützung für die kontextlose Ausführung eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2012">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-2013">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2013">AMS</span></span>
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="f6f7d-2016">Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2016">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="f6f7d-2017">Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2017">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2018">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2018">AppService</span></span>
* <span data-ttu-id="f6f7d-2019">Unterstützung für `--logs` zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2019">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="f6f7d-2020">Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2020">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="f6f7d-2021">Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2021">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="f6f7d-2022">[BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2022">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="f6f7d-2023">Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2023">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="f6f7d-2024">Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2024">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="f6f7d-2025">Unterstützung für Einstellungen zum Aufskalieren für den Azure Functions-Premium-Plan hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2025">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="f6f7d-2026">CDN</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2026">CDN</span></span>
* <span data-ttu-id="f6f7d-2027">Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2027">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="f6f7d-2028">Feedback</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2028">Feedback</span></span>
* <span data-ttu-id="f6f7d-2029">`feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2029">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="f6f7d-2030">`feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2030">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="f6f7d-2031">`feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2031">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-2032">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2032">Monitor</span></span>
* <span data-ttu-id="f6f7d-2033">Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2033">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="f6f7d-2034">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2034">Network</span></span>
* <span data-ttu-id="f6f7d-2035">Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2035">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="f6f7d-2036">Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2036">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="f6f7d-2037">Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2037">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="f6f7d-2038">Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2038">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="f6f7d-2039">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2039">PrivateDNS</span></span>
* <span data-ttu-id="f6f7d-2040">`network private-dns` für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2040">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-2041">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2041">Resource</span></span>
* <span data-ttu-id="f6f7d-2042">Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2042">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-2043">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2043">Role</span></span>
* <span data-ttu-id="f6f7d-2044">`create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2044">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="f6f7d-2045">[BREAKING CHANGE]`role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2045">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-2046">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2046">SQL</span></span>
* <span data-ttu-id="f6f7d-2047">`sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2047">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2048">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2048">Storage</span></span>
* <span data-ttu-id="f6f7d-2049">[BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2049">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="f6f7d-2050">`--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2050">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="f6f7d-2051">`--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2051">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="f6f7d-2052">`storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2052">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="f6f7d-2053">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2053">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="f6f7d-2054">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2054">Core</span></span>
* <span data-ttu-id="f6f7d-2055">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2055">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="f6f7d-2056">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2056">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="f6f7d-2057">Cloud</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2057">Cloud</span></span>
* <span data-ttu-id="f6f7d-2058">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2058">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2059">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2059">ACR</span></span>
* <span data-ttu-id="f6f7d-2060">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2060">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="f6f7d-2061">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2061">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="f6f7d-2062">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2062">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="f6f7d-2063">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2063">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2064">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2064">AppService</span></span>
* <span data-ttu-id="f6f7d-2065">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2065">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="f6f7d-2066">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2066">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="f6f7d-2067">Bot Service</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2067">BOT Service</span></span>
* <span data-ttu-id="f6f7d-2068">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2068">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="f6f7d-2069">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2069">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="f6f7d-2070">[BREAKING CHANGE]`--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2070">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="f6f7d-2071">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2071">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="f6f7d-2072">CDN</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2072">CDN</span></span>
* <span data-ttu-id="f6f7d-2073">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2073">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="f6f7d-2074">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2074">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="f6f7d-2075">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2075">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="f6f7d-2076">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2076">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6f7d-2077">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2077">Cosmosdb</span></span>
* <span data-ttu-id="f6f7d-2078">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2078">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="f6f7d-2079">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2079">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-2080">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2080">Interactive</span></span>
* <span data-ttu-id="f6f7d-2081">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2081">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-2082">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2082">Monitor</span></span>
* <span data-ttu-id="f6f7d-2083">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2083">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2084">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2084">Network</span></span>
* <span data-ttu-id="f6f7d-2085">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2085">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-2086">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2086">Profile</span></span>
* <span data-ttu-id="f6f7d-2087">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2087">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="f6f7d-2088">Postgres</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2088">Postgres</span></span> 
* <span data-ttu-id="f6f7d-2089">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2089">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="f6f7d-2090">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2090">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-2091">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2091">Resource</span></span>
* <span data-ttu-id="f6f7d-2092">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2092">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="f6f7d-2093">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2093">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="f6f7d-2094">Graph</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2094">Graph</span></span>
* <span data-ttu-id="f6f7d-2095">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2095">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="f6f7d-2096">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2096">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="f6f7d-2097">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2097">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="f6f7d-2098">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2098">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="f6f7d-2099">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2099">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2100">storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2100">storage</span></span>
* <span data-ttu-id="f6f7d-2101">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2101">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="f6f7d-2102">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2102">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="f6f7d-2103">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2103">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="f6f7d-2104">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2104">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2105">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2105">VM</span></span>
* <span data-ttu-id="f6f7d-2106">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2106">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="f6f7d-2107">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2107">March 12, 2019</span></span>

<span data-ttu-id="f6f7d-2108">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2108">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2109">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2109">Core</span></span>

* <span data-ttu-id="f6f7d-2110">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2110">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2111">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2111">ACR</span></span>

* <span data-ttu-id="f6f7d-2112">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2112">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2113">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2113">ACS</span></span>

* <span data-ttu-id="f6f7d-2114">Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2114">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="f6f7d-2115">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2115">AppService</span></span>

* <span data-ttu-id="f6f7d-2116">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2116">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="f6f7d-2117">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2117">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="f6f7d-2118">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2118">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="f6f7d-2119">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2119">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="f6f7d-2120">Botservice</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2120">Botservice</span></span>

* <span data-ttu-id="f6f7d-2121">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2121">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="f6f7d-2122">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2122">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="f6f7d-2123">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2123">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="f6f7d-2124">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2124">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-2125">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2125">Container</span></span>

* <span data-ttu-id="f6f7d-2126">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2126">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="f6f7d-2127">EventHub</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2127">EventHub</span></span>

* <span data-ttu-id="f6f7d-2128">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2128">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="f6f7d-2129">Suchen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2129">Find</span></span>

* <span data-ttu-id="f6f7d-2130">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2130">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-2131">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2131">HDInsight</span></span>

* <span data-ttu-id="f6f7d-2132">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2132">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2133">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2133">Network</span></span>

* <span data-ttu-id="f6f7d-2134">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2134">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-2135">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2135">Rdbms</span></span>

* <span data-ttu-id="f6f7d-2136">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2136">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-2137">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2137">Role</span></span>

* <span data-ttu-id="f6f7d-2138">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2138">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="f6f7d-2139">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2139">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f6f7d-2140">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2140">Service Fabric</span></span>

* <span data-ttu-id="f6f7d-2141">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2141">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="f6f7d-2142">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2142">February 26, 2019</span></span>

<span data-ttu-id="f6f7d-2143">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2143">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2144">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2144">Core</span></span>

* <span data-ttu-id="f6f7d-2145">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2145">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2146">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2146">ACR</span></span>

* <span data-ttu-id="f6f7d-2147">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2147">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="f6f7d-2148">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2148">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2149">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2149">ACS</span></span>

* <span data-ttu-id="f6f7d-2150">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2150">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2151">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2151">AppService</span></span>

* <span data-ttu-id="f6f7d-2152">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2152">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-2153">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2153">Batch</span></span>
* <span data-ttu-id="f6f7d-2154">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2154">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="f6f7d-2155">[BREAKING CHANGE]`Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2155">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="f6f7d-2156">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2156">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="f6f7d-2157">[BREAKING CHANGE]`--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2157">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="f6f7d-2158">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2158">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="f6f7d-2159">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2159">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6f7d-2160">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2160">CosmosDB</span></span>

* <span data-ttu-id="f6f7d-2161">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2161">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="f6f7d-2162">Kusto</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2162">Kusto</span></span>

* <span data-ttu-id="f6f7d-2163">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2163">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2164">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2164">Network</span></span>

* <span data-ttu-id="f6f7d-2165">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2165">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="f6f7d-2166">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2166">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="f6f7d-2167">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2167">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="f6f7d-2168">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2168">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="f6f7d-2169">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2169">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="f6f7d-2170">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2170">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="f6f7d-2171">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2171">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-2172">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2172">Resource</span></span>

* <span data-ttu-id="f6f7d-2173">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2173">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="f6f7d-2174">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2174">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="f6f7d-2175">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2175">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="f6f7d-2176">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2176">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="f6f7d-2177">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2177">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-2178">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2178">Role</span></span>

* <span data-ttu-id="f6f7d-2179">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2179">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2180">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2180">VM</span></span>

* <span data-ttu-id="f6f7d-2181">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2181">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="f6f7d-2182">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2182">February 12, 2019</span></span>

<span data-ttu-id="f6f7d-2183">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2183">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2184">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2184">Core</span></span>

* <span data-ttu-id="f6f7d-2185">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2185">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="f6f7d-2186">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2186">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2187">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2187">ACR</span></span>
* <span data-ttu-id="f6f7d-2188">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2188">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="f6f7d-2189">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2189">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2190">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2190">ACS</span></span>
* <span data-ttu-id="f6f7d-2191">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2191">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="f6f7d-2192">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2192">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="f6f7d-2193">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2193">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-2194">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2194">AMS</span></span>
* <span data-ttu-id="f6f7d-2195">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2195">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="f6f7d-2196">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2196">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2197">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2197">Appservice</span></span>
* <span data-ttu-id="f6f7d-2198">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2198">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="f6f7d-2199">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2199">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="f6f7d-2200">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2200">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="f6f7d-2201">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2201">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="f6f7d-2202">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2202">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="f6f7d-2203">Botservice</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2203">Botservice</span></span>
* <span data-ttu-id="f6f7d-2204">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2204">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="f6f7d-2205">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2205">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="f6f7d-2206">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2206">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="f6f7d-2207">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2207">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="f6f7d-2208">[VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2208">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="f6f7d-2209">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2209">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="f6f7d-2210">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2210">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="f6f7d-2211">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2211">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="f6f7d-2212">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2212">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="f6f7d-2213">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2213">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6f7d-2214">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2214">Key Vault</span></span>
* <span data-ttu-id="f6f7d-2215">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2215">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-2216">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2216">Monitor</span></span>
* <span data-ttu-id="f6f7d-2217">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2217">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2218">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2218">Network</span></span>
* <span data-ttu-id="f6f7d-2219">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2219">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="f6f7d-2220">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2220">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="f6f7d-2221">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2221">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="f6f7d-2222">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2222">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="f6f7d-2223">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2223">Policy Insights</span></span>
* <span data-ttu-id="f6f7d-2224">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2224">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-2225">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2225">RDBMS</span></span>
* <span data-ttu-id="f6f7d-2226">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2226">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="f6f7d-2227">Redis</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2227">Redis</span></span>
* <span data-ttu-id="f6f7d-2228">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2228">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="f6f7d-2229">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2229">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="f6f7d-2230">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2230">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="f6f7d-2231">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2231">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="f6f7d-2232">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2232">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="f6f7d-2233">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2233">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="f6f7d-2234">[VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2234">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-2235">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2235">Role</span></span>
* <span data-ttu-id="f6f7d-2236">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2236">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="f6f7d-2237">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2237">SQL VM</span></span>
* <span data-ttu-id="f6f7d-2238">[VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2238">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2239">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2239">VM</span></span>
* <span data-ttu-id="f6f7d-2240">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2240">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="f6f7d-2241">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2241">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="f6f7d-2242">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2242">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="f6f7d-2243">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2243">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="f6f7d-2244">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2244">January 31, 2019</span></span>

<span data-ttu-id="f6f7d-2245">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2245">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2246">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2246">Core</span></span>

* <span data-ttu-id="f6f7d-2247">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2247">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="f6f7d-2248">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2248">January 28, 2019</span></span>

<span data-ttu-id="f6f7d-2249">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2249">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2250">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2250">ACR</span></span>
* <span data-ttu-id="f6f7d-2251">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2251">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2252">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2252">ACS</span></span>
* <span data-ttu-id="f6f7d-2253">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2253">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="f6f7d-2254">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2254">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="f6f7d-2255">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2255">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-2256">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2256">AMS</span></span>
* <span data-ttu-id="f6f7d-2257">[BREAKING CHANGE]`ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2257">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="f6f7d-2258">[BREAKING CHANGE]`ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2258">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2259">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2259">Appservice</span></span>
* <span data-ttu-id="f6f7d-2260">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2260">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="f6f7d-2261">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2261">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="f6f7d-2262">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2262">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-2263">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2263">Container</span></span>
* <span data-ttu-id="f6f7d-2264">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2264">Added `container start` command</span></span>
* <span data-ttu-id="f6f7d-2265">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2265">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f6f7d-2266">EventGrid</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2266">EventGrid</span></span>
* <span data-ttu-id="f6f7d-2267">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2267">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="f6f7d-2268">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2268">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="f6f7d-2269">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2269">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="f6f7d-2270">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2270">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="f6f7d-2271">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2271">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-2272">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2272">HDInsight</span></span>
* <span data-ttu-id="f6f7d-2273">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2273">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="f6f7d-2274">[BREAKING CHANGE]`hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2274">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="f6f7d-2275">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2275">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="f6f7d-2276">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2276">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="f6f7d-2277">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2277">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="f6f7d-2278">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2278">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-2279">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2279">IoT</span></span>
* <span data-ttu-id="f6f7d-2280">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2280">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="f6f7d-2281">Kusto</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2281">Kusto</span></span>
* <span data-ttu-id="f6f7d-2282">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2282">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-2283">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2283">Monitor</span></span>
* <span data-ttu-id="f6f7d-2284">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2284">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-2285">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2285">Profile</span></span>
* <span data-ttu-id="f6f7d-2286">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2286">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2287">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2287">Network</span></span>
* <span data-ttu-id="f6f7d-2288">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2288">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="f6f7d-2289">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2289">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-2290">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2290">Resource</span></span>
* <span data-ttu-id="f6f7d-2291">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2291">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="f6f7d-2292">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2292">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="f6f7d-2293">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2293">SQL Virtual Machine</span></span>
* <span data-ttu-id="f6f7d-2294">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2294">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2295">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2295">Storage</span></span>
* <span data-ttu-id="f6f7d-2296">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2296">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="f6f7d-2297">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2297">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2298">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2298">VM</span></span>
* <span data-ttu-id="f6f7d-2299">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2299">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="f6f7d-2300">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2300">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="f6f7d-2301">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2301">January 15, 2019</span></span>

<span data-ttu-id="f6f7d-2302">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2302">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2303">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2303">ACR</span></span>
* <span data-ttu-id="f6f7d-2304">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2304">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="f6f7d-2305">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2305">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="f6f7d-2306">[VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2306">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="f6f7d-2307">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2307">ACS</span></span>
* <span data-ttu-id="f6f7d-2308">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2308">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2309">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2309">Appservice</span></span>
* <span data-ttu-id="f6f7d-2310">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2310">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="f6f7d-2311">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2311">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="f6f7d-2312">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2312">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="f6f7d-2313">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2313">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="f6f7d-2314">Botservice</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2314">Botservice</span></span>
* <span data-ttu-id="f6f7d-2315">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2315">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="f6f7d-2316">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2316">Configure</span></span>
* <span data-ttu-id="f6f7d-2317">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2317">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6f7d-2318">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2318">CosmosDB</span></span>
* <span data-ttu-id="f6f7d-2319">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2319">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-2320">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2320">HDInsight</span></span>
* <span data-ttu-id="f6f7d-2321">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2321">Added commands for managing applications</span></span>
* <span data-ttu-id="f6f7d-2322">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2322">Added commands for managing script actions</span></span>
* <span data-ttu-id="f6f7d-2323">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2323">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="f6f7d-2324">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2324">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="f6f7d-2325">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2325">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2326">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2326">Network</span></span>
* <span data-ttu-id="f6f7d-2327">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2327">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="f6f7d-2328">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2328">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="f6f7d-2329">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2329">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="f6f7d-2330">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2330">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-2331">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2331">Role</span></span>
* <span data-ttu-id="f6f7d-2332">[VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2332">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="f6f7d-2333">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2333">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="f6f7d-2334">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2334">Security</span></span>
* <span data-ttu-id="f6f7d-2335">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2335">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2336">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2336">Storage</span></span>
* <span data-ttu-id="f6f7d-2337">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2337">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="f6f7d-2338">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2338">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="f6f7d-2339">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2339">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="f6f7d-2340">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2340">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="f6f7d-2341">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2341">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2342">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2342">VM</span></span>
* <span data-ttu-id="f6f7d-2343">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2343">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="f6f7d-2344">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2344">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6f7d-2345">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2345">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="f6f7d-2346">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2346">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="f6f7d-2347">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2347">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="f6f7d-2348">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2348">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="f6f7d-2349">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2349">December 20, 2018</span></span>

<span data-ttu-id="f6f7d-2350">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2350">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="f6f7d-2351">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2351">Appservice</span></span>
* <span data-ttu-id="f6f7d-2352">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2352">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="f6f7d-2353">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2353">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="f6f7d-2354">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2354">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="f6f7d-2355">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2355">IoTCentral</span></span>
* <span data-ttu-id="f6f7d-2356">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2356">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-2357">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2357">Role</span></span>
* <span data-ttu-id="f6f7d-2358">[BREAKING CHANGE]`ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2358">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-2359">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2359">SQL</span></span>
* <span data-ttu-id="f6f7d-2360">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2360">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2361">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2361">VM</span></span>
* <span data-ttu-id="f6f7d-2362">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2362">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="f6f7d-2363">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2363">December 18, 2018</span></span>

<span data-ttu-id="f6f7d-2364">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2364">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="f6f7d-2365">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2365">ACR</span></span>
* <span data-ttu-id="f6f7d-2366">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2366">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="f6f7d-2367">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2367">Condensed the table layout for task list</span></span>
* <span data-ttu-id="f6f7d-2368">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2368">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2369">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2369">ACS</span></span>
* <span data-ttu-id="f6f7d-2370">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2370">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="f6f7d-2371">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2371">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="f6f7d-2372">[VERALTET]`az acs`-Befehle als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2372">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="f6f7d-2373">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2373">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="f6f7d-2374">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2374">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="f6f7d-2375">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2375">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2376">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2376">Appservice</span></span>
* <span data-ttu-id="f6f7d-2377">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2377">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="f6f7d-2378">Botservice</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2378">Botservice</span></span>
* <span data-ttu-id="f6f7d-2379">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2379">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="f6f7d-2380">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2380">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="f6f7d-2381">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2381">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="f6f7d-2382">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2382">Reduced Kudu network calls</span></span>
* <span data-ttu-id="f6f7d-2383">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2383">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="f6f7d-2384">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2384">Consumption</span></span>
* <span data-ttu-id="f6f7d-2385">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2385">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6f7d-2386">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2386">CosmosDB</span></span>
* <span data-ttu-id="f6f7d-2387">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2387">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="f6f7d-2388">Karten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2388">Maps</span></span>
* <span data-ttu-id="f6f7d-2389">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2389">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2390">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2390">Network</span></span>
* <span data-ttu-id="f6f7d-2391">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2391">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="f6f7d-2392">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2392">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-2393">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2393">Resource</span></span>
* <span data-ttu-id="f6f7d-2394">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2394">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="f6f7d-2395">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2395">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2396">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2396">Storage</span></span>
*  <span data-ttu-id="f6f7d-2397">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2397">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2398">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2398">VM</span></span>
* <span data-ttu-id="f6f7d-2399">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2399">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="f6f7d-2400">4\. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2400">December 4, 2018</span></span>

<span data-ttu-id="f6f7d-2401">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2401">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="f6f7d-2402">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2402">Core</span></span>
* <span data-ttu-id="f6f7d-2403">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2403">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="f6f7d-2404">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2404">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2405">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2405">Appservice</span></span>
* <span data-ttu-id="f6f7d-2406">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2406">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="f6f7d-2407">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2407">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2408">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2408">Network</span></span>
* <span data-ttu-id="f6f7d-2409">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2409">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-2410">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2410">Role</span></span>
* <span data-ttu-id="f6f7d-2411">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2411">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="f6f7d-2412">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2412">VM</span></span>
* <span data-ttu-id="f6f7d-2413">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2413">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="f6f7d-2414">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2414">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="f6f7d-2415">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2415">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="f6f7d-2416">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2416">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="f6f7d-2417">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2417">November 20, 2018</span></span>

<span data-ttu-id="f6f7d-2418">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2418">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="f6f7d-2419">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2419">Core</span></span>
* <span data-ttu-id="f6f7d-2420">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2420">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2421">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2421">ACR</span></span>
* <span data-ttu-id="f6f7d-2422">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2422">Added context token to task step</span></span>
* <span data-ttu-id="f6f7d-2423">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2423">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="f6f7d-2424">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2424">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2425">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2425">Appservice</span></span>
* <span data-ttu-id="f6f7d-2426">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2426">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="f6f7d-2427">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2427">Updated the default `node_version`.</span></span> <span data-ttu-id="f6f7d-2428">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2428">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="f6f7d-2429">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2429">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="f6f7d-2430">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2430">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="f6f7d-2431">IotCentral</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2431">IotCentral</span></span>
* <span data-ttu-id="f6f7d-2432">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2432">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-2433">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2433">KeyVault</span></span>
* <span data-ttu-id="f6f7d-2434">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2434">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2435">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2435">Network</span></span>
* <span data-ttu-id="f6f7d-2436">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2436">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="f6f7d-2437">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2437">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="f6f7d-2438">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2438">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="f6f7d-2439">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2439">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-2440">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2440">Rdbms</span></span>
* <span data-ttu-id="f6f7d-2441">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2441">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="f6f7d-2442">RBAC</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2442">Rbac</span></span>
* <span data-ttu-id="f6f7d-2443">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2443">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="f6f7d-2444">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2444">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="f6f7d-2445">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2445">Storage</span></span>
* <span data-ttu-id="f6f7d-2446">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2446">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="f6f7d-2447">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2447">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="f6f7d-2448">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2448">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="f6f7d-2449">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2449">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2450">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2450">VM</span></span>
* <span data-ttu-id="f6f7d-2451">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2451">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="f6f7d-2452">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2452">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="f6f7d-2453">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2453">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="f6f7d-2454">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2454">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="f6f7d-2455">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2455">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="f6f7d-2456">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2456">Added `snapshot wait` command</span></span>
* <span data-ttu-id="f6f7d-2457">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2457">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="f6f7d-2458">6\. November 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2458">November 6, 2018</span></span>

<span data-ttu-id="f6f7d-2459">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2459">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2460">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2460">Core</span></span>
* <span data-ttu-id="f6f7d-2461">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2461">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2462">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2462">ACR</span></span>
* <span data-ttu-id="f6f7d-2463">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2463">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="f6f7d-2464">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2464">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2465">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2465">ACS</span></span>
* <span data-ttu-id="f6f7d-2466">[BREAKING CHANGE]`enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2466">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="f6f7d-2467">Advisor</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2467">Advisor</span></span>
* <span data-ttu-id="f6f7d-2468">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2468">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-2469">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2469">AMS</span></span>
* <span data-ttu-id="f6f7d-2470">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2470">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="f6f7d-2471">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2471">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="f6f7d-2472">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2472">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="f6f7d-2473">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2473">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="f6f7d-2474">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2474">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="f6f7d-2475">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2475">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="f6f7d-2476">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2476">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="f6f7d-2477">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2477">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="f6f7d-2478">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2478">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="f6f7d-2479">[BREAKING CHANGE]`--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2479">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="f6f7d-2480">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2480">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="f6f7d-2481">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2481">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="f6f7d-2482">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2482">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="f6f7d-2483">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2483">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="f6f7d-2484">[BREAKING CHANGE]`--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2484">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="f6f7d-2485">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2485">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="f6f7d-2486">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2486">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2487">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2487">AppService</span></span>
* <span data-ttu-id="f6f7d-2488">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2488">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="f6f7d-2489">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2489">Configure</span></span>
* <span data-ttu-id="f6f7d-2490">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2490">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-2491">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2491">Container</span></span>
* <span data-ttu-id="f6f7d-2492">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2492">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="f6f7d-2493">EventHub</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2493">EventHub</span></span>
* <span data-ttu-id="f6f7d-2494">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2494">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-2495">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2495">Interactive</span></span>
* <span data-ttu-id="f6f7d-2496">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2496">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-2497">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2497">Monitor</span></span>
* <span data-ttu-id="f6f7d-2498">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2498">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2499">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2499">Network</span></span>
* <span data-ttu-id="f6f7d-2500">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2500">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="f6f7d-2501">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2501">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="f6f7d-2502">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2502">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="f6f7d-2503">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2503">Profile</span></span>
* <span data-ttu-id="f6f7d-2504">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2504">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-2505">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2505">RDBMS</span></span>
* <span data-ttu-id="f6f7d-2506">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2506">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-2507">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2507">Resource</span></span>
* <span data-ttu-id="f6f7d-2508">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2508">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-2509">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2509">Role</span></span>
* <span data-ttu-id="f6f7d-2510">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2510">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="f6f7d-2511">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2511">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="f6f7d-2512">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2512">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2513">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2513">Storage</span></span>
* <span data-ttu-id="f6f7d-2514">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2514">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2515">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2515">VM</span></span>
* <span data-ttu-id="f6f7d-2516">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2516">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="f6f7d-2517">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2517">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="f6f7d-2518">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2518">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="f6f7d-2519">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2519">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="f6f7d-2520">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2520">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="f6f7d-2521">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2521">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="f6f7d-2522">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2522">October 23, 2018</span></span>

<span data-ttu-id="f6f7d-2523">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2523">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2524">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2524">Core</span></span>
* <span data-ttu-id="f6f7d-2525">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2525">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="f6f7d-2526">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2526">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2527">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2527">ACR</span></span>
* <span data-ttu-id="f6f7d-2528">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2528">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="f6f7d-2529">CDN</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2529">CDN</span></span>
* <span data-ttu-id="f6f7d-2530">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2530">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="f6f7d-2531">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2531">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-2532">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2532">Container</span></span>
* <span data-ttu-id="f6f7d-2533">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2533">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="f6f7d-2534">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2534">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="f6f7d-2535">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2535">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="f6f7d-2536">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2536">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="f6f7d-2537">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2537">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="f6f7d-2538">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2538">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="f6f7d-2539">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2539">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6f7d-2540">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2540">CosmosDB</span></span>
* <span data-ttu-id="f6f7d-2541">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2541">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-2542">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2542">Interactive</span></span>
* <span data-ttu-id="f6f7d-2543">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2543">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="f6f7d-2544">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2544">IoT Central</span></span>
* <span data-ttu-id="f6f7d-2545">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2545">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="f6f7d-2546">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2546">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-2547">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2547">Monitor</span></span>
* <span data-ttu-id="f6f7d-2548">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2548">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="f6f7d-2549">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2549">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="f6f7d-2550">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2550">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="f6f7d-2551">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2551">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="f6f7d-2552">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2552">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="f6f7d-2553">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2553">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="f6f7d-2554">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2554">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="f6f7d-2555">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2555">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="f6f7d-2556">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2556">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="f6f7d-2557">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2557">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2558">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2558">Network</span></span>
* <span data-ttu-id="f6f7d-2559">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2559">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="f6f7d-2560">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2560">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="f6f7d-2561">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2561">ServiceBus</span></span>
* <span data-ttu-id="f6f7d-2562">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2562">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-2563">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2563">SQL</span></span>
* <span data-ttu-id="f6f7d-2564">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2564">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2565">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2565">Storage</span></span>
* <span data-ttu-id="f6f7d-2566">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2566">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="f6f7d-2567">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2567">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2568">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2568">VM</span></span>
* <span data-ttu-id="f6f7d-2569">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2569">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6f7d-2570">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2570">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="f6f7d-2571">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2571">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="f6f7d-2572">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2572">October 16, 2018</span></span>

<span data-ttu-id="f6f7d-2573">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2573">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2574">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2574">VM</span></span>
* <span data-ttu-id="f6f7d-2575">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2575">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="f6f7d-2576">9\. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2576">October 9, 2018</span></span>

<span data-ttu-id="f6f7d-2577">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2577">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2578">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2578">Core</span></span>
* <span data-ttu-id="f6f7d-2579">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2579">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2580">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2580">ACR</span></span>
* <span data-ttu-id="f6f7d-2581">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2581">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2582">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2582">ACS</span></span>
* <span data-ttu-id="f6f7d-2583">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2583">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="f6f7d-2584">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2584">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="f6f7d-2585">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2585">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="f6f7d-2586">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2586">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-2587">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2587">Container</span></span>
* <span data-ttu-id="f6f7d-2588">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2588">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="f6f7d-2589">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2589">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="f6f7d-2590">Event Hub</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2590">Event Hub</span></span>
* <span data-ttu-id="f6f7d-2591">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2591">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="f6f7d-2592">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2592">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="f6f7d-2593">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2593">Extensions</span></span>
* <span data-ttu-id="f6f7d-2594">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2594">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f6f7d-2595">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2595">HDInsight</span></span>
* <span data-ttu-id="f6f7d-2596">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2596">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-2597">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2597">IoT</span></span>
* <span data-ttu-id="f6f7d-2598">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2598">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-2599">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2599">KeyVault</span></span>
* <span data-ttu-id="f6f7d-2600">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2600">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2601">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2601">Network</span></span>
* <span data-ttu-id="f6f7d-2602">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2602">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="f6f7d-2603">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2603">See #6052</span></span>
* <span data-ttu-id="f6f7d-2604">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2604">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="f6f7d-2605">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2605">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="f6f7d-2606">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2606">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="f6f7d-2607">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2607">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="f6f7d-2608">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2608">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="f6f7d-2609">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2609">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-2610">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2610">Role</span></span>
* <span data-ttu-id="f6f7d-2611">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2611">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="f6f7d-2612">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2612">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="f6f7d-2613">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2613">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="f6f7d-2614">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2614">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="f6f7d-2615">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2615">Service Bus</span></span>
* <span data-ttu-id="f6f7d-2616">[BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2616">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2617">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2617">VM</span></span>
* <span data-ttu-id="f6f7d-2618">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2618">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="f6f7d-2619">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2619">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="f6f7d-2620">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2620">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="f6f7d-2621">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2621">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="f6f7d-2622">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2622">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="f6f7d-2623">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2623">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="f6f7d-2624">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2624">September 21, 2018</span></span>

<span data-ttu-id="f6f7d-2625">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2625">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2626">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2626">ACR</span></span>
* <span data-ttu-id="f6f7d-2627">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2627">Added ACR Task commands</span></span>
* <span data-ttu-id="f6f7d-2628">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2628">Added quick run command</span></span>
* <span data-ttu-id="f6f7d-2629">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2629">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="f6f7d-2630">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2630">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="f6f7d-2631">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2631">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="f6f7d-2632">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2632">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2633">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2633">ACS</span></span>
* <span data-ttu-id="f6f7d-2634">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2634">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="f6f7d-2635">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2635">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2636">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2636">AppService</span></span>

* <span data-ttu-id="f6f7d-2637">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2637">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="f6f7d-2638">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2638">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="f6f7d-2639">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2639">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="f6f7d-2640">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2640">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-2641">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2641">Batch</span></span>
* <span data-ttu-id="f6f7d-2642">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2642">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="f6f7d-2643">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2643">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="f6f7d-2644">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2644">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="f6f7d-2645">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2645">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f6f7d-2646">Batch KI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2646">Batch AI</span></span> 
* <span data-ttu-id="f6f7d-2647">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2647">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6f7d-2648">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2648">Cognitive Services</span></span>
* <span data-ttu-id="f6f7d-2649">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2649">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="f6f7d-2650">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2650">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="f6f7d-2651">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2651">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="f6f7d-2652">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2652">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="f6f7d-2653">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2653">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="f6f7d-2654">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2654">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-2655">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2655">Container</span></span>
* <span data-ttu-id="f6f7d-2656">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2656">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="f6f7d-2657">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2657">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="f6f7d-2658">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2658">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="f6f7d-2659">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2659">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="f6f7d-2660">Data Lake</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2660">Datalake</span></span>
* <span data-ttu-id="f6f7d-2661">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2661">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="f6f7d-2662">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2662">Interactive Shell</span></span>
* <span data-ttu-id="f6f7d-2663">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2663">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="f6f7d-2664">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2664">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-2665">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2665">IoT</span></span>
* <span data-ttu-id="f6f7d-2666">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2666">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6f7d-2667">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2667">Key Vault</span></span>
* <span data-ttu-id="f6f7d-2668">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2668">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2669">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2669">Network</span></span>
* <span data-ttu-id="f6f7d-2670">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2670">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="f6f7d-2671">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2671">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="f6f7d-2672">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2672">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="f6f7d-2673">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2673">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="f6f7d-2674">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2674">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="f6f7d-2675">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2675">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="f6f7d-2676">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2676">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="f6f7d-2677">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2677">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="f6f7d-2678">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2678">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="f6f7d-2679">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2679">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="f6f7d-2680">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2680">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="f6f7d-2681">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2681">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="f6f7d-2682">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2682">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="f6f7d-2683">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2683">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="f6f7d-2684">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2684">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="f6f7d-2685">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2685">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="f6f7d-2686">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2686">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="f6f7d-2687">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2687">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-2688">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2688">RDBMS</span></span>
* <span data-ttu-id="f6f7d-2689">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2689">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="f6f7d-2690">Reservierung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2690">Reservation</span></span>
* <span data-ttu-id="f6f7d-2691">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2691">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="f6f7d-2692">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2692">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="f6f7d-2693">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2693">Manage App</span></span>
* <span data-ttu-id="f6f7d-2694">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2694">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="f6f7d-2695">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2695">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-2696">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2696">Role</span></span>
* <span data-ttu-id="f6f7d-2697">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2697">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="f6f7d-2698">SignalR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2698">SignalR</span></span>
* <span data-ttu-id="f6f7d-2699">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2699">First release</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2700">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2700">Storage</span></span>
* <span data-ttu-id="f6f7d-2701">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2701">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="f6f7d-2702">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2702">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2703">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2703">VM</span></span>
* <span data-ttu-id="f6f7d-2704">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2704">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="f6f7d-2705">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2705">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="f6f7d-2706">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2706">August 28, 2018</span></span>

<span data-ttu-id="f6f7d-2707">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2707">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2708">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2708">Core</span></span>

* <span data-ttu-id="f6f7d-2709">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2709">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="f6f7d-2710">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2710">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2711">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2711">ACR</span></span>

* <span data-ttu-id="f6f7d-2712">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2712">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="f6f7d-2713">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2713">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2714">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2714">ACS</span></span>

* <span data-ttu-id="f6f7d-2715">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2715">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="f6f7d-2716">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2716">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2717">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2717">AppService</span></span>

* <span data-ttu-id="f6f7d-2718">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2718">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="f6f7d-2719">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2719">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="f6f7d-2720">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2720">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-2721">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2721">Backup</span></span>

* <span data-ttu-id="f6f7d-2722">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2722">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="f6f7d-2723">Botdienst</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2723">Bot Service</span></span>

* <span data-ttu-id="f6f7d-2724">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2724">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6f7d-2725">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2725">Cognitive Services</span></span>

* <span data-ttu-id="f6f7d-2726">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2726">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-2727">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2727">IoT</span></span>

* <span data-ttu-id="f6f7d-2728">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2728">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-2729">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2729">Monitor</span></span>

* <span data-ttu-id="f6f7d-2730">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2730">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="f6f7d-2731">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2731">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2732">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2732">Network</span></span>

* <span data-ttu-id="f6f7d-2733">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2733">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-2734">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2734">Resource</span></span>

* <span data-ttu-id="f6f7d-2735">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2735">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2736">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2736">Storage</span></span>

* <span data-ttu-id="f6f7d-2737">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2737">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2738">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2738">VM</span></span>

* <span data-ttu-id="f6f7d-2739">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2739">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="f6f7d-2740">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2740">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="f6f7d-2741">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2741">Auguest 14, 2018</span></span>

<span data-ttu-id="f6f7d-2742">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2742">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2743">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2743">Core</span></span>

* <span data-ttu-id="f6f7d-2744">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2744">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="f6f7d-2745">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2745">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="f6f7d-2746">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2746">Telemetry</span></span>

* <span data-ttu-id="f6f7d-2747">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2747">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2748">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2748">ACR</span></span>

* <span data-ttu-id="f6f7d-2749">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2749">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="f6f7d-2750">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2750">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2751">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2751">ACS</span></span>

* <span data-ttu-id="f6f7d-2752">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2752">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="f6f7d-2753">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2753">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="f6f7d-2754">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2754">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="f6f7d-2755">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2755">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="f6f7d-2756">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2756">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="f6f7d-2757">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2757">AppService</span></span>

* <span data-ttu-id="f6f7d-2758">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2758">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="f6f7d-2759">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2759">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="f6f7d-2760">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2760">BatchAI</span></span>

* <span data-ttu-id="f6f7d-2761">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen *gruppe* “ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2761">Changed logger output for auto-storage account creation to specifies "resource *group* ".</span></span>        

### <a name="container"></a><span data-ttu-id="f6f7d-2762">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2762">Container</span></span>

* <span data-ttu-id="f6f7d-2763">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2763">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="f6f7d-2764">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2764">IoT</span></span>

* <span data-ttu-id="f6f7d-2765">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2765">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="f6f7d-2766">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2766">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="f6f7d-2767">Iot Central</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2767">Iot Central</span></span>

* <span data-ttu-id="f6f7d-2768">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2768">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-2769">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2769">KeyVault</span></span>


* <span data-ttu-id="f6f7d-2770">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2770">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="f6f7d-2771">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2771">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="f6f7d-2772">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2772">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="f6f7d-2773">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2773">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="f6f7d-2774">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2774">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="f6f7d-2775">Relay</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2775">Relay</span></span>

* <span data-ttu-id="f6f7d-2776">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2776">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-2777">Sql</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2777">Sql</span></span>

* <span data-ttu-id="f6f7d-2778">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2778">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2779">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2779">Storage</span></span>

* <span data-ttu-id="f6f7d-2780">[BREAKING CHANGE]`storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2780">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="f6f7d-2781">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2781">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="f6f7d-2782">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2782">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="f6f7d-2783">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2783">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="f6f7d-2784">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2784">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2785">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2785">VM</span></span>

* <span data-ttu-id="f6f7d-2786">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2786">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="f6f7d-2787">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2787">July 31, 2018</span></span>

<span data-ttu-id="f6f7d-2788">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2788">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2789">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2789">ACR</span></span>

* <span data-ttu-id="f6f7d-2790">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2790">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="f6f7d-2791">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2791">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2792">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2792">ACS</span></span>

* <span data-ttu-id="f6f7d-2793">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2793">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-2794">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2794">Batch</span></span>

* <span data-ttu-id="f6f7d-2795">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2795">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-2796">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2796">Container</span></span>

* <span data-ttu-id="f6f7d-2797">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2797">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2798">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2798">Network</span></span>

* <span data-ttu-id="f6f7d-2799">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2799">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="f6f7d-2800">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2800">Resource</span></span>

* <span data-ttu-id="f6f7d-2801">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2801">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="f6f7d-2802">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2802">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-2803">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2803">Role</span></span>

* <span data-ttu-id="f6f7d-2804">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2804">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="f6f7d-2805">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2805">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="f6f7d-2806">Suchen,</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2806">Search</span></span>

* <span data-ttu-id="f6f7d-2807">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2807">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="f6f7d-2808">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2808">Service Bus</span></span>

* <span data-ttu-id="f6f7d-2809">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2809">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="f6f7d-2810">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2810">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="f6f7d-2811">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2811">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="f6f7d-2812">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2812">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2813">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2813">Storage</span></span>

* <span data-ttu-id="f6f7d-2814">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2814">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="f6f7d-2815">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2815">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2816">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2816">VM</span></span>

* <span data-ttu-id="f6f7d-2817">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2817">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="f6f7d-2818">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2818">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="f6f7d-2819">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2819">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="f6f7d-2820">[BREAKING CHANGE]`[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2820">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="f6f7d-2821">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2821">July 18, 2018</span></span>

<span data-ttu-id="f6f7d-2822">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2822">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2823">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2823">Core</span></span>

* <span data-ttu-id="f6f7d-2824">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2824">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="f6f7d-2825">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2825">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="f6f7d-2826">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2826">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2827">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2827">ACR</span></span>

* <span data-ttu-id="f6f7d-2828">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2828">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="f6f7d-2829">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2829">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="f6f7d-2830">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2830">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="f6f7d-2831">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2831">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2832">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2832">ACS</span></span>

* <span data-ttu-id="f6f7d-2833">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2833">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2834">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2834">AppService</span></span>

* <span data-ttu-id="f6f7d-2835">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2835">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-2836">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2836">Batch</span></span>

* <span data-ttu-id="f6f7d-2837">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2837">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="f6f7d-2838">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2838">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f6f7d-2839">Batch KI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2839">Batch AI</span></span>

* <span data-ttu-id="f6f7d-2840">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2840">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-2841">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2841">Container</span></span>

* <span data-ttu-id="f6f7d-2842">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2842">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="f6f7d-2843">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2843">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2844">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2844">Network</span></span>

* <span data-ttu-id="f6f7d-2845">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2845">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="f6f7d-2846">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2846">Added `network nic wait`</span></span>
* <span data-ttu-id="f6f7d-2847">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2847">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="f6f7d-2848">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2848">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="f6f7d-2849">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2849">Resource</span></span>

* <span data-ttu-id="f6f7d-2850">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2850">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="f6f7d-2851">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2851">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="f6f7d-2852">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2852">Added `deployment wait` command</span></span>
* <span data-ttu-id="f6f7d-2853">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2853">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-2854">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2854">SQL</span></span>

* <span data-ttu-id="f6f7d-2855">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2855">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="f6f7d-2856">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2856">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="f6f7d-2857">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2857">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2858">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2858">Storage</span></span>

* <span data-ttu-id="f6f7d-2859">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2859">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2860">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2860">VM</span></span>

* <span data-ttu-id="f6f7d-2861">[BREAKING CHANGE]`vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2861">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="f6f7d-2862">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2862">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="f6f7d-2863">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2863">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f6f7d-2864">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2864">July 3, 2018</span></span>

<span data-ttu-id="f6f7d-2865">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2865">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-2866">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2866">AKS</span></span>

* <span data-ttu-id="f6f7d-2867">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2867">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f6f7d-2868">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2868">July 3, 2018</span></span>

<span data-ttu-id="f6f7d-2869">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2869">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2870">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2870">Core</span></span>

* <span data-ttu-id="f6f7d-2871">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2871">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2872">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2872">ACR</span></span>

* <span data-ttu-id="f6f7d-2873">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2873">Added polling build status</span></span>
* <span data-ttu-id="f6f7d-2874">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2874">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="f6f7d-2875">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2875">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2876">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2876">ACS</span></span>

* <span data-ttu-id="f6f7d-2877">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2877">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="f6f7d-2878">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2878">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="f6f7d-2879">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2879">Updated options for `aks browse` command.</span></span> <span data-ttu-id="f6f7d-2880">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2880">Added `--listen-port` support</span></span>
* <span data-ttu-id="f6f7d-2881">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2881">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="f6f7d-2882">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2882">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="f6f7d-2883">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2883">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2884">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2884">AppService</span></span>

* <span data-ttu-id="f6f7d-2885">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2885">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="f6f7d-2886">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2886">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-2887">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2887">Backup</span></span>

* <span data-ttu-id="f6f7d-2888">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2888">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="f6f7d-2889">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2889">BatchAI</span></span>

* <span data-ttu-id="f6f7d-2890">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2890">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="f6f7d-2891">Cloud</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2891">Cloud</span></span>

* <span data-ttu-id="f6f7d-2892">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2892">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-2893">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2893">Container</span></span>

* <span data-ttu-id="f6f7d-2894">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2894">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="f6f7d-2895">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2895">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="f6f7d-2896">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2896">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-2897">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2897">Extension</span></span>

* <span data-ttu-id="f6f7d-2898">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2898">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2899">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2899">Network</span></span>

* <span data-ttu-id="f6f7d-2900">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2900">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-2901">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2901">Rdbms</span></span>

* <span data-ttu-id="f6f7d-2902">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2902">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-2903">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2903">Resource</span></span>

* <span data-ttu-id="f6f7d-2904">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2904">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2905">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2905">VM</span></span>

* <span data-ttu-id="f6f7d-2906">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2906">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="f6f7d-2907">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2907">June 25, 2018</span></span>

<span data-ttu-id="f6f7d-2908">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2908">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="f6f7d-2909">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2909">CLI</span></span>

* <span data-ttu-id="f6f7d-2910">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2910">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="f6f7d-2911">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2911">June 19, 2018</span></span>

<span data-ttu-id="f6f7d-2912">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2912">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2913">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2913">Core</span></span>

* <span data-ttu-id="f6f7d-2914">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2914">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-2915">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2915">ACR</span></span>

* <span data-ttu-id="f6f7d-2916">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2916">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="f6f7d-2917">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2917">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-2918">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2918">ACS</span></span>

* <span data-ttu-id="f6f7d-2919">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2919">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="f6f7d-2920">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2920">Added `--update` support</span></span>
* <span data-ttu-id="f6f7d-2921">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2921">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="f6f7d-2922">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2922">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="f6f7d-2923">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2923">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="f6f7d-2924">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2924">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="f6f7d-2925">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2925">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="f6f7d-2926">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2926">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2927">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2927">AppService</span></span>

* <span data-ttu-id="f6f7d-2928">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2928">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="f6f7d-2929">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2929">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-2930">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2930">Batch</span></span>

* <span data-ttu-id="f6f7d-2931">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2931">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f6f7d-2932">Batch KI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2932">Batch AI</span></span>

* <span data-ttu-id="f6f7d-2933">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2933">Added support for workspaces.</span></span> <span data-ttu-id="f6f7d-2934">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2934">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="f6f7d-2935">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2935">Added support for experiments.</span></span> <span data-ttu-id="f6f7d-2936">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2936">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="f6f7d-2937">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2937">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="f6f7d-2938">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2938">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="f6f7d-2939">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2939">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="f6f7d-2940">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2940">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="f6f7d-2941">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2941">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="f6f7d-2942">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2942">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="f6f7d-2943">[BREAKING CHANGE]`--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2943">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="f6f7d-2944">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2944">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="f6f7d-2945">[BREAKING CHANGE]`--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2945">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="f6f7d-2946">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2946">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="f6f7d-2947">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2947">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="f6f7d-2948">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2948">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="f6f7d-2949">[BREAKING CHANGE]`--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2949">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="f6f7d-2950">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2950">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="f6f7d-2951">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2951">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="f6f7d-2952">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2952">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="f6f7d-2953">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2953">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="f6f7d-2954">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2954">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="f6f7d-2955">Karten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2955">Maps</span></span>

* <span data-ttu-id="f6f7d-2956">[BREAKING CHANGE]`maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2956">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-2957">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2957">Network</span></span>

* <span data-ttu-id="f6f7d-2958">Unterstützung für `https` zu `network lb probe create` hinzugefügt [Nr. 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2958">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="f6f7d-2959">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2959">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="f6f7d-2960">#6502</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2960">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="f6f7d-2961">Reservations</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2961">Reservations</span></span>

* <span data-ttu-id="f6f7d-2962">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2962">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="f6f7d-2963">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2963">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="f6f7d-2964">[BREAKING CHANGE]`kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2964">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="f6f7d-2965">[BREAKING CHANGE]`capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2965">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="f6f7d-2966">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2966">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="f6f7d-2967">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2967">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-2968">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2968">Role</span></span>

* <span data-ttu-id="f6f7d-2969">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2969">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-2970">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2970">SQL</span></span>

* <span data-ttu-id="f6f7d-2971">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2971">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-2972">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2972">Storage</span></span>

* <span data-ttu-id="f6f7d-2973">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2973">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-2974">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2974">VM</span></span>

* <span data-ttu-id="f6f7d-2975">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2975">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="f6f7d-2976">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2976">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="f6f7d-2977">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2977">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f6f7d-2978">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2978">June 13, 2018</span></span>

<span data-ttu-id="f6f7d-2979">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2979">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2980">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2980">Core</span></span>

* <span data-ttu-id="f6f7d-2981">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2981">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f6f7d-2982">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2982">June 13, 2018</span></span>

<span data-ttu-id="f6f7d-2983">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2983">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-2984">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2984">AKS</span></span>

* <span data-ttu-id="f6f7d-2985">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2985">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="f6f7d-2986">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2986">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="f6f7d-2987">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2987">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="f6f7d-2988">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2988">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="f6f7d-2989">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2989">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-2990">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2990">AppService</span></span>

* <span data-ttu-id="f6f7d-2991">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2991">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f6f7d-2992">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2992">June 5, 2018</span></span>

<span data-ttu-id="f6f7d-2993">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2993">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-2994">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2994">Interactive</span></span>

* <span data-ttu-id="f6f7d-2995">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2995">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f6f7d-2996">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2996">June 5, 2018</span></span>

<span data-ttu-id="f6f7d-2997">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2997">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-2998">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2998">Core</span></span>

* <span data-ttu-id="f6f7d-2999">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-2999">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="f6f7d-3000">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3000">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-3001">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3001">ACR</span></span>

* <span data-ttu-id="f6f7d-3002">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3002">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="f6f7d-3003">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3003">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="f6f7d-3004">AKS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3004">AKS</span></span>

* <span data-ttu-id="f6f7d-3005">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3005">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-3006">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3006">Batch</span></span>

* <span data-ttu-id="f6f7d-3007">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3007">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-3008">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3008">IOT</span></span>

* <span data-ttu-id="f6f7d-3009">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3009">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3010">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3010">Network</span></span>

* <span data-ttu-id="f6f7d-3011">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3011">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="f6f7d-3012">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3012">Policy Insights</span></span>

* <span data-ttu-id="f6f7d-3013">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3013">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="f6f7d-3014">ARM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3014">ARM</span></span>

* <span data-ttu-id="f6f7d-3015">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3015">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-3016">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3016">SQL</span></span>

* <span data-ttu-id="f6f7d-3017">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3017">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="f6f7d-3018">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3018">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="f6f7d-3019">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3019">Storage</span></span>

* <span data-ttu-id="f6f7d-3020">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3020">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3021">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3021">VM</span></span>

* <span data-ttu-id="f6f7d-3022">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3022">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="f6f7d-3023">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3023">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="f6f7d-3024">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3024">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="f6f7d-3025">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3025">May 22, 2018</span></span>

<span data-ttu-id="f6f7d-3026">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3026">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-3027">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3027">Core</span></span>

* <span data-ttu-id="f6f7d-3028">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3028">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3029">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3029">ACS</span></span>

* <span data-ttu-id="f6f7d-3030">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3030">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="f6f7d-3031">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3031">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3032">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3032">AppService</span></span>

* <span data-ttu-id="f6f7d-3033">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3033">Improved generic update commands</span></span>
* <span data-ttu-id="f6f7d-3034">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3034">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-3035">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3035">Container</span></span>

* <span data-ttu-id="f6f7d-3036">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3036">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="f6f7d-3037">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3037">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-3038">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3038">Extension</span></span>

* <span data-ttu-id="f6f7d-3039">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3039">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-3040">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3040">Interactive</span></span>

* <span data-ttu-id="f6f7d-3041">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3041">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="f6f7d-3042">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3042">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-3043">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3043">KeyVault</span></span>

* <span data-ttu-id="f6f7d-3044">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3044">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3045">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3045">Network</span></span>

* <span data-ttu-id="f6f7d-3046">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3046">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="f6f7d-3047">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3047">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-3048">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3048">SQL</span></span>

* <span data-ttu-id="f6f7d-3049">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3049">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="f6f7d-3050">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3050">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="f6f7d-3051">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3051">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="f6f7d-3052">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3052">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="f6f7d-3053">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3053">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="f6f7d-3054">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3054">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="f6f7d-3055">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3055">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="f6f7d-3056">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3056">`edition`.</span></span> <span data-ttu-id="f6f7d-3057">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3057">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="f6f7d-3058">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3058">`elasticPoolName`.</span></span> <span data-ttu-id="f6f7d-3059">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3059">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="f6f7d-3060">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3060">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="f6f7d-3061">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3061">`edition`.</span></span> <span data-ttu-id="f6f7d-3062">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3062">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="f6f7d-3063">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3063">`dtu`.</span></span> <span data-ttu-id="f6f7d-3064">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3064">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="f6f7d-3065">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3065">`databaseDtuMin`.</span></span> <span data-ttu-id="f6f7d-3066">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3066">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="f6f7d-3067">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3067">`databaseDtuMax`.</span></span> <span data-ttu-id="f6f7d-3068">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3068">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="f6f7d-3069">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3069">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="f6f7d-3070">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3070">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3071">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3071">Storage</span></span>

* <span data-ttu-id="f6f7d-3072">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3072">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="f6f7d-3073">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3073">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3074">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3074">VM</span></span>

* <span data-ttu-id="f6f7d-3075">[BREAKING CHANGE]`--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3075">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="f6f7d-3076">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3076">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="f6f7d-3077">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3077">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="f6f7d-3078">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3078">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="f6f7d-3079">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3079">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="f6f7d-3080">7\. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3080">May 7, 2018</span></span>

<span data-ttu-id="f6f7d-3081">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3081">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-3082">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3082">Core</span></span>

* <span data-ttu-id="f6f7d-3083">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3083">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="f6f7d-3084">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3084">Added limited support for positional arguments</span></span>
* <span data-ttu-id="f6f7d-3085">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3085">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="f6f7d-3086">#5591</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3086">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="f6f7d-3087">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3087">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="f6f7d-3088">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3088">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="f6f7d-3089">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3089">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="f6f7d-3090">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3090">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="f6f7d-3091">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3091">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-3092">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3092">ACR</span></span>

* <span data-ttu-id="f6f7d-3093">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3093">Added ACR Build commands</span></span>
* <span data-ttu-id="f6f7d-3094">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3094">Improved resource not found error messages</span></span>
* <span data-ttu-id="f6f7d-3095">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3095">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="f6f7d-3096">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3096">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="f6f7d-3097">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3097">Improved repository commands error messages</span></span>
* <span data-ttu-id="f6f7d-3098">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3098">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3099">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3099">ACS</span></span>

* <span data-ttu-id="f6f7d-3100">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3100">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="f6f7d-3101">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3101">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="f6f7d-3102">AMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3102">AMS</span></span>

* <span data-ttu-id="f6f7d-3103">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3103">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3104">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3104">Appservice</span></span>

* <span data-ttu-id="f6f7d-3105">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3105">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="f6f7d-3106">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3106">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="f6f7d-3107">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3107">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="f6f7d-3108">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3108">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f6f7d-3109">Batch KI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3109">Batch AI</span></span>

* <span data-ttu-id="f6f7d-3110">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3110">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6f7d-3111">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3111">Cognitive Services</span></span>

* <span data-ttu-id="f6f7d-3112">Tippfehler im Beispiel für `cognitiveservices account create` behoben [Nr. 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3112">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="f6f7d-3113">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3113">Consumption</span></span>

* <span data-ttu-id="f6f7d-3114">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3114">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-3115">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3115">Container</span></span>

* <span data-ttu-id="f6f7d-3116">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3116">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f6f7d-3117">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3117">Cosmos DB</span></span>

* <span data-ttu-id="f6f7d-3118">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3118">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="f6f7d-3119">DMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3119">DMS</span></span>

* <span data-ttu-id="f6f7d-3120">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3120">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-3121">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3121">Extension</span></span>

* <span data-ttu-id="f6f7d-3122">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3122">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-3123">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3123">Interactive</span></span>

* <span data-ttu-id="f6f7d-3124">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3124">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="f6f7d-3125">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3125">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="f6f7d-3126">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3126">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="f6f7d-3127">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3127">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="f6f7d-3128">Labor</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3128">Lab</span></span>

* <span data-ttu-id="f6f7d-3129">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3129">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3130">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3130">Network</span></span>

* <span data-ttu-id="f6f7d-3131">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3131">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="f6f7d-3132">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3132">Profile</span></span>

* <span data-ttu-id="f6f7d-3133">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3133">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="f6f7d-3134">[BREAKING CHANGE]`--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3134">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="f6f7d-3135">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3135">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="f6f7d-3136">Redis</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3136">Redis</span></span>

* <span data-ttu-id="f6f7d-3137">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3137">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="f6f7d-3138">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3138">Deprecated `redis list-all`.</span></span> <span data-ttu-id="f6f7d-3139">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3139">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="f6f7d-3140">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3140">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="f6f7d-3141">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3141">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-3142">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3142">Role</span></span>

* <span data-ttu-id="f6f7d-3143">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3143">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3144">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3144">Storage</span></span>

* <span data-ttu-id="f6f7d-3145">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3145">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="f6f7d-3146">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3146">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="f6f7d-3147">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3147">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="f6f7d-3148">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3148">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="f6f7d-3149">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3149">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3150">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3150">VM</span></span>

* <span data-ttu-id="f6f7d-3151">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3151">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="f6f7d-3152">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3152">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="f6f7d-3153">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3153">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="f6f7d-3154">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3154">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="f6f7d-3155">[BREAKING CHANGE]`--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3155">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="f6f7d-3156">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3156">Added write accelerator support</span></span>
* <span data-ttu-id="f6f7d-3157">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3157">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="f6f7d-3158">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3158">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="f6f7d-3159">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3159">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="f6f7d-3160">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3160">April 10, 2018</span></span>

<span data-ttu-id="f6f7d-3161">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3161">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-3162">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3162">ACR</span></span>

* <span data-ttu-id="f6f7d-3163">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3163">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3164">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3164">ACS</span></span>

* <span data-ttu-id="f6f7d-3165">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3165">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3166">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3166">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="f6f7d-3168">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3168">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="f6f7d-3169">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3169">BatchAI</span></span>

* <span data-ttu-id="f6f7d-3170">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3170">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="f6f7d-3171">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3171">Job level mounting</span></span>
  - <span data-ttu-id="f6f7d-3172">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3172">Environment variables with secret values</span></span>
  - <span data-ttu-id="f6f7d-3173">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3173">Performance counters settings</span></span>
  - <span data-ttu-id="f6f7d-3174">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3174">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="f6f7d-3175">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3175">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="f6f7d-3176">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3176">Usage and limits reporting</span></span>
  - <span data-ttu-id="f6f7d-3177">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3177">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="f6f7d-3178">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3178">Support for custom images</span></span>
  - <span data-ttu-id="f6f7d-3179">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3179">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="f6f7d-3180">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3180">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="f6f7d-3181">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch KI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3181">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="f6f7d-3182">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3182">National clouds are supported</span></span>
* <span data-ttu-id="f6f7d-3183">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3183">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="f6f7d-3184">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3184">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="f6f7d-3185">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch KI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3185">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="f6f7d-3186">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3186">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="f6f7d-3187">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3187">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="f6f7d-3188">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3188">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="f6f7d-3189">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3189">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="f6f7d-3190">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3190">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="f6f7d-3191">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3191">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="f6f7d-3192">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3192">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="f6f7d-3193">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3193">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="f6f7d-3194">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3194">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="f6f7d-3195">[BREAKING CHANGE]`--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3195">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="f6f7d-3196">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3196">Billing</span></span>

* <span data-ttu-id="f6f7d-3197">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3197">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="f6f7d-3198">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3198">Consumption</span></span>

* <span data-ttu-id="f6f7d-3199">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3199">Added `marketplace` commands</span></span>
* <span data-ttu-id="f6f7d-3200">[BREAKING CHANGE]`reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3200">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="f6f7d-3201">[BREAKING CHANGE]`reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3201">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="f6f7d-3202">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3202">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="f6f7d-3203">[BREAKING CHANGE]`--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3203">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="f6f7d-3204">[BREAKING CHANGE]`--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3204">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-3205">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3205">Container</span></span>

* <span data-ttu-id="f6f7d-3206">Parameter für die Volumebereitstellung für das Git-Repository hinzugefügt: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3206">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="f6f7d-3207">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3207">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-3208">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3208">Extension</span></span>

* <span data-ttu-id="f6f7d-3209">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3209">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-3210">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3210">Interactive</span></span>

* <span data-ttu-id="f6f7d-3211">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3211">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="f6f7d-3212">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3212">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="f6f7d-3213">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3213">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3214">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3214">Network</span></span>

* <span data-ttu-id="f6f7d-3215">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3215">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="f6f7d-3216">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3216">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="f6f7d-3217">#4910</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3217">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="f6f7d-3218">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3218">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="f6f7d-3219">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3219">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="f6f7d-3220">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3220">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="f6f7d-3221">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3221">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="f6f7d-3222">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3222">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-3223">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3223">Profile</span></span>

* <span data-ttu-id="f6f7d-3224">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3224">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="f6f7d-3225">[BREAKING CHANGE]`--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3225">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-3226">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3226">RDBMS</span></span>

* <span data-ttu-id="f6f7d-3227">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3227">Added `georestore` command</span></span>
* <span data-ttu-id="f6f7d-3228">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3228">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-3229">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3229">Resource</span></span>

* <span data-ttu-id="f6f7d-3230">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3230">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="f6f7d-3231">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3231">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-3232">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3232">SQL</span></span>

* <span data-ttu-id="f6f7d-3233">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3233">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3234">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3234">Storage</span></span>

* <span data-ttu-id="f6f7d-3235">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3235">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3236">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3236">VM</span></span>

* <span data-ttu-id="f6f7d-3237">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3237">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="f6f7d-3238">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3238">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="f6f7d-3240">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3240">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="f6f7d-3241">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3241">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="f6f7d-3242">#5718</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3242">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="f6f7d-3243">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3243">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="f6f7d-3244">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3244">March 27, 2018</span></span>

<span data-ttu-id="f6f7d-3245">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3245">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-3246">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3246">Core</span></span>

* <span data-ttu-id="f6f7d-3247">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3247">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3248">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3248">ACS</span></span>

* <span data-ttu-id="f6f7d-3249">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3249">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3250">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3250">Appservice</span></span>

* <span data-ttu-id="f6f7d-3251">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3251">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="f6f7d-3252">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3252">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-3253">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3253">Backup</span></span>

* <span data-ttu-id="f6f7d-3254">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3254">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="f6f7d-3255">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3255">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="f6f7d-3256">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3256">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="f6f7d-3257">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3257">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-3258">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3258">Container</span></span>

* <span data-ttu-id="f6f7d-3259">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3259">Added `container exec` command.</span></span> <span data-ttu-id="f6f7d-3260">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3260">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="f6f7d-3261">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3261">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-3262">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3262">Extension</span></span>

* <span data-ttu-id="f6f7d-3263">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3263">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="f6f7d-3264">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3264">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="f6f7d-3265">[BREAKING CHANGE]`extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3265">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-3266">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3266">Interactive</span></span>

* <span data-ttu-id="f6f7d-3267">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3267">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="f6f7d-3268">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3268">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="f6f7d-3269">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3269">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="f6f7d-3270">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3270">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="f6f7d-3271">Labor</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3271">Lab</span></span>

* <span data-ttu-id="f6f7d-3272">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3272">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-3273">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3273">Monitor</span></span>

* <span data-ttu-id="f6f7d-3274">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3274">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="f6f7d-3275">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3275">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="f6f7d-3276">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3276">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3277">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3277">Network</span></span>

* <span data-ttu-id="f6f7d-3278">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3278">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-3279">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3279">Profile</span></span>

* <span data-ttu-id="f6f7d-3280">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3280">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-3281">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3281">RDBMS</span></span>

* <span data-ttu-id="f6f7d-3282">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3282">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-3283">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3283">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="f6f7d-3285">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3285">Role</span></span>

* <span data-ttu-id="f6f7d-3286">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3286">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="f6f7d-3287">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3287">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="f6f7d-3288">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3288">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="f6f7d-3289">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3289">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="f6f7d-3290">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3290">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3291">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3291">Storage</span></span>

* <span data-ttu-id="f6f7d-3292">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3292">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="f6f7d-3293">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3293">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3294">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3294">VM</span></span>

* <span data-ttu-id="f6f7d-3295">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3295">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="f6f7d-3296">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3296">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="f6f7d-3297">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3297">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="f6f7d-3298">[BREAKING CHANGE]`vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3298">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="f6f7d-3299">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3299">March 13, 2018</span></span>

<span data-ttu-id="f6f7d-3300">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3300">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-3301">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3301">ACR</span></span>

* <span data-ttu-id="f6f7d-3302">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3302">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="f6f7d-3303">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3303">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="f6f7d-3304">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3304">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3305">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3305">ACS</span></span>

* <span data-ttu-id="f6f7d-3306">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3306">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="f6f7d-3307">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3307">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="f6f7d-3308">Advisor</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3308">Advisor</span></span>

* <span data-ttu-id="f6f7d-3309">[BREAKING CHANGE]`advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3309">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="f6f7d-3310">[BREAKING CHANGE]`advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3310">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="f6f7d-3311">[BREAKING CHANGE]`advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3311">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="f6f7d-3312">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3312">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="f6f7d-3313">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3313">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3314">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3314">Appservice</span></span>

* <span data-ttu-id="f6f7d-3315">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3315">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="f6f7d-3316">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3316">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f6f7d-3317">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3317">Eventhubs</span></span>

* <span data-ttu-id="f6f7d-3318">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3318">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-3319">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3319">Extension</span></span>

* <span data-ttu-id="f6f7d-3320">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3320">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-3321">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3321">Interactive</span></span>

* <span data-ttu-id="f6f7d-3322">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3322">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="f6f7d-3323">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3323">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="f6f7d-3324">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3324">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="f6f7d-3325">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3325">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-3326">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3326">Monitor</span></span>

* <span data-ttu-id="f6f7d-3327">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3327">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="f6f7d-3328">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3328">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="f6f7d-3329">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3329">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="f6f7d-3330">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3330">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3331">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3331">Network</span></span>

* <span data-ttu-id="f6f7d-3332">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3332">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="f6f7d-3333">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3333">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="f6f7d-3334">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3334">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="f6f7d-3335">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3335">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-3336">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3336">Profile</span></span>

* <span data-ttu-id="f6f7d-3337">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3337">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="f6f7d-3338">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3338">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-3339">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3339">RDBMS</span></span>

* <span data-ttu-id="f6f7d-3340">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3340">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="f6f7d-3341">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3341">Service Bus</span></span>

* <span data-ttu-id="f6f7d-3342">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3342">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3343">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3343">Storage</span></span>

* <span data-ttu-id="f6f7d-3344">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3344">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="f6f7d-3345">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3345">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3346">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3346">VM</span></span>

* <span data-ttu-id="f6f7d-3347">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3347">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="f6f7d-3348">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3348">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="f6f7d-3349">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3349">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="f6f7d-3350">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3350">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="f6f7d-3351">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3351">February 27, 2018</span></span>

<span data-ttu-id="f6f7d-3352">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3352">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-3353">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3353">Core</span></span>

* <span data-ttu-id="f6f7d-3354">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3354">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="f6f7d-3355">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3355">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="f6f7d-3356">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3356">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3357">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3357">ACS</span></span>

* <span data-ttu-id="f6f7d-3358">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3358">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="f6f7d-3359">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3359">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="f6f7d-3360">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3360">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="f6f7d-3361">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3361">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3362">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3362">Appservice</span></span>

* <span data-ttu-id="f6f7d-3363">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3363">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="f6f7d-3364">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3364">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f6f7d-3365">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3365">Cognitive Services</span></span>

* <span data-ttu-id="f6f7d-3366">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3366">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="f6f7d-3367">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3367">Consumption</span></span>

* <span data-ttu-id="f6f7d-3368">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3368">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="f6f7d-3369">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3369">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-3370">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3370">Container</span></span>

* <span data-ttu-id="f6f7d-3371">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3371">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3372">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3372">Network</span></span>

* <span data-ttu-id="f6f7d-3373">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3373">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-3374">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3374">Resource</span></span>

* <span data-ttu-id="f6f7d-3375">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3375">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-3376">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3376">Role</span></span>

* <span data-ttu-id="f6f7d-3377">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3377">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-3378">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3378">SQL</span></span>

* <span data-ttu-id="f6f7d-3379">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3379">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3380">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3380">Storage</span></span>

* <span data-ttu-id="f6f7d-3381">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3381">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3382">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3382">VM</span></span>

* <span data-ttu-id="f6f7d-3383">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3383">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="f6f7d-3384">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3384">February 13, 2018</span></span>

<span data-ttu-id="f6f7d-3385">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3385">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-3386">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3386">Core</span></span>

* <span data-ttu-id="f6f7d-3387">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3387">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3388">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3388">ACS</span></span>

* <span data-ttu-id="f6f7d-3389">[BREAKING CHANGE]`aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3389">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="f6f7d-3390">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3390">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="f6f7d-3391">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3391">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="f6f7d-3392">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3392">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="f6f7d-3393">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3393">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="f6f7d-3394">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3394">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="f6f7d-3395">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3395">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="f6f7d-3396">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3396">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3397">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3397">Appservice</span></span>

* <span data-ttu-id="f6f7d-3398">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3398">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="f6f7d-3399">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3399">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="f6f7d-3400">CDN</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3400">CDN</span></span>

* <span data-ttu-id="f6f7d-3401">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3401">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-3402">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3402">Container</span></span>

* <span data-ttu-id="f6f7d-3403">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3403">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="f6f7d-3404">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3404">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6f7d-3405">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3405">CosmosDB</span></span>

* <span data-ttu-id="f6f7d-3406">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3406">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-3407">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3407">Extension</span></span>

* <span data-ttu-id="f6f7d-3408">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3408">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="f6f7d-3409">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3409">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="f6f7d-3410">Feedback</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3410">Feedback</span></span>

* <span data-ttu-id="f6f7d-3411">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3411">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-3412">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3412">Interactive</span></span>

* <span data-ttu-id="f6f7d-3413">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3413">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="f6f7d-3414">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3414">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-3415">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3415">IoT</span></span>

* <span data-ttu-id="f6f7d-3416">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3416">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f6f7d-3417">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3417">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f6f7d-3418">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3418">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="f6f7d-3419">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3419">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-3420">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3420">Monitor</span></span>

* <span data-ttu-id="f6f7d-3421">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3421">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3422">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3422">Network</span></span>

* <span data-ttu-id="f6f7d-3423">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3423">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="f6f7d-3424">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3424">Profile</span></span>

* <span data-ttu-id="f6f7d-3425">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3425">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-3426">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3426">Resource</span></span>

* <span data-ttu-id="f6f7d-3427">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3427">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-3428">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3428">Role</span></span>

* <span data-ttu-id="f6f7d-3429">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3429">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-3430">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3430">SQL</span></span>

* <span data-ttu-id="f6f7d-3431">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3431">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="f6f7d-3432">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3432">Added `sql db rename`</span></span>
* <span data-ttu-id="f6f7d-3433">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3433">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3434">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3434">Storage</span></span>

* <span data-ttu-id="f6f7d-3435">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3435">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3436">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3436">VM</span></span>

* <span data-ttu-id="f6f7d-3437">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3437">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="f6f7d-3438">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3438">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="f6f7d-3439">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3439">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="f6f7d-3440">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3440">January 31, 2018</span></span>

<span data-ttu-id="f6f7d-3441">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3441">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-3442">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3442">Core</span></span>

* <span data-ttu-id="f6f7d-3443">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3443">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="f6f7d-3444">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3444">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="f6f7d-3445">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3445">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="f6f7d-3446">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3446">Use `--verbose` to see</span></span>
* <span data-ttu-id="f6f7d-3447">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3447">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3448">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3448">ACS</span></span>

* <span data-ttu-id="f6f7d-3449">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3449">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="f6f7d-3450">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3450">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3451">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3451">Appservice</span></span>

* <span data-ttu-id="f6f7d-3452">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3452">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="f6f7d-3453">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3453">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="f6f7d-3454">CDN</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3454">CDN</span></span>

* <span data-ttu-id="f6f7d-3455">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3455">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6f7d-3456">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3456">CosmosDB</span></span>

* <span data-ttu-id="f6f7d-3457">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3457">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-3458">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3458">Interactive</span></span>

* <span data-ttu-id="f6f7d-3459">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3459">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3460">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3460">Network</span></span>

* <span data-ttu-id="f6f7d-3461">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3461">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="f6f7d-3462">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3462">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="f6f7d-3463">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3463">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="f6f7d-3464">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3464">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="f6f7d-3465">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3465">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="f6f7d-3466">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3466">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="f6f7d-3467">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3467">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="f6f7d-3468">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3468">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="f6f7d-3469">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3469">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="f6f7d-3470">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3470">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-3471">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3471">Profile</span></span>

* <span data-ttu-id="f6f7d-3472">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3472">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-3473">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3473">Resource</span></span>

* <span data-ttu-id="f6f7d-3474">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3474">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3475">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3475">Storage</span></span>

* <span data-ttu-id="f6f7d-3476">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3476">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="f6f7d-3477">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3477">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="f6f7d-3478">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3478">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="f6f7d-3479">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3479">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="f6f7d-3480">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3480">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3481">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3481">VM</span></span>

* <span data-ttu-id="f6f7d-3482">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3482">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="f6f7d-3483">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3483">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="f6f7d-3484">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3484">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="f6f7d-3485">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3485">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="f6f7d-3486">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3486">January 17, 2018</span></span>

<span data-ttu-id="f6f7d-3487">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3487">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-3488">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3488">ACR</span></span>

* <span data-ttu-id="f6f7d-3489">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3489">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="f6f7d-3490">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3490">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3491">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3491">ACS</span></span>

* <span data-ttu-id="f6f7d-3492">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3492">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="f6f7d-3493">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3493">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3494">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3494">Appservice</span></span>

* <span data-ttu-id="f6f7d-3495">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3495">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="f6f7d-3496">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3496">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="f6f7d-3497">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3497">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-3498">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3498">Backup</span></span>

* <span data-ttu-id="f6f7d-3499">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3499">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="f6f7d-3500">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3500">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="f6f7d-3501">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3501">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="f6f7d-3502">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3502">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="f6f7d-3503">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3503">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-3504">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3504">Batch</span></span>

* <span data-ttu-id="f6f7d-3505">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3505">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="f6f7d-3506">Cloud</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3506">Cloud</span></span>

* <span data-ttu-id="f6f7d-3507">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3507">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="f6f7d-3508">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3508">Consumption</span></span>

* <span data-ttu-id="f6f7d-3509">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3509">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="f6f7d-3510">Event Grid</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3510">Event Grid</span></span>

* <span data-ttu-id="f6f7d-3511">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3511">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f6f7d-3512">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3512">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f6f7d-3513">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3513">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="f6f7d-3514">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3514">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="f6f7d-3515">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3515">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="f6f7d-3516">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3516">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="f6f7d-3517">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3517">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="f6f7d-3518">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3518">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-3519">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3519">Interactive</span></span>

* <span data-ttu-id="f6f7d-3520">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3520">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="f6f7d-3521">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3521">Fixed errors on startup</span></span>
* <span data-ttu-id="f6f7d-3522">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3522">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-3523">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3523">IoT</span></span>

* <span data-ttu-id="f6f7d-3524">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3524">Added support for device provisioning service</span></span>
* <span data-ttu-id="f6f7d-3525">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3525">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="f6f7d-3526">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3526">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-3527">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3527">Monitor</span></span>

* <span data-ttu-id="f6f7d-3528">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3528">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="f6f7d-3529">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3529">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="f6f7d-3530">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3530">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3531">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3531">Network</span></span>

* <span data-ttu-id="f6f7d-3532">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3532">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="f6f7d-3533">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3533">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-3534">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3534">Profile</span></span>

* <span data-ttu-id="f6f7d-3535">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3535">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-3536">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3536">Role</span></span>

* <span data-ttu-id="f6f7d-3537">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3537">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f6f7d-3538">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3538">Service Fabric</span></span>

* <span data-ttu-id="f6f7d-3539">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3539">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="f6f7d-3540">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3540">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3541">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3541">VM</span></span>

* <span data-ttu-id="f6f7d-3542">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3542">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="f6f7d-3543">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3543">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="f6f7d-3544">[BREAKING CHANGE]`externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3544">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="f6f7d-3545">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3545">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="f6f7d-3546">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3546">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="f6f7d-3547">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3547">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6f7d-3548">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3548">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6f7d-3549">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3549">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="f6f7d-3550">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3550">December 19, 2017</span></span>

<span data-ttu-id="f6f7d-3551">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3551">Version 2.0.23</span></span>

* <span data-ttu-id="f6f7d-3552">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3552">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-3553">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3553">Container</span></span>

* <span data-ttu-id="f6f7d-3554">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3554">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3555">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3555">Network</span></span>

* <span data-ttu-id="f6f7d-3556">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3556">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="f6f7d-3557">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3557">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3558">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3558">Storage</span></span>

* <span data-ttu-id="f6f7d-3559">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3559">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3560">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3560">VM</span></span>

* <span data-ttu-id="f6f7d-3561">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3561">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="f6f7d-3562">5\. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3562">December 5, 2017</span></span>

<span data-ttu-id="f6f7d-3563">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3563">Version 2.0.22</span></span>

* <span data-ttu-id="f6f7d-3564">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3564">Removed `az component` commands.</span></span> <span data-ttu-id="f6f7d-3565">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3565">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-3566">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3566">Core</span></span>
* <span data-ttu-id="f6f7d-3567">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3567">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="f6f7d-3568">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3568">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3569">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3569">ACS</span></span>

* <span data-ttu-id="f6f7d-3570">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3570">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="f6f7d-3571">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3571">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="f6f7d-3572">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3572">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="f6f7d-3573">Advisor</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3573">Advisor</span></span>

* <span data-ttu-id="f6f7d-3574">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3574">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3575">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3575">Appservice</span></span>

* <span data-ttu-id="f6f7d-3576">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3576">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="f6f7d-3577">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3577">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="f6f7d-3578">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3578">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="f6f7d-3579">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3579">Consumption</span></span>

* <span data-ttu-id="f6f7d-3580">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3580">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-3581">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3581">Container</span></span>

* <span data-ttu-id="f6f7d-3582">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3582">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-3583">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3583">Monitor</span></span>

* <span data-ttu-id="f6f7d-3584">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3584">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-3585">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3585">Resource</span></span>

* <span data-ttu-id="f6f7d-3586">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3586">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-3587">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3587">Role</span></span>

* <span data-ttu-id="f6f7d-3588">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3588">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="f6f7d-3589">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3589">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="f6f7d-3590">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3590">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-3591">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3591">SQL</span></span>

* <span data-ttu-id="f6f7d-3592">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3592">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="f6f7d-3593">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3593">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3594">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3594">VM</span></span>

* <span data-ttu-id="f6f7d-3595">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3595">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="f6f7d-3596">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3596">November 14, 2017</span></span>

<span data-ttu-id="f6f7d-3597">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3597">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-3598">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3598">ACR</span></span>

* <span data-ttu-id="f6f7d-3599">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3599">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="f6f7d-3600">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3600">ACS</span></span>

* <span data-ttu-id="f6f7d-3601">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3601">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="f6f7d-3602">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3602">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="f6f7d-3603">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3603">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="f6f7d-3604">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3604">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="f6f7d-3605">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3605">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3606">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3606">Appservice</span></span>

* <span data-ttu-id="f6f7d-3607">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3607">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="f6f7d-3608">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3608">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="f6f7d-3609">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3609">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="f6f7d-3610">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3610">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="f6f7d-3611">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3611">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="f6f7d-3612">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3612">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-3613">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3613">Batch</span></span>

* <span data-ttu-id="f6f7d-3614">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3614">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="f6f7d-3615">BatchAI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3615">Batchai</span></span>

* <span data-ttu-id="f6f7d-3616">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3616">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="f6f7d-3617">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3617">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="f6f7d-3618">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3618">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="f6f7d-3619">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3619">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="f6f7d-3620">Cloud</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3620">Cloud</span></span>

* <span data-ttu-id="f6f7d-3621">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3621">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-3622">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3622">Container</span></span>

* <span data-ttu-id="f6f7d-3623">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3623">Added support to open multiple ports</span></span>
* <span data-ttu-id="f6f7d-3624">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3624">Added container group restart policy</span></span>
* <span data-ttu-id="f6f7d-3625">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3625">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="f6f7d-3626">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3626">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f6f7d-3627">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3627">Data Lake Analytics</span></span>

* <span data-ttu-id="f6f7d-3628">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3628">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f6f7d-3629">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3629">Data Lake Store</span></span>

* <span data-ttu-id="f6f7d-3630">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3630">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-3631">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3631">Extension</span></span>

* <span data-ttu-id="f6f7d-3632">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3632">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="f6f7d-3633">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3633">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-3634">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3634">IoT</span></span>

* <span data-ttu-id="f6f7d-3635">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3635">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-3636">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3636">Monitor</span></span>

* <span data-ttu-id="f6f7d-3637">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3637">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3638">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3638">Network</span></span>

* <span data-ttu-id="f6f7d-3639">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3639">Added support for CAA DNS records</span></span>
* <span data-ttu-id="f6f7d-3640">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3640">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="f6f7d-3641">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3641">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="f6f7d-3642">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3642">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="f6f7d-3643">Reservations</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3643">Reservations</span></span>

* <span data-ttu-id="f6f7d-3644">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3644">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-3645">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3645">Resource</span></span>

* <span data-ttu-id="f6f7d-3646">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3646">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-3647">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3647">SQL</span></span>

* <span data-ttu-id="f6f7d-3648">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3648">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3649">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3649">Storage</span></span>

* <span data-ttu-id="f6f7d-3650">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3650">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="f6f7d-3651">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3651">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="f6f7d-3652">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3652">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="f6f7d-3653">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3653">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="f6f7d-3654">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3654">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="f6f7d-3655">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3655">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="f6f7d-3656">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3656">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3657">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3657">VM</span></span>

* <span data-ttu-id="f6f7d-3658">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3658">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="f6f7d-3659">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3659">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="f6f7d-3660">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3660">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="f6f7d-3661">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3661">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="f6f7d-3662">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3662">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="f6f7d-3663">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3663">October 24, 2017</span></span>

<span data-ttu-id="f6f7d-3664">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3664">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-3665">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3665">Core</span></span>

* <span data-ttu-id="f6f7d-3666">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3666">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-3667">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3667">ACR</span></span>

* <span data-ttu-id="f6f7d-3668">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3668">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="f6f7d-3669">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3669">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="f6f7d-3670">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3670">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3671">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3671">ACS</span></span>

* <span data-ttu-id="f6f7d-3672">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3672">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="f6f7d-3673">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3673">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3674">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3674">Appservice</span></span>

* <span data-ttu-id="f6f7d-3675">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3675">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="f6f7d-3676">Komponente</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3676">Component</span></span>

* <span data-ttu-id="f6f7d-3677">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3677">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-3678">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3678">Monitor</span></span>

* <span data-ttu-id="f6f7d-3679">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3679">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-3680">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3680">Resource</span></span>

* <span data-ttu-id="f6f7d-3681">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3681">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="f6f7d-3682">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3682">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3683">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3683">VM</span></span>

* <span data-ttu-id="f6f7d-3684">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3684">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="f6f7d-3685">9\. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3685">October 9, 2017</span></span>

<span data-ttu-id="f6f7d-3686">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3686">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-3687">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3687">Core</span></span>

* <span data-ttu-id="f6f7d-3688">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3688">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3689">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3689">Appservice</span></span>

* <span data-ttu-id="f6f7d-3690">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3690">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-3691">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3691">Batch</span></span>

* <span data-ttu-id="f6f7d-3692">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3692">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="f6f7d-3693">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3693">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="f6f7d-3694">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3694">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="f6f7d-3695">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3695">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="f6f7d-3696">BatchAI</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3696">Batchai</span></span>

* <span data-ttu-id="f6f7d-3697">Erste Version des Batch KI-Moduls</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3697">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-3698">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3698">Keyvault</span></span>

* <span data-ttu-id="f6f7d-3699">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3699">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="f6f7d-3700">(#4448)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3700">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="f6f7d-3701">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3701">Network</span></span>

* <span data-ttu-id="f6f7d-3702">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3702">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="f6f7d-3703">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3703">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-3704">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3704">Resource</span></span>

* <span data-ttu-id="f6f7d-3705">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3705">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="f6f7d-3706">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3706">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="f6f7d-3707">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3707">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="f6f7d-3708">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3708">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-3709">Sql</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3709">Sql</span></span>

* <span data-ttu-id="f6f7d-3710">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3710">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="f6f7d-3711">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3711">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="f6f7d-3712">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3712">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3713">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3713">Storage</span></span>

* <span data-ttu-id="f6f7d-3714">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3714">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3715">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3715">Vm</span></span>

* <span data-ttu-id="f6f7d-3716">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3716">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="f6f7d-3717">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3717">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="f6f7d-3718">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3718">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="f6f7d-3719">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3719">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="f6f7d-3720">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3720">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="f6f7d-3721">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3721">September 22, 2017</span></span>

<span data-ttu-id="f6f7d-3722">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3722">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-3723">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3723">Resource</span></span>

* <span data-ttu-id="f6f7d-3724">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3724">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="f6f7d-3725">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3725">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="f6f7d-3726">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3726">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="f6f7d-3727">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3727">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3728">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3728">Network</span></span>

* <span data-ttu-id="f6f7d-3729">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3729">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="f6f7d-3730">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3730">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="f6f7d-3731">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3731">Added `asg` application security group commands</span></span>
* <span data-ttu-id="f6f7d-3732">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3732">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="f6f7d-3733">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3733">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f6f7d-3734">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3734">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="f6f7d-3735">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3735">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3736">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3736">Storage</span></span>

* <span data-ttu-id="f6f7d-3737">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3737">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f6f7d-3738">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3738">Eventgrid</span></span>

* <span data-ttu-id="f6f7d-3739">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3739">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-3740">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3740">SQL</span></span>

* <span data-ttu-id="f6f7d-3741">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3741">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="f6f7d-3742">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3742">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="f6f7d-3743">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3743">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-3744">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3744">Keyvault</span></span>

* <span data-ttu-id="f6f7d-3745">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3745">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3746">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3746">VM</span></span>

* <span data-ttu-id="f6f7d-3747">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3747">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="f6f7d-3748">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3748">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="f6f7d-3749">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3749">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="f6f7d-3750">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3750">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="f6f7d-3751">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3751">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="f6f7d-3752">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3752">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3753">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3753">ACS</span></span>

* <span data-ttu-id="f6f7d-3754">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3754">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3755">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3755">Appservice</span></span>

* <span data-ttu-id="f6f7d-3756">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3756">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f6f7d-3757">Backup</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3757">Backup</span></span>

* <span data-ttu-id="f6f7d-3758">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3758">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="f6f7d-3759">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3759">September 11, 2017</span></span>

<span data-ttu-id="f6f7d-3760">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3760">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="f6f7d-3761">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3761">Core</span></span>

* <span data-ttu-id="f6f7d-3762">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3762">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="f6f7d-3763">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3763">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3764">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3764">Acs</span></span>

* <span data-ttu-id="f6f7d-3765">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3765">Added `acs list-locations` command</span></span>
* <span data-ttu-id="f6f7d-3766">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3766">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3767">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3767">Appservice</span></span>

* <span data-ttu-id="f6f7d-3768">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3768">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="f6f7d-3769">CDN</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3769">CDN</span></span>

* <span data-ttu-id="f6f7d-3770">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3770">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="f6f7d-3771">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3771">Extension</span></span>

* <span data-ttu-id="f6f7d-3772">Erstrelease</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3772">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-3773">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3773">Keyvault</span></span>

* <span data-ttu-id="f6f7d-3774">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3774">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3775">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3775">Network</span></span>

* <span data-ttu-id="f6f7d-3776">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3776">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f6f7d-3777">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3777">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="f6f7d-3778">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3778">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="f6f7d-3779">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3779">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f6f7d-3780">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3780">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-3781">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3781">Resource</span></span>

* <span data-ttu-id="f6f7d-3782">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3782">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="f6f7d-3783">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3783">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="f6f7d-3784">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3784">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="f6f7d-3785">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3785">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-3786">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3786">SQL</span></span>

* <span data-ttu-id="f6f7d-3787">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3787">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3788">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3788">VM</span></span>

* <span data-ttu-id="f6f7d-3789">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3789">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="f6f7d-3790">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3790">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="f6f7d-3791">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3791">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="f6f7d-3792">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3792">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="f6f7d-3793">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3793">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="f6f7d-3794">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3794">August 31, 2017</span></span>

<span data-ttu-id="f6f7d-3795">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3795">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-3796">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3796">Keyvault</span></span>

* <span data-ttu-id="f6f7d-3797">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3797">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="f6f7d-3798">Sf</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3798">Sf</span></span>

* <span data-ttu-id="f6f7d-3799">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3799">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3800">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3800">Storage</span></span>

* <span data-ttu-id="f6f7d-3801">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3801">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="f6f7d-3802">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3802">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="f6f7d-3803">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3803">August 28, 2017</span></span>

<span data-ttu-id="f6f7d-3804">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3804">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="f6f7d-3805">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3805">CLI</span></span>

* <span data-ttu-id="f6f7d-3806">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3806">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3807">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3807">ACS</span></span>

* <span data-ttu-id="f6f7d-3808">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3808">Corrected preview regions</span></span>
* <span data-ttu-id="f6f7d-3809">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3809">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="f6f7d-3810">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3810">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3811">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3811">Appservice</span></span>

* <span data-ttu-id="f6f7d-3812">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3812">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="f6f7d-3813">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3813">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="f6f7d-3814">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3814">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="f6f7d-3815">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3815">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="f6f7d-3816">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3816">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-3817">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3817">IoT</span></span>

* <span data-ttu-id="f6f7d-3818">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3818">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3819">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3819">Network</span></span>

* <span data-ttu-id="f6f7d-3820">[BREAKING CHANGE]`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3820">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f6f7d-3821">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3821">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="f6f7d-3822">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3822">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f6f7d-3823">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3823">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f6f7d-3824">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3824">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-3825">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3825">Profile</span></span>

* <span data-ttu-id="f6f7d-3826">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3826">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f6f7d-3827">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3827">Service Fabric</span></span>

* <span data-ttu-id="f6f7d-3828">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3828">Preview release</span></span>
* <span data-ttu-id="f6f7d-3829">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3829">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="f6f7d-3830">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3830">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="f6f7d-3831">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3831">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3832">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3832">Storage</span></span>

* <span data-ttu-id="f6f7d-3833">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3833">Enabled setting blob tier</span></span>
* <span data-ttu-id="f6f7d-3834">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3834">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="f6f7d-3835">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3835">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="f6f7d-3836">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3836">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="f6f7d-3837">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3837">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="f6f7d-3838">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3838">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3839">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3839">VM</span></span>

* <span data-ttu-id="f6f7d-3840">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3840">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="f6f7d-3841">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3841">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="f6f7d-3842">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3842">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="f6f7d-3843">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3843">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="f6f7d-3844">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3844">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="f6f7d-3845">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3845">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="f6f7d-3846">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3846">August 15, 2017</span></span>

<span data-ttu-id="f6f7d-3847">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3847">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3848">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3848">ACS</span></span>

* <span data-ttu-id="f6f7d-3849">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3849">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3850">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3850">Appservice</span></span>

* <span data-ttu-id="f6f7d-3851">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3851">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="f6f7d-3852">Event Grid</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3852">Event Grid</span></span>

* <span data-ttu-id="f6f7d-3853">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3853">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="f6f7d-3854">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3854">August 11, 2017</span></span>

<span data-ttu-id="f6f7d-3855">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3855">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3856">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3856">ACS</span></span>

* <span data-ttu-id="f6f7d-3857">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3857">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-3858">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3858">Batch</span></span>

* <span data-ttu-id="f6f7d-3859">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3859">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="f6f7d-3860">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3860">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="f6f7d-3861">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3861">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="f6f7d-3862">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3862">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="f6f7d-3863">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3863">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="f6f7d-3864">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3864">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="f6f7d-3865">Komponente</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3865">Component</span></span>

* <span data-ttu-id="f6f7d-3866">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3866">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="f6f7d-3867">Container</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3867">Container</span></span>

* <span data-ttu-id="f6f7d-3868">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3868">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="f6f7d-3869">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3869">Data Lake Store</span></span>

* <span data-ttu-id="f6f7d-3870">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3870">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="f6f7d-3871">Event Grid</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3871">Event Grid</span></span>

* <span data-ttu-id="f6f7d-3872">Erste Veröffentlichung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3872">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3873">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3873">Network</span></span>

* <span data-ttu-id="f6f7d-3874">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3874">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="f6f7d-3875">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3875">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="f6f7d-3876">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3876">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="f6f7d-3877">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3877">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-3878">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3878">Profile</span></span>

* <span data-ttu-id="f6f7d-3879">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3879">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-3880">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3880">Storage</span></span>

* <span data-ttu-id="f6f7d-3881">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3881">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-3882">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3882">VM</span></span>

* <span data-ttu-id="f6f7d-3883">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3883">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="f6f7d-3884">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3884">Exposed `list-skus` command</span></span>
* <span data-ttu-id="f6f7d-3885">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3885">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="f6f7d-3886">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3886">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="f6f7d-3887">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3887">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="f6f7d-3888">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3888">July 28, 2017</span></span>

<span data-ttu-id="f6f7d-3889">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3889">Version 2.0.12</span></span>

* <span data-ttu-id="f6f7d-3890">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3890">Added container commands</span></span>
* <span data-ttu-id="f6f7d-3891">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3891">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="f6f7d-3892">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3892">Core</span></span>

* <span data-ttu-id="f6f7d-3893">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3893">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="f6f7d-3894">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3894">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="f6f7d-3895">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3895">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="f6f7d-3896">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3896">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="f6f7d-3897">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3897">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="f6f7d-3898">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3898">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="f6f7d-3899">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3899">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f6f7d-3900">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3900">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="f6f7d-3901">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3901">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="f6f7d-3902">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3902">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="f6f7d-3903">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3903">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="f6f7d-3904">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3904">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="f6f7d-3905">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3905">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="f6f7d-3906">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3906">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="f6f7d-3907">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3907">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="f6f7d-3908">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3908">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="f6f7d-3909">ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3909">ACR</span></span>

* <span data-ttu-id="f6f7d-3910">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3910">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="f6f7d-3911">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3911">Support SKU update for managed registries</span></span>
* <span data-ttu-id="f6f7d-3912">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3912">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="f6f7d-3913">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3913">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="f6f7d-3914">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3914">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="f6f7d-3915">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3915">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-3916">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3916">ACS</span></span>

* <span data-ttu-id="f6f7d-3917">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3917">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-3918">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3918">Appservice</span></span>

* <span data-ttu-id="f6f7d-3919">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3919">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="f6f7d-3920">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3920">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="f6f7d-3921">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3921">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="f6f7d-3922">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3922">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="f6f7d-3923">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3923">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="f6f7d-3924">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3924">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="f6f7d-3925">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3925">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="f6f7d-3926">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3926">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="f6f7d-3927">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3927">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="f6f7d-3928">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3928">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="f6f7d-3929">Batch</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3929">Batch</span></span>

* <span data-ttu-id="f6f7d-3930">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3930">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="f6f7d-3931">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3931">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="f6f7d-3932">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3932">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="f6f7d-3933">CDN</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3933">CDN</span></span>

* <span data-ttu-id="f6f7d-3934">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3934">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="f6f7d-3935">Cloud</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3935">Cloud</span></span>

* <span data-ttu-id="f6f7d-3936">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3936">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="f6f7d-3937">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3937">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="f6f7d-3938">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3938">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="f6f7d-3939">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3939">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="f6f7d-3940">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3940">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6f7d-3941">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3941">CosmosDB</span></span>

* <span data-ttu-id="f6f7d-3942">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3942">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="f6f7d-3943">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3943">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f6f7d-3944">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3944">Data Lake Analytics</span></span>

* <span data-ttu-id="f6f7d-3945">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3945">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="f6f7d-3946">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3946">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="f6f7d-3947">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3947">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f6f7d-3948">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3948">Data Lake Store</span></span>

* <span data-ttu-id="f6f7d-3949">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3949">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="f6f7d-3950">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3950">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="f6f7d-3951">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3951">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="f6f7d-3952">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3952">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="f6f7d-3953">Interactive</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3953">Interactive</span></span>

* <span data-ttu-id="f6f7d-3954">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3954">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="f6f7d-3955">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3955">Increased test coverage</span></span>
* <span data-ttu-id="f6f7d-3956">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3956">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="f6f7d-3957">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3957">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="f6f7d-3958">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3958">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="f6f7d-3959">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3959">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="f6f7d-3960">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3960">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f6f7d-3961">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3961">Added `--progress` flag</span></span>
* <span data-ttu-id="f6f7d-3962">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3962">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="f6f7d-3963">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3963">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="f6f7d-3964">IoT</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3964">IoT</span></span>

* <span data-ttu-id="f6f7d-3965">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3965">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="f6f7d-3966">(3934)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3966">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="f6f7d-3967">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3967">Key vault</span></span>

* <span data-ttu-id="f6f7d-3968">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3968">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="f6f7d-3969">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3969">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="f6f7d-3970">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3970">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f6f7d-3971">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3971">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f6f7d-3972">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3972">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="f6f7d-3973">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3973">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="f6f7d-3974">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3974">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="f6f7d-3975">(3307)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3975">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="f6f7d-3976">Labor</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3976">Lab</span></span>

* <span data-ttu-id="f6f7d-3977">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3977">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="f6f7d-3978">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3978">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-3979">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3979">Monitor</span></span>

* <span data-ttu-id="f6f7d-3980">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3980">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="f6f7d-3981">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3981">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="f6f7d-3982">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3982">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="f6f7d-3983">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3983">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="f6f7d-3984">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3984">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="f6f7d-3985">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3985">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="f6f7d-3986">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3986">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="f6f7d-3987">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3987">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="f6f7d-3988">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3988">`location` no longer required</span></span>
  * <span data-ttu-id="f6f7d-3989">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3989">Add name and ID support for target</span></span>
  * <span data-ttu-id="f6f7d-3990">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3990">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="f6f7d-3991">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3991">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="f6f7d-3992">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3992">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="f6f7d-3993">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3993">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="f6f7d-3994">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3994">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="f6f7d-3995">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3995">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-3996">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3996">Network</span></span>

* <span data-ttu-id="f6f7d-3997">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3997">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="f6f7d-3998">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3998">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="f6f7d-3999">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-3999">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="f6f7d-4000">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4000">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="f6f7d-4001">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4001">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="f6f7d-4002">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4002">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="f6f7d-4003">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4003">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="f6f7d-4004">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4004">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="f6f7d-4005">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4005">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="f6f7d-4006">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4006">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="f6f7d-4007">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4007">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="f6f7d-4008">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4008">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="f6f7d-4009">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4009">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="f6f7d-4010">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4010">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="f6f7d-4011">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4011">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="f6f7d-4012">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4012">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="f6f7d-4013">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4013">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="f6f7d-4014">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4014">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="f6f7d-4015">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4015">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="f6f7d-4016">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4016">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="f6f7d-4017">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4017">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="f6f7d-4018">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4018">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="f6f7d-4019">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4019">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="f6f7d-4020">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4020">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="f6f7d-4021">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4021">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="f6f7d-4022">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4022">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="f6f7d-4023">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4023">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-4024">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4024">Profile</span></span>

* <span data-ttu-id="f6f7d-4025">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4025">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="f6f7d-4026">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4026">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="f6f7d-4027">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4027">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="f6f7d-4028">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4028">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="f6f7d-4029">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4029">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="f6f7d-4030">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4030">RDBMS</span></span>

* <span data-ttu-id="f6f7d-4031">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4031">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="f6f7d-4032">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4032">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="f6f7d-4033">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4033">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="f6f7d-4034">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4034">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-4035">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4035">Resource</span></span>

* <span data-ttu-id="f6f7d-4036">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4036">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="f6f7d-4037">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4037">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="f6f7d-4038">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4038">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="f6f7d-4039">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4039">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="f6f7d-4040">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4040">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="f6f7d-4041">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4041">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="f6f7d-4042">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4042">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="f6f7d-4043">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4043">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-4044">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4044">Role</span></span>

* <span data-ttu-id="f6f7d-4045">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4045">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="f6f7d-4046">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4046">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="f6f7d-4047">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4047">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="f6f7d-4048">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4048">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="f6f7d-4049">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4049">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f6f7d-4050">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4050">Service Fabric</span></span>
* <span data-ttu-id="f6f7d-4051">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4051">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="f6f7d-4052">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4052">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="f6f7d-4053">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4053">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-4054">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4054">SQL</span></span>

* <span data-ttu-id="f6f7d-4055">Fehlerhafte1 Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4055">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="f6f7d-4056">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4056">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="f6f7d-4057">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4057">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-4058">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4058">Storage</span></span>

* <span data-ttu-id="f6f7d-4059">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4059">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="f6f7d-4060">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4060">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="f6f7d-4061">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4061">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="f6f7d-4062">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4062">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="f6f7d-4063">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4063">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="f6f7d-4064">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4064">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-4065">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4065">VM</span></span>

* <span data-ttu-id="f6f7d-4066">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4066">Support configuring nsg</span></span>
* <span data-ttu-id="f6f7d-4067">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4067">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="f6f7d-4068">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4068">Support managed service identities</span></span>
* <span data-ttu-id="f6f7d-4069">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4069">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="f6f7d-4070">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4070">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="f6f7d-4071">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4071">May 10, 2017</span></span>

<span data-ttu-id="f6f7d-4072">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4072">Version 2.0.6</span></span>

* <span data-ttu-id="f6f7d-4073">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4073">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="f6f7d-4074">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4074">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="f6f7d-4075">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4075">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="f6f7d-4076">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4076">Include Cognitive Services module</span></span>
* <span data-ttu-id="f6f7d-4077">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4077">Include Service Fabric module</span></span>
* <span data-ttu-id="f6f7d-4078">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4078">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="f6f7d-4079">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4079">Add support for CDN commands</span></span>
* <span data-ttu-id="f6f7d-4080">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4080">Remove Container module</span></span>
* <span data-ttu-id="f6f7d-4081">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4081">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="f6f7d-4082">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4082">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="f6f7d-4083">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4083">Core</span></span>

* <span data-ttu-id="f6f7d-4084">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4084">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="f6f7d-4085">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4085">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="f6f7d-4086">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4086">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="f6f7d-4087">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4087">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="f6f7d-4088">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4088">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="f6f7d-4089">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4089">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="f6f7d-4090">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4090">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="f6f7d-4091">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4091">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="f6f7d-4092">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4092">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="f6f7d-4093">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4093">core: Improved performance</span></span>
* <span data-ttu-id="f6f7d-4094">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4094">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="f6f7d-4095">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4095">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-4096">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4096">ACS</span></span>

* <span data-ttu-id="f6f7d-4097">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4097">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="f6f7d-4098">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4098">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="f6f7d-4099">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4099">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="f6f7d-4100">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4100">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-4101">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4101">AppService</span></span>

* <span data-ttu-id="f6f7d-4102">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4102">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="f6f7d-4103">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4103">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="f6f7d-4104">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4104">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="f6f7d-4105">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4105">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="f6f7d-4106">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4106">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="f6f7d-4107">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4107">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="f6f7d-4108">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4108">support slot swap with preview</span></span>
* <span data-ttu-id="f6f7d-4109">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4109">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="f6f7d-4110">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4110">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f6f7d-4111">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4111">CosmosDB</span></span>

* <span data-ttu-id="f6f7d-4112">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4112">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="f6f7d-4113">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4113">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="f6f7d-4114">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4114">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="f6f7d-4115">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4115">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f6f7d-4116">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4116">Data Lake Analytics</span></span>

* <span data-ttu-id="f6f7d-4117">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4117">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="f6f7d-4118">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4118">Add support for new catalog item type: package.</span></span> <span data-ttu-id="f6f7d-4119">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4119">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="f6f7d-4120">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4120">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="f6f7d-4121">Tabelle</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4121">Table</span></span>
  * <span data-ttu-id="f6f7d-4122">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4122">Table valued function</span></span>
  * <span data-ttu-id="f6f7d-4123">Sicht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4123">View</span></span>
  * <span data-ttu-id="f6f7d-4124">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4124">Table Statistics.</span></span> <span data-ttu-id="f6f7d-4125">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4125">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f6f7d-4126">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4126">Data Lake Store</span></span>

* <span data-ttu-id="f6f7d-4127">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4127">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="f6f7d-4128">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4128">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="f6f7d-4129">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4129">missed help for access show.</span></span> <span data-ttu-id="f6f7d-4130">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4130">adding it.</span></span> <span data-ttu-id="f6f7d-4131">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4131">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="f6f7d-4132">Suchen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4132">Find</span></span>

* <span data-ttu-id="f6f7d-4133">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4133">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="f6f7d-4134">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4134">KeyVault</span></span>

* <span data-ttu-id="f6f7d-4135">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4135">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="f6f7d-4136">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4136">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="f6f7d-4137">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4137">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="f6f7d-4138">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4138">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="f6f7d-4139">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4139">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="f6f7d-4140">Labor</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4140">Lab</span></span>

* <span data-ttu-id="f6f7d-4141">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4141">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="f6f7d-4142">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4142">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="f6f7d-4143">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4143">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="f6f7d-4144">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4144">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="f6f7d-4145">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4145">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="f6f7d-4146">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4146">Monitor</span></span>

* <span data-ttu-id="f6f7d-4147">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4147">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="f6f7d-4148">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4148">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="f6f7d-4149">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4149">Network</span></span>

* <span data-ttu-id="f6f7d-4150">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4150">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="f6f7d-4151">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4151">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="f6f7d-4152">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4152">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="f6f7d-4153">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4153">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="f6f7d-4154">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4154">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="f6f7d-4155">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4155">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="f6f7d-4156">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4156">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="f6f7d-4157">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4157">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="f6f7d-4158">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4158">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="f6f7d-4159">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4159">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="f6f7d-4160">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4160">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="f6f7d-4161">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4161">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="f6f7d-4162">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4162">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="f6f7d-4163">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4163">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="f6f7d-4164">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4164">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="f6f7d-4165">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4165">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="f6f7d-4166">Profil</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4166">Profile</span></span>

* <span data-ttu-id="f6f7d-4167">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4167">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="f6f7d-4168">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4168">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="f6f7d-4169">Redis</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4169">Redis</span></span>

* <span data-ttu-id="f6f7d-4170">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4170">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="f6f7d-4171">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4171">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="f6f7d-4172">Resource</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4172">Resource</span></span>

* <span data-ttu-id="f6f7d-4173">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4173">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="f6f7d-4174">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4174">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="f6f7d-4175">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4175">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="f6f7d-4176">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4176">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="f6f7d-4177">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4177">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="f6f7d-4178">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4178">Add docs for az lock update.</span></span> <span data-ttu-id="f6f7d-4179">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4179">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="f6f7d-4180">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4180">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="f6f7d-4181">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4181">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="f6f7d-4182">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4182">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="f6f7d-4183">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4183">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="f6f7d-4184">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4184">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="f6f7d-4185">Role</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4185">Role</span></span>

* <span data-ttu-id="f6f7d-4186">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4186">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="f6f7d-4187">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4187">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="f6f7d-4188">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4188">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="f6f7d-4189">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4189">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="f6f7d-4190">SQL</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4190">SQL</span></span>

* <span data-ttu-id="f6f7d-4191">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4191">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="f6f7d-4192">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4192">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="f6f7d-4193">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4193">Storage</span></span>

* <span data-ttu-id="f6f7d-4194">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4194">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="f6f7d-4195">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4195">Add support for incremental blob copy</span></span>
* <span data-ttu-id="f6f7d-4196">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4196">Add support for large block blob upload</span></span>
* <span data-ttu-id="f6f7d-4197">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4197">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-4198">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4198">VM</span></span>

* <span data-ttu-id="f6f7d-4199">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4199">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="f6f7d-4200">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4200">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="f6f7d-4201">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4201">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="f6f7d-4202">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4202">az vm/vmss disk</span></span>
  3. <span data-ttu-id="f6f7d-4203">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4203">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="f6f7d-4204">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4204">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="f6f7d-4205">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4205">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="f6f7d-4206">3\. April 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4206">April 3, 2017</span></span>

<span data-ttu-id="f6f7d-4207">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4207">Version 2.0.2</span></span>

<span data-ttu-id="f6f7d-4208">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4208">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="f6f7d-4209">Core</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4209">Core</span></span>

* <span data-ttu-id="f6f7d-4210">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4210">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="f6f7d-4211">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4211">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="f6f7d-4212">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4212">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="f6f7d-4213">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4213">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f6f7d-4214">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4214">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="f6f7d-4215">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4215">Add prompting for missing template parameters.</span></span> <span data-ttu-id="f6f7d-4216">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4216">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="f6f7d-4217">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4217">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="f6f7d-4218">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4218">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="f6f7d-4219">ACS</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4219">ACS</span></span>

* <span data-ttu-id="f6f7d-4220">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4220">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="f6f7d-4221">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4221">Add support for ssh key password prompting.</span></span> <span data-ttu-id="f6f7d-4222">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4222">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="f6f7d-4223">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4223">Add support for windows clusters.</span></span> <span data-ttu-id="f6f7d-4224">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4224">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="f6f7d-4225">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4225">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="f6f7d-4226">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4226">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="f6f7d-4227">AppService</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4227">AppService</span></span>

* <span data-ttu-id="f6f7d-4228">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4228">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="f6f7d-4229">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4229">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="f6f7d-4230">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4230">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="f6f7d-4231">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4231">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="f6f7d-4232">DataLake</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4232">DataLake</span></span>

* <span data-ttu-id="f6f7d-4233">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4233">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="f6f7d-4234">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4234">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="f6f7d-4235">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4235">DocuemntDB</span></span>

* <span data-ttu-id="f6f7d-4236">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4236">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="f6f7d-4237">VM</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4237">VM</span></span>

* <span data-ttu-id="f6f7d-4238">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4238">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="f6f7d-4239">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4239">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="f6f7d-4240">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4240">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="f6f7d-4241">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4241">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f6f7d-4242">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4242">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="f6f7d-4243">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4243">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="f6f7d-4244">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4244">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="f6f7d-4245">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4245">February 27, 2017</span></span>

<span data-ttu-id="f6f7d-4246">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4246">Version 2.0.0</span></span>

<span data-ttu-id="f6f7d-4247">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4247">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="f6f7d-4248">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4248">Container Service (acs)</span></span>
- <span data-ttu-id="f6f7d-4249">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4249">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="f6f7d-4250">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4250">Networking</span></span>
- <span data-ttu-id="f6f7d-4251">Storage</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4251">Storage</span></span>

<span data-ttu-id="f6f7d-4252">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4252">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="f6f7d-4253">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4253">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="f6f7d-4254">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4254">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="f6f7d-4255">Einige Befehlsmodule verfügen über das Postfix „b *n* “ oder „rc *n* “. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4255">Some of the command modules have a "b *n* " or "rc *n* " postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="f6f7d-4256">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4256">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="f6f7d-4257">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4257">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="f6f7d-4258">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4258">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="f6f7d-4259">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4259">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="f6f7d-4260">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4260">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="f6f7d-4261">Versionshinweise zur Betaversion</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4261">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="f6f7d-4262">Die Azure CLI-Betaversion ist eine Migration der Authentifizierungsmethode der AAD-Plattform (v1.0) zu [Microsoft Identity Platform (v2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4262">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="f6f7d-4263">23. Juni 2020</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4263">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="f6f7d-4264">Wissenswertes über die neue Azure CLI-Betaversion</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4264">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="f6f7d-4265">Die Betaversion der Azure CLI unterstützt alle CLI-Befehle, die in der aktuellen veröffentlichten Version verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4265">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="f6f7d-4266">Nach der Installation der Betaversion ist eine erneute Anmeldung erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4266">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="f6f7d-4267">Die Betaversion unterstützt nur die Windows-Plattform.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4267">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="f6f7d-4268">Azure Stack wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4268">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="f6f7d-4269">Parameter `--use-cert-sn-issuer` wird nicht unterstützt, wenn für die Authentifizierung ein Dienstprinzipalschlüssel verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4269">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="f6f7d-4270">Das Überspringen der SSL-Überprüfung über die Umgebung `ADAL_PYTHON_SSL_NO_VERIFY` wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4270">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="f6f7d-4271">Sollten Probleme in der Betaversion auftreten, können Sie auf [GitHub](https://github.com/Azure/azure-cli/issues/new/choose) gerne Kommentare für das Azure CLI-Entwicklungsteam hinterlassen.</span><span class="sxs-lookup"><span data-stu-id="f6f7d-4271">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---

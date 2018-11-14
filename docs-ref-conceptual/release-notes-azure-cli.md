---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/06/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 51b8b8cad6d25f916006b8e68b8f300587f5d45b
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222564"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="f1254-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f1254-103">Azure CLI release notes</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="f1254-104">6. November 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-104">November 6, 2018</span></span>

<span data-ttu-id="f1254-105">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="f1254-105">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="f1254-106">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-106">Core</span></span>
* <span data-ttu-id="f1254-107">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-107">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-108">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-108">ACR</span></span>
* <span data-ttu-id="f1254-109">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-109">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="f1254-110">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="f1254-110">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-111">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-111">ACS</span></span>
* <span data-ttu-id="f1254-112">[WICHTIGE ÄNDERUNG] `enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="f1254-112">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="f1254-113">Advisor</span><span class="sxs-lookup"><span data-stu-id="f1254-113">Advisor</span></span>
* <span data-ttu-id="f1254-114">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="f1254-114">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="f1254-115">AMS</span><span class="sxs-lookup"><span data-stu-id="f1254-115">AMS</span></span>
* <span data-ttu-id="f1254-116">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f1254-116">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="f1254-117">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f1254-117">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="f1254-118">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-118">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="f1254-119">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="f1254-119">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="f1254-120">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-120">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="f1254-121">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-121">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="f1254-122">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-122">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="f1254-123">[WICHTIGE ÄNDERUNG] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="f1254-123">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="f1254-124">[WICHTIGE ÄNDERUNG] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f1254-124">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="f1254-125">[WICHTIGE ÄNDERUNG] `--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-125">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="f1254-126">[WICHTIGE ÄNDERUNG] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="f1254-126">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="f1254-127">[WICHTIGE ÄNDERUNG] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f1254-127">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="f1254-128">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="f1254-128">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="f1254-129">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="f1254-129">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="f1254-130">[WICHTIGE ÄNDERUNG] `--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="f1254-130">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="f1254-131">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="f1254-131">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="f1254-132">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="f1254-132">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-133">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-133">AppService</span></span>
* <span data-ttu-id="f1254-134">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="f1254-134">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="f1254-135">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="f1254-135">Configure</span></span>
* <span data-ttu-id="f1254-136">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-136">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="f1254-137">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-137">Container</span></span>
* <span data-ttu-id="f1254-138">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="f1254-138">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="f1254-139">EventHub</span><span class="sxs-lookup"><span data-stu-id="f1254-139">EventHub</span></span>
* <span data-ttu-id="f1254-140">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f1254-140">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="f1254-141">Interactive</span><span class="sxs-lookup"><span data-stu-id="f1254-141">Interactive</span></span>
* <span data-ttu-id="f1254-142">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-142">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="f1254-143">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f1254-143">Monitor</span></span>
* <span data-ttu-id="f1254-144">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-144">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="f1254-145">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-145">Network</span></span>
* <span data-ttu-id="f1254-146">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f1254-146">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="f1254-147">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="f1254-147">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="f1254-148">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="f1254-148">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="f1254-149">Profil</span><span class="sxs-lookup"><span data-stu-id="f1254-149">Profile</span></span>
* <span data-ttu-id="f1254-150">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-150">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="f1254-151">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f1254-151">RDBMS</span></span>
* <span data-ttu-id="f1254-152">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-152">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-153">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-153">Resource</span></span>
* <span data-ttu-id="f1254-154">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-154">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="f1254-155">Rolle</span><span class="sxs-lookup"><span data-stu-id="f1254-155">Role</span></span>
* <span data-ttu-id="f1254-156">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-156">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="f1254-157">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="f1254-157">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="f1254-158">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-158">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-159">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-159">Storage</span></span>
* <span data-ttu-id="f1254-160">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="f1254-160">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-161">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-161">VM</span></span>
* <span data-ttu-id="f1254-162">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-162">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="f1254-163">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="f1254-163">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="f1254-164">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f1254-164">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="f1254-165">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="f1254-165">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="f1254-166">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="f1254-166">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="f1254-167">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-167">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="f1254-168">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-168">October 23, 2018</span></span>

<span data-ttu-id="f1254-169">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="f1254-169">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="f1254-170">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-170">Core</span></span>
* <span data-ttu-id="f1254-171">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="f1254-171">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="f1254-172">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="f1254-172">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-173">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-173">ACR</span></span>
* <span data-ttu-id="f1254-174">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-174">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="f1254-175">CDN</span><span class="sxs-lookup"><span data-stu-id="f1254-175">CDN</span></span>
* <span data-ttu-id="f1254-176">[WICHTIGE ÄNDERUNG] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="f1254-176">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="f1254-177">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f1254-177">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="f1254-178">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-178">Container</span></span>
* <span data-ttu-id="f1254-179">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-179">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="f1254-180">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="f1254-180">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="f1254-181">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-181">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="f1254-182">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="f1254-182">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="f1254-183">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="f1254-183">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="f1254-184">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="f1254-184">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="f1254-185">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-185">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f1254-186">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f1254-186">CosmosDB</span></span>
* <span data-ttu-id="f1254-187">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-187">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="f1254-188">Interactive</span><span class="sxs-lookup"><span data-stu-id="f1254-188">Interactive</span></span>
* <span data-ttu-id="f1254-189">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="f1254-189">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="f1254-190">IoT Central</span><span class="sxs-lookup"><span data-stu-id="f1254-190">IoT Central</span></span>
* <span data-ttu-id="f1254-191">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-191">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="f1254-192">[WICHTIGE ÄNDERUNG] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="f1254-192">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="f1254-193">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f1254-193">Monitor</span></span>
* <span data-ttu-id="f1254-194">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="f1254-194">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="f1254-195">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-195">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="f1254-196">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-196">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="f1254-197">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-197">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="f1254-198">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-198">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="f1254-199">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="f1254-199">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="f1254-200">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="f1254-200">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="f1254-201">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-201">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="f1254-202">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-202">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="f1254-203">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-203">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="f1254-204">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-204">Network</span></span>
* <span data-ttu-id="f1254-205">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f1254-205">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="f1254-206">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f1254-206">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="f1254-207">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f1254-207">ServiceBus</span></span>
* <span data-ttu-id="f1254-208">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f1254-208">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-209">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-209">SQL</span></span>
* <span data-ttu-id="f1254-210">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="f1254-210">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-211">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-211">Storage</span></span>
* <span data-ttu-id="f1254-212">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="f1254-212">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="f1254-213">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-213">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-214">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-214">VM</span></span>
* <span data-ttu-id="f1254-215">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="f1254-215">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="f1254-216">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f1254-216">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="f1254-217">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-217">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="f1254-218">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-218">October 16, 2018</span></span>

<span data-ttu-id="f1254-219">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="f1254-219">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-220">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-220">VM</span></span>
* <span data-ttu-id="f1254-221">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="f1254-221">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="f1254-222">9. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-222">October 9, 2018</span></span>

<span data-ttu-id="f1254-223">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="f1254-223">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="f1254-224">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-224">Core</span></span>
* <span data-ttu-id="f1254-225">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="f1254-225">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-226">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-226">ACR</span></span>
* <span data-ttu-id="f1254-227">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-227">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-228">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-228">ACS</span></span>
* <span data-ttu-id="f1254-229">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="f1254-229">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="f1254-230">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="f1254-230">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="f1254-231">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="f1254-231">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="f1254-232">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="f1254-232">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="f1254-233">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-233">Container</span></span>
* <span data-ttu-id="f1254-234">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="f1254-234">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="f1254-235">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-235">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="f1254-236">Event Hub</span><span class="sxs-lookup"><span data-stu-id="f1254-236">Event Hub</span></span>
* <span data-ttu-id="f1254-237">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-237">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="f1254-238">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f1254-238">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="f1254-239">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="f1254-239">Extensions</span></span>
* <span data-ttu-id="f1254-240">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="f1254-240">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="f1254-241">HDInsight</span><span class="sxs-lookup"><span data-stu-id="f1254-241">HDInsight</span></span>
* <span data-ttu-id="f1254-242">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f1254-242">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="f1254-243">IoT</span><span class="sxs-lookup"><span data-stu-id="f1254-243">IoT</span></span>
* <span data-ttu-id="f1254-244">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-244">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="f1254-245">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1254-245">KeyVault</span></span>
* <span data-ttu-id="f1254-246">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="f1254-246">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="f1254-247">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-247">Network</span></span>
* <span data-ttu-id="f1254-248">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="f1254-248">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="f1254-249">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="f1254-249">See #6052</span></span>
* <span data-ttu-id="f1254-250">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="f1254-250">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="f1254-251">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="f1254-251">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="f1254-252">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-252">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="f1254-253">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-253">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="f1254-254">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="f1254-254">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="f1254-255">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-255">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="f1254-256">Rolle</span><span class="sxs-lookup"><span data-stu-id="f1254-256">Role</span></span>
* <span data-ttu-id="f1254-257">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-257">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="f1254-258">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-258">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="f1254-259">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="f1254-259">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="f1254-260">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="f1254-260">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="f1254-261">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f1254-261">Service Bus</span></span>
* <span data-ttu-id="f1254-262">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f1254-262">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-263">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-263">VM</span></span>
* <span data-ttu-id="f1254-264">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-264">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="f1254-265">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="f1254-265">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="f1254-266">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-266">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="f1254-267">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-267">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="f1254-268">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="f1254-268">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="f1254-269">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="f1254-269">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="f1254-270">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-270">September 21, 2018</span></span>

<span data-ttu-id="f1254-271">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="f1254-271">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-272">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-272">ACR</span></span>
* <span data-ttu-id="f1254-273">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-273">Added ACR Task commands</span></span>
* <span data-ttu-id="f1254-274">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-274">Added quick run command</span></span>
* <span data-ttu-id="f1254-275">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f1254-275">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="f1254-276">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f1254-276">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="f1254-277">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-277">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="f1254-278">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-278">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-279">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-279">ACS</span></span>
* <span data-ttu-id="f1254-280">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-280">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="f1254-281">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-281">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-282">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-282">AppService</span></span>

* <span data-ttu-id="f1254-283">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="f1254-283">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="f1254-284">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-284">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="f1254-285">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-285">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="f1254-286">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-286">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="f1254-287">Batch</span><span class="sxs-lookup"><span data-stu-id="f1254-287">Batch</span></span>
* <span data-ttu-id="f1254-288">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f1254-288">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="f1254-289">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f1254-289">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="f1254-290">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-290">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="f1254-291">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-291">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f1254-292">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f1254-292">Batch AI</span></span> 
* <span data-ttu-id="f1254-293">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-293">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f1254-294">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f1254-294">Cognitive Services</span></span>
* <span data-ttu-id="f1254-295">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-295">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="f1254-296">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-296">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="f1254-297">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-297">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="f1254-298">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-298">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="f1254-299">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f1254-299">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="f1254-300">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="f1254-300">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="f1254-301">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-301">Container</span></span>
* <span data-ttu-id="f1254-302">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-302">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="f1254-303">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-303">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="f1254-304">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-304">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="f1254-305">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="f1254-305">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="f1254-306">Data Lake</span><span class="sxs-lookup"><span data-stu-id="f1254-306">Datalake</span></span>
* <span data-ttu-id="f1254-307">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-307">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="f1254-308">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="f1254-308">Interactive Shell</span></span>
* <span data-ttu-id="f1254-309">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-309">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="f1254-310">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-310">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="f1254-311">IoT</span><span class="sxs-lookup"><span data-stu-id="f1254-311">IoT</span></span>
* <span data-ttu-id="f1254-312">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-312">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="f1254-313">Key Vault</span><span class="sxs-lookup"><span data-stu-id="f1254-313">Key Vault</span></span>
* <span data-ttu-id="f1254-314">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-314">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="f1254-315">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-315">Network</span></span>
* <span data-ttu-id="f1254-316">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f1254-316">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="f1254-317">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f1254-317">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="f1254-318">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f1254-318">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="f1254-319">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="f1254-319">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="f1254-320">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-320">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="f1254-321">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-321">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="f1254-322">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f1254-322">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="f1254-323">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="f1254-323">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="f1254-324">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-324">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="f1254-325">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-325">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="f1254-326">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-326">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="f1254-327">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-327">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="f1254-328">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f1254-328">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="f1254-329">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="f1254-329">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="f1254-330">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-330">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="f1254-331">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="f1254-331">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="f1254-332">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-332">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="f1254-333">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-333">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="f1254-334">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f1254-334">RDBMS</span></span>
* <span data-ttu-id="f1254-335">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-335">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="f1254-336">Reservierung</span><span class="sxs-lookup"><span data-stu-id="f1254-336">Reservation</span></span>
* <span data-ttu-id="f1254-337">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-337">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="f1254-338">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-338">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="f1254-339">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="f1254-339">Manage App</span></span>
* <span data-ttu-id="f1254-340">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="f1254-340">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="f1254-341">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="f1254-341">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="f1254-342">Rolle</span><span class="sxs-lookup"><span data-stu-id="f1254-342">Role</span></span>
* <span data-ttu-id="f1254-343">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-343">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="f1254-344">SignalR</span><span class="sxs-lookup"><span data-stu-id="f1254-344">SignalR</span></span>
* <span data-ttu-id="f1254-345">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f1254-345">First release</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-346">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-346">Storage</span></span>
* <span data-ttu-id="f1254-347">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-347">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="f1254-348">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-348">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-349">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-349">VM</span></span>
* <span data-ttu-id="f1254-350">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="f1254-350">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="f1254-351">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-351">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="f1254-352">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-352">August 28, 2018</span></span>

<span data-ttu-id="f1254-353">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="f1254-353">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="f1254-354">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-354">Core</span></span>

* <span data-ttu-id="f1254-355">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="f1254-355">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="f1254-356">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-356">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-357">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-357">ACR</span></span>

* <span data-ttu-id="f1254-358">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-358">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="f1254-359">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="f1254-359">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-360">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-360">ACS</span></span>

* <span data-ttu-id="f1254-361">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="f1254-361">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="f1254-362">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="f1254-362">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-363">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-363">AppService</span></span>

* <span data-ttu-id="f1254-364">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-364">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="f1254-365">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-365">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="f1254-366">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f1254-366">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="f1254-367">Backup</span><span class="sxs-lookup"><span data-stu-id="f1254-367">Backup</span></span>

* <span data-ttu-id="f1254-368">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f1254-368">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="f1254-369">Botdienst</span><span class="sxs-lookup"><span data-stu-id="f1254-369">Bot Service</span></span>

* <span data-ttu-id="f1254-370">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="f1254-370">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f1254-371">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f1254-371">Cognitive Services</span></span>

* <span data-ttu-id="f1254-372">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="f1254-372">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="f1254-373">IoT</span><span class="sxs-lookup"><span data-stu-id="f1254-373">IoT</span></span>

* <span data-ttu-id="f1254-374">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-374">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="f1254-375">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f1254-375">Monitor</span></span>

* <span data-ttu-id="f1254-376">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-376">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="f1254-377">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f1254-377">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f1254-378">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-378">Network</span></span>

* <span data-ttu-id="f1254-379">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f1254-379">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-380">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-380">Resource</span></span>

* <span data-ttu-id="f1254-381">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f1254-381">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-382">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-382">Storage</span></span>

* <span data-ttu-id="f1254-383">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f1254-383">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-384">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-384">VM</span></span>

* <span data-ttu-id="f1254-385">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="f1254-385">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="f1254-386">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="f1254-386">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="f1254-387">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-387">Auguest 14, 2018</span></span>

<span data-ttu-id="f1254-388">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="f1254-388">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="f1254-389">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-389">Core</span></span>

* <span data-ttu-id="f1254-390">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-390">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="f1254-391">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-391">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="f1254-392">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="f1254-392">Telemetry</span></span>

* <span data-ttu-id="f1254-393">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="f1254-393">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-394">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-394">ACR</span></span>

* <span data-ttu-id="f1254-395">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-395">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="f1254-396">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="f1254-396">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-397">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-397">ACS</span></span>

* <span data-ttu-id="f1254-398">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-398">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="f1254-399">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="f1254-399">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="f1254-400">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="f1254-400">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="f1254-401">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="f1254-401">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="f1254-402">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="f1254-402">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="f1254-403">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-403">AppService</span></span>

* <span data-ttu-id="f1254-404">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="f1254-404">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="f1254-405">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-405">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="f1254-406">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f1254-406">BatchAI</span></span>

* <span data-ttu-id="f1254-407">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="f1254-407">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="f1254-408">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-408">Container</span></span>

* <span data-ttu-id="f1254-409">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-409">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="f1254-410">IoT</span><span class="sxs-lookup"><span data-stu-id="f1254-410">IoT</span></span>

* <span data-ttu-id="f1254-411">[WICHTIGE ÄNDERUNG] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-411">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="f1254-412">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="f1254-412">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="f1254-413">Iot Central</span><span class="sxs-lookup"><span data-stu-id="f1254-413">Iot Central</span></span>

* <span data-ttu-id="f1254-414">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="f1254-414">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f1254-415">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1254-415">KeyVault</span></span>


* <span data-ttu-id="f1254-416">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-416">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="f1254-417">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-417">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="f1254-418">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-418">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="f1254-419">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-419">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="f1254-420">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-420">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="f1254-421">Relay</span><span class="sxs-lookup"><span data-stu-id="f1254-421">Relay</span></span>

* <span data-ttu-id="f1254-422">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f1254-422">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-423">Sql</span><span class="sxs-lookup"><span data-stu-id="f1254-423">Sql</span></span>

* <span data-ttu-id="f1254-424">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-424">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-425">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-425">Storage</span></span>

* <span data-ttu-id="f1254-426">[WICHTIGE ÄNDERUNG] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="f1254-426">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="f1254-427">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="f1254-427">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="f1254-428">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-428">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="f1254-429">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="f1254-429">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="f1254-430">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="f1254-430">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-431">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-431">VM</span></span>

* <span data-ttu-id="f1254-432">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-432">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="f1254-433">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-433">July 31, 2018</span></span>

<span data-ttu-id="f1254-434">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="f1254-434">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-435">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-435">ACR</span></span>

* <span data-ttu-id="f1254-436">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-436">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="f1254-437">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-437">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-438">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-438">ACS</span></span>

* <span data-ttu-id="f1254-439">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="f1254-439">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="f1254-440">Batch</span><span class="sxs-lookup"><span data-stu-id="f1254-440">Batch</span></span>

* <span data-ttu-id="f1254-441">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f1254-441">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="f1254-442">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-442">Container</span></span>

* <span data-ttu-id="f1254-443">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-443">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="f1254-444">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-444">Network</span></span>

* <span data-ttu-id="f1254-445">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-445">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="f1254-446">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-446">Resource</span></span>

* <span data-ttu-id="f1254-447">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="f1254-447">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="f1254-448">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="f1254-448">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="f1254-449">Rolle</span><span class="sxs-lookup"><span data-stu-id="f1254-449">Role</span></span>

* <span data-ttu-id="f1254-450">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-450">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="f1254-451">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="f1254-451">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="f1254-452">Suchen,</span><span class="sxs-lookup"><span data-stu-id="f1254-452">Search</span></span>

* <span data-ttu-id="f1254-453">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-453">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="f1254-454">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f1254-454">Service Bus</span></span>

* <span data-ttu-id="f1254-455">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="f1254-455">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="f1254-456">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-456">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="f1254-457">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="f1254-457">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="f1254-458">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="f1254-458">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-459">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-459">Storage</span></span>

* <span data-ttu-id="f1254-460">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-460">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="f1254-461">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="f1254-461">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-462">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-462">VM</span></span>

* <span data-ttu-id="f1254-463">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-463">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="f1254-464">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-464">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="f1254-465">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-465">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="f1254-466">[WICHTIGE ÄNDERUNG] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="f1254-466">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="f1254-467">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-467">July 18, 2018</span></span>

<span data-ttu-id="f1254-468">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="f1254-468">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="f1254-469">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-469">Core</span></span>

* <span data-ttu-id="f1254-470">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-470">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="f1254-471">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-471">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="f1254-472">[WICHTIGE ÄNDERUNG] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="f1254-472">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-473">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-473">ACR</span></span>

* <span data-ttu-id="f1254-474">[WICHTIGE ÄNDERUNG] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-474">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="f1254-475">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-475">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="f1254-476">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f1254-476">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="f1254-477">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-477">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-478">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-478">ACS</span></span>

* <span data-ttu-id="f1254-479">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="f1254-479">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-480">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-480">AppService</span></span>

* <span data-ttu-id="f1254-481">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-481">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="f1254-482">Batch</span><span class="sxs-lookup"><span data-stu-id="f1254-482">Batch</span></span>

* <span data-ttu-id="f1254-483">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="f1254-483">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="f1254-484">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="f1254-484">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f1254-485">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f1254-485">Batch AI</span></span>

* <span data-ttu-id="f1254-486">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-486">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="f1254-487">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-487">Container</span></span>

* <span data-ttu-id="f1254-488">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-488">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="f1254-489">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-489">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="f1254-490">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-490">Network</span></span>

* <span data-ttu-id="f1254-491">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-491">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="f1254-492">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-492">Added `network nic wait`</span></span>
* <span data-ttu-id="f1254-493">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f1254-493">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="f1254-494">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="f1254-494">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="f1254-495">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-495">Resource</span></span>

* <span data-ttu-id="f1254-496">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-496">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="f1254-497">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-497">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="f1254-498">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-498">Added `deployment wait` command</span></span>
* <span data-ttu-id="f1254-499">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-499">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-500">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-500">SQL</span></span>

* <span data-ttu-id="f1254-501">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-501">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="f1254-502">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="f1254-502">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="f1254-503">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-503">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-504">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-504">Storage</span></span>

* <span data-ttu-id="f1254-505">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="f1254-505">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-506">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-506">VM</span></span>

* <span data-ttu-id="f1254-507">[WICHTIGE ÄNDERUNG] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f1254-507">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="f1254-508">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-508">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="f1254-509">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-509">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f1254-510">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-510">July 3, 2018</span></span>

<span data-ttu-id="f1254-511">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="f1254-511">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="f1254-512">AKS</span><span class="sxs-lookup"><span data-stu-id="f1254-512">AKS</span></span>

* <span data-ttu-id="f1254-513">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f1254-513">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f1254-514">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-514">July 3, 2018</span></span>

<span data-ttu-id="f1254-515">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="f1254-515">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="f1254-516">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-516">Core</span></span>

* <span data-ttu-id="f1254-517">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-517">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-518">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-518">ACR</span></span>

* <span data-ttu-id="f1254-519">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-519">Added polling build status</span></span>
* <span data-ttu-id="f1254-520">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-520">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="f1254-521">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-521">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-522">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-522">ACS</span></span>

* <span data-ttu-id="f1254-523">[WICHTIGE ÄNDERUNG] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="f1254-523">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="f1254-524">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="f1254-524">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="f1254-525">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f1254-525">Updated options for `aks browse` command.</span></span> <span data-ttu-id="f1254-526">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-526">Added `--listen-port` support</span></span>
* <span data-ttu-id="f1254-527">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f1254-527">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="f1254-528">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="f1254-528">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="f1254-529">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-529">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-530">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-530">AppService</span></span>

* <span data-ttu-id="f1254-531">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-531">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="f1254-532">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-532">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="f1254-533">Backup</span><span class="sxs-lookup"><span data-stu-id="f1254-533">Backup</span></span>

* <span data-ttu-id="f1254-534">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f1254-534">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="f1254-535">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f1254-535">BatchAI</span></span>

* <span data-ttu-id="f1254-536">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-536">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="f1254-537">Cloud</span><span class="sxs-lookup"><span data-stu-id="f1254-537">Cloud</span></span>

* <span data-ttu-id="f1254-538">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-538">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="f1254-539">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-539">Container</span></span>

* <span data-ttu-id="f1254-540">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-540">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="f1254-541">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-541">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="f1254-542">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-542">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="f1254-543">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f1254-543">Extension</span></span>

* <span data-ttu-id="f1254-544">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="f1254-544">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="f1254-545">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-545">Network</span></span>

* <span data-ttu-id="f1254-546">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="f1254-546">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="f1254-547">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f1254-547">Rdbms</span></span>

* <span data-ttu-id="f1254-548">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-548">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-549">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-549">Resource</span></span>

* <span data-ttu-id="f1254-550">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-550">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-551">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-551">VM</span></span>

* <span data-ttu-id="f1254-552">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-552">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="f1254-553">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-553">June 25, 2018</span></span>

<span data-ttu-id="f1254-554">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="f1254-554">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="f1254-555">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="f1254-555">CLI</span></span>

* <span data-ttu-id="f1254-556">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="f1254-556">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="f1254-557">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-557">June 19, 2018</span></span>

<span data-ttu-id="f1254-558">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="f1254-558">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="f1254-559">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-559">Core</span></span>

* <span data-ttu-id="f1254-560">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-560">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-561">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-561">ACR</span></span>

* <span data-ttu-id="f1254-562">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-562">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="f1254-563">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="f1254-563">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-564">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-564">ACS</span></span>

* <span data-ttu-id="f1254-565">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f1254-565">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="f1254-566">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-566">Added `--update` support</span></span>
* <span data-ttu-id="f1254-567">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="f1254-567">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="f1254-568">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f1254-568">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="f1254-569">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-569">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="f1254-570">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="f1254-570">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="f1254-571">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-571">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="f1254-572">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-572">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-573">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-573">AppService</span></span>

* <span data-ttu-id="f1254-574">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-574">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="f1254-575">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-575">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="f1254-576">Batch</span><span class="sxs-lookup"><span data-stu-id="f1254-576">Batch</span></span>

* <span data-ttu-id="f1254-577">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-577">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f1254-578">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f1254-578">Batch AI</span></span>

* <span data-ttu-id="f1254-579">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-579">Added support for workspaces.</span></span> <span data-ttu-id="f1254-580">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="f1254-580">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="f1254-581">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-581">Added support for experiments.</span></span> <span data-ttu-id="f1254-582">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="f1254-582">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="f1254-583">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="f1254-583">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="f1254-584">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-584">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="f1254-585">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="f1254-585">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="f1254-586">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-586">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="f1254-587">[WICHTIGE ÄNDERUNG] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="f1254-587">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="f1254-588">[WICHTIGE ÄNDERUNG] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="f1254-588">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="f1254-589">[WICHTIGE ÄNDERUNG] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f1254-589">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="f1254-590">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="f1254-590">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="f1254-591">[WICHTIGE ÄNDERUNG] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f1254-591">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="f1254-592">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="f1254-592">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="f1254-593">[WICHTIGE ÄNDERUNG] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="f1254-593">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="f1254-594">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="f1254-594">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="f1254-595">[WICHTIGE ÄNDERUNG] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f1254-595">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="f1254-596">[WICHTIGE ÄNDERUNG] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="f1254-596">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="f1254-597">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-597">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="f1254-598">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-598">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="f1254-599">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-599">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="f1254-600">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-600">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="f1254-601">Karten</span><span class="sxs-lookup"><span data-stu-id="f1254-601">Maps</span></span>

* <span data-ttu-id="f1254-602">[WICHTIGE ÄNDERUNG] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="f1254-602">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="f1254-603">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-603">Network</span></span>

* <span data-ttu-id="f1254-604">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="f1254-604">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="f1254-605">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="f1254-605">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="f1254-606">#6502</span><span class="sxs-lookup"><span data-stu-id="f1254-606">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="f1254-607">Reservations</span><span class="sxs-lookup"><span data-stu-id="f1254-607">Reservations</span></span>

* <span data-ttu-id="f1254-608">[WICHTIGE ÄNDERUNG] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-608">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="f1254-609">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-609">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="f1254-610">[WICHTIGE ÄNDERUNG] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-610">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="f1254-611">[WICHTIGE ÄNDERUNG] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-611">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="f1254-612">[WICHTIGE ÄNDERUNG] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-612">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="f1254-613">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-613">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="f1254-614">Rolle</span><span class="sxs-lookup"><span data-stu-id="f1254-614">Role</span></span>

* <span data-ttu-id="f1254-615">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-615">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-616">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-616">SQL</span></span>

* <span data-ttu-id="f1254-617">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="f1254-617">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-618">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-618">Storage</span></span>

* <span data-ttu-id="f1254-619">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-619">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-620">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-620">VM</span></span>

* <span data-ttu-id="f1254-621">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="f1254-621">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="f1254-622">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="f1254-622">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="f1254-623">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="f1254-623">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f1254-624">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-624">June 13, 2018</span></span>

<span data-ttu-id="f1254-625">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="f1254-625">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="f1254-626">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-626">Core</span></span>

* <span data-ttu-id="f1254-627">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="f1254-627">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f1254-628">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-628">June 13, 2018</span></span>

<span data-ttu-id="f1254-629">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="f1254-629">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="f1254-630">AKS</span><span class="sxs-lookup"><span data-stu-id="f1254-630">AKS</span></span>

* <span data-ttu-id="f1254-631">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-631">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="f1254-632">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-632">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="f1254-633">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-633">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="f1254-634">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-634">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="f1254-635">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-635">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-636">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-636">AppService</span></span>

* <span data-ttu-id="f1254-637">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-637">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f1254-638">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-638">June 5, 2018</span></span>

<span data-ttu-id="f1254-639">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="f1254-639">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="f1254-640">Interactive</span><span class="sxs-lookup"><span data-stu-id="f1254-640">Interactive</span></span>

* <span data-ttu-id="f1254-641">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-641">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f1254-642">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-642">June 5, 2018</span></span>

<span data-ttu-id="f1254-643">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="f1254-643">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="f1254-644">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-644">Core</span></span>

* <span data-ttu-id="f1254-645">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-645">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="f1254-646">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="f1254-646">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-647">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-647">ACR</span></span>

* <span data-ttu-id="f1254-648">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-648">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="f1254-649">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-649">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="f1254-650">AKS</span><span class="sxs-lookup"><span data-stu-id="f1254-650">AKS</span></span>

* <span data-ttu-id="f1254-651">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f1254-651">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="f1254-652">Batch</span><span class="sxs-lookup"><span data-stu-id="f1254-652">Batch</span></span>

* <span data-ttu-id="f1254-653">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="f1254-653">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="f1254-654">IoT</span><span class="sxs-lookup"><span data-stu-id="f1254-654">IOT</span></span>

* <span data-ttu-id="f1254-655">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-655">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="f1254-656">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-656">Network</span></span>

* <span data-ttu-id="f1254-657">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="f1254-657">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="f1254-658">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="f1254-658">Policy Insights</span></span>

* <span data-ttu-id="f1254-659">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f1254-659">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="f1254-660">ARM</span><span class="sxs-lookup"><span data-stu-id="f1254-660">ARM</span></span>

* <span data-ttu-id="f1254-661">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-661">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-662">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-662">SQL</span></span>

* <span data-ttu-id="f1254-663">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f1254-663">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="f1254-664">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f1254-664">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="f1254-665">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-665">Storage</span></span>

* <span data-ttu-id="f1254-666">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="f1254-666">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-667">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-667">VM</span></span>

* <span data-ttu-id="f1254-668">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="f1254-668">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="f1254-669">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-669">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="f1254-670">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-670">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="f1254-671">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-671">May 22, 2018</span></span>

<span data-ttu-id="f1254-672">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="f1254-672">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="f1254-673">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-673">Core</span></span>

* <span data-ttu-id="f1254-674">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-674">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-675">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-675">ACS</span></span>

* <span data-ttu-id="f1254-676">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-676">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="f1254-677">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-677">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-678">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-678">AppService</span></span>

* <span data-ttu-id="f1254-679">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="f1254-679">Improved generic update commands</span></span>
* <span data-ttu-id="f1254-680">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-680">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="f1254-681">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-681">Container</span></span>

* <span data-ttu-id="f1254-682">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-682">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="f1254-683">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-683">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f1254-684">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f1254-684">Extension</span></span>

* <span data-ttu-id="f1254-685">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="f1254-685">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="f1254-686">Interactive</span><span class="sxs-lookup"><span data-stu-id="f1254-686">Interactive</span></span>

* <span data-ttu-id="f1254-687">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="f1254-687">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="f1254-688">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="f1254-688">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="f1254-689">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1254-689">KeyVault</span></span>

* <span data-ttu-id="f1254-690">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="f1254-690">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="f1254-691">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-691">Network</span></span>

* <span data-ttu-id="f1254-692">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="f1254-692">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="f1254-693">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="f1254-693">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-694">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-694">SQL</span></span>

* <span data-ttu-id="f1254-695">[WICHTIGE ÄNDERUNG] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="f1254-695">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="f1254-696">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-696">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="f1254-697">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-697">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="f1254-698">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="f1254-698">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="f1254-699">[WICHTIGE ÄNDERUNG] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="f1254-699">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="f1254-700">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="f1254-700">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="f1254-701">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="f1254-701">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="f1254-702">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f1254-702">`edition`.</span></span> <span data-ttu-id="f1254-703">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="f1254-703">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="f1254-704">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="f1254-704">`elasticPoolName`.</span></span> <span data-ttu-id="f1254-705">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="f1254-705">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="f1254-706">[WICHTIGE ÄNDERUNG] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="f1254-706">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="f1254-707">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f1254-707">`edition`.</span></span> <span data-ttu-id="f1254-708">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="f1254-708">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="f1254-709">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="f1254-709">`dtu`.</span></span> <span data-ttu-id="f1254-710">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="f1254-710">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="f1254-711">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="f1254-711">`databaseDtuMin`.</span></span> <span data-ttu-id="f1254-712">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="f1254-712">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="f1254-713">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="f1254-713">`databaseDtuMax`.</span></span> <span data-ttu-id="f1254-714">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="f1254-714">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="f1254-715">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-715">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="f1254-716">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-716">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-717">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-717">Storage</span></span>

* <span data-ttu-id="f1254-718">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-718">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="f1254-719">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-719">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-720">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-720">VM</span></span>

* <span data-ttu-id="f1254-721">[WICHTIGE ÄNDERUNG] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="f1254-721">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="f1254-722">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="f1254-722">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="f1254-723">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-723">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="f1254-724">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-724">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="f1254-725">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-725">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="f1254-726">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-726">May 7, 2018</span></span>

<span data-ttu-id="f1254-727">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="f1254-727">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="f1254-728">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-728">Core</span></span>

* <span data-ttu-id="f1254-729">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="f1254-729">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="f1254-730">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-730">Added limited support for positional arguments</span></span>
* <span data-ttu-id="f1254-731">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f1254-731">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="f1254-732">#5591</span><span class="sxs-lookup"><span data-stu-id="f1254-732">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="f1254-733">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-733">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="f1254-734">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="f1254-734">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="f1254-735">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="f1254-735">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="f1254-736">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="f1254-736">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="f1254-737">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-737">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-738">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-738">ACR</span></span>

* <span data-ttu-id="f1254-739">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-739">Added ACR Build commands</span></span>
* <span data-ttu-id="f1254-740">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-740">Improved resource not found error messages</span></span>
* <span data-ttu-id="f1254-741">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="f1254-741">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="f1254-742">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="f1254-742">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="f1254-743">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="f1254-743">Improved repository commands error messages</span></span>
* <span data-ttu-id="f1254-744">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f1254-744">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-745">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-745">ACS</span></span>

* <span data-ttu-id="f1254-746">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="f1254-746">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="f1254-747">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="f1254-747">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="f1254-748">AMS</span><span class="sxs-lookup"><span data-stu-id="f1254-748">AMS</span></span>

* <span data-ttu-id="f1254-749">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="f1254-749">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-750">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-750">Appservice</span></span>

* <span data-ttu-id="f1254-751">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="f1254-751">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="f1254-752">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-752">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="f1254-753">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-753">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="f1254-754">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-754">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f1254-755">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f1254-755">Batch AI</span></span>

* <span data-ttu-id="f1254-756">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="f1254-756">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f1254-757">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f1254-757">Cognitive Services</span></span>

* <span data-ttu-id="f1254-758">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="f1254-758">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="f1254-759">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f1254-759">Consumption</span></span>

* <span data-ttu-id="f1254-760">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-760">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="f1254-761">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-761">Container</span></span>

* <span data-ttu-id="f1254-762">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="f1254-762">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f1254-763">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f1254-763">Cosmos DB</span></span>

* <span data-ttu-id="f1254-764">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f1254-764">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="f1254-765">DMS</span><span class="sxs-lookup"><span data-stu-id="f1254-765">DMS</span></span>

* <span data-ttu-id="f1254-766">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1254-766">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="f1254-767">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f1254-767">Extension</span></span>

* <span data-ttu-id="f1254-768">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-768">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="f1254-769">Interactive</span><span class="sxs-lookup"><span data-stu-id="f1254-769">Interactive</span></span>

* <span data-ttu-id="f1254-770">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="f1254-770">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="f1254-771">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="f1254-771">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="f1254-772">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-772">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="f1254-773">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-773">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="f1254-774">Labor</span><span class="sxs-lookup"><span data-stu-id="f1254-774">Lab</span></span>

* <span data-ttu-id="f1254-775">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-775">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="f1254-776">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-776">Network</span></span>

* <span data-ttu-id="f1254-777">[WICHTIGE ÄNDERUNG] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="f1254-777">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="f1254-778">Profil</span><span class="sxs-lookup"><span data-stu-id="f1254-778">Profile</span></span>

* <span data-ttu-id="f1254-779">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-779">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="f1254-780">[WICHTIGE ÄNDERUNG] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="f1254-780">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="f1254-781">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-781">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="f1254-782">Redis</span><span class="sxs-lookup"><span data-stu-id="f1254-782">Redis</span></span>

* <span data-ttu-id="f1254-783">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f1254-783">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="f1254-784">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f1254-784">Deprecated `redis list-all`.</span></span> <span data-ttu-id="f1254-785">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="f1254-785">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="f1254-786">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f1254-786">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="f1254-787">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-787">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="f1254-788">Rolle</span><span class="sxs-lookup"><span data-stu-id="f1254-788">Role</span></span>

* <span data-ttu-id="f1254-789">[WICHTIGE ÄNDERUNG] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-789">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-790">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-790">Storage</span></span>

* <span data-ttu-id="f1254-791">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="f1254-791">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="f1254-792">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="f1254-792">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="f1254-793">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="f1254-793">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="f1254-794">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="f1254-794">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="f1254-795">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="f1254-795">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-796">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-796">VM</span></span>

* <span data-ttu-id="f1254-797">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-797">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="f1254-798">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-798">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="f1254-799">[WICHTIGE ÄNDERUNG] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="f1254-799">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="f1254-800">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-800">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="f1254-801">[WICHTIGE ÄNDERUNG] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="f1254-801">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="f1254-802">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-802">Added write accelerator support</span></span>
* <span data-ttu-id="f1254-803">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-803">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="f1254-804">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="f1254-804">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="f1254-805">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="f1254-805">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="f1254-806">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-806">April 10, 2018</span></span>

<span data-ttu-id="f1254-807">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="f1254-807">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-808">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-808">ACR</span></span>

* <span data-ttu-id="f1254-809">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="f1254-809">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-810">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-810">ACS</span></span>

* <span data-ttu-id="f1254-811">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-811">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-812">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-812">Appservice</span></span>

* [WICHTIGE ÄNDERUNG]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="f1254-814">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-814">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="f1254-815">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f1254-815">BatchAI</span></span>

* <span data-ttu-id="f1254-816">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-816">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="f1254-817">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="f1254-817">Job level mounting</span></span>
  - <span data-ttu-id="f1254-818">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="f1254-818">Environment variables with secret values</span></span>
  - <span data-ttu-id="f1254-819">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="f1254-819">Performance counters settings</span></span>
  - <span data-ttu-id="f1254-820">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="f1254-820">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="f1254-821">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="f1254-821">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="f1254-822">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="f1254-822">Usage and limits reporting</span></span>
  - <span data-ttu-id="f1254-823">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="f1254-823">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="f1254-824">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="f1254-824">Support for custom images</span></span>
  - <span data-ttu-id="f1254-825">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-825">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="f1254-826">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="f1254-826">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="f1254-827">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="f1254-827">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="f1254-828">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1254-828">National clouds are supported</span></span>
* <span data-ttu-id="f1254-829">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-829">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="f1254-830">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="f1254-830">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="f1254-831">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-831">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="f1254-832">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="f1254-832">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="f1254-833">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="f1254-833">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="f1254-834">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="f1254-834">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="f1254-835">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="f1254-835">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="f1254-836">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-836">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="f1254-837">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="f1254-837">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="f1254-838">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-838">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="f1254-839">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="f1254-839">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="f1254-840">[WICHTIGE ÄNDERUNG] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="f1254-840">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="f1254-841">[WICHTIGE ÄNDERUNG] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="f1254-841">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="f1254-842">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="f1254-842">Billing</span></span>

* <span data-ttu-id="f1254-843">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-843">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="f1254-844">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f1254-844">Consumption</span></span>

* <span data-ttu-id="f1254-845">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-845">Added `marketplace` commands</span></span>
* <span data-ttu-id="f1254-846">[WICHTIGE ÄNDERUNG] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-846">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="f1254-847">[WICHTIGE ÄNDERUNG] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-847">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="f1254-848">[WICHTIGE ÄNDERUNG] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-848">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="f1254-849">[WICHTIGE ÄNDERUNG] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-849">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="f1254-850">[WICHTIGE ÄNDERUNG] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-850">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="f1254-851">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-851">Container</span></span>

* <span data-ttu-id="f1254-852">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-852">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="f1254-853">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="f1254-853">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="f1254-854">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f1254-854">Extension</span></span>

* <span data-ttu-id="f1254-855">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-855">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="f1254-856">Interactive</span><span class="sxs-lookup"><span data-stu-id="f1254-856">Interactive</span></span>

* <span data-ttu-id="f1254-857">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="f1254-857">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="f1254-858">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-858">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="f1254-859">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-859">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="f1254-860">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-860">Network</span></span>

* <span data-ttu-id="f1254-861">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="f1254-861">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="f1254-862">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-862">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="f1254-863">#4910</span><span class="sxs-lookup"><span data-stu-id="f1254-863">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="f1254-864">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-864">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="f1254-865">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-865">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="f1254-866">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-866">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="f1254-867">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-867">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="f1254-868">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-868">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="f1254-869">Profil</span><span class="sxs-lookup"><span data-stu-id="f1254-869">Profile</span></span>

* <span data-ttu-id="f1254-870">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-870">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="f1254-871">[WICHTIGE ÄNDERUNG] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-871">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="f1254-872">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f1254-872">RDBMS</span></span>

* <span data-ttu-id="f1254-873">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-873">Added `georestore` command</span></span>
* <span data-ttu-id="f1254-874">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-874">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-875">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-875">Resource</span></span>

* <span data-ttu-id="f1254-876">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-876">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="f1254-877">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-877">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-878">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-878">SQL</span></span>

* <span data-ttu-id="f1254-879">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-879">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-880">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-880">Storage</span></span>

* <span data-ttu-id="f1254-881">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-881">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-882">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-882">VM</span></span>

* <span data-ttu-id="f1254-883">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-883">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="f1254-884">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="f1254-884">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="f1254-886">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-886">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="f1254-887">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="f1254-887">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="f1254-888">#5718</span><span class="sxs-lookup"><span data-stu-id="f1254-888">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="f1254-889">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="f1254-889">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="f1254-890">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-890">March 27, 2018</span></span>

<span data-ttu-id="f1254-891">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="f1254-891">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="f1254-892">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-892">Core</span></span>

* <span data-ttu-id="f1254-893">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="f1254-893">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-894">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-894">ACS</span></span>

* <span data-ttu-id="f1254-895">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f1254-895">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-896">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-896">Appservice</span></span>

* <span data-ttu-id="f1254-897">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-897">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="f1254-898">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-898">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f1254-899">Backup</span><span class="sxs-lookup"><span data-stu-id="f1254-899">Backup</span></span>

* <span data-ttu-id="f1254-900">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-900">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="f1254-901">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="f1254-901">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="f1254-902">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="f1254-902">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="f1254-903">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="f1254-903">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="f1254-904">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-904">Container</span></span>

* <span data-ttu-id="f1254-905">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-905">Added `container exec` command.</span></span> <span data-ttu-id="f1254-906">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="f1254-906">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="f1254-907">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="f1254-907">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f1254-908">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f1254-908">Extension</span></span>

* <span data-ttu-id="f1254-909">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="f1254-909">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="f1254-910">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f1254-910">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="f1254-911">[WICHTIGE ÄNDERUNG] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f1254-911">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="f1254-912">Interactive</span><span class="sxs-lookup"><span data-stu-id="f1254-912">Interactive</span></span>

* <span data-ttu-id="f1254-913">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="f1254-913">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="f1254-914">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-914">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="f1254-915">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f1254-915">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="f1254-916">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="f1254-916">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="f1254-917">Labor</span><span class="sxs-lookup"><span data-stu-id="f1254-917">Lab</span></span>

* <span data-ttu-id="f1254-918">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-918">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="f1254-919">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f1254-919">Monitor</span></span>

* <span data-ttu-id="f1254-920">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="f1254-920">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="f1254-921">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken.</span><span class="sxs-lookup"><span data-stu-id="f1254-921">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="f1254-922">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="f1254-922">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="f1254-923">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-923">Network</span></span>

* <span data-ttu-id="f1254-924">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-924">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="f1254-925">Profil</span><span class="sxs-lookup"><span data-stu-id="f1254-925">Profile</span></span>

* <span data-ttu-id="f1254-926">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-926">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f1254-927">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f1254-927">RDBMS</span></span>

* <span data-ttu-id="f1254-928">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-928">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-929">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-929">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="f1254-931">Rolle</span><span class="sxs-lookup"><span data-stu-id="f1254-931">Role</span></span>

* <span data-ttu-id="f1254-932">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-932">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="f1254-933">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="f1254-933">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="f1254-934">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-934">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="f1254-935">[WICHTIGE ÄNDERUNG] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-935">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="f1254-936">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-936">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-937">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-937">Storage</span></span>

* <span data-ttu-id="f1254-938">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-938">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="f1254-939">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursachten</span><span class="sxs-lookup"><span data-stu-id="f1254-939">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-940">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-940">VM</span></span>

* <span data-ttu-id="f1254-941">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-941">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="f1254-942">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-942">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="f1254-943">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="f1254-943">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="f1254-944">[WICHTIGE ÄNDERUNG] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="f1254-944">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="f1254-945">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-945">March 13, 2018</span></span>

<span data-ttu-id="f1254-946">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="f1254-946">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-947">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-947">ACR</span></span>

* <span data-ttu-id="f1254-948">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-948">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="f1254-949">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f1254-949">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="f1254-950">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-950">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-951">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-951">ACS</span></span>

* <span data-ttu-id="f1254-952">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-952">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="f1254-953">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-953">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="f1254-954">Advisor</span><span class="sxs-lookup"><span data-stu-id="f1254-954">Advisor</span></span>

* <span data-ttu-id="f1254-955">[WICHTIGE ÄNDERUNG] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-955">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="f1254-956">[WICHTIGE ÄNDERUNG] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-956">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="f1254-957">[WICHTIGE ÄNDERUNG] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-957">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="f1254-958">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-958">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="f1254-959">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-959">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-960">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-960">Appservice</span></span>

* <span data-ttu-id="f1254-961">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f1254-961">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="f1254-962">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-962">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f1254-963">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="f1254-963">Eventhubs</span></span>

* <span data-ttu-id="f1254-964">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f1254-964">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="f1254-965">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f1254-965">Extension</span></span>

* <span data-ttu-id="f1254-966">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="f1254-966">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="f1254-967">Interactive</span><span class="sxs-lookup"><span data-stu-id="f1254-967">Interactive</span></span>

* <span data-ttu-id="f1254-968">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="f1254-968">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="f1254-969">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="f1254-969">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="f1254-970">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse nicht angezeigt, wenn beim Laden der Befehlstabelle Ausnahme auftrat</span><span class="sxs-lookup"><span data-stu-id="f1254-970">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="f1254-971">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-971">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="f1254-972">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f1254-972">Monitor</span></span>

* <span data-ttu-id="f1254-973">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f1254-973">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="f1254-974">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-974">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="f1254-975">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-975">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="f1254-976">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-976">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="f1254-977">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-977">Network</span></span>

* <span data-ttu-id="f1254-978">[WICHTIGE ÄNDERUNG] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-978">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="f1254-979">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="f1254-979">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="f1254-980">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-980">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="f1254-981">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-981">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="f1254-982">Profil</span><span class="sxs-lookup"><span data-stu-id="f1254-982">Profile</span></span>

* <span data-ttu-id="f1254-983">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f1254-983">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="f1254-984">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-984">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f1254-985">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f1254-985">RDBMS</span></span>

* <span data-ttu-id="f1254-986">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f1254-986">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="f1254-987">Service Bus</span><span class="sxs-lookup"><span data-stu-id="f1254-987">Service Bus</span></span>

* <span data-ttu-id="f1254-988">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f1254-988">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-989">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-989">Storage</span></span>

* <span data-ttu-id="f1254-990">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="f1254-990">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="f1254-991">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: `storage blob [delete-batch|download-batch|upload-batch]`-Batchbefehle lösen bei Vorbedingungsfehlern keinen Fehler mehr aus.</span><span class="sxs-lookup"><span data-stu-id="f1254-991">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-992">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-992">VM</span></span>

* <span data-ttu-id="f1254-993">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="f1254-993">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="f1254-994">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="f1254-994">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="f1254-995">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-995">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="f1254-996">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-996">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="f1254-997">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-997">February 27, 2018</span></span>

<span data-ttu-id="f1254-998">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="f1254-998">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="f1254-999">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-999">Core</span></span>

* <span data-ttu-id="f1254-1000">[5184](https://github.com/Azure/azure-cli/issues/5184) (Problem beim Installieren von Homebrew) behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1000">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="f1254-1001">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1001">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="f1254-1002">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1002">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1003">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1003">ACS</span></span>

* <span data-ttu-id="f1254-1004">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f1254-1004">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="f1254-1005">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="f1254-1005">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="f1254-1006">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1006">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="f1254-1007">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-1007">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1008">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1008">Appservice</span></span>

* <span data-ttu-id="f1254-1009">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="f1254-1009">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="f1254-1010">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="f1254-1010">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f1254-1011">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f1254-1011">Cognitive Services</span></span>

* <span data-ttu-id="f1254-1012">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1012">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="f1254-1013">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f1254-1013">Consumption</span></span>

* <span data-ttu-id="f1254-1014">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1014">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="f1254-1015">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1015">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="f1254-1016">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-1016">Container</span></span>

* <span data-ttu-id="f1254-1017">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="f1254-1017">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="f1254-1018">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1018">Network</span></span>

* <span data-ttu-id="f1254-1019">[5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="f1254-1019">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-1020">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-1020">Resource</span></span>

* <span data-ttu-id="f1254-1021">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="f1254-1021">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="f1254-1022">Rolle</span><span class="sxs-lookup"><span data-stu-id="f1254-1022">Role</span></span>

* <span data-ttu-id="f1254-1023">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-1023">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-1024">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-1024">SQL</span></span>

* <span data-ttu-id="f1254-1025">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="f1254-1025">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-1026">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-1026">Storage</span></span>

* <span data-ttu-id="f1254-1027">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f1254-1027">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1028">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1028">VM</span></span>

* <span data-ttu-id="f1254-1029">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1029">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="f1254-1030">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-1030">February 13, 2018</span></span>

<span data-ttu-id="f1254-1031">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="f1254-1031">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="f1254-1032">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-1032">Core</span></span>

* <span data-ttu-id="f1254-1033">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-1033">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1034">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1034">ACS</span></span>

* <span data-ttu-id="f1254-1035">[WICHTIGE ÄNDERUNG] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-1035">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="f1254-1036">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-1036">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="f1254-1037">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-1037">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="f1254-1038">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1038">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="f1254-1039">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-1039">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="f1254-1040">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-1040">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="f1254-1041">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="f1254-1041">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="f1254-1042">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="f1254-1042">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1043">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1043">Appservice</span></span>

* <span data-ttu-id="f1254-1044">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="f1254-1044">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="f1254-1045">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1045">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="f1254-1046">CDN</span><span class="sxs-lookup"><span data-stu-id="f1254-1046">CDN</span></span>

* <span data-ttu-id="f1254-1047">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1047">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="f1254-1048">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-1048">Container</span></span>

* <span data-ttu-id="f1254-1049">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1049">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="f1254-1050">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1050">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f1254-1051">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f1254-1051">CosmosDB</span></span>

* <span data-ttu-id="f1254-1052">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1052">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="f1254-1053">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f1254-1053">Extension</span></span>

* <span data-ttu-id="f1254-1054">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1054">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="f1254-1055">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1055">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="f1254-1056">Feedback</span><span class="sxs-lookup"><span data-stu-id="f1254-1056">Feedback</span></span>

* <span data-ttu-id="f1254-1057">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1057">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="f1254-1058">Interactive</span><span class="sxs-lookup"><span data-stu-id="f1254-1058">Interactive</span></span>

* <span data-ttu-id="f1254-1059">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="f1254-1059">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="f1254-1060">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1060">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="f1254-1061">IoT</span><span class="sxs-lookup"><span data-stu-id="f1254-1061">IoT</span></span>

* <span data-ttu-id="f1254-1062">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="f1254-1062">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f1254-1063">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="f1254-1063">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f1254-1064">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1064">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="f1254-1065">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-1065">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="f1254-1066">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f1254-1066">Monitor</span></span>

* <span data-ttu-id="f1254-1067">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1067">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="f1254-1068">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1068">Network</span></span>

* <span data-ttu-id="f1254-1069">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="f1254-1069">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="f1254-1070">Profil</span><span class="sxs-lookup"><span data-stu-id="f1254-1070">Profile</span></span>

* <span data-ttu-id="f1254-1071">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="f1254-1071">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-1072">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-1072">Resource</span></span>

* <span data-ttu-id="f1254-1073">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1073">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="f1254-1074">Rolle</span><span class="sxs-lookup"><span data-stu-id="f1254-1074">Role</span></span>

* <span data-ttu-id="f1254-1075">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1075">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-1076">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-1076">SQL</span></span>

* <span data-ttu-id="f1254-1077">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1077">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="f1254-1078">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1078">Added `sql db rename`</span></span>
* <span data-ttu-id="f1254-1079">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1079">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-1080">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-1080">Storage</span></span>

* <span data-ttu-id="f1254-1081">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-1081">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1082">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1082">VM</span></span>

* <span data-ttu-id="f1254-1083">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1083">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="f1254-1084">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1084">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="f1254-1085">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="f1254-1085">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="f1254-1086">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-1086">January 31, 2018</span></span>

<span data-ttu-id="f1254-1087">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="f1254-1087">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="f1254-1088">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-1088">Core</span></span>

* <span data-ttu-id="f1254-1089">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1089">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="f1254-1090">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-1090">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="f1254-1091">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="f1254-1091">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="f1254-1092">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="f1254-1092">Use `--verbose` to see</span></span>
* <span data-ttu-id="f1254-1093">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1093">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1094">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1094">ACS</span></span>

* <span data-ttu-id="f1254-1095">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="f1254-1095">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="f1254-1096">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-1096">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1097">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1097">Appservice</span></span>

* <span data-ttu-id="f1254-1098">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="f1254-1098">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="f1254-1099">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-1099">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="f1254-1100">CDN</span><span class="sxs-lookup"><span data-stu-id="f1254-1100">CDN</span></span>

* <span data-ttu-id="f1254-1101">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1101">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f1254-1102">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f1254-1102">CosmosDB</span></span>

* <span data-ttu-id="f1254-1103">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1103">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="f1254-1104">Interactive</span><span class="sxs-lookup"><span data-stu-id="f1254-1104">Interactive</span></span>

* <span data-ttu-id="f1254-1105">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-1105">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="f1254-1106">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1106">Network</span></span>

* <span data-ttu-id="f1254-1107">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1107">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="f1254-1108">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="f1254-1108">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="f1254-1109">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1109">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="f1254-1110">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1110">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="f1254-1111">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1111">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="f1254-1112">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="f1254-1112">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="f1254-1113">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-1113">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="f1254-1114">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-1114">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="f1254-1115">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-1115">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="f1254-1116">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="f1254-1116">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="f1254-1117">Profil</span><span class="sxs-lookup"><span data-stu-id="f1254-1117">Profile</span></span>

* <span data-ttu-id="f1254-1118">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1118">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-1119">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-1119">Resource</span></span>

* <span data-ttu-id="f1254-1120">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="f1254-1120">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-1121">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-1121">Storage</span></span>

* <span data-ttu-id="f1254-1122">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1122">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="f1254-1123">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1123">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="f1254-1124">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="f1254-1124">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="f1254-1125">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1125">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="f1254-1126">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="f1254-1126">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1127">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1127">VM</span></span>

* <span data-ttu-id="f1254-1128">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-1128">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="f1254-1129">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="f1254-1129">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="f1254-1130">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1130">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="f1254-1131">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1131">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="f1254-1132">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="f1254-1132">January 17, 2018</span></span>

<span data-ttu-id="f1254-1133">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="f1254-1133">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-1134">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-1134">ACR</span></span>

* <span data-ttu-id="f1254-1135">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1135">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="f1254-1136">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="f1254-1136">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1137">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1137">ACS</span></span>

* <span data-ttu-id="f1254-1138">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1138">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="f1254-1139">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-1139">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1140">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1140">Appservice</span></span>

* <span data-ttu-id="f1254-1141">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="f1254-1141">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="f1254-1142">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1142">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="f1254-1143">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1143">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="f1254-1144">Backup</span><span class="sxs-lookup"><span data-stu-id="f1254-1144">Backup</span></span>

* <span data-ttu-id="f1254-1145">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="f1254-1145">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="f1254-1146">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1146">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="f1254-1147">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="f1254-1147">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="f1254-1148">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="f1254-1148">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="f1254-1149">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="f1254-1149">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="f1254-1150">Batch</span><span class="sxs-lookup"><span data-stu-id="f1254-1150">Batch</span></span>

* <span data-ttu-id="f1254-1151">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="f1254-1151">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="f1254-1152">Cloud</span><span class="sxs-lookup"><span data-stu-id="f1254-1152">Cloud</span></span>

* <span data-ttu-id="f1254-1153">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1153">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="f1254-1154">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f1254-1154">Consumption</span></span>

* <span data-ttu-id="f1254-1155">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="f1254-1155">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="f1254-1156">Event Grid</span><span class="sxs-lookup"><span data-stu-id="f1254-1156">Event Grid</span></span>

* <span data-ttu-id="f1254-1157">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="f1254-1157">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f1254-1158">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="f1254-1158">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f1254-1159">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1159">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="f1254-1160">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="f1254-1160">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="f1254-1161">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1161">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="f1254-1162">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1162">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="f1254-1163">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1163">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="f1254-1164">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1164">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="f1254-1165">Interactive</span><span class="sxs-lookup"><span data-stu-id="f1254-1165">Interactive</span></span>

* <span data-ttu-id="f1254-1166">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f1254-1166">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="f1254-1167">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1167">Fixed errors on startup</span></span>
* <span data-ttu-id="f1254-1168">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="f1254-1168">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="f1254-1169">IoT</span><span class="sxs-lookup"><span data-stu-id="f1254-1169">IoT</span></span>

* <span data-ttu-id="f1254-1170">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1170">Added support for device provisioning service</span></span>
* <span data-ttu-id="f1254-1171">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1171">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="f1254-1172">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="f1254-1172">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="f1254-1173">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f1254-1173">Monitor</span></span>

* <span data-ttu-id="f1254-1174">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1174">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="f1254-1175">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f1254-1175">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="f1254-1176">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1176">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="f1254-1177">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1177">Network</span></span>

* <span data-ttu-id="f1254-1178">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="f1254-1178">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="f1254-1179">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1179">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="f1254-1180">Profil</span><span class="sxs-lookup"><span data-stu-id="f1254-1180">Profile</span></span>

* <span data-ttu-id="f1254-1181">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1181">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="f1254-1182">Rolle</span><span class="sxs-lookup"><span data-stu-id="f1254-1182">Role</span></span>

* <span data-ttu-id="f1254-1183">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="f1254-1183">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f1254-1184">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f1254-1184">Service Fabric</span></span>

* <span data-ttu-id="f1254-1185">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1185">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="f1254-1186">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1186">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1187">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1187">VM</span></span>

* <span data-ttu-id="f1254-1188">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="f1254-1188">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="f1254-1189">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-1189">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="f1254-1190">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="f1254-1190">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="f1254-1191">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1191">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="f1254-1192">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1192">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="f1254-1193">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1193">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="f1254-1194">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1194">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="f1254-1195">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1195">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="f1254-1196">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1196">December 19, 2017</span></span>

<span data-ttu-id="f1254-1197">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="f1254-1197">Version 2.0.23</span></span>

* <span data-ttu-id="f1254-1198">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1198">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="f1254-1199">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-1199">Container</span></span>

* <span data-ttu-id="f1254-1200">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1200">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="f1254-1201">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1201">Network</span></span>

* <span data-ttu-id="f1254-1202">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1202">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="f1254-1203">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1203">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-1204">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-1204">Storage</span></span>

* <span data-ttu-id="f1254-1205">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1205">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1206">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1206">VM</span></span>

* <span data-ttu-id="f1254-1207">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1207">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="f1254-1208">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1208">December 5, 2017</span></span>

<span data-ttu-id="f1254-1209">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="f1254-1209">Version 2.0.22</span></span>

* <span data-ttu-id="f1254-1210">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1210">Removed `az component` commands.</span></span> <span data-ttu-id="f1254-1211">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="f1254-1211">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="f1254-1212">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-1212">Core</span></span>
* <span data-ttu-id="f1254-1213">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="f1254-1213">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="f1254-1214">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-1214">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1215">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1215">ACS</span></span>

* <span data-ttu-id="f1254-1216">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1216">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="f1254-1217">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="f1254-1217">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="f1254-1218">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="f1254-1218">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="f1254-1219">Advisor</span><span class="sxs-lookup"><span data-stu-id="f1254-1219">Advisor</span></span>

* <span data-ttu-id="f1254-1220">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f1254-1220">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1221">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1221">Appservice</span></span>

* <span data-ttu-id="f1254-1222">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="f1254-1222">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="f1254-1223">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="f1254-1223">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="f1254-1224">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1224">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="f1254-1225">Nutzung</span><span class="sxs-lookup"><span data-stu-id="f1254-1225">Consumption</span></span>

* <span data-ttu-id="f1254-1226">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1226">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="f1254-1227">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-1227">Container</span></span>

* <span data-ttu-id="f1254-1228">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="f1254-1228">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="f1254-1229">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f1254-1229">Monitor</span></span>

* <span data-ttu-id="f1254-1230">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1230">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-1231">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-1231">Resource</span></span>

* <span data-ttu-id="f1254-1232">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1232">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="f1254-1233">Rolle</span><span class="sxs-lookup"><span data-stu-id="f1254-1233">Role</span></span>

* <span data-ttu-id="f1254-1234">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1234">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="f1254-1235">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1235">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="f1254-1236">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f1254-1236">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-1237">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-1237">SQL</span></span>

* <span data-ttu-id="f1254-1238">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1238">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="f1254-1239">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1239">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1240">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1240">VM</span></span>

* <span data-ttu-id="f1254-1241">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1241">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="f1254-1242">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1242">November 14, 2017</span></span>

<span data-ttu-id="f1254-1243">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="f1254-1243">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-1244">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-1244">ACR</span></span>

* <span data-ttu-id="f1254-1245">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1245">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="f1254-1246">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1246">ACS</span></span>

* <span data-ttu-id="f1254-1247">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-1247">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="f1254-1248">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="f1254-1248">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="f1254-1249">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="f1254-1249">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="f1254-1250">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1250">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="f1254-1251">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1251">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1252">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1252">Appservice</span></span>

* <span data-ttu-id="f1254-1253">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1253">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="f1254-1254">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1254">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="f1254-1255">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-1255">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="f1254-1256">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-1256">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="f1254-1257">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1257">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="f1254-1258">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="f1254-1258">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="f1254-1259">Batch</span><span class="sxs-lookup"><span data-stu-id="f1254-1259">Batch</span></span>

* <span data-ttu-id="f1254-1260">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="f1254-1260">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="f1254-1261">BatchAI</span><span class="sxs-lookup"><span data-stu-id="f1254-1261">Batchai</span></span>

* <span data-ttu-id="f1254-1262">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1262">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="f1254-1263">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1263">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="f1254-1264">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1264">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="f1254-1265">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1265">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="f1254-1266">Cloud</span><span class="sxs-lookup"><span data-stu-id="f1254-1266">Cloud</span></span>

* <span data-ttu-id="f1254-1267">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="f1254-1267">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="f1254-1268">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-1268">Container</span></span>

* <span data-ttu-id="f1254-1269">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1269">Added support to open multiple ports</span></span>
* <span data-ttu-id="f1254-1270">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1270">Added container group restart policy</span></span>
* <span data-ttu-id="f1254-1271">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1271">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="f1254-1272">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1272">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f1254-1273">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f1254-1273">Data Lake Analytics</span></span>

* <span data-ttu-id="f1254-1274">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="f1254-1274">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f1254-1275">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f1254-1275">Data Lake Store</span></span>

* <span data-ttu-id="f1254-1276">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="f1254-1276">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="f1254-1277">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f1254-1277">Extension</span></span>

* <span data-ttu-id="f1254-1278">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-1278">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="f1254-1279">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="f1254-1279">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="f1254-1280">IoT</span><span class="sxs-lookup"><span data-stu-id="f1254-1280">IoT</span></span>

* <span data-ttu-id="f1254-1281">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1281">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="f1254-1282">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f1254-1282">Monitor</span></span>

* <span data-ttu-id="f1254-1283">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1283">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f1254-1284">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1284">Network</span></span>

* <span data-ttu-id="f1254-1285">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1285">Added support for CAA DNS records</span></span>
* <span data-ttu-id="f1254-1286">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="f1254-1286">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="f1254-1287">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="f1254-1287">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="f1254-1288">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-1288">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="f1254-1289">Reservations</span><span class="sxs-lookup"><span data-stu-id="f1254-1289">Reservations</span></span>

* <span data-ttu-id="f1254-1290">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="f1254-1290">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-1291">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-1291">Resource</span></span>

* <span data-ttu-id="f1254-1292">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1292">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-1293">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-1293">SQL</span></span>

* <span data-ttu-id="f1254-1294">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1294">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-1295">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-1295">Storage</span></span>

* <span data-ttu-id="f1254-1296">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="f1254-1296">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="f1254-1297">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="f1254-1297">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="f1254-1298">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="f1254-1298">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="f1254-1299">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1299">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="f1254-1300">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1300">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="f1254-1301">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1301">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="f1254-1302">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-1302">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1303">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1303">VM</span></span>

* <span data-ttu-id="f1254-1304">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="f1254-1304">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="f1254-1305">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1305">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="f1254-1306">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="f1254-1306">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="f1254-1307">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-1307">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="f1254-1308">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1308">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="f1254-1309">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1309">October 24, 2017</span></span>

<span data-ttu-id="f1254-1310">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="f1254-1310">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="f1254-1311">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-1311">Core</span></span>

* <span data-ttu-id="f1254-1312">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="f1254-1312">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-1313">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-1313">ACR</span></span>

* <span data-ttu-id="f1254-1314">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="f1254-1314">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="f1254-1315">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="f1254-1315">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="f1254-1316">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1316">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1317">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1317">ACS</span></span>

* <span data-ttu-id="f1254-1318">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1318">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="f1254-1319">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1319">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1320">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1320">Appservice</span></span>

* <span data-ttu-id="f1254-1321">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="f1254-1321">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="f1254-1322">Komponente</span><span class="sxs-lookup"><span data-stu-id="f1254-1322">Component</span></span>

* <span data-ttu-id="f1254-1323">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1323">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="f1254-1324">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f1254-1324">Monitor</span></span>

* <span data-ttu-id="f1254-1325">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1325">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-1326">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-1326">Resource</span></span>

* <span data-ttu-id="f1254-1327">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1327">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="f1254-1328">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="f1254-1328">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1329">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1329">VM</span></span>

* <span data-ttu-id="f1254-1330">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1330">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="f1254-1331">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1331">October 9, 2017</span></span>

<span data-ttu-id="f1254-1332">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="f1254-1332">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="f1254-1333">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-1333">Core</span></span>

* <span data-ttu-id="f1254-1334">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1334">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1335">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1335">Appservice</span></span>

* <span data-ttu-id="f1254-1336">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1336">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="f1254-1337">Batch</span><span class="sxs-lookup"><span data-stu-id="f1254-1337">Batch</span></span>

* <span data-ttu-id="f1254-1338">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="f1254-1338">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="f1254-1339">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f1254-1339">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="f1254-1340">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1340">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="f1254-1341">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-1341">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="f1254-1342">BatchAI</span><span class="sxs-lookup"><span data-stu-id="f1254-1342">Batchai</span></span>

* <span data-ttu-id="f1254-1343">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="f1254-1343">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f1254-1344">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1254-1344">Keyvault</span></span>

* <span data-ttu-id="f1254-1345">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="f1254-1345">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="f1254-1346">(#4448)</span><span class="sxs-lookup"><span data-stu-id="f1254-1346">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="f1254-1347">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1347">Network</span></span>

* <span data-ttu-id="f1254-1348">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="f1254-1348">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="f1254-1349">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f1254-1349">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-1350">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-1350">Resource</span></span>

* <span data-ttu-id="f1254-1351">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1351">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="f1254-1352">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f1254-1352">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="f1254-1353">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f1254-1353">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="f1254-1354">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f1254-1354">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-1355">Sql</span><span class="sxs-lookup"><span data-stu-id="f1254-1355">Sql</span></span>

* <span data-ttu-id="f1254-1356">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1356">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="f1254-1357">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f1254-1357">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="f1254-1358">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="f1254-1358">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-1359">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-1359">Storage</span></span>

* <span data-ttu-id="f1254-1360">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1360">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1361">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1361">Vm</span></span>

* <span data-ttu-id="f1254-1362">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="f1254-1362">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="f1254-1363">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1363">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="f1254-1364">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1364">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="f1254-1365">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1365">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="f1254-1366">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1366">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="f1254-1367">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1367">September 22, 2017</span></span>

<span data-ttu-id="f1254-1368">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="f1254-1368">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-1369">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-1369">Resource</span></span>

* <span data-ttu-id="f1254-1370">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1370">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="f1254-1371">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1371">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="f1254-1372">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1372">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="f1254-1373">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="f1254-1373">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="f1254-1374">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1374">Network</span></span>

* <span data-ttu-id="f1254-1375">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1375">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="f1254-1376">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1376">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="f1254-1377">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1377">Added `asg` application security group commands</span></span>
* <span data-ttu-id="f1254-1378">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1378">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="f1254-1379">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1379">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f1254-1380">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1380">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="f1254-1381">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1381">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-1382">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-1382">Storage</span></span>

* <span data-ttu-id="f1254-1383">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="f1254-1383">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f1254-1384">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="f1254-1384">Eventgrid</span></span>

* <span data-ttu-id="f1254-1385">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1385">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-1386">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-1386">SQL</span></span>

* <span data-ttu-id="f1254-1387">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="f1254-1387">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="f1254-1388">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1254-1388">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="f1254-1389">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1389">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="f1254-1390">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1254-1390">Keyvault</span></span>

* <span data-ttu-id="f1254-1391">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1391">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1392">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1392">VM</span></span>

* <span data-ttu-id="f1254-1393">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1393">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="f1254-1394">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="f1254-1394">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="f1254-1395">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1395">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="f1254-1396">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1396">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="f1254-1397">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1397">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="f1254-1398">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1398">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1399">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1399">ACS</span></span>

* <span data-ttu-id="f1254-1400">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1400">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1401">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1401">Appservice</span></span>

* <span data-ttu-id="f1254-1402">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="f1254-1402">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f1254-1403">Backup</span><span class="sxs-lookup"><span data-stu-id="f1254-1403">Backup</span></span>

* <span data-ttu-id="f1254-1404">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="f1254-1404">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="f1254-1405">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1405">September 11, 2017</span></span>

<span data-ttu-id="f1254-1406">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="f1254-1406">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="f1254-1407">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-1407">Core</span></span>

* <span data-ttu-id="f1254-1408">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="f1254-1408">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="f1254-1409">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="f1254-1409">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1410">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1410">Acs</span></span>

* <span data-ttu-id="f1254-1411">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1411">Added `acs list-locations` command</span></span>
* <span data-ttu-id="f1254-1412">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="f1254-1412">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1413">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1413">Appservice</span></span>

* <span data-ttu-id="f1254-1414">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="f1254-1414">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="f1254-1415">CDN</span><span class="sxs-lookup"><span data-stu-id="f1254-1415">CDN</span></span>

* <span data-ttu-id="f1254-1416">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="f1254-1416">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="f1254-1417">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="f1254-1417">Extension</span></span>

* <span data-ttu-id="f1254-1418">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f1254-1418">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="f1254-1419">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1254-1419">Keyvault</span></span>

* <span data-ttu-id="f1254-1420">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="f1254-1420">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="f1254-1421">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1421">Network</span></span>

* <span data-ttu-id="f1254-1422">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-1422">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f1254-1423">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1423">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="f1254-1424">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1424">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="f1254-1425">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1425">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f1254-1426">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1426">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-1427">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-1427">Resource</span></span>

* <span data-ttu-id="f1254-1428">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="f1254-1428">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="f1254-1429">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="f1254-1429">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="f1254-1430">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="f1254-1430">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="f1254-1431">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="f1254-1431">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-1432">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-1432">SQL</span></span>

* <span data-ttu-id="f1254-1433">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1433">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1434">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1434">VM</span></span>

* <span data-ttu-id="f1254-1435">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="f1254-1435">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="f1254-1436">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="f1254-1436">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="f1254-1437">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-1437">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="f1254-1438">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="f1254-1438">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="f1254-1439">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="f1254-1439">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="f1254-1440">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1440">August 31, 2017</span></span>

<span data-ttu-id="f1254-1441">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="f1254-1441">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="f1254-1442">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1254-1442">Keyvault</span></span>

* <span data-ttu-id="f1254-1443">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="f1254-1443">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="f1254-1444">Sf</span><span class="sxs-lookup"><span data-stu-id="f1254-1444">Sf</span></span>

* <span data-ttu-id="f1254-1445">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1445">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-1446">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-1446">Storage</span></span>

* <span data-ttu-id="f1254-1447">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="f1254-1447">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="f1254-1448">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="f1254-1448">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="f1254-1449">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1449">August 28, 2017</span></span>

<span data-ttu-id="f1254-1450">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="f1254-1450">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="f1254-1451">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="f1254-1451">CLI</span></span>

* <span data-ttu-id="f1254-1452">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1452">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1453">ACS</span></span>

* <span data-ttu-id="f1254-1454">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1454">Corrected preview regions</span></span>
* <span data-ttu-id="f1254-1455">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1455">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="f1254-1456">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1456">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1457">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1457">Appservice</span></span>

* <span data-ttu-id="f1254-1458">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1458">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="f1254-1459">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1459">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="f1254-1460">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f1254-1460">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="f1254-1461">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="f1254-1461">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="f1254-1462">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="f1254-1462">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="f1254-1463">IoT</span><span class="sxs-lookup"><span data-stu-id="f1254-1463">IoT</span></span>

* <span data-ttu-id="f1254-1464">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="f1254-1464">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="f1254-1465">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1465">Network</span></span>

* <span data-ttu-id="f1254-1466">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-1466">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f1254-1467">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-1467">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="f1254-1468">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1468">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f1254-1469">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1469">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f1254-1470">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1470">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="f1254-1471">Profil</span><span class="sxs-lookup"><span data-stu-id="f1254-1471">Profile</span></span>

* <span data-ttu-id="f1254-1472">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f1254-1472">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f1254-1473">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f1254-1473">Service Fabric</span></span>

* <span data-ttu-id="f1254-1474">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="f1254-1474">Preview release</span></span>
* <span data-ttu-id="f1254-1475">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="f1254-1475">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="f1254-1476">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1476">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="f1254-1477">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1477">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-1478">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-1478">Storage</span></span>

* <span data-ttu-id="f1254-1479">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f1254-1479">Enabled setting blob tier</span></span>
* <span data-ttu-id="f1254-1480">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1480">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="f1254-1481">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1481">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="f1254-1482">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f1254-1482">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="f1254-1483">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-1483">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="f1254-1484">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="f1254-1484">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1485">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1485">VM</span></span>

* <span data-ttu-id="f1254-1486">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-1486">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="f1254-1487">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f1254-1487">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="f1254-1488">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-1488">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="f1254-1489">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="f1254-1489">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="f1254-1490">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1490">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="f1254-1491">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f1254-1491">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="f1254-1492">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1492">August 15, 2017</span></span>

<span data-ttu-id="f1254-1493">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="f1254-1493">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1494">ACS</span></span>

* <span data-ttu-id="f1254-1495">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1495">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1496">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1496">Appservice</span></span>

* <span data-ttu-id="f1254-1497">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1497">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="f1254-1498">Event Grid</span><span class="sxs-lookup"><span data-stu-id="f1254-1498">Event Grid</span></span>

* <span data-ttu-id="f1254-1499">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1499">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="f1254-1500">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1500">August 11, 2017</span></span>

<span data-ttu-id="f1254-1501">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="f1254-1501">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1502">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1502">ACS</span></span>

* <span data-ttu-id="f1254-1503">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1503">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="f1254-1504">Batch</span><span class="sxs-lookup"><span data-stu-id="f1254-1504">Batch</span></span>

* <span data-ttu-id="f1254-1505">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1505">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="f1254-1506">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1506">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="f1254-1507">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1507">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="f1254-1508">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="f1254-1508">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="f1254-1509">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="f1254-1509">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="f1254-1510">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1510">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="f1254-1511">Komponente</span><span class="sxs-lookup"><span data-stu-id="f1254-1511">Component</span></span>

* <span data-ttu-id="f1254-1512">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1512">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="f1254-1513">Container</span><span class="sxs-lookup"><span data-stu-id="f1254-1513">Container</span></span>

* <span data-ttu-id="f1254-1514">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="f1254-1514">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="f1254-1515">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f1254-1515">Data Lake Store</span></span>

* <span data-ttu-id="f1254-1516">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f1254-1516">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="f1254-1517">Event Grid</span><span class="sxs-lookup"><span data-stu-id="f1254-1517">Event Grid</span></span>

* <span data-ttu-id="f1254-1518">Erste Version</span><span class="sxs-lookup"><span data-stu-id="f1254-1518">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="f1254-1519">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1519">Network</span></span>

* <span data-ttu-id="f1254-1520">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-1520">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="f1254-1521">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="f1254-1521">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="f1254-1522">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="f1254-1522">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="f1254-1523">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="f1254-1523">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="f1254-1524">Profil</span><span class="sxs-lookup"><span data-stu-id="f1254-1524">Profile</span></span>

* <span data-ttu-id="f1254-1525">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="f1254-1525">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-1526">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-1526">Storage</span></span>

* <span data-ttu-id="f1254-1527">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f1254-1527">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1528">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1528">VM</span></span>

* <span data-ttu-id="f1254-1529">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f1254-1529">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="f1254-1530">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f1254-1530">Exposed `list-skus` command</span></span>
* <span data-ttu-id="f1254-1531">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="f1254-1531">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="f1254-1532">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="f1254-1532">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="f1254-1533">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-1533">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="f1254-1534">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1534">July 28, 2017</span></span>

<span data-ttu-id="f1254-1535">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="f1254-1535">Version 2.0.12</span></span>

* <span data-ttu-id="f1254-1536">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1536">Added container commands</span></span>
* <span data-ttu-id="f1254-1537">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1537">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="f1254-1538">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-1538">Core</span></span>

* <span data-ttu-id="f1254-1539">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="f1254-1539">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="f1254-1540">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1540">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="f1254-1541">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="f1254-1541">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="f1254-1542">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="f1254-1542">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="f1254-1543">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="f1254-1543">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="f1254-1544">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="f1254-1544">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="f1254-1545">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="f1254-1545">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f1254-1546">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="f1254-1546">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="f1254-1547">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="f1254-1547">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="f1254-1548">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="f1254-1548">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="f1254-1549">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="f1254-1549">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="f1254-1550">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="f1254-1550">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="f1254-1551">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="f1254-1551">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="f1254-1552">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="f1254-1552">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="f1254-1553">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f1254-1553">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="f1254-1554">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="f1254-1554">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="f1254-1555">ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-1555">ACR</span></span>

* <span data-ttu-id="f1254-1556">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1556">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="f1254-1557">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="f1254-1557">Support SKU update for managed registries</span></span>
* <span data-ttu-id="f1254-1558">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1558">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="f1254-1559">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1559">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="f1254-1560">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1560">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="f1254-1561">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1561">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1562">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1562">ACS</span></span>

* <span data-ttu-id="f1254-1563">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="f1254-1563">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1564">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1564">Appservice</span></span>

* <span data-ttu-id="f1254-1565">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="f1254-1565">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="f1254-1566">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="f1254-1566">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="f1254-1567">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="f1254-1567">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="f1254-1568">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="f1254-1568">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="f1254-1569">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="f1254-1569">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="f1254-1570">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="f1254-1570">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="f1254-1571">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="f1254-1571">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="f1254-1572">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="f1254-1572">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="f1254-1573">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1573">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="f1254-1574">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="f1254-1574">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="f1254-1575">Batch</span><span class="sxs-lookup"><span data-stu-id="f1254-1575">Batch</span></span>

* <span data-ttu-id="f1254-1576">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1576">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="f1254-1577">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-1577">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="f1254-1578">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1578">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="f1254-1579">CDN</span><span class="sxs-lookup"><span data-stu-id="f1254-1579">CDN</span></span>

* <span data-ttu-id="f1254-1580">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="f1254-1580">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="f1254-1581">Cloud</span><span class="sxs-lookup"><span data-stu-id="f1254-1581">Cloud</span></span>

* <span data-ttu-id="f1254-1582">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="f1254-1582">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="f1254-1583">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="f1254-1583">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="f1254-1584">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="f1254-1584">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="f1254-1585">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="f1254-1585">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="f1254-1586">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="f1254-1586">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f1254-1587">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f1254-1587">CosmosDB</span></span>

* <span data-ttu-id="f1254-1588">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="f1254-1588">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="f1254-1589">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1589">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f1254-1590">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f1254-1590">Data Lake Analytics</span></span>

* <span data-ttu-id="f1254-1591">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1591">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="f1254-1592">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1592">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="f1254-1593">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1593">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f1254-1594">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f1254-1594">Data Lake Store</span></span>

* <span data-ttu-id="f1254-1595">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1595">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="f1254-1596">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="f1254-1596">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="f1254-1597">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1597">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="f1254-1598">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="f1254-1598">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="f1254-1599">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="f1254-1599">Interactive</span></span>

* <span data-ttu-id="f1254-1600">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-1600">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="f1254-1601">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-1601">Increased test coverage</span></span>
* <span data-ttu-id="f1254-1602">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="f1254-1602">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="f1254-1603">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="f1254-1603">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="f1254-1604">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="f1254-1604">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="f1254-1605">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="f1254-1605">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="f1254-1606">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="f1254-1606">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f1254-1607">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1607">Added `--progress` flag</span></span>
* <span data-ttu-id="f1254-1608">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-1608">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="f1254-1609">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="f1254-1609">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="f1254-1610">IoT</span><span class="sxs-lookup"><span data-stu-id="f1254-1610">IoT</span></span>

* <span data-ttu-id="f1254-1611">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="f1254-1611">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="f1254-1612">(3934)</span><span class="sxs-lookup"><span data-stu-id="f1254-1612">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="f1254-1613">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="f1254-1613">Key vault</span></span>

* <span data-ttu-id="f1254-1614">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="f1254-1614">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="f1254-1615">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f1254-1615">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="f1254-1616">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f1254-1616">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f1254-1617">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f1254-1617">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f1254-1618">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="f1254-1618">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="f1254-1619">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="f1254-1619">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="f1254-1620">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1620">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="f1254-1621">(3307)</span><span class="sxs-lookup"><span data-stu-id="f1254-1621">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="f1254-1622">Labor</span><span class="sxs-lookup"><span data-stu-id="f1254-1622">Lab</span></span>

* <span data-ttu-id="f1254-1623">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1623">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="f1254-1624">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1624">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="f1254-1625">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f1254-1625">Monitor</span></span>

* <span data-ttu-id="f1254-1626">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="f1254-1626">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="f1254-1627">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-1627">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="f1254-1628">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-1628">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="f1254-1629">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-1629">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="f1254-1630">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="f1254-1630">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="f1254-1631">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="f1254-1631">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="f1254-1632">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="f1254-1632">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="f1254-1633">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="f1254-1633">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="f1254-1634">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="f1254-1634">`location` no longer required</span></span>
  * <span data-ttu-id="f1254-1635">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="f1254-1635">Add name and ID support for target</span></span>
  * <span data-ttu-id="f1254-1636">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="f1254-1636">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="f1254-1637">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="f1254-1637">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="f1254-1638">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1638">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="f1254-1639">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="f1254-1639">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="f1254-1640">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="f1254-1640">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="f1254-1641">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1641">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="f1254-1642">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1642">Network</span></span>

* <span data-ttu-id="f1254-1643">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1643">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="f1254-1644">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1644">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="f1254-1645">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="f1254-1645">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="f1254-1646">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="f1254-1646">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="f1254-1647">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="f1254-1647">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="f1254-1648">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1648">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="f1254-1649">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="f1254-1649">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="f1254-1650">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="f1254-1650">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="f1254-1651">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="f1254-1651">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="f1254-1652">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="f1254-1652">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="f1254-1653">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1653">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="f1254-1654">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1654">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="f1254-1655">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="f1254-1655">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="f1254-1656">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1656">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="f1254-1657">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1657">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="f1254-1658">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-1658">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="f1254-1659">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1659">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="f1254-1660">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="f1254-1660">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="f1254-1661">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1661">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="f1254-1662">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1662">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="f1254-1663">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="f1254-1663">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="f1254-1664">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="f1254-1664">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="f1254-1665">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-1665">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="f1254-1666">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f1254-1666">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="f1254-1667">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f1254-1667">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="f1254-1668">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f1254-1668">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="f1254-1669">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="f1254-1669">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="f1254-1670">Profil</span><span class="sxs-lookup"><span data-stu-id="f1254-1670">Profile</span></span>

* <span data-ttu-id="f1254-1671">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="f1254-1671">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="f1254-1672">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="f1254-1672">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="f1254-1673">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="f1254-1673">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="f1254-1674">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1674">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="f1254-1675">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="f1254-1675">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="f1254-1676">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f1254-1676">RDBMS</span></span>

* <span data-ttu-id="f1254-1677">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="f1254-1677">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="f1254-1678">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="f1254-1678">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="f1254-1679">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="f1254-1679">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="f1254-1680">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="f1254-1680">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-1681">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-1681">Resource</span></span>

* <span data-ttu-id="f1254-1682">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-1682">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="f1254-1683">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="f1254-1683">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="f1254-1684">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-1684">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="f1254-1685">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="f1254-1685">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="f1254-1686">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="f1254-1686">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="f1254-1687">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="f1254-1687">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="f1254-1688">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="f1254-1688">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="f1254-1689">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1689">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="f1254-1690">Rolle</span><span class="sxs-lookup"><span data-stu-id="f1254-1690">Role</span></span>

* <span data-ttu-id="f1254-1691">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f1254-1691">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="f1254-1692">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="f1254-1692">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="f1254-1693">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="f1254-1693">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="f1254-1694">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="f1254-1694">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="f1254-1695">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1695">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f1254-1696">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f1254-1696">Service Fabric</span></span>
* <span data-ttu-id="f1254-1697">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="f1254-1697">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="f1254-1698">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="f1254-1698">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="f1254-1699">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="f1254-1699">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-1700">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-1700">SQL</span></span>

* <span data-ttu-id="f1254-1701">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-1701">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="f1254-1702">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="f1254-1702">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="f1254-1703">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1703">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-1704">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-1704">Storage</span></span>

* <span data-ttu-id="f1254-1705">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="f1254-1705">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="f1254-1706">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="f1254-1706">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="f1254-1707">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="f1254-1707">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="f1254-1708">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="f1254-1708">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="f1254-1709">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="f1254-1709">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="f1254-1710">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="f1254-1710">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1711">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1711">VM</span></span>

* <span data-ttu-id="f1254-1712">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="f1254-1712">Support configuring nsg</span></span>
* <span data-ttu-id="f1254-1713">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="f1254-1713">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="f1254-1714">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="f1254-1714">Support managed service identities</span></span>
* <span data-ttu-id="f1254-1715">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="f1254-1715">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="f1254-1716">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="f1254-1716">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="f1254-1717">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1717">May 10, 2017</span></span>

<span data-ttu-id="f1254-1718">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="f1254-1718">Version 2.0.6</span></span>

* <span data-ttu-id="f1254-1719">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="f1254-1719">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="f1254-1720">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="f1254-1720">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="f1254-1721">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="f1254-1721">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="f1254-1722">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="f1254-1722">Include Cognitive Services module</span></span>
* <span data-ttu-id="f1254-1723">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="f1254-1723">Include Service Fabric module</span></span>
* <span data-ttu-id="f1254-1724">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="f1254-1724">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="f1254-1725">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="f1254-1725">Add support for CDN commands</span></span>
* <span data-ttu-id="f1254-1726">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="f1254-1726">Remove Container module</span></span>
* <span data-ttu-id="f1254-1727">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="f1254-1727">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="f1254-1728">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f1254-1728">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="f1254-1729">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-1729">Core</span></span>

* <span data-ttu-id="f1254-1730">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="f1254-1730">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="f1254-1731">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="f1254-1731">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="f1254-1732">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="f1254-1732">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="f1254-1733">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="f1254-1733">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="f1254-1734">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="f1254-1734">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="f1254-1735">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="f1254-1735">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="f1254-1736">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="f1254-1736">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="f1254-1737">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="f1254-1737">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="f1254-1738">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="f1254-1738">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="f1254-1739">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="f1254-1739">core: Improved performance</span></span>
* <span data-ttu-id="f1254-1740">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="f1254-1740">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="f1254-1741">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="f1254-1741">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1742">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1742">ACS</span></span>

* <span data-ttu-id="f1254-1743">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f1254-1743">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="f1254-1744">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="f1254-1744">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="f1254-1745">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="f1254-1745">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="f1254-1746">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="f1254-1746">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1747">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1747">AppService</span></span>

* <span data-ttu-id="f1254-1748">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="f1254-1748">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="f1254-1749">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="f1254-1749">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="f1254-1750">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="f1254-1750">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="f1254-1751">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="f1254-1751">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="f1254-1752">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="f1254-1752">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="f1254-1753">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="f1254-1753">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="f1254-1754">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="f1254-1754">support slot swap with preview</span></span>
* <span data-ttu-id="f1254-1755">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="f1254-1755">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="f1254-1756">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="f1254-1756">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f1254-1757">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f1254-1757">CosmosDB</span></span>

* <span data-ttu-id="f1254-1758">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="f1254-1758">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="f1254-1759">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="f1254-1759">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="f1254-1760">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="f1254-1760">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="f1254-1761">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="f1254-1761">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f1254-1762">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f1254-1762">Data Lake Analytics</span></span>

* <span data-ttu-id="f1254-1763">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="f1254-1763">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="f1254-1764">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="f1254-1764">Add support for new catalog item type: package.</span></span> <span data-ttu-id="f1254-1765">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="f1254-1765">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="f1254-1766">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="f1254-1766">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="f1254-1767">Table</span><span class="sxs-lookup"><span data-stu-id="f1254-1767">Table</span></span>
  * <span data-ttu-id="f1254-1768">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="f1254-1768">Table valued function</span></span>
  * <span data-ttu-id="f1254-1769">Sicht</span><span class="sxs-lookup"><span data-stu-id="f1254-1769">View</span></span>
  * <span data-ttu-id="f1254-1770">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="f1254-1770">Table Statistics.</span></span> <span data-ttu-id="f1254-1771">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="f1254-1771">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f1254-1772">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f1254-1772">Data Lake Store</span></span>

* <span data-ttu-id="f1254-1773">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="f1254-1773">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="f1254-1774">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f1254-1774">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="f1254-1775">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="f1254-1775">missed help for access show.</span></span> <span data-ttu-id="f1254-1776">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="f1254-1776">adding it.</span></span> <span data-ttu-id="f1254-1777">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="f1254-1777">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="f1254-1778">Suchen</span><span class="sxs-lookup"><span data-stu-id="f1254-1778">Find</span></span>

* <span data-ttu-id="f1254-1779">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="f1254-1779">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="f1254-1780">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f1254-1780">KeyVault</span></span>

* <span data-ttu-id="f1254-1781">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="f1254-1781">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="f1254-1782">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="f1254-1782">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="f1254-1783">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="f1254-1783">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="f1254-1784">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="f1254-1784">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="f1254-1785">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="f1254-1785">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="f1254-1786">Labor</span><span class="sxs-lookup"><span data-stu-id="f1254-1786">Lab</span></span>

* <span data-ttu-id="f1254-1787">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="f1254-1787">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="f1254-1788">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="f1254-1788">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="f1254-1789">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="f1254-1789">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="f1254-1790">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="f1254-1790">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="f1254-1791">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="f1254-1791">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="f1254-1792">Überwachen</span><span class="sxs-lookup"><span data-stu-id="f1254-1792">Monitor</span></span>

* <span data-ttu-id="f1254-1793">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="f1254-1793">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="f1254-1794">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="f1254-1794">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="f1254-1795">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1795">Network</span></span>

* <span data-ttu-id="f1254-1796">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="f1254-1796">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="f1254-1797">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="f1254-1797">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="f1254-1798">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="f1254-1798">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="f1254-1799">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="f1254-1799">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="f1254-1800">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="f1254-1800">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="f1254-1801">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="f1254-1801">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="f1254-1802">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="f1254-1802">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="f1254-1803">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="f1254-1803">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="f1254-1804">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="f1254-1804">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="f1254-1805">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="f1254-1805">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="f1254-1806">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="f1254-1806">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="f1254-1807">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="f1254-1807">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="f1254-1808">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="f1254-1808">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="f1254-1809">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="f1254-1809">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="f1254-1810">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="f1254-1810">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="f1254-1811">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="f1254-1811">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="f1254-1812">Profil</span><span class="sxs-lookup"><span data-stu-id="f1254-1812">Profile</span></span>

* <span data-ttu-id="f1254-1813">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="f1254-1813">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="f1254-1814">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="f1254-1814">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="f1254-1815">Redis</span><span class="sxs-lookup"><span data-stu-id="f1254-1815">Redis</span></span>

* <span data-ttu-id="f1254-1816">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="f1254-1816">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="f1254-1817">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="f1254-1817">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="f1254-1818">Ressource</span><span class="sxs-lookup"><span data-stu-id="f1254-1818">Resource</span></span>

* <span data-ttu-id="f1254-1819">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="f1254-1819">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="f1254-1820">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="f1254-1820">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="f1254-1821">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="f1254-1821">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="f1254-1822">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="f1254-1822">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="f1254-1823">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="f1254-1823">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="f1254-1824">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="f1254-1824">Add docs for az lock update.</span></span> <span data-ttu-id="f1254-1825">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="f1254-1825">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="f1254-1826">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="f1254-1826">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="f1254-1827">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="f1254-1827">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="f1254-1828">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="f1254-1828">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="f1254-1829">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="f1254-1829">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="f1254-1830">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="f1254-1830">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="f1254-1831">Rolle</span><span class="sxs-lookup"><span data-stu-id="f1254-1831">Role</span></span>

* <span data-ttu-id="f1254-1832">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="f1254-1832">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="f1254-1833">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="f1254-1833">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="f1254-1834">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="f1254-1834">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="f1254-1835">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="f1254-1835">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="f1254-1836">SQL</span><span class="sxs-lookup"><span data-stu-id="f1254-1836">SQL</span></span>

* <span data-ttu-id="f1254-1837">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="f1254-1837">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="f1254-1838">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="f1254-1838">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="f1254-1839">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-1839">Storage</span></span>

* <span data-ttu-id="f1254-1840">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="f1254-1840">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="f1254-1841">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="f1254-1841">Add support for incremental blob copy</span></span>
* <span data-ttu-id="f1254-1842">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="f1254-1842">Add support for large block blob upload</span></span>
* <span data-ttu-id="f1254-1843">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="f1254-1843">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1844">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1844">VM</span></span>

* <span data-ttu-id="f1254-1845">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="f1254-1845">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="f1254-1846">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="f1254-1846">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="f1254-1847">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="f1254-1847">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="f1254-1848">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="f1254-1848">az vm/vmss disk</span></span>
  3. <span data-ttu-id="f1254-1849">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="f1254-1849">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="f1254-1850">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="f1254-1850">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="f1254-1851">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="f1254-1851">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="f1254-1852">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1852">April 3, 2017</span></span>

<span data-ttu-id="f1254-1853">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="f1254-1853">Version 2.0.2</span></span>

<span data-ttu-id="f1254-1854">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1854">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="f1254-1855">Core</span><span class="sxs-lookup"><span data-stu-id="f1254-1855">Core</span></span>

* <span data-ttu-id="f1254-1856">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="f1254-1856">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="f1254-1857">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="f1254-1857">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="f1254-1858">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="f1254-1858">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="f1254-1859">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f1254-1859">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f1254-1860">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="f1254-1860">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="f1254-1861">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="f1254-1861">Add prompting for missing template parameters.</span></span> <span data-ttu-id="f1254-1862">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="f1254-1862">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="f1254-1863">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1863">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="f1254-1864">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="f1254-1864">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="f1254-1865">ACS</span><span class="sxs-lookup"><span data-stu-id="f1254-1865">ACS</span></span>

* <span data-ttu-id="f1254-1866">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="f1254-1866">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="f1254-1867">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="f1254-1867">Add support for ssh key password prompting.</span></span> <span data-ttu-id="f1254-1868">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="f1254-1868">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="f1254-1869">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="f1254-1869">Add support for windows clusters.</span></span> <span data-ttu-id="f1254-1870">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="f1254-1870">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="f1254-1871">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="f1254-1871">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="f1254-1872">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="f1254-1872">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="f1254-1873">AppService</span><span class="sxs-lookup"><span data-stu-id="f1254-1873">AppService</span></span>

* <span data-ttu-id="f1254-1874">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="f1254-1874">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="f1254-1875">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="f1254-1875">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="f1254-1876">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="f1254-1876">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="f1254-1877">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="f1254-1877">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="f1254-1878">DataLake</span><span class="sxs-lookup"><span data-stu-id="f1254-1878">DataLake</span></span>

* <span data-ttu-id="f1254-1879">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="f1254-1879">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="f1254-1880">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="f1254-1880">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="f1254-1881">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="f1254-1881">DocuemntDB</span></span>

* <span data-ttu-id="f1254-1882">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="f1254-1882">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="f1254-1883">VM</span><span class="sxs-lookup"><span data-stu-id="f1254-1883">VM</span></span>

* <span data-ttu-id="f1254-1884">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="f1254-1884">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="f1254-1885">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="f1254-1885">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="f1254-1886">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="f1254-1886">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="f1254-1887">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f1254-1887">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f1254-1888">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="f1254-1888">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="f1254-1889">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="f1254-1889">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="f1254-1890">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="f1254-1890">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="f1254-1891">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="f1254-1891">February 27, 2017</span></span>

<span data-ttu-id="f1254-1892">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="f1254-1892">Version 2.0.0</span></span>

<span data-ttu-id="f1254-1893">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="f1254-1893">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="f1254-1894">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="f1254-1894">Container Service (acs)</span></span>
- <span data-ttu-id="f1254-1895">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="f1254-1895">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="f1254-1896">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="f1254-1896">Networking</span></span>
- <span data-ttu-id="f1254-1897">Speicher</span><span class="sxs-lookup"><span data-stu-id="f1254-1897">Storage</span></span>

<span data-ttu-id="f1254-1898">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="f1254-1898">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="f1254-1899">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="f1254-1899">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="f1254-1900">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="f1254-1900">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="f1254-1901">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="f1254-1901">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="f1254-1902">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="f1254-1902">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="f1254-1903">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="f1254-1903">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="f1254-1904">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="f1254-1904">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="f1254-1905">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="f1254-1905">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="f1254-1906">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="f1254-1906">Provide feedback from the command line with the `az feedback` command</span></span>


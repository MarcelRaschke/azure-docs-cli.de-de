---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 08/27/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 156ff2e6d011104ebbb1608ff33bad8ebb6396ed
ms.sourcegitcommit: df2be5609a6cbeecb9f8ef0928a9fabfb207e7f9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/27/2019
ms.locfileid: "70047270"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="e62c1-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e62c1-103">Azure CLI release notes</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="e62c1-104">27. August 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-104">August 27, 2019</span></span>

<span data-ttu-id="e62c1-105">Version 2.0.72</span><span class="sxs-lookup"><span data-stu-id="e62c1-105">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-106">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-106">ACR</span></span>

* <span data-ttu-id="e62c1-107">[WICHTIGE ÄNDERUNG] Unterstützung für die SKU `classic` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-107">[BREAKING CHNAGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="e62c1-108">API Management</span><span class="sxs-lookup"><span data-stu-id="e62c1-108">API Management</span></span>

* <span data-ttu-id="e62c1-109">[VORSCHAU] Befehlsgruppe `apim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-109">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-110">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-110">AppService</span></span>

* <span data-ttu-id="e62c1-111">Problem mit dem Befehl `webapp webjob continuous start` bei Angabe eines Slots behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-111">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="e62c1-112">`webapp up` geändert, um den Ordner `env` zu erkennen und aus der für die Bereitstellung verwendeten Datei zu entfernen</span><span class="sxs-lookup"><span data-stu-id="e62c1-112">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="e62c1-113">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e62c1-113">Keyvault</span></span>

* <span data-ttu-id="e62c1-114">Fehler in `keyvault secret set` behoben, aufgrund dessen das Argument `--expires` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-114">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-115">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-115">Network</span></span>

* <span data-ttu-id="e62c1-116">Unterstützung für IPv6-Adressen zu Argumenten vom Typ `--private-ip-address-version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-116">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="e62c1-117">Neue Befehle vom Typ `network private-endpoint [create|update|list-types]` für die Verwaltung privater Endpunkte hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-117">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="e62c1-118">Befehlsgruppe `network private-link-service` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-118">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="e62c1-119">Argumente `--private-endpoint-network-policies` und `--private-link-service-network-policies` zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-119">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="e62c1-120">RBAC</span><span class="sxs-lookup"><span data-stu-id="e62c1-120">RBAC</span></span>

* <span data-ttu-id="e62c1-121">Problem mit `ad app update --homepage` behoben, aufgrund dessen die Startseite nicht aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-121">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="e62c1-122">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e62c1-122">ServiceFabric</span></span>

* <span data-ttu-id="e62c1-123">Unterstützung für Key Vault-Namen mit Groß- und Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-123">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="e62c1-124">Problem bei der Verwendung von Zertifikaten in Key Vault behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-124">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="e62c1-125">Problem bei der Verwendung von PFX-Zertifikatdateien behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-125">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="e62c1-126">Problem mit `sf cluster certificate add` behoben, wenn keine Key Vault-Ressourcengruppe angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-126">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="e62c1-127">Problem behoben, aufgrund dessen `sf cluster set` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="e62c1-127">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="e62c1-128">SignalR</span><span class="sxs-lookup"><span data-stu-id="e62c1-128">SignalR</span></span>

* <span data-ttu-id="e62c1-129">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-129">Added new commands:</span></span>
  * <span data-ttu-id="e62c1-130">`signalr cors`: Verwalten von CORS für SignalR</span><span class="sxs-lookup"><span data-stu-id="e62c1-130">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="e62c1-131">`signalr restart`: Starten eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="e62c1-131">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="e62c1-132">`signalr update`: Aktualisieren eines SignalR-Diensts</span><span class="sxs-lookup"><span data-stu-id="e62c1-132">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="e62c1-133">Argument `--service-mode` zu `signalr create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-133">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-134">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-134">Storage</span></span>

* <span data-ttu-id="e62c1-135">Befehl `storage account revoke-delegation-keys` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-135">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="e62c1-136">13. August 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-136">August 13, 2019</span></span>

<span data-ttu-id="e62c1-137">Version 2.0.71</span><span class="sxs-lookup"><span data-stu-id="e62c1-137">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-138">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-138">AppService</span></span>

* <span data-ttu-id="e62c1-139">Problem behoben, aufgrund dessen bei Befehlen vom Typ `webapp webjob continuous` für Slots Fehler auftraten</span><span class="sxs-lookup"><span data-stu-id="e62c1-139">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="e62c1-140">BotService</span><span class="sxs-lookup"><span data-stu-id="e62c1-140">BotService</span></span>

* <span data-ttu-id="e62c1-141">[BREAKING CHANGE] Unterstützung für die Erstellung von Bots der Version 3 entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-141">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="e62c1-142">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="e62c1-142">CognitiveServices</span></span>

* <span data-ttu-id="e62c1-143">Befehle vom Typ `cognitiveservices account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-143">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e62c1-144">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e62c1-144">Cosmos DB</span></span>

* <span data-ttu-id="e62c1-145">Beim Aktualisieren mehrerer Schreibstandorte wurde eine Warnung entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-145">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="e62c1-146">CRUD-Befehle für CosmosDB SQL-, MongoDB-, Cassandra-, Gremlin- und Tabellenressourcen sowie den Ressourcendurchsatz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-146">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e62c1-147">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e62c1-147">HDInsight</span></span>

<span data-ttu-id="e62c1-148">Dieses Release enthält zahlreiche wichtige Änderungen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-148">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="e62c1-149">[BREAKING CHANGE] Parameter für `hdinsight create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-149">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="e62c1-150">`--storage-default-container` in `--storage-container` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-150">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="e62c1-151">`--storage-default-filesystem` in `--storage-filesystem` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-151">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="e62c1-152">[BREAKING CHANGE] Das Argument `--name` von `application create` wurde so geändert, dass es den Anwendungsnamen anstelle des Clusternamens darstellt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-152">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="e62c1-153">Argument `--cluster-name` zu `application create` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="e62c1-153">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="e62c1-154">[BREAKING CHANGE] Parameter für `application create` umbenannt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-154">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="e62c1-155">`--application-type` in `--type` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-155">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="e62c1-156">`--marketplace-identifier` in `--marketplace-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-156">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="e62c1-157">`--https-endpoint-access-mode` in `--access-mode` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-157">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="e62c1-158">`--https-endpoint-destination-port` in `--destination-port` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-158">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="e62c1-159">[BREAKING CHANGE] Parameter für `application create` entfernt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-159">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="e62c1-160">[WICHTIGE ÄNDERUNG] `--target-instance-count` für `hdinsight resize` in `--workernode-count` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-160">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="e62c1-161">[BREAKING CHANGE] Alle Befehle in der Gruppe `hdinsight script-action` wurden so geändert, dass sie den Parameter `--name` als Namen der Skriptaktion verwenden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-161">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="e62c1-162">Argument `--cluster-name` zu allen Befehlen vom Typ `hdinsight script-action` hinzugefügt, um die alte Funktion `--name` zu ersetzen</span><span class="sxs-lookup"><span data-stu-id="e62c1-162">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="e62c1-163">[BREAKING CHANGE] `--script-execution-id` für alle Befehle vom Typ `hdinsight script-action` in `--execution-id` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-163">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="e62c1-164">[BREAKING CHANGE] `hdinsight script-action show` in `hdinsight script-action show-execution-details` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-164">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="e62c1-165">[WICHTIGE ÄNDERUNG] Parameter in `hdinsight script-action execute --roles` geändert, sodass sie durch Leerzeichen anstelle von Kommas getrennt sind</span><span class="sxs-lookup"><span data-stu-id="e62c1-165">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="e62c1-166">[BREAKING CHANGE] Parameter `--persisted` für `hdinsight script-action list` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-166">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="e62c1-167">Der Parameter `hdinsight create --cluster-configurations` wurde so geändert, dass er einen Pfad zu einer lokalen JSON-Datei oder JSON-Zeichenfolge akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-167">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="e62c1-168">Befehl `hdinsight script-action list-execution-history` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-168">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="e62c1-169">`hdinsight monitor enable --workspace` geändert, um die ID oder den Namen eines Log Analytics-Arbeitsbereichs zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-169">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="e62c1-170">Argument `hdinsight monitor enable --primary-key` hinzugefügt. Dieses Argument wird benötigt, wenn eine Arbeitsbereichs-ID als Parameter angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="e62c1-170">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="e62c1-171">Weitere Beispiele und aktualisierte Beschreibungen für Hilfemeldungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-171">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-172">Interactive</span><span class="sxs-lookup"><span data-stu-id="e62c1-172">Interactive</span></span>

* <span data-ttu-id="e62c1-173">Ladefehler behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-173">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="e62c1-174">kubernetes</span><span class="sxs-lookup"><span data-stu-id="e62c1-174">Kubernetes</span></span>

* <span data-ttu-id="e62c1-175">Änderung, um `https` zu verwenden, wenn der Dashboardcontainerport `https` verwendet</span><span class="sxs-lookup"><span data-stu-id="e62c1-175">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-176">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-176">Network</span></span>

* <span data-ttu-id="e62c1-177">Argument `--yes` hinzugefügt zu `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="e62c1-177">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="e62c1-178">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-178">Profile</span></span>

* <span data-ttu-id="e62c1-179">Argument `--resource-type` zu `account get-access-token` zum Abrufen von Ressourcenzugriffstoken hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-179">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="e62c1-180">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e62c1-180">ServiceFabric</span></span>

* <span data-ttu-id="e62c1-181">Alle unterstützten Betriebssystemversionen für „sf cluster create“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-181">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="e62c1-182">Fehler beim Überprüfen des primären Zertifikats behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-182">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-183">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-183">Storage</span></span>

* <span data-ttu-id="e62c1-184">Befehl `storage copy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-184">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="e62c1-185">30. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-185">July 30, 2019</span></span>

<span data-ttu-id="e62c1-186">Version 2.0.70</span><span class="sxs-lookup"><span data-stu-id="e62c1-186">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-187">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-187">ACR</span></span>

* <span data-ttu-id="e62c1-188">Problem #9952 behoben (Regression im Befehl `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="e62c1-188">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="e62c1-189">Standardname des Generatorimages in `acr pack build` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-189">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-190">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-190">Appservice</span></span>

* <span data-ttu-id="e62c1-191">`webapp config ssl` geändert, um eine Meldung anzuzeigen, wenn eine Ressource nicht gefunden wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-191">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="e62c1-192">Problem behoben, aufgrund dessen `functionapp create` den Speicherkontotypen `Standard_RAGRS` nicht akzeptiert hat</span><span class="sxs-lookup"><span data-stu-id="e62c1-192">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="e62c1-193">Problem behoben, aufgrund dessen für `webapp up` ein Fehler auftrat, wenn für die Ausführung ältere Python-Versionen verwendet wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-193">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-194">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-194">Network</span></span>

* <span data-ttu-id="e62c1-195">Ungültiger Parameter `--ids` aus `network nic ip-config add` entfernt (Fehlerbehebungen #9861)</span><span class="sxs-lookup"><span data-stu-id="e62c1-195">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="e62c1-196">Fehlerbehebungen #9604.</span><span class="sxs-lookup"><span data-stu-id="e62c1-196">Fixes #9604.</span></span> <span data-ttu-id="e62c1-197">Parameter `--root-certs` zu `network application-gateway http-settings [create|update]` hinzugefügt, um vom Benutzer zugewiesene vertrauenswürdige Stammzertifikate zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-197">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="e62c1-198">Argument `--subscription` für `network dns record-set ns create` korrigiert (#9965)</span><span class="sxs-lookup"><span data-stu-id="e62c1-198">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="e62c1-199">RBAC</span><span class="sxs-lookup"><span data-stu-id="e62c1-199">RBAC</span></span>

* <span data-ttu-id="e62c1-200">Befehl `user update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-200">Added `user update` command</span></span>
* <span data-ttu-id="e62c1-201">[VERALTET] `--upn-or-object-id` in benutzerbezogenen Befehlen als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-201">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="e62c1-202">Verwenden Sie das Ersatzargument `--id`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-202">Use replacement argument `--id`</span></span>
* <span data-ttu-id="e62c1-203">Argument `--id` zu benutzerbezogenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-203">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-204">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-204">SQL</span></span>

* <span data-ttu-id="e62c1-205">Verwaltungsbefehle für Schlüssel verwalteter Instanzen und TDE-Schutzvorrichtung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-205">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-206">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-206">Storage</span></span>

* <span data-ttu-id="e62c1-207">Befehl `storage remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-207">Added `storage remove` command</span></span>
* <span data-ttu-id="e62c1-208">Problem mit `storage blob update` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-208">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-209">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-209">VM</span></span>

* <span data-ttu-id="e62c1-210">`list-skus` wurde geändert, um eine neuere API-Version für die Ausgabe von Zonendetails zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-210">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="e62c1-211">Standardwert `--single-placement-group` für `vmss create` in `false` geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-211">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="e62c1-212">Möglichkeit zum Auswählen von ZRS-Speicher-SKUs für `[snapshot|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-212">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="e62c1-213">Neue Befehlsgruppe `vm host` zur Unterstützung dedizierter Hosts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-213">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="e62c1-214">Parameter `--host` und `--host-group` für `vm create` hinzugefügt, um den dedizierten VM-Host festzulegen</span><span class="sxs-lookup"><span data-stu-id="e62c1-214">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="e62c1-215">16. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-215">July 16, 2019</span></span>

<span data-ttu-id="e62c1-216">Version 2.0.69</span><span class="sxs-lookup"><span data-stu-id="e62c1-216">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-217">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-217">Appservice</span></span>

* <span data-ttu-id="e62c1-218">`webapp identity`-Befehle geändert, um eine korrekte Fehlermeldung zurückzugeben, wenn „ResourceGroupName“ oder der App-Name ungültig sind</span><span class="sxs-lookup"><span data-stu-id="e62c1-218">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="e62c1-219">`webapp list` korrigiert, sodass der korrekte Wert für „numberOfSites“ zurückgegeben wird, wenn „ResourceGroup“ nicht angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-219">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="e62c1-220">Nebeneffekte von `appservice plan create` und `webapp create` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-220">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-221">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-221">Core</span></span>

* <span data-ttu-id="e62c1-222">Problem behoben, aufgrund dessen `--subscription` angezeigt wurde, obwohl nicht anwendbar</span><span class="sxs-lookup"><span data-stu-id="e62c1-222">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-223">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-223">Batch</span></span>

* <span data-ttu-id="e62c1-224">[BREAKING CHANGE] `batch pool node-agent-skus list` durch `batch pool supported-images list` ersetzt</span><span class="sxs-lookup"><span data-stu-id="e62c1-224">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="e62c1-225">Unterstützung für Sicherheitsregeln hinzugefügt, die den Netzwerkzugriff auf einen Pool basierend auf dem Quellport des Datenverkehrs blockieren, wenn die Option `--json-file` von `batch pool create network` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-225">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="e62c1-226">Unterstützung für die Ausführung der Aufgabe im Arbeitsverzeichnis des Containers oder der Batch-Aufgabe hinzugefügt, wenn die Option `--json-file` von `batch task create` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-226">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="e62c1-227">Fehler in Option `--application-package-references` von `batch pool create` behoben, aufgrund dessen nur Standardeinstellungen möglich waren</span><span class="sxs-lookup"><span data-stu-id="e62c1-227">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="e62c1-228">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="e62c1-228">Eventhubs</span></span>

* <span data-ttu-id="e62c1-229">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-229">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="e62c1-230">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-230">RDBMS</span></span>

* <span data-ttu-id="e62c1-231">Optionaler Parameter zum Angeben der Replikat-SKU für den Befehl zum Erstellen von Replikaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-231">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="e62c1-232">Problem mit CI-Testfehler bei der Erstellung von MySQL-Replikaten behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-232">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="e62c1-233">Relay</span><span class="sxs-lookup"><span data-stu-id="e62c1-233">Relay</span></span>

* <span data-ttu-id="e62c1-234">Problem mit Hybridverbindung behoben, wenn die Client-Autorisierung deaktiviert ist [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="e62c1-234">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="e62c1-235">Parameter `--requires-transport-security` zu `relay wcfrelay create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-235">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="e62c1-236">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="e62c1-236">Servicebus</span></span>

* <span data-ttu-id="e62c1-237">Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-237">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-238">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-238">Storage</span></span>

* <span data-ttu-id="e62c1-239">AADDS für Files für Speicherkontoaktualisierung aktiviert</span><span class="sxs-lookup"><span data-stu-id="e62c1-239">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="e62c1-240">Problem `storage blob service-properties update --set` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-240">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="e62c1-241">2\. Juli 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-241">July 2, 2019</span></span>

<span data-ttu-id="e62c1-242">Version 2.0.68</span><span class="sxs-lookup"><span data-stu-id="e62c1-242">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-243">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-243">Core</span></span>

* <span data-ttu-id="e62c1-244">Befehlsmodule sind jetzt in einer einzelnen verteilbaren Python-Komponente zusammengefasst.</span><span class="sxs-lookup"><span data-stu-id="e62c1-244">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="e62c1-245">Die direkte Verwendung zahlreicher Pakete vom Typ `azure-cli-` in PyPI ist daher veraltet.</span><span class="sxs-lookup"><span data-stu-id="e62c1-245">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="e62c1-246">Dadurch sollte sich die Installationsgröße reduzieren. Darüber hinaus sollte es nur Benutzer betreffen, die eine direkte Installation über `pip` ausgeführt haben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-246">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-247">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-247">ACR</span></span>

* <span data-ttu-id="e62c1-248">Unterstützung für Trigger mit Timer zu Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-248">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-249">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-249">Appservice</span></span>

* <span data-ttu-id="e62c1-250">`functionapp create` wurde so geändert, das Application Insights standardmäßig aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="e62c1-250">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="e62c1-251">[BREAKING CHANGE] Veralteter Befehl `functionapp devops-build` entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-251">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="e62c1-252">Verwenden Sie stattdessen den neuen Befehl `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-252">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="e62c1-253">Unterstützung des Funktions-App-Plans für Linux-Verbrauch zu `functionapp deployment config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-253">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e62c1-254">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e62c1-254">Cosmos DB</span></span>

* <span data-ttu-id="e62c1-255">Unterstützung für das Deaktivieren von TTL hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-255">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="e62c1-256">DLS</span><span class="sxs-lookup"><span data-stu-id="e62c1-256">DLS</span></span>

* <span data-ttu-id="e62c1-257">Aktualisierte ADLS-Version (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="e62c1-257">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="e62c1-258">Feedback</span><span class="sxs-lookup"><span data-stu-id="e62c1-258">Feedback</span></span>

* <span data-ttu-id="e62c1-259">Wird ein fehlgeschlagener Erweiterungsbefehl gemeldet, versucht `az feedback` nun, über den Index die Projekt-/Repository-URL der Erweiterung im Browser zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-259">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e62c1-260">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e62c1-260">HDInsight</span></span>

* <span data-ttu-id="e62c1-261">[BREAKING CHANGE] Der Befehlsgruppenname `oms` wurde in `monitor` geändert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-261">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="e62c1-262">[BREAKING CHANGE] `--http-password/-p` als erforderlicher Parameter festgelegt</span><span class="sxs-lookup"><span data-stu-id="e62c1-262">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="e62c1-263">Vervollständigungen für `--cluster-admin-account` und `cluster-users-group-dns` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-263">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="e62c1-264">Parameter `cluster-users-group-dns` so geändert, dass er erforderlich ist, wenn `—esp` vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-264">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="e62c1-265">Timeout für alle vorhandenen automatischen Argumentvervollständigungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-265">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="e62c1-266">Timeout für das Transformieren des Ressourcennamens in eine Ressourcen-ID hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-266">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="e62c1-267">Die automatischen Vervollständigungen wurden so geändert, dass Ressourcen aus einer beliebigen Ressourcengruppe ausgewählt werden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-267">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="e62c1-268">Dabei kann es sich um eine andere Ressourcengruppe als die mit `-g` angegebene Gruppe handeln.</span><span class="sxs-lookup"><span data-stu-id="e62c1-268">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="e62c1-269">Unterstützung für die Parameter `--sub-domain-suffix` und `--disable_gateway_auth` im Befehl `hdinsight application create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-269">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="e62c1-270">Verwaltete Dienste</span><span class="sxs-lookup"><span data-stu-id="e62c1-270">Managed Services</span></span>

* <span data-ttu-id="e62c1-271">Befehlsmodul für verwaltete Dienste als Vorschau eingeführt</span><span class="sxs-lookup"><span data-stu-id="e62c1-271">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="e62c1-272">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-272">Profile</span></span>
* <span data-ttu-id="e62c1-273">Argument `--subscription` für Abmeldebefehl unterdrückt</span><span class="sxs-lookup"><span data-stu-id="e62c1-273">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="e62c1-274">RBAC</span><span class="sxs-lookup"><span data-stu-id="e62c1-274">RBAC</span></span>

* <span data-ttu-id="e62c1-275">[BREAKING CHANGE] Argument `--password` für `create-for-rbac` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-275">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="e62c1-276">Parameter `--assignee-principal-type` zum Befehl `create` hinzugefügt, um zeitweilige Fehler zu vermeiden, die durch die Replikationswartezeit des AAD-Graph-Servers verursacht werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-276">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="e62c1-277">Absturz in `ad signed-in-user` beim Auflisten von in Besitz befindlichen Objekten behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-277">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="e62c1-278">Problem behoben, aufgrund dessen `ad sp` nicht die richtige Anwendung über einen Dienstprinzipal fand</span><span class="sxs-lookup"><span data-stu-id="e62c1-278">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="e62c1-279">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-279">RDBMS</span></span>

* <span data-ttu-id="e62c1-280">Unterstützung für die Replikation für MariaDB hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-280">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-281">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-281">SQL</span></span>

* <span data-ttu-id="e62c1-282">Zulässige Werte für `sql db create --sample-name` dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-282">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-283">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-283">Storage</span></span>

* <span data-ttu-id="e62c1-284">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage blob generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-284">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="e62c1-285">Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage container generate-sas` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-285">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="e62c1-286">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-286">VM</span></span>

* <span data-ttu-id="e62c1-287">Fehler behoben, aufgrund dessen `vmss create` bei der Ausführung mit `--no-wait` eine Fehlermeldung zurückgab</span><span class="sxs-lookup"><span data-stu-id="e62c1-287">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="e62c1-288">Die clientseitige Validierung für `vmss create --single-placement-group` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-288">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="e62c1-289">Es tritt kein Fehler auf, wenn `--single-placement-group` auf `true` und für `--instance-count` ein größerer Wert als 100 festgelegt wird oder wenn Verfügbarkeitszonen angegeben werden. Diese Validierung wird jedoch dem Computedienst überlassen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-289">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="e62c1-290">Problem behoben, aufgrund dessen bei der Verwendung von `--latest` für `[vm|vmss] extension image list` ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="e62c1-290">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="e62c1-291">18. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-291">June 18, 2019</span></span>

<span data-ttu-id="e62c1-292">Version 2.0.67</span><span class="sxs-lookup"><span data-stu-id="e62c1-292">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-293">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-293">Core</span></span>

<span data-ttu-id="e62c1-294">In diesem Release wird das neue [Preview]-Tag eingeführt, um Kunden gegenüber deutlich zu machen, dass sich eine Befehlsgruppe, ein Befehl oder ein Argument in der Vorschauphase befindet.</span><span class="sxs-lookup"><span data-stu-id="e62c1-294">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="e62c1-295">Diese Information war zuvor im Hilfetext oder implizit durch die Versionsnummer des Befehlsmoduls angegeben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-295">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="e62c1-296">Die Befehlszeilenschnittstelle wird künftig Versionsnummern für einzelne Pakete entfernen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-296">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="e62c1-297">Wenn sich ein Befehl in der Vorschauphase befindet, gilt dies auch für alle seine Argumente.</span><span class="sxs-lookup"><span data-stu-id="e62c1-297">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="e62c1-298">Wenn eine Befehlsgruppe als Vorschau gekennzeichnet ist, befinden sich auch alle Befehle und Argumente in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="e62c1-298">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="e62c1-299">Infolge dieser Änderung befinden sich in diesem Release verschiedene Befehlsgruppen anscheinend „plötzlich“ in der Vorschauphase.</span><span class="sxs-lookup"><span data-stu-id="e62c1-299">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="e62c1-300">Tatsächlich ist es jedoch so, dass sich die meisten Pakete in der Vorschauphase befanden, in diesem Release jedoch als allgemein verfügbar gelten.</span><span class="sxs-lookup"><span data-stu-id="e62c1-300">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-301">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-301">ACR</span></span>
* <span data-ttu-id="e62c1-302">Befehl „acr check-health“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-302">Added 'acr check-health' command</span></span>
* <span data-ttu-id="e62c1-303">Verbesserte Fehlerbehandlung für AAD-Token und für das Abrufen externer Befehle</span><span class="sxs-lookup"><span data-stu-id="e62c1-303">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-304">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-304">ACS</span></span>
* <span data-ttu-id="e62c1-305">Veraltete ACS-Befehle werden jetzt in der Hilfeansicht ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="e62c1-305">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="e62c1-306">AMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-306">AMS</span></span>
* <span data-ttu-id="e62c1-307">[BREAKING CHANGE] Änderung, damit ISO 8601-Zeitzeichenfolgen für „archive-window-length“ und „key-frame-interval-duration“ zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-307">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-308">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-308">AppService</span></span>
* <span data-ttu-id="e62c1-309">Standortbasiertes Routing für `webapp deleted list` und `webapp deleted restore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-309">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="e62c1-310">Problem behoben, aufgrund dessen in Azure Cloud Shell nicht auf die von einer Web-App protokollierte Ziel-URL („Sie können die App starten unter...“) geklickt werden konnte</span><span class="sxs-lookup"><span data-stu-id="e62c1-310">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="e62c1-311">Problem behoben, aufgrund dessen beim Erstellen von Apps bei einigen SKUs ein AlwaysOn-Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="e62c1-311">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="e62c1-312">Vorabüberprüfung zu `[appservice|webapp] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-312">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="e62c1-313">`[webapp|functionapp] traffic-routing` korrigiert, damit der richtige actionHostName-Wert verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-313">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="e62c1-314">Slotunterstützung zu `functionapp`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-314">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-315">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-315">Batch</span></span>
* <span data-ttu-id="e62c1-316">AAD-Authentifizierungsregression korrigiert, die von übermäßiger Berichterstellung für Authentifizierung mit gemeinsam verwendetem Schlüssel verursacht wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-316">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="e62c1-317">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e62c1-317">BatchAI</span></span>
* <span data-ttu-id="e62c1-318">BatchAI-Befehle sind jetzt veraltet und ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="e62c1-318">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="e62c1-319">BotService</span><span class="sxs-lookup"><span data-stu-id="e62c1-319">BotService</span></span>
* <span data-ttu-id="e62c1-320">Für Befehle, die Version 3 des SDK unterstützen, wurden die Warnmeldungen „Support eingestellt“/„Wartungsmodus“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-320">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e62c1-321">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e62c1-321">CosmosDB</span></span>
* <span data-ttu-id="e62c1-322">[VERALTET] Der Befehl `cosmosdb list-keys` wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="e62c1-322">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="e62c1-323">Befehl `cosmosdb keys list` hinzugefügt, er ersetzt `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-323">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="e62c1-324">`cosmsodb create/update`: Neues Format für „--location“ hinzugefügt, um das Festlegen der Eigenschaft „isZoneRedundant“ zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-324">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="e62c1-325">Das alte Format wurde als veraltet gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="e62c1-325">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e62c1-326">EventGrid</span><span class="sxs-lookup"><span data-stu-id="e62c1-326">EventGrid</span></span>
* <span data-ttu-id="e62c1-327">`eventgrid domain`-Befehle für CRUD-Vorgänge für Domänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-327">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="e62c1-328">`eventgrid domain topic`-Befehle für CRUD-Vorgänge für Domänenthemen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-328">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="e62c1-329">Argument `--odata-query` zu `eventgrid [topic|event-subscription] list` zum Filtern der Ergebnisse mithilfe von OData-Syntax hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-329">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="e62c1-330">`event-subscription create/update`: „servicebusqueue“ als neue Werte für den Parameter `--endpoint-type` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-330">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="e62c1-331">[BREAKING CHANGE] Unterstützung für `--included-event-types All` mit `eventgrid event-subscription [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-331">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e62c1-332">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e62c1-332">HDInsight</span></span>
* <span data-ttu-id="e62c1-333">Unterstützung für den Parameter `--ssh-public-key` im Befehl vom Typ `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-333">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="e62c1-334">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-334">IoT</span></span>
* <span data-ttu-id="e62c1-335">Unterstützung für das erneute Generieren von Autorisierungsrichtlinienschlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-335">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="e62c1-336">SDK und Unterstützung für den Bereitstellungsdienst des DigitalTwin-Repositorys hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-336">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-337">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-337">Network</span></span>
* <span data-ttu-id="e62c1-338">Zonenunterstützung für NAT Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-338">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="e62c1-339">Befehl `network list-service-tags` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-339">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="e62c1-340">Problem mit `dns zone import` behoben, aufgrund dessen Benutzer keine A-Platzhaltereinträge importieren konnten</span><span class="sxs-lookup"><span data-stu-id="e62c1-340">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="e62c1-341">Problem mit `watcher flow-log configure` behoben, aufgrund dessen die Flowprotokollierung in bestimmten Regionen nicht aktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="e62c1-341">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-342">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-342">Resource</span></span>
* <span data-ttu-id="e62c1-343">Befehl `az rest` zum Ausführen von REST-Aufrufen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-343">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="e62c1-344">Fehler behoben, der bei Verwendung von `policy assignment list` mit `--scope` auf Ressourcengruppen- oder Abonnementebene auftrat</span><span class="sxs-lookup"><span data-stu-id="e62c1-344">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="e62c1-345">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="e62c1-345">ServiceBus</span></span>
* <span data-ttu-id="e62c1-346">Problem mit `servicebus topic create --max-size` behoben [#9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="e62c1-346">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-347">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-347">SQL</span></span>
* <span data-ttu-id="e62c1-348">`--location` wurde geändert und ist nun für `sql [server|mi] create` optional. Ohne Angabe wird der Ressourcengruppenstandort verwendet.</span><span class="sxs-lookup"><span data-stu-id="e62c1-348">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="e62c1-349">Der Fehler, dass das Objekt „NoneType“ nicht wiederholbar ist, wurde für `sql db list-editions --available` behoben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-349">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="e62c1-350">SQLVm</span><span class="sxs-lookup"><span data-stu-id="e62c1-350">SQLVm</span></span>
* <span data-ttu-id="e62c1-351">[WICHTIGE ÄNDERUNG] `sql vm create` wurde geändert und erfordert nun den Parameter `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-351">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="e62c1-352">Änderung, um beim Erstellen oder Aktualisieren einer SQL-VM das Festlegen der SQL-Image-SKU zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-352">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-353">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-353">Storage</span></span>
* <span data-ttu-id="e62c1-354">Problem mit fehlendem Kontoschlüssel für `storage container generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-354">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="e62c1-355">Problem mit `storage blob sync` unter Linux behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-355">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-356">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-356">VM</span></span>
* <span data-ttu-id="e62c1-357">[VORSCHAU] Befehle vom Typ `vm image template` zum Erstellen von VM-Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-357">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="e62c1-358">4\. Juni 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-358">June 4, 2019</span></span>

<span data-ttu-id="e62c1-359">Version 2.0.66</span><span class="sxs-lookup"><span data-stu-id="e62c1-359">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-360">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-360">Core</span></span>
* <span data-ttu-id="e62c1-361">Fehler behoben, aufgrund dessen bei Befehlen ein Fehler auftrat, wenn `--output yaml` mit `--query` verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-361">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-362">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-362">ACR</span></span>
* <span data-ttu-id="e62c1-363">Befehlsgruppe „acr pack“ zum Erstellen von Aufgaben zur Schnellerstellung mit Buildpacks hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-363">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-364">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-364">ACS</span></span>
* <span data-ttu-id="e62c1-365">Zulassen der Aktivierung/Deaktivierung des AKS-Add-Ons für das Kube-Dashboard</span><span class="sxs-lookup"><span data-stu-id="e62c1-365">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="e62c1-366">Ausgeben einer benutzerfreundlichen Nachricht, wenn das Abonnement nicht in der Whitelist zur Verwendung von Azure Red Hat OpenShift enthalten ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-366">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-367">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-367">Batch</span></span>
* <span data-ttu-id="e62c1-368">Bessere Fehlerbehandlung, wenn der Benutzer nicht bei einem Konto angemeldet ist \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="e62c1-368">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="e62c1-369">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-369">IoT</span></span>
* <span data-ttu-id="e62c1-370">Unterstützung für manuelles Failover hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-370">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-371">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-371">Network</span></span>
* <span data-ttu-id="e62c1-372">Befehle vom Typ `network application-gateway waf-policy` hinzugefügt, um benutzerdefinierte WAF-Regeln zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-372">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="e62c1-373">Argumente `--waf-policy` und `--max-capacity` zu `network application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-373">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="e62c1-374">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-374">Resource</span></span>
* <span data-ttu-id="e62c1-375">Verbesserte Fehlermeldungen aus `deployment create`, wenn TTY nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-375">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-376">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-376">Role</span></span>
* <span data-ttu-id="e62c1-377">Hilfetext aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-377">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="e62c1-378">Compute</span><span class="sxs-lookup"><span data-stu-id="e62c1-378">Compute</span></span>
* <span data-ttu-id="e62c1-379">Unterstützung zu `vm create` für virtuelle Computer aus einem verwalteten Image mit Datenträger-LUNs hinzugefügt, die nicht bei 0 beginnen oder die Nummern überspringen</span><span class="sxs-lookup"><span data-stu-id="e62c1-379">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="e62c1-380">21. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-380">May 21, 2019</span></span>

<span data-ttu-id="e62c1-381">Version 2.0.65</span><span class="sxs-lookup"><span data-stu-id="e62c1-381">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-382">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-382">Core</span></span>
* <span data-ttu-id="e62c1-383">Besseres Feedback für Authentifizierungsfehler hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-383">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="e62c1-384">Problem behoben, aufgrund dessen die CLI Erweiterungen lädt, die nicht mit der Core-Version kompatibel waren</span><span class="sxs-lookup"><span data-stu-id="e62c1-384">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="e62c1-385">Problem beim Starten behoben, wenn `clouds.config` beschädigt ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-385">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-386">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-386">ACR</span></span>
* <span data-ttu-id="e62c1-387">Unterstützung für verwaltete Identitäten zu Aufgaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-387">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-388">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-388">ACS</span></span>
* <span data-ttu-id="e62c1-389">`openshift create`-Befehl bei der Verwendung mit dem AAD-Kundenclient korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-389">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-390">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-390">AppService</span></span>
* <span data-ttu-id="e62c1-391">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet – wird in der nächsten Version entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-391">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="e62c1-392">`functionapp devops-pipeline` geändert, um das Buildprotokoll von Azure DevOps im ausführlichen Modus abzurufen</span><span class="sxs-lookup"><span data-stu-id="e62c1-392">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="e62c1-393">[BREAKING CHANGE] Flag `--use_local_settings` aus dem Befehl `functionapp devops-pipeline` entfernt – kein Vorgang wurde ausgeführt</span><span class="sxs-lookup"><span data-stu-id="e62c1-393">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="e62c1-394">`webapp up` geändert, sodass die JSON-Ausgabe zurückgegeben wird, wenn `--logs` nicht verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-394">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="e62c1-395">Unterstützung hinzugefügt zum Schreiben von Standardressourcen in die lokale Konfiguration für `webapp up`</span><span class="sxs-lookup"><span data-stu-id="e62c1-395">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="e62c1-396">Unterstützung zu `webapp up` hinzugefügt für die erneute Bereitstellung einer App ohne Verwendung des `--location`-Arguments</span><span class="sxs-lookup"><span data-stu-id="e62c1-396">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="e62c1-397">Problem behoben, bei dem für die ASP-Erstellung der Linux-SKU „Free“ der SKU-Wert „Free“ nicht funktioniert hat</span><span class="sxs-lookup"><span data-stu-id="e62c1-397">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="e62c1-398">BotService</span><span class="sxs-lookup"><span data-stu-id="e62c1-398">BotService</span></span>
* <span data-ttu-id="e62c1-399">Geändert, sodass Groß-/Kleinschreibung für `--lang`-Parameter für Befehle zulässig ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-399">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="e62c1-400">Beschreibung für das Befehlsmodul aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-400">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="e62c1-401">Nutzung</span><span class="sxs-lookup"><span data-stu-id="e62c1-401">Consumption</span></span>
* <span data-ttu-id="e62c1-402">Fehlende erforderliche Parameter bei der Ausführung von `consumption usage list --billing-period-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-402">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="e62c1-403">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-403">IoT</span></span>
* <span data-ttu-id="e62c1-404">Unterstützung für das Auflisten aller Schlüssel hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-404">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-405">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-405">Network</span></span>
* [BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="e62c1-407">`--nat-gateway`-Argument zu `network vnet subnet [create|update]` für das Anfügen an ein NAT-Gateway hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-407">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="e62c1-408">Problem mit `dns zone import` behoben, aufgrund dessen Eintragsnamen keinem Datensatztyp entsprochen haben</span><span class="sxs-lookup"><span data-stu-id="e62c1-408">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="e62c1-409">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-409">RDBMS</span></span>
* <span data-ttu-id="e62c1-410">Postgres- und MySLQ-Unterstützung für die Georeplikation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-410">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="e62c1-411">RBAC</span><span class="sxs-lookup"><span data-stu-id="e62c1-411">RBAC</span></span>
* <span data-ttu-id="e62c1-412">Unterstützung für den Verwaltungsgruppenumfang zu `role assignment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-412">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-413">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-413">Storage</span></span>
* <span data-ttu-id="e62c1-414">`storage blob sync`: Synchronisierungsbefehl für Speicherblob hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-414">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="e62c1-415">Compute</span><span class="sxs-lookup"><span data-stu-id="e62c1-415">Compute</span></span>
* <span data-ttu-id="e62c1-416">`--computer-name` zu `vm create` zum Festlegen des Computernamens eines virtuellen Computers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-416">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="e62c1-417">`--ssh-key-value` umbenannt in `--ssh-key-values` für `[vm|vmss] create`: Jetzt können mehrere öffentliche SSH-Schlüsselwerte oder -pfade akzeptiert werden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-417">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="e62c1-418">__Hinweis__: Dies ist **kein** Breaking Change: `--ssh-key-value` wird korrekt analysiert, da nur eine Übereinstimmung mit `--ssh-key-values` besteht.</span><span class="sxs-lookup"><span data-stu-id="e62c1-418">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="e62c1-419">`--type`-Argument von `ppg create` in optionales Argument geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-419">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="e62c1-420">6\. Mai 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-420">May 6, 2019</span></span>

<span data-ttu-id="e62c1-421">Version 2.0.64</span><span class="sxs-lookup"><span data-stu-id="e62c1-421">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-422">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-422">ACS</span></span>
* <span data-ttu-id="e62c1-423">[BREAKING CHANGE] Flag `--fqdn` aus den `openshift`-Befehlen entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-423">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="e62c1-424">Geändert, sodass die allgemein verfügbare Azure Red Hat Openshift-API-Version verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-424">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="e62c1-425">Flag `customer-admin-group-id` wurde zu `openshift create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-425">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="e62c1-426">[ALLGEMEIN VERFÜGBAR] `(PREVIEW)` aus der `aks create`-Option `--network-policy` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-426">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-427">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-427">Appservice</span></span>
* <span data-ttu-id="e62c1-428">[VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="e62c1-428">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="e62c1-429">Umbenannt in `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="e62c1-429">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="e62c1-430">Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte</span><span class="sxs-lookup"><span data-stu-id="e62c1-430">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="e62c1-431">Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-431">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="e62c1-432">Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-432">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="e62c1-433">Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-433">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="e62c1-434">Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-434">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="e62c1-435">`webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln</span><span class="sxs-lookup"><span data-stu-id="e62c1-435">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="e62c1-436">Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-436">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="e62c1-437">Befehl `create-remote-connection` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-437">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-438">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-438">Batch</span></span>
* <span data-ttu-id="e62c1-439">Fehler im Validierungssteuerelement für `--application-package-references`-Optionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-439">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="e62c1-440">Botservice</span><span class="sxs-lookup"><span data-stu-id="e62c1-440">Botservice</span></span>
* <span data-ttu-id="e62c1-441">[BREAKING CHANGE] `bot create -v v4 -k webapp` geändert, sodass standardmäßig eine leerer Web-App-Bot erstellt wird (d. h. kein Bot wird in App Service bereitgestellt)</span><span class="sxs-lookup"><span data-stu-id="e62c1-441">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="e62c1-442">`--echo`-Flag zu `bot create` hinzugefügt, sodass das alte Verhalten mit `-v v4` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-442">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="e62c1-443">[BREAKING CHANGE] Standardwert von `--version` in `v4` geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-443">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="e62c1-444">__HINWEIS:__ `bot prepare-publish` verwendet weiterhin den alten Standard.</span><span class="sxs-lookup"><span data-stu-id="e62c1-444">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="e62c1-445">[BREAKING CHANGE] `--lang` geändert, sodass der Standard nicht mehr `Csharp` ist.</span><span class="sxs-lookup"><span data-stu-id="e62c1-445">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="e62c1-446">Wenn der Befehl `--lang` erfordert und dies nicht angegeben ist, wird der Befehl nun mit Fehler beendet.</span><span class="sxs-lookup"><span data-stu-id="e62c1-446">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="e62c1-447">[BREAKING CHANGE] `--appid`- und `--password`-Argumente für `bot create` in erforderlich geändert, sie können jetzt über `ad app create` erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-447">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="e62c1-448">`--appid`- und `--password`-Validierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-448">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="e62c1-449">[BREAKING CHANGE] `bot create -v v4` geändert, sodass kein Speicherkonto bzw. keine Application Insights-Instanz erstellt oder verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-449">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="e62c1-450">[BREAKING CHANGE] `bot create -v v3` geändert, sodass eine Region erforderlich ist, in der Application Insights verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-450">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="e62c1-451">[BREAKING CHANGE] `bot update` geändert, sodass es sich jetzt nur auf spezifische Eigenschaften eines Bots auswirkt</span><span class="sxs-lookup"><span data-stu-id="e62c1-451">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="e62c1-452">[BREAKING CHANGE] `--lang`-Flags geändert, sodass `Javascript` anstelle von `Node` akzeptiert wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-452">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="e62c1-453">[BREAKING CHANGE] `Node` als zulässiger `--lang`-Wert entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-453">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="e62c1-454">[BREAKING CHANGE] `bot create -v v4 -k webapp` geändert, sodass `SCM_DO_BUILD_DURING_DEPLOYMENT` nicht mehr auf TRUE festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="e62c1-454">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="e62c1-455">Alle Bereitstellungen über Kudu fungieren ihrem Standardverhalten entsprechend.</span><span class="sxs-lookup"><span data-stu-id="e62c1-455">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="e62c1-456">`bot download` für Bots ohne `.bot`-Dateien geändert, sodass die sprachspezifische Konfigurationsdatei mit Werten aus den Anwendungseinstellungen für den Bot erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="e62c1-456">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="e62c1-457">Unterstützung für `Typescript` zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-457">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="e62c1-458">Warnmeldung zu `bot prepare-deploy` für `Javascript`- und `Typescript`-Bots hinzugefügt, wenn `package.json` in `--code-dir` nicht enthalten ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-458">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="e62c1-459">`bot prepare-deploy` geändert, sodass bei Erfolg `true` zurückgegeben wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-459">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="e62c1-460">Ausführliche Protokollierung zu `bot prepare-deploy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-460">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="e62c1-461">Mehr verfügbare Application Insights-Regionen zu `az bot create -v v3` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-461">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="e62c1-462">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-462">Configure</span></span>
* <span data-ttu-id="e62c1-463">Unterstützung für die ordnerbasierte Argument-Standardwertkonfigurationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-463">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="e62c1-464">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="e62c1-464">Eventhubs</span></span>
* <span data-ttu-id="e62c1-465">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-465">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="e62c1-466">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-466">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-467">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-467">Network</span></span>
* <span data-ttu-id="e62c1-468">[BREAKING CHANGE] `--cache`-Argument mit `--defer` für `vnet [create|update]` ersetzt</span><span class="sxs-lookup"><span data-stu-id="e62c1-468">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="e62c1-469">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="e62c1-469">Policy Insights</span></span>
* <span data-ttu-id="e62c1-470">Unterstützung für `--expand PolicyEvaluationDetails` hinzugefügt, sodass Richtlinienauswertungsdetails von der Ressource abgefragt werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-470">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-471">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-471">Role</span></span>
* <span data-ttu-id="e62c1-472">[VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-472">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="e62c1-473">Service Bus</span><span class="sxs-lookup"><span data-stu-id="e62c1-473">Service Bus</span></span>
* <span data-ttu-id="e62c1-474">Befehle vom Typ `namespace network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-474">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="e62c1-475">`--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-475">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="e62c1-476">`topic [create|update]` korrigiert, sodass `--max-size`-Unterstützung für 10-, 20-, 40- und 80-GB-Werte mit Premium-SKU zulässig ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-476">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-477">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-477">SQL</span></span>
* <span data-ttu-id="e62c1-478">Befehle vom Typ `sql virtual-cluster [list|show|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-478">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-479">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-479">VM</span></span>
* <span data-ttu-id="e62c1-480">`--protect-from-scale-in` und `--protect-from-scale-set-actions` zu `vmss update` hinzugefügt, sodass Aktualisierungen der Schutzrichtlinie von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="e62c1-480">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="e62c1-481">`--instance-id` zu `vmss update` hinzugefügt, sodass allgemeine Aktualisierungen von VMSS-VM-Instanzen aktiviert sind</span><span class="sxs-lookup"><span data-stu-id="e62c1-481">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="e62c1-482">`--instance-id` zu `vmss wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-482">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="e62c1-483">Neue `ppg`-Befehlsgruppe für die Verwaltung von Näherungsplatzierungsgruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-483">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="e62c1-484">`--ppg` zu `[vm|vmss] create` und `vm availability-set create` für die Verwaltung von PPGs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-484">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="e62c1-485">Parameter `--hyper-v-generation` zu `image create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-485">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="e62c1-486">23. April 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-486">April 23, 2019</span></span>

<span data-ttu-id="e62c1-487">Version 2.0.63</span><span class="sxs-lookup"><span data-stu-id="e62c1-487">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-488">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-488">ACS</span></span>
* <span data-ttu-id="e62c1-489">`aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-489">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="e62c1-490">`(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-490">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="e62c1-491">AMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-491">AMS</span></span>
* <span data-ttu-id="e62c1-492">Fehler bei der Objekt- und Kontofilteraktualisierung behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-492">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-493">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-493">AppService</span></span>
* <span data-ttu-id="e62c1-494">Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-494">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="e62c1-495">Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-495">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="e62c1-496">`--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-496">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="e62c1-497">`--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-497">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="e62c1-498">Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-498">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="e62c1-499">Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-499">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="e62c1-500">`webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen</span><span class="sxs-lookup"><span data-stu-id="e62c1-500">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="e62c1-501">`-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten</span><span class="sxs-lookup"><span data-stu-id="e62c1-501">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="e62c1-502">`webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln</span><span class="sxs-lookup"><span data-stu-id="e62c1-502">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="e62c1-503">Bereitstellungs-Manager</span><span class="sxs-lookup"><span data-stu-id="e62c1-503">Deployment Manager</span></span>
* <span data-ttu-id="e62c1-504">[VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-504">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="e62c1-505">Labor</span><span class="sxs-lookup"><span data-stu-id="e62c1-505">Lab</span></span>
* <span data-ttu-id="e62c1-506">Fehler behoben, der zu einer vorzeitigen Beendigung führen würde</span><span class="sxs-lookup"><span data-stu-id="e62c1-506">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-507">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-507">Network</span></span>
* <span data-ttu-id="e62c1-508">Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-508">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-509">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-509">Resource</span></span>
* <span data-ttu-id="e62c1-510">[VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-510">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="e62c1-511">Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-511">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="e62c1-512">Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="e62c1-512">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="e62c1-513">Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte</span><span class="sxs-lookup"><span data-stu-id="e62c1-513">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-514">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-514">SQL</span></span>
* <span data-ttu-id="e62c1-515">Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-515">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="e62c1-516">Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen</span><span class="sxs-lookup"><span data-stu-id="e62c1-516">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="e62c1-517">Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-517">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="e62c1-518">Befehl `sql server wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-518">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-519">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-519">Storage</span></span>
* <span data-ttu-id="e62c1-520">Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-520">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-521">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-521">VM</span></span>
* <span data-ttu-id="e62c1-522">`--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-522">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="e62c1-523">`--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-523">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="e62c1-524">`--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen</span><span class="sxs-lookup"><span data-stu-id="e62c1-524">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="e62c1-525">9\. April 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-525">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-526">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-526">Core</span></span>
* <span data-ttu-id="e62c1-527">Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="e62c1-527">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-528">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-528">ACR</span></span>
* <span data-ttu-id="e62c1-529">Unterstützung für die kontextlose Ausführung eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-529">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="e62c1-530">AMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-530">AMS</span></span>
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="e62c1-533">Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-533">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="e62c1-534">Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-534">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-535">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-535">AppService</span></span>
* <span data-ttu-id="e62c1-536">Unterstützung für `--logs` zu `webapp up` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-536">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="e62c1-537">Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-537">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="e62c1-538">Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-538">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="e62c1-539">[BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch</span><span class="sxs-lookup"><span data-stu-id="e62c1-539">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="e62c1-540">Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-540">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="e62c1-541">Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-541">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="e62c1-542">Unterstützung für Einstellungen zum horizontalen Hochskalieren für den Azure Functions-Premium-Plan hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-542">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="e62c1-543">CDN</span><span class="sxs-lookup"><span data-stu-id="e62c1-543">CDN</span></span>
* <span data-ttu-id="e62c1-544">Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="e62c1-544">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="e62c1-545">Feedback</span><span class="sxs-lookup"><span data-stu-id="e62c1-545">Feedback</span></span>
* <span data-ttu-id="e62c1-546">`feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-546">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="e62c1-547">`feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)</span><span class="sxs-lookup"><span data-stu-id="e62c1-547">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="e62c1-548">`feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben</span><span class="sxs-lookup"><span data-stu-id="e62c1-548">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-549">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-549">Monitor</span></span>
* <span data-ttu-id="e62c1-550">Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war</span><span class="sxs-lookup"><span data-stu-id="e62c1-550">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="e62c1-551">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-551">Network</span></span>
* <span data-ttu-id="e62c1-552">Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-552">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="e62c1-553">Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-553">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="e62c1-554">Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-554">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="e62c1-555">Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="e62c1-555">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="e62c1-556">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="e62c1-556">PrivateDNS</span></span>
* <span data-ttu-id="e62c1-557">`network private-dns` für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-557">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-558">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-558">Resource</span></span>
* <span data-ttu-id="e62c1-559">Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="e62c1-559">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-560">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-560">Role</span></span>
* <span data-ttu-id="e62c1-561">`create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten</span><span class="sxs-lookup"><span data-stu-id="e62c1-561">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="e62c1-562">[BREAKING CHANGE] `role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-562">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-563">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-563">SQL</span></span>
* <span data-ttu-id="e62c1-564">`sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-564">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-565">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-565">Storage</span></span>
* <span data-ttu-id="e62c1-566">[BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-566">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="e62c1-567">`--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen</span><span class="sxs-lookup"><span data-stu-id="e62c1-567">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="e62c1-568">`--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-568">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="e62c1-569">`storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="e62c1-569">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="e62c1-570">26. März 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-570">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="e62c1-571">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-571">Core</span></span>
* <span data-ttu-id="e62c1-572">Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-572">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="e62c1-573">Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.</span><span class="sxs-lookup"><span data-stu-id="e62c1-573">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="e62c1-574">Cloud</span><span class="sxs-lookup"><span data-stu-id="e62c1-574">Cloud</span></span>
* <span data-ttu-id="e62c1-575">Fehler „Abonnement nicht gefunden“ in `cloud set` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-575">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-576">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-576">ACR</span></span>
* <span data-ttu-id="e62c1-577">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-577">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="e62c1-578">`--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-578">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="e62c1-579">Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-579">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="e62c1-580">„--no-wait“ zum Befehl `acr build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-580">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-581">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-581">AppService</span></span>
* <span data-ttu-id="e62c1-582">Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-582">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="e62c1-583">Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="e62c1-583">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="e62c1-584">Bot Service</span><span class="sxs-lookup"><span data-stu-id="e62c1-584">BOT Service</span></span>
* <span data-ttu-id="e62c1-585">`bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten</span><span class="sxs-lookup"><span data-stu-id="e62c1-585">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="e62c1-586">`bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-586">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="e62c1-587">[BREAKING CHANGE] `--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.</span><span class="sxs-lookup"><span data-stu-id="e62c1-587">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="e62c1-588">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-588">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="e62c1-589">CDN</span><span class="sxs-lookup"><span data-stu-id="e62c1-589">CDN</span></span>
* <span data-ttu-id="e62c1-590">Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-590">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="e62c1-591">[BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-591">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="e62c1-592">Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-592">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="e62c1-593">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-593">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e62c1-594">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="e62c1-594">Cosmosdb</span></span>
* <span data-ttu-id="e62c1-595">Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-595">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="e62c1-596">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-596">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-597">Interactive</span><span class="sxs-lookup"><span data-stu-id="e62c1-597">Interactive</span></span>
* <span data-ttu-id="e62c1-598">Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-598">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-599">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-599">Monitor</span></span>
* <span data-ttu-id="e62c1-600">Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-600">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-601">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-601">Network</span></span>
* <span data-ttu-id="e62c1-602">Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-602">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="e62c1-603">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-603">Profile</span></span>
* <span data-ttu-id="e62c1-604">Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-604">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="e62c1-605">Postgres</span><span class="sxs-lookup"><span data-stu-id="e62c1-605">Postgres</span></span> 
* <span data-ttu-id="e62c1-606">postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-606">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="e62c1-607">Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="e62c1-607">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-608">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-608">Resource</span></span>
* <span data-ttu-id="e62c1-609">Verbesserte Tabellenausgabe für `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="e62c1-609">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="e62c1-610">Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-610">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="e62c1-611">Graph</span><span class="sxs-lookup"><span data-stu-id="e62c1-611">Graph</span></span>
* <span data-ttu-id="e62c1-612">Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-612">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="e62c1-613">Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-613">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="e62c1-614">Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen</span><span class="sxs-lookup"><span data-stu-id="e62c1-614">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="e62c1-615">Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält</span><span class="sxs-lookup"><span data-stu-id="e62c1-615">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="e62c1-616">`ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-616">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-617">storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-617">storage</span></span>
* <span data-ttu-id="e62c1-618">`--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-618">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="e62c1-619">Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt</span><span class="sxs-lookup"><span data-stu-id="e62c1-619">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="e62c1-620">Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat</span><span class="sxs-lookup"><span data-stu-id="e62c1-620">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="e62c1-621">Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-621">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-622">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-622">VM</span></span>
* <span data-ttu-id="e62c1-623">Befehl `image update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-623">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="e62c1-624">12. März 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-624">March 12, 2019</span></span>

<span data-ttu-id="e62c1-625">Version 2.0.60</span><span class="sxs-lookup"><span data-stu-id="e62c1-625">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-626">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-626">Core</span></span>

* <span data-ttu-id="e62c1-627">Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-627">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-628">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-628">ACR</span></span>

* <span data-ttu-id="e62c1-629">Redundante Quellen im Imageimport korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-629">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-630">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-630">ACS</span></span>

* <span data-ttu-id="e62c1-631">Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-631">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="e62c1-632">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-632">AppService</span></span>

* <span data-ttu-id="e62c1-633">`[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen</span><span class="sxs-lookup"><span data-stu-id="e62c1-633">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="e62c1-634">Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-634">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="e62c1-635">`functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen</span><span class="sxs-lookup"><span data-stu-id="e62c1-635">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="e62c1-636">Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-636">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="e62c1-637">Botservice</span><span class="sxs-lookup"><span data-stu-id="e62c1-637">Botservice</span></span>

* <span data-ttu-id="e62c1-638">`SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-638">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="e62c1-639">`Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-639">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="e62c1-640">Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-640">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="e62c1-641">`bot publish` wurde geändert und ist jetzt asynchron.</span><span class="sxs-lookup"><span data-stu-id="e62c1-641">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-642">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-642">Container</span></span>

* <span data-ttu-id="e62c1-643">Argument `--no-wait` zu `container [start|restart]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-643">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="e62c1-644">EventHub</span><span class="sxs-lookup"><span data-stu-id="e62c1-644">EventHub</span></span>

* <span data-ttu-id="e62c1-645">Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-645">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="e62c1-646">Suchen</span><span class="sxs-lookup"><span data-stu-id="e62c1-646">Find</span></span>

* <span data-ttu-id="e62c1-647">Umfangreiches Funktionsupdate</span><span class="sxs-lookup"><span data-stu-id="e62c1-647">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e62c1-648">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e62c1-648">HDInsight</span></span>

* <span data-ttu-id="e62c1-649">Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-649">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-650">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-650">Network</span></span>

* <span data-ttu-id="e62c1-651">Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug</span><span class="sxs-lookup"><span data-stu-id="e62c1-651">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="e62c1-652">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e62c1-652">Rdbms</span></span>

* <span data-ttu-id="e62c1-653">Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="e62c1-653">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-654">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-654">Role</span></span>

* <span data-ttu-id="e62c1-655">`role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-655">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="e62c1-656">`ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-656">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e62c1-657">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e62c1-657">Service Fabric</span></span>

* <span data-ttu-id="e62c1-658">Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-658">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="e62c1-659">26. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-659">February 26, 2019</span></span>

<span data-ttu-id="e62c1-660">Version 2.0.59</span><span class="sxs-lookup"><span data-stu-id="e62c1-660">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-661">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-661">Core</span></span>

* <span data-ttu-id="e62c1-662">Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat</span><span class="sxs-lookup"><span data-stu-id="e62c1-662">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-663">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-663">ACR</span></span>

* <span data-ttu-id="e62c1-664">Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-664">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="e62c1-665">Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht</span><span class="sxs-lookup"><span data-stu-id="e62c1-665">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-666">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-666">ACS</span></span>

* <span data-ttu-id="e62c1-667">Option `--listen-address` zu `aks port-forward` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-667">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-668">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-668">AppService</span></span>

* <span data-ttu-id="e62c1-669">Befehl `functionapp devops-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-669">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-670">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-670">Batch</span></span>
* <span data-ttu-id="e62c1-671">[BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-671">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="e62c1-672">[BREAKING CHANGE] `Pacakges`-Eigenschaft aus `Application`-Antworten entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-672">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="e62c1-673">Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-673">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="e62c1-674">[BREAKING CHANGE] `--application-id` in allen `batch application`-Befehlen in `--application-name` geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-674">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="e62c1-675">Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-675">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="e62c1-676">Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt</span><span class="sxs-lookup"><span data-stu-id="e62c1-676">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e62c1-677">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e62c1-677">CosmosDB</span></span>

* <span data-ttu-id="e62c1-678">Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-678">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="e62c1-679">Kusto</span><span class="sxs-lookup"><span data-stu-id="e62c1-679">Kusto</span></span>

* <span data-ttu-id="e62c1-680">[BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-680">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-681">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-681">Network</span></span>

* <span data-ttu-id="e62c1-682">Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-682">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="e62c1-683">Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-683">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="e62c1-684">Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-684">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="e62c1-685">Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-685">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="e62c1-686">Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-686">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="e62c1-687">Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-687">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="e62c1-688">Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-688">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-689">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-689">Resource</span></span>

* <span data-ttu-id="e62c1-690">Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-690">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="e62c1-691">Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-691">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="e62c1-692">Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-692">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="e62c1-693">Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-693">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="e62c1-694">Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-694">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-695">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-695">Role</span></span>

* <span data-ttu-id="e62c1-696">Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-696">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-697">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-697">VM</span></span>

* <span data-ttu-id="e62c1-698">Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war</span><span class="sxs-lookup"><span data-stu-id="e62c1-698">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="e62c1-699">12. Februar 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-699">February 12, 2019</span></span>

<span data-ttu-id="e62c1-700">Version 2.0.58</span><span class="sxs-lookup"><span data-stu-id="e62c1-700">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-701">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-701">Core</span></span>

* <span data-ttu-id="e62c1-702">`az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="e62c1-702">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="e62c1-703">Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-703">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-704">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-704">ACR</span></span>
* <span data-ttu-id="e62c1-705">[BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-705">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="e62c1-706">[BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-706">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-707">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-707">ACS</span></span>
* <span data-ttu-id="e62c1-708">Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-708">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="e62c1-709">Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-709">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="e62c1-710">Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-710">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="e62c1-711">AMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-711">AMS</span></span>
* <span data-ttu-id="e62c1-712">Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-712">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="e62c1-713">Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-713">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-714">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-714">Appservice</span></span>
* <span data-ttu-id="e62c1-715">Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-715">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="e62c1-716">Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-716">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="e62c1-717">Die Hilfe für `appservice-plan-update` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-717">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="e62c1-718">Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-718">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="e62c1-719">Probleme mit der Web-App SSH wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-719">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="e62c1-720">Botservice</span><span class="sxs-lookup"><span data-stu-id="e62c1-720">Botservice</span></span>
* <span data-ttu-id="e62c1-721">Die Benutzeroberfläche für `bot publish` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-721">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="e62c1-722">Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-722">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="e62c1-723">Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-723">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="e62c1-724">Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.</span><span class="sxs-lookup"><span data-stu-id="e62c1-724">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="e62c1-725">[VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-725">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="e62c1-726">`az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="e62c1-726">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="e62c1-727">Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.</span><span class="sxs-lookup"><span data-stu-id="e62c1-727">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="e62c1-728">Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-728">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="e62c1-729">Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.</span><span class="sxs-lookup"><span data-stu-id="e62c1-729">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="e62c1-730">`"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-730">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="e62c1-731">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e62c1-731">Key Vault</span></span>
* <span data-ttu-id="e62c1-732">Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.</span><span class="sxs-lookup"><span data-stu-id="e62c1-732">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-733">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-733">Monitor</span></span>
* <span data-ttu-id="e62c1-734">`monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.</span><span class="sxs-lookup"><span data-stu-id="e62c1-734">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-735">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-735">Network</span></span>
* <span data-ttu-id="e62c1-736">`dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-736">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="e62c1-737">Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-737">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="e62c1-738">Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-738">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="e62c1-739">`--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-739">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="e62c1-740">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="e62c1-740">Policy Insights</span></span>
* <span data-ttu-id="e62c1-741">`policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-741">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="e62c1-742">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-742">RDBMS</span></span>
* <span data-ttu-id="e62c1-743">Hilfemeldung und Befehlsparameter wurden verbessert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-743">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="e62c1-744">Redis</span><span class="sxs-lookup"><span data-stu-id="e62c1-744">Redis</span></span>
* <span data-ttu-id="e62c1-745">Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-745">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="e62c1-746">Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-746">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="e62c1-747">Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-747">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="e62c1-748">Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-748">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="e62c1-749">[BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-749">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="e62c1-750">[BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-750">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="e62c1-751">[VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-751">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-752">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-752">Role</span></span>
* <span data-ttu-id="e62c1-753">[BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-753">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="e62c1-754">SQL-VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-754">SQL VM</span></span>
* <span data-ttu-id="e62c1-755">[VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-755">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-756">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-756">VM</span></span>
* <span data-ttu-id="e62c1-757">`vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="e62c1-757">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="e62c1-758">`vmss run-command [invoke | list | show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-758">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="e62c1-759">Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.</span><span class="sxs-lookup"><span data-stu-id="e62c1-759">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="e62c1-760">[BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-760">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="e62c1-761">31. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-761">January 31, 2019</span></span>

<span data-ttu-id="e62c1-762">Version 2.0.57</span><span class="sxs-lookup"><span data-stu-id="e62c1-762">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-763">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-763">Core</span></span>

* <span data-ttu-id="e62c1-764">Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="e62c1-764">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="e62c1-765">28. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-765">January 28, 2019</span></span>

<span data-ttu-id="e62c1-766">Version 2.0.56</span><span class="sxs-lookup"><span data-stu-id="e62c1-766">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-767">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-767">ACR</span></span>
* <span data-ttu-id="e62c1-768">Unterstützung für VNet/IP-Regeln wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-768">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-769">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-769">ACS</span></span>
* <span data-ttu-id="e62c1-770">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-770">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="e62c1-771">Verwaltete OpenShift-Befehle wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-771">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="e62c1-772">Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-772">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="e62c1-773">AMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-773">AMS</span></span>
* <span data-ttu-id="e62c1-774">[BREAKING CHANGE] `ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-774">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="e62c1-775">[BREAKING CHANGE] `ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-775">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-776">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-776">Appservice</span></span>
* <span data-ttu-id="e62c1-777">Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-777">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="e62c1-778">Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-778">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="e62c1-779">Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-779">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-780">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-780">Container</span></span>
* <span data-ttu-id="e62c1-781">Befehl `container start` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-781">Added `container start` command</span></span>
* <span data-ttu-id="e62c1-782">Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-782">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e62c1-783">EventGrid</span><span class="sxs-lookup"><span data-stu-id="e62c1-783">EventGrid</span></span>
* <span data-ttu-id="e62c1-784">Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-784">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="e62c1-785">„storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-785">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="e62c1-786">Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-786">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="e62c1-787">Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e62c1-787">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="e62c1-788">Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-788">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e62c1-789">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e62c1-789">HDInsight</span></span>
* <span data-ttu-id="e62c1-790">[BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-790">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="e62c1-791">[BREAKING CHANGE] `hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.</span><span class="sxs-lookup"><span data-stu-id="e62c1-791">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="e62c1-792">Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-792">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="e62c1-793">Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-793">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="e62c1-794">Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-794">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="e62c1-795">Befehl `hdinsight update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-795">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="e62c1-796">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-796">IoT</span></span>
* <span data-ttu-id="e62c1-797">Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-797">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="e62c1-798">Kusto</span><span class="sxs-lookup"><span data-stu-id="e62c1-798">Kusto</span></span>
* <span data-ttu-id="e62c1-799">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="e62c1-799">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-800">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-800">Monitor</span></span>
* <span data-ttu-id="e62c1-801">ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.</span><span class="sxs-lookup"><span data-stu-id="e62c1-801">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="e62c1-802">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-802">Profile</span></span>
* <span data-ttu-id="e62c1-803">Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-803">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-804">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-804">Network</span></span>
* <span data-ttu-id="e62c1-805">Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.</span><span class="sxs-lookup"><span data-stu-id="e62c1-805">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="e62c1-806">Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.</span><span class="sxs-lookup"><span data-stu-id="e62c1-806">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-807">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-807">Resource</span></span>
* <span data-ttu-id="e62c1-808">Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-808">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="e62c1-809">Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-809">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="e62c1-810">Virtueller SQL-Computer</span><span class="sxs-lookup"><span data-stu-id="e62c1-810">SQL Virtual Machine</span></span>
* <span data-ttu-id="e62c1-811">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="e62c1-811">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-812">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-812">Storage</span></span>
* <span data-ttu-id="e62c1-813">Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-813">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="e62c1-814">Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-814">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-815">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-815">VM</span></span>
* <span data-ttu-id="e62c1-816">`vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="e62c1-816">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="e62c1-817">Flag `--force` wurde zu `vm encryption enable` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-817">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="e62c1-818">15. Januar 2019</span><span class="sxs-lookup"><span data-stu-id="e62c1-818">January 15, 2019</span></span>

<span data-ttu-id="e62c1-819">Version 2.0.55</span><span class="sxs-lookup"><span data-stu-id="e62c1-819">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-820">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-820">ACR</span></span>
* <span data-ttu-id="e62c1-821">Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-821">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="e62c1-822">Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-822">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="e62c1-823">[VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:</span><span class="sxs-lookup"><span data-stu-id="e62c1-823">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="e62c1-824">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-824">ACS</span></span>
* <span data-ttu-id="e62c1-825">Unterstützung für neue ACI-Regionen wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-825">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-826">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-826">Appservice</span></span>
* <span data-ttu-id="e62c1-827">Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.</span><span class="sxs-lookup"><span data-stu-id="e62c1-827">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="e62c1-828">`webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e62c1-828">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="e62c1-829">`[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="e62c1-829">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="e62c1-830">Befehl `webapp ssh` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-830">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="e62c1-831">Botservice</span><span class="sxs-lookup"><span data-stu-id="e62c1-831">Botservice</span></span>
* <span data-ttu-id="e62c1-832">Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-832">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="e62c1-833">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-833">Configure</span></span>
* <span data-ttu-id="e62c1-834">`none` wurde als konfigurierbares Ausgabeformat hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-834">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e62c1-835">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e62c1-835">CosmosDB</span></span>
* <span data-ttu-id="e62c1-836">Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-836">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e62c1-837">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e62c1-837">HDInsight</span></span>
* <span data-ttu-id="e62c1-838">Befehle zum Verwalten von Anwendungen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-838">Added commands for managing applications</span></span>
* <span data-ttu-id="e62c1-839">Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-839">Added commands for managing script actions</span></span>
* <span data-ttu-id="e62c1-840">Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-840">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="e62c1-841">Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-841">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="e62c1-842">[BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-842">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-843">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-843">Network</span></span>
* <span data-ttu-id="e62c1-844">Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-844">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="e62c1-845">Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue</span><span class="sxs-lookup"><span data-stu-id="e62c1-845">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="e62c1-846">Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-846">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="e62c1-847">Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.</span><span class="sxs-lookup"><span data-stu-id="e62c1-847">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-848">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-848">Role</span></span>
* <span data-ttu-id="e62c1-849">[VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-849">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="e62c1-850">Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.</span><span class="sxs-lookup"><span data-stu-id="e62c1-850">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="e62c1-851">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="e62c1-851">Security</span></span>
* <span data-ttu-id="e62c1-852">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e62c1-852">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-853">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-853">Storage</span></span>
* <span data-ttu-id="e62c1-854">[BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-854">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="e62c1-855">Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-855">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="e62c1-856">Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-856">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="e62c1-857">Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-857">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="e62c1-858">Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-858">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-859">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-859">VM</span></span>
* <span data-ttu-id="e62c1-860">`vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.</span><span class="sxs-lookup"><span data-stu-id="e62c1-860">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="e62c1-861">Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-861">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="e62c1-862">Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-862">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="e62c1-863">Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-863">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="e62c1-864">Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-864">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="e62c1-865">Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.</span><span class="sxs-lookup"><span data-stu-id="e62c1-865">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="e62c1-866">20. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-866">December 20, 2018</span></span>

<span data-ttu-id="e62c1-867">Version 2.0.54</span><span class="sxs-lookup"><span data-stu-id="e62c1-867">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="e62c1-868">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-868">Appservice</span></span>
* <span data-ttu-id="e62c1-869">Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte</span><span class="sxs-lookup"><span data-stu-id="e62c1-869">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="e62c1-870">Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-870">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="e62c1-871">Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-871">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="e62c1-872">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="e62c1-872">IoTCentral</span></span>
* <span data-ttu-id="e62c1-873">Fehler bei API-Aufruf für update-Befehl behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-873">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-874">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-874">Role</span></span>
* <span data-ttu-id="e62c1-875">[BREAKING CHANGE] `ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-875">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-876">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-876">SQL</span></span>
* <span data-ttu-id="e62c1-877">Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-877">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-878">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-878">VM</span></span>
* <span data-ttu-id="e62c1-879">Parameter `---os-type` zu `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-879">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="e62c1-880">18. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-880">December 18, 2018</span></span>

<span data-ttu-id="e62c1-881">Version 2.0.53</span><span class="sxs-lookup"><span data-stu-id="e62c1-881">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="e62c1-882">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-882">ACR</span></span>
* <span data-ttu-id="e62c1-883">Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-883">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="e62c1-884">Tabellenlayout für Aufgabenliste komprimiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-884">Condensed the table layout for task list</span></span>
* <span data-ttu-id="e62c1-885">Unterstützung für Azure DevOps-URLs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-885">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-886">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-886">ACS</span></span>
* <span data-ttu-id="e62c1-887">Virtuelle Knoten (Vorschau) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-887">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="e62c1-888">„(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-888">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="e62c1-889">[VERALTET] `az acs`-Befehle als veraltet markiert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-889">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="e62c1-890">ACS wird am 31. Januar 2020 eingestellt</span><span class="sxs-lookup"><span data-stu-id="e62c1-890">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="e62c1-891">Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-891">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="e62c1-892">Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-892">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-893">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-893">Appservice</span></span>
* <span data-ttu-id="e62c1-894">Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-894">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="e62c1-895">Botservice</span><span class="sxs-lookup"><span data-stu-id="e62c1-895">Botservice</span></span>
* <span data-ttu-id="e62c1-896">Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-896">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="e62c1-897">Fehler bei der AppInsights-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-897">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="e62c1-898">Leerzeichenfehler bei Dateipfaden behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-898">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="e62c1-899">Kudu-Netzwerkaufrufe reduziert</span><span class="sxs-lookup"><span data-stu-id="e62c1-899">Reduced Kudu network calls</span></span>
* <span data-ttu-id="e62c1-900">Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt</span><span class="sxs-lookup"><span data-stu-id="e62c1-900">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="e62c1-901">Nutzung</span><span class="sxs-lookup"><span data-stu-id="e62c1-901">Consumption</span></span>
* <span data-ttu-id="e62c1-902">Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-902">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e62c1-903">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e62c1-903">CosmosDB</span></span>
* <span data-ttu-id="e62c1-904">Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-904">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="e62c1-905">Karten</span><span class="sxs-lookup"><span data-stu-id="e62c1-905">Maps</span></span>
* <span data-ttu-id="e62c1-906">Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-906">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-907">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-907">Network</span></span>
* <span data-ttu-id="e62c1-908">Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-908">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="e62c1-909">Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="e62c1-909">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-910">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-910">Resource</span></span>
* <span data-ttu-id="e62c1-911">Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-911">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="e62c1-912">Neuen Befehl `resource wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-912">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-913">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-913">Storage</span></span>
*  <span data-ttu-id="e62c1-914">Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-914">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-915">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-915">VM</span></span>
* <span data-ttu-id="e62c1-916">Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren</span><span class="sxs-lookup"><span data-stu-id="e62c1-916">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="e62c1-917">4\. Dezember 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-917">December 4, 2018</span></span>

<span data-ttu-id="e62c1-918">Version 2.0.52</span><span class="sxs-lookup"><span data-stu-id="e62c1-918">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="e62c1-919">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-919">Core</span></span>
* <span data-ttu-id="e62c1-920">Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-920">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="e62c1-921">Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-921">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-922">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-922">Appservice</span></span>
* <span data-ttu-id="e62c1-923">[VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt</span><span class="sxs-lookup"><span data-stu-id="e62c1-923">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="e62c1-924">Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat</span><span class="sxs-lookup"><span data-stu-id="e62c1-924">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-925">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-925">Network</span></span>
* <span data-ttu-id="e62c1-926">Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-926">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-927">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-927">Role</span></span>
* <span data-ttu-id="e62c1-928">Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-928">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="e62c1-929">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-929">VM</span></span>
* <span data-ttu-id="e62c1-930">[VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-930">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="e62c1-931">Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen</span><span class="sxs-lookup"><span data-stu-id="e62c1-931">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="e62c1-932">`[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen</span><span class="sxs-lookup"><span data-stu-id="e62c1-932">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="e62c1-933">Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen</span><span class="sxs-lookup"><span data-stu-id="e62c1-933">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="e62c1-934">20. November 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-934">November 20, 2018</span></span>

<span data-ttu-id="e62c1-935">Version 2.0.51</span><span class="sxs-lookup"><span data-stu-id="e62c1-935">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="e62c1-936">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-936">Core</span></span>
* <span data-ttu-id="e62c1-937">MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-937">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-938">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-938">ACR</span></span>
* <span data-ttu-id="e62c1-939">Kontexttoken zum Aufgabenschritt hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-939">Added context token to task step</span></span>
* <span data-ttu-id="e62c1-940">Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-940">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="e62c1-941">Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-941">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-942">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-942">Appservice</span></span>
* <span data-ttu-id="e62c1-943">Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-943">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="e62c1-944">Aktualisierung der standardmäßigen `node_version`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-944">Updated the default `node_version`.</span></span> <span data-ttu-id="e62c1-945">Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.</span><span class="sxs-lookup"><span data-stu-id="e62c1-945">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="e62c1-946">Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-946">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="e62c1-947">Behebung eines Fehlers beim Abrufen des ZipDeploy-Status</span><span class="sxs-lookup"><span data-stu-id="e62c1-947">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="e62c1-948">IotCentral</span><span class="sxs-lookup"><span data-stu-id="e62c1-948">IotCentral</span></span>
* <span data-ttu-id="e62c1-949">Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-949">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="e62c1-950">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e62c1-950">KeyVault</span></span>
* <span data-ttu-id="e62c1-951">Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-951">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-952">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-952">Network</span></span>
* <span data-ttu-id="e62c1-953">`root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-953">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="e62c1-954">Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-954">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="e62c1-955">`--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-955">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="e62c1-956">Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-956">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e62c1-957">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e62c1-957">Rdbms</span></span>
* <span data-ttu-id="e62c1-958">MariaDB-VNET-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-958">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="e62c1-959">RBAC</span><span class="sxs-lookup"><span data-stu-id="e62c1-959">Rbac</span></span>
* <span data-ttu-id="e62c1-960">Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-960">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="e62c1-961">Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-961">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="e62c1-962">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-962">Storage</span></span>
* <span data-ttu-id="e62c1-963">Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-963">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="e62c1-964">Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete</span><span class="sxs-lookup"><span data-stu-id="e62c1-964">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="e62c1-965">Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-965">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="e62c1-966">Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-966">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-967">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-967">VM</span></span>
* <span data-ttu-id="e62c1-968">Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-968">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="e62c1-969">Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-969">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="e62c1-970">`sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt</span><span class="sxs-lookup"><span data-stu-id="e62c1-970">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="e62c1-971">Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-971">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="e62c1-972">Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-972">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="e62c1-973">Befehl `snapshot wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-973">Added `snapshot wait` command</span></span>
* <span data-ttu-id="e62c1-974">Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-974">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="e62c1-975">6\. November 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-975">November 6, 2018</span></span>

<span data-ttu-id="e62c1-976">Version 2.0.50</span><span class="sxs-lookup"><span data-stu-id="e62c1-976">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-977">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-977">Core</span></span>
* <span data-ttu-id="e62c1-978">Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-978">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-979">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-979">ACR</span></span>
* <span data-ttu-id="e62c1-980">Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-980">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="e62c1-981">Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-981">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-982">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-982">ACS</span></span>
* <span data-ttu-id="e62c1-983">[BREAKING CHANGE] `enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-983">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="e62c1-984">Advisor</span><span class="sxs-lookup"><span data-stu-id="e62c1-984">Advisor</span></span>
* <span data-ttu-id="e62c1-985">Allgemein verfügbares Release</span><span class="sxs-lookup"><span data-stu-id="e62c1-985">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="e62c1-986">AMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-986">AMS</span></span>
* <span data-ttu-id="e62c1-987">Neue Befehlsgruppen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-987">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="e62c1-988">Neue Befehle hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-988">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="e62c1-989">Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-989">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="e62c1-990">Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-990">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="e62c1-991">Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-991">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="e62c1-992">Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-992">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="e62c1-993">Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-993">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="e62c1-994">[BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt</span><span class="sxs-lookup"><span data-stu-id="e62c1-994">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="e62c1-995">[BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-995">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="e62c1-996">[BREAKING CHANGE] `--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-996">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="e62c1-997">[BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt</span><span class="sxs-lookup"><span data-stu-id="e62c1-997">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="e62c1-998">[BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-998">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="e62c1-999">Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.)</span><span class="sxs-lookup"><span data-stu-id="e62c1-999">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="e62c1-1000">Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1000">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="e62c1-1001">[BREAKING CHANGE] `--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1001">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="e62c1-1002">Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1002">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="e62c1-1003">Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1003">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1004">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1004">AppService</span></span>
* <span data-ttu-id="e62c1-1005">Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war</span><span class="sxs-lookup"><span data-stu-id="e62c1-1005">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="e62c1-1006">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-1006">Configure</span></span>
* <span data-ttu-id="e62c1-1007">YAML zu Ausgabeformatoptionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1007">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-1008">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1008">Container</span></span>
* <span data-ttu-id="e62c1-1009">Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1009">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="e62c1-1010">EventHub</span><span class="sxs-lookup"><span data-stu-id="e62c1-1010">EventHub</span></span>
* <span data-ttu-id="e62c1-1011">Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1011">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-1012">Interactive</span><span class="sxs-lookup"><span data-stu-id="e62c1-1012">Interactive</span></span>
* <span data-ttu-id="e62c1-1013">Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1013">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-1014">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1014">Monitor</span></span>
* <span data-ttu-id="e62c1-1015">Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1015">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1016">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1016">Network</span></span>
* <span data-ttu-id="e62c1-1017">Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1017">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="e62c1-1018">Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1018">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="e62c1-1019">Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1019">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="e62c1-1020">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-1020">Profile</span></span>
* <span data-ttu-id="e62c1-1021">`--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1021">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="e62c1-1022">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1022">RDBMS</span></span>
* <span data-ttu-id="e62c1-1023">MySQL-Replikatbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1023">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-1024">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-1024">Resource</span></span>
* <span data-ttu-id="e62c1-1025">Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1025">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-1026">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-1026">Role</span></span>
* <span data-ttu-id="e62c1-1027">Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1027">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="e62c1-1028">`ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können</span><span class="sxs-lookup"><span data-stu-id="e62c1-1028">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="e62c1-1029">Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1029">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1030">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1030">Storage</span></span>
* <span data-ttu-id="e62c1-1031">Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1031">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1032">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1032">VM</span></span>
* <span data-ttu-id="e62c1-1033">Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1033">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="e62c1-1034">Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte</span><span class="sxs-lookup"><span data-stu-id="e62c1-1034">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="e62c1-1035">Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1035">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="e62c1-1036">`vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1036">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="e62c1-1037">Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1037">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="e62c1-1038">Argumentüberprüfung für `vm create --image` verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1038">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="e62c1-1039">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1039">October 23, 2018</span></span>

<span data-ttu-id="e62c1-1040">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="e62c1-1040">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1041">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1041">Core</span></span>
* <span data-ttu-id="e62c1-1042">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="e62c1-1042">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="e62c1-1043">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1043">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-1044">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1044">ACR</span></span>
* <span data-ttu-id="e62c1-1045">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1045">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="e62c1-1046">CDN</span><span class="sxs-lookup"><span data-stu-id="e62c1-1046">CDN</span></span>
* <span data-ttu-id="e62c1-1047">[BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1047">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="e62c1-1048">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1048">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-1049">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1049">Container</span></span>
* <span data-ttu-id="e62c1-1050">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1050">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="e62c1-1051">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1051">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="e62c1-1052">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1052">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="e62c1-1053">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1053">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="e62c1-1054">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1054">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="e62c1-1055">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1055">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="e62c1-1056">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1056">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e62c1-1057">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e62c1-1057">CosmosDB</span></span>
* <span data-ttu-id="e62c1-1058">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1058">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-1059">Interactive</span><span class="sxs-lookup"><span data-stu-id="e62c1-1059">Interactive</span></span>
* <span data-ttu-id="e62c1-1060">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1060">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="e62c1-1061">IoT Central</span><span class="sxs-lookup"><span data-stu-id="e62c1-1061">IoT Central</span></span>
* <span data-ttu-id="e62c1-1062">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1062">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="e62c1-1063">[BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1063">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-1064">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1064">Monitor</span></span>
* <span data-ttu-id="e62c1-1065">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1065">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="e62c1-1066">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1066">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="e62c1-1067">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1067">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="e62c1-1068">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1068">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="e62c1-1069">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1069">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="e62c1-1070">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1070">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="e62c1-1071">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1071">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="e62c1-1072">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1072">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="e62c1-1073">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1073">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="e62c1-1074">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1074">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1075">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1075">Network</span></span>
* <span data-ttu-id="e62c1-1076">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1076">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="e62c1-1077">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1077">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="e62c1-1078">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="e62c1-1078">ServiceBus</span></span>
* <span data-ttu-id="e62c1-1079">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1079">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-1080">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-1080">SQL</span></span>
* <span data-ttu-id="e62c1-1081">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1081">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1082">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1082">Storage</span></span>
* <span data-ttu-id="e62c1-1083">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1083">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="e62c1-1084">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1084">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1085">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1085">VM</span></span>
* <span data-ttu-id="e62c1-1086">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1086">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="e62c1-1087">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1087">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="e62c1-1088">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1088">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="e62c1-1089">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1089">October 16, 2018</span></span>

<span data-ttu-id="e62c1-1090">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="e62c1-1090">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1091">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1091">VM</span></span>
* <span data-ttu-id="e62c1-1092">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="e62c1-1092">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="e62c1-1093">9\. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1093">October 9, 2018</span></span>

<span data-ttu-id="e62c1-1094">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="e62c1-1094">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1095">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1095">Core</span></span>
* <span data-ttu-id="e62c1-1096">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="e62c1-1096">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-1097">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1097">ACR</span></span>
* <span data-ttu-id="e62c1-1098">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1098">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1099">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1099">ACS</span></span>
* <span data-ttu-id="e62c1-1100">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="e62c1-1100">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="e62c1-1101">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1101">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="e62c1-1102">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1102">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="e62c1-1103">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="e62c1-1103">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-1104">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1104">Container</span></span>
* <span data-ttu-id="e62c1-1105">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1105">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="e62c1-1106">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1106">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="e62c1-1107">Event Hub</span><span class="sxs-lookup"><span data-stu-id="e62c1-1107">Event Hub</span></span>
* <span data-ttu-id="e62c1-1108">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1108">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="e62c1-1109">[BREAKING CHANGE] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1109">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="e62c1-1110">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1110">Extensions</span></span>
* <span data-ttu-id="e62c1-1111">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1111">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e62c1-1112">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e62c1-1112">HDInsight</span></span>
* <span data-ttu-id="e62c1-1113">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e62c1-1113">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="e62c1-1114">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-1114">IoT</span></span>
* <span data-ttu-id="e62c1-1115">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1115">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="e62c1-1116">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e62c1-1116">KeyVault</span></span>
* <span data-ttu-id="e62c1-1117">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="e62c1-1117">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1118">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1118">Network</span></span>
* <span data-ttu-id="e62c1-1119">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1119">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="e62c1-1120">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="e62c1-1120">See #6052</span></span>
* <span data-ttu-id="e62c1-1121">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1121">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="e62c1-1122">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1122">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="e62c1-1123">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1123">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="e62c1-1124">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1124">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="e62c1-1125">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="e62c1-1125">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="e62c1-1126">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1126">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-1127">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-1127">Role</span></span>
* <span data-ttu-id="e62c1-1128">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1128">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="e62c1-1129">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1129">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="e62c1-1130">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-1130">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="e62c1-1131">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1131">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="e62c1-1132">Service Bus</span><span class="sxs-lookup"><span data-stu-id="e62c1-1132">Service Bus</span></span>
* <span data-ttu-id="e62c1-1133">[BREAKING CHANGE] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1133">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1134">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1134">VM</span></span>
* <span data-ttu-id="e62c1-1135">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1135">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="e62c1-1136">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1136">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="e62c1-1137">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1137">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="e62c1-1138">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1138">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="e62c1-1139">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1139">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="e62c1-1140">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1140">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="e62c1-1141">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1141">September 21, 2018</span></span>

<span data-ttu-id="e62c1-1142">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="e62c1-1142">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-1143">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1143">ACR</span></span>
* <span data-ttu-id="e62c1-1144">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1144">Added ACR Task commands</span></span>
* <span data-ttu-id="e62c1-1145">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1145">Added quick run command</span></span>
* <span data-ttu-id="e62c1-1146">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1146">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="e62c1-1147">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1147">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="e62c1-1148">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1148">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="e62c1-1149">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1149">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1150">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1150">ACS</span></span>
* <span data-ttu-id="e62c1-1151">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1151">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="e62c1-1152">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1152">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1153">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1153">AppService</span></span>

* <span data-ttu-id="e62c1-1154">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="e62c1-1154">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="e62c1-1155">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1155">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="e62c1-1156">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1156">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="e62c1-1157">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1157">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-1158">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-1158">Batch</span></span>
* <span data-ttu-id="e62c1-1159">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1159">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="e62c1-1160">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1160">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="e62c1-1161">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1161">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="e62c1-1162">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1162">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e62c1-1163">Batch KI</span><span class="sxs-lookup"><span data-stu-id="e62c1-1163">Batch AI</span></span> 
* <span data-ttu-id="e62c1-1164">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1164">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e62c1-1165">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e62c1-1165">Cognitive Services</span></span>
* <span data-ttu-id="e62c1-1166">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1166">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="e62c1-1167">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1167">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="e62c1-1168">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1168">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="e62c1-1169">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1169">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="e62c1-1170">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1170">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="e62c1-1171">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="e62c1-1171">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-1172">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1172">Container</span></span>
* <span data-ttu-id="e62c1-1173">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1173">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="e62c1-1174">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1174">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="e62c1-1175">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1175">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="e62c1-1176">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1176">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="e62c1-1177">Data Lake</span><span class="sxs-lookup"><span data-stu-id="e62c1-1177">Datalake</span></span>
* <span data-ttu-id="e62c1-1178">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1178">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="e62c1-1179">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="e62c1-1179">Interactive Shell</span></span>
* <span data-ttu-id="e62c1-1180">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1180">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="e62c1-1181">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1181">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="e62c1-1182">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-1182">IoT</span></span>
* <span data-ttu-id="e62c1-1183">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1183">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="e62c1-1184">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e62c1-1184">Key Vault</span></span>
* <span data-ttu-id="e62c1-1185">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1185">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1186">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1186">Network</span></span>
* <span data-ttu-id="e62c1-1187">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1187">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="e62c1-1188">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1188">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="e62c1-1189">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1189">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="e62c1-1190">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1190">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="e62c1-1191">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1191">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="e62c1-1192">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1192">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="e62c1-1193">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="e62c1-1193">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="e62c1-1194">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="e62c1-1194">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="e62c1-1195">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1195">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="e62c1-1196">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1196">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="e62c1-1197">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1197">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="e62c1-1198">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1198">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="e62c1-1199">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1199">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="e62c1-1200">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1200">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="e62c1-1201">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1201">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="e62c1-1202">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1202">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="e62c1-1203">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1203">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="e62c1-1204">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1204">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="e62c1-1205">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1205">RDBMS</span></span>
* <span data-ttu-id="e62c1-1206">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1206">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="e62c1-1207">Reservierung</span><span class="sxs-lookup"><span data-stu-id="e62c1-1207">Reservation</span></span>
* <span data-ttu-id="e62c1-1208">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1208">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="e62c1-1209">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1209">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="e62c1-1210">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="e62c1-1210">Manage App</span></span>
* <span data-ttu-id="e62c1-1211">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="e62c1-1211">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="e62c1-1212">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="e62c1-1212">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-1213">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-1213">Role</span></span>
* <span data-ttu-id="e62c1-1214">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1214">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="e62c1-1215">SignalR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1215">SignalR</span></span>
* <span data-ttu-id="e62c1-1216">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e62c1-1216">First release</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1217">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1217">Storage</span></span>
* <span data-ttu-id="e62c1-1218">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1218">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="e62c1-1219">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1219">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1220">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1220">VM</span></span>
* <span data-ttu-id="e62c1-1221">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="e62c1-1221">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="e62c1-1222">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1222">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="e62c1-1223">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1223">August 28, 2018</span></span>

<span data-ttu-id="e62c1-1224">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="e62c1-1224">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1225">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1225">Core</span></span>

* <span data-ttu-id="e62c1-1226">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1226">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="e62c1-1227">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1227">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-1228">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1228">ACR</span></span>

* <span data-ttu-id="e62c1-1229">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1229">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="e62c1-1230">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1230">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1231">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1231">ACS</span></span>

* <span data-ttu-id="e62c1-1232">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1232">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="e62c1-1233">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1233">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1234">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1234">AppService</span></span>

* <span data-ttu-id="e62c1-1235">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1235">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="e62c1-1236">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1236">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="e62c1-1237">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1237">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="e62c1-1238">Backup</span><span class="sxs-lookup"><span data-stu-id="e62c1-1238">Backup</span></span>

* <span data-ttu-id="e62c1-1239">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1239">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="e62c1-1240">Botdienst</span><span class="sxs-lookup"><span data-stu-id="e62c1-1240">Bot Service</span></span>

* <span data-ttu-id="e62c1-1241">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="e62c1-1241">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e62c1-1242">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e62c1-1242">Cognitive Services</span></span>

* <span data-ttu-id="e62c1-1243">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1243">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="e62c1-1244">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-1244">IoT</span></span>

* <span data-ttu-id="e62c1-1245">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1245">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-1246">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1246">Monitor</span></span>

* <span data-ttu-id="e62c1-1247">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1247">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="e62c1-1248">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1248">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1249">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1249">Network</span></span>

* <span data-ttu-id="e62c1-1250">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1250">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-1251">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-1251">Resource</span></span>

* <span data-ttu-id="e62c1-1252">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1252">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1253">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1253">Storage</span></span>

* <span data-ttu-id="e62c1-1254">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1254">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1255">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1255">VM</span></span>

* <span data-ttu-id="e62c1-1256">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1256">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="e62c1-1257">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1257">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="e62c1-1258">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1258">Auguest 14, 2018</span></span>

<span data-ttu-id="e62c1-1259">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="e62c1-1259">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1260">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1260">Core</span></span>

* <span data-ttu-id="e62c1-1261">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1261">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="e62c1-1262">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1262">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="e62c1-1263">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="e62c1-1263">Telemetry</span></span>

* <span data-ttu-id="e62c1-1264">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="e62c1-1264">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-1265">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1265">ACR</span></span>

* <span data-ttu-id="e62c1-1266">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1266">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="e62c1-1267">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-1267">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1268">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1268">ACS</span></span>

* <span data-ttu-id="e62c1-1269">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1269">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="e62c1-1270">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-1270">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="e62c1-1271">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="e62c1-1271">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="e62c1-1272">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1272">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="e62c1-1273">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1273">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="e62c1-1274">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1274">AppService</span></span>

* <span data-ttu-id="e62c1-1275">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="e62c1-1275">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="e62c1-1276">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1276">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="e62c1-1277">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e62c1-1277">BatchAI</span></span>

* <span data-ttu-id="e62c1-1278">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1278">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="e62c1-1279">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1279">Container</span></span>

* <span data-ttu-id="e62c1-1280">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1280">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="e62c1-1281">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-1281">IoT</span></span>

* <span data-ttu-id="e62c1-1282">[BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1282">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="e62c1-1283">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1283">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="e62c1-1284">Iot Central</span><span class="sxs-lookup"><span data-stu-id="e62c1-1284">Iot Central</span></span>

* <span data-ttu-id="e62c1-1285">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="e62c1-1285">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e62c1-1286">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e62c1-1286">KeyVault</span></span>


* <span data-ttu-id="e62c1-1287">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1287">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="e62c1-1288">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1288">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="e62c1-1289">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1289">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="e62c1-1290">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1290">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="e62c1-1291">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1291">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="e62c1-1292">Relay</span><span class="sxs-lookup"><span data-stu-id="e62c1-1292">Relay</span></span>

* <span data-ttu-id="e62c1-1293">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e62c1-1293">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-1294">Sql</span><span class="sxs-lookup"><span data-stu-id="e62c1-1294">Sql</span></span>

* <span data-ttu-id="e62c1-1295">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1295">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1296">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1296">Storage</span></span>

* <span data-ttu-id="e62c1-1297">[BREAKING CHANGE] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="e62c1-1297">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="e62c1-1298">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1298">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="e62c1-1299">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1299">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="e62c1-1300">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1300">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="e62c1-1301">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1301">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1302">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1302">VM</span></span>

* <span data-ttu-id="e62c1-1303">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1303">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="e62c1-1304">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1304">July 31, 2018</span></span>

<span data-ttu-id="e62c1-1305">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="e62c1-1305">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-1306">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1306">ACR</span></span>

* <span data-ttu-id="e62c1-1307">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1307">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="e62c1-1308">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1308">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1309">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1309">ACS</span></span>

* <span data-ttu-id="e62c1-1310">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1310">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-1311">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-1311">Batch</span></span>

* <span data-ttu-id="e62c1-1312">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e62c1-1312">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-1313">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1313">Container</span></span>

* <span data-ttu-id="e62c1-1314">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1314">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1315">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1315">Network</span></span>

* <span data-ttu-id="e62c1-1316">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1316">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="e62c1-1317">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-1317">Resource</span></span>

* <span data-ttu-id="e62c1-1318">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1318">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="e62c1-1319">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="e62c1-1319">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-1320">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-1320">Role</span></span>

* <span data-ttu-id="e62c1-1321">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1321">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="e62c1-1322">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="e62c1-1322">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="e62c1-1323">Suchen,</span><span class="sxs-lookup"><span data-stu-id="e62c1-1323">Search</span></span>

* <span data-ttu-id="e62c1-1324">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1324">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="e62c1-1325">Service Bus</span><span class="sxs-lookup"><span data-stu-id="e62c1-1325">Service Bus</span></span>

* <span data-ttu-id="e62c1-1326">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-1326">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="e62c1-1327">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1327">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="e62c1-1328">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="e62c1-1328">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="e62c1-1329">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="e62c1-1329">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1330">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1330">Storage</span></span>

* <span data-ttu-id="e62c1-1331">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1331">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="e62c1-1332">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-1332">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1333">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1333">VM</span></span>

* <span data-ttu-id="e62c1-1334">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1334">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="e62c1-1335">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1335">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="e62c1-1336">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1336">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="e62c1-1337">[BREAKING CHANGE] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1337">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="e62c1-1338">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1338">July 18, 2018</span></span>

<span data-ttu-id="e62c1-1339">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="e62c1-1339">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1340">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1340">Core</span></span>

* <span data-ttu-id="e62c1-1341">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1341">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="e62c1-1342">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1342">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="e62c1-1343">[BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1343">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-1344">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1344">ACR</span></span>

* <span data-ttu-id="e62c1-1345">[BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1345">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="e62c1-1346">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1346">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="e62c1-1347">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1347">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="e62c1-1348">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1348">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1349">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1349">ACS</span></span>

* <span data-ttu-id="e62c1-1350">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1350">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1351">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1351">AppService</span></span>

* <span data-ttu-id="e62c1-1352">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1352">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-1353">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-1353">Batch</span></span>

* <span data-ttu-id="e62c1-1354">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="e62c1-1354">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="e62c1-1355">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1355">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e62c1-1356">Batch KI</span><span class="sxs-lookup"><span data-stu-id="e62c1-1356">Batch AI</span></span>

* <span data-ttu-id="e62c1-1357">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1357">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-1358">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1358">Container</span></span>

* <span data-ttu-id="e62c1-1359">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1359">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="e62c1-1360">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1360">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1361">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1361">Network</span></span>

* <span data-ttu-id="e62c1-1362">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1362">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="e62c1-1363">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1363">Added `network nic wait`</span></span>
* <span data-ttu-id="e62c1-1364">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1364">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="e62c1-1365">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1365">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="e62c1-1366">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-1366">Resource</span></span>

* <span data-ttu-id="e62c1-1367">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1367">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="e62c1-1368">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1368">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="e62c1-1369">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1369">Added `deployment wait` command</span></span>
* <span data-ttu-id="e62c1-1370">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1370">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-1371">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-1371">SQL</span></span>

* <span data-ttu-id="e62c1-1372">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1372">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="e62c1-1373">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="e62c1-1373">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="e62c1-1374">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1374">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1375">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1375">Storage</span></span>

* <span data-ttu-id="e62c1-1376">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1376">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1377">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1377">VM</span></span>

* <span data-ttu-id="e62c1-1378">[BREAKING CHANGE] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1378">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="e62c1-1379">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1379">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="e62c1-1380">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1380">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e62c1-1381">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1381">July 3, 2018</span></span>

<span data-ttu-id="e62c1-1382">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="e62c1-1382">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="e62c1-1383">AKS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1383">AKS</span></span>

* <span data-ttu-id="e62c1-1384">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1384">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e62c1-1385">3\. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1385">July 3, 2018</span></span>

<span data-ttu-id="e62c1-1386">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="e62c1-1386">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1387">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1387">Core</span></span>

* <span data-ttu-id="e62c1-1388">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1388">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1389">ACR</span></span>

* <span data-ttu-id="e62c1-1390">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1390">Added polling build status</span></span>
* <span data-ttu-id="e62c1-1391">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1391">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="e62c1-1392">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1392">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1393">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1393">ACS</span></span>

* <span data-ttu-id="e62c1-1394">[BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e62c1-1394">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="e62c1-1395">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1395">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="e62c1-1396">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1396">Updated options for `aks browse` command.</span></span> <span data-ttu-id="e62c1-1397">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1397">Added `--listen-port` support</span></span>
* <span data-ttu-id="e62c1-1398">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1398">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="e62c1-1399">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="e62c1-1399">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="e62c1-1400">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1400">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1401">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1401">AppService</span></span>

* <span data-ttu-id="e62c1-1402">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1402">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="e62c1-1403">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1403">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="e62c1-1404">Backup</span><span class="sxs-lookup"><span data-stu-id="e62c1-1404">Backup</span></span>

* <span data-ttu-id="e62c1-1405">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1405">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="e62c1-1406">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e62c1-1406">BatchAI</span></span>

* <span data-ttu-id="e62c1-1407">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1407">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="e62c1-1408">Cloud</span><span class="sxs-lookup"><span data-stu-id="e62c1-1408">Cloud</span></span>

* <span data-ttu-id="e62c1-1409">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1409">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-1410">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1410">Container</span></span>

* <span data-ttu-id="e62c1-1411">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1411">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="e62c1-1412">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1412">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="e62c1-1413">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1413">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="e62c1-1414">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e62c1-1414">Extension</span></span>

* <span data-ttu-id="e62c1-1415">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1415">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1416">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1416">Network</span></span>

* <span data-ttu-id="e62c1-1417">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="e62c1-1417">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="e62c1-1418">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e62c1-1418">Rdbms</span></span>

* <span data-ttu-id="e62c1-1419">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1419">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-1420">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-1420">Resource</span></span>

* <span data-ttu-id="e62c1-1421">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1421">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1422">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1422">VM</span></span>

* <span data-ttu-id="e62c1-1423">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1423">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="e62c1-1424">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1424">June 25, 2018</span></span>

<span data-ttu-id="e62c1-1425">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="e62c1-1425">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="e62c1-1426">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="e62c1-1426">CLI</span></span>

* <span data-ttu-id="e62c1-1427">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1427">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="e62c1-1428">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1428">June 19, 2018</span></span>

<span data-ttu-id="e62c1-1429">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="e62c1-1429">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1430">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1430">Core</span></span>

* <span data-ttu-id="e62c1-1431">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1431">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-1432">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1432">ACR</span></span>

* <span data-ttu-id="e62c1-1433">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1433">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="e62c1-1434">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1434">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1435">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1435">ACS</span></span>

* <span data-ttu-id="e62c1-1436">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1436">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="e62c1-1437">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1437">Added `--update` support</span></span>
* <span data-ttu-id="e62c1-1438">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1438">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="e62c1-1439">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="e62c1-1439">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="e62c1-1440">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1440">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="e62c1-1441">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1441">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="e62c1-1442">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1442">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="e62c1-1443">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1443">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1444">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1444">AppService</span></span>

* <span data-ttu-id="e62c1-1445">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1445">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="e62c1-1446">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1446">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-1447">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-1447">Batch</span></span>

* <span data-ttu-id="e62c1-1448">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1448">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e62c1-1449">Batch KI</span><span class="sxs-lookup"><span data-stu-id="e62c1-1449">Batch AI</span></span>

* <span data-ttu-id="e62c1-1450">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1450">Added support for workspaces.</span></span> <span data-ttu-id="e62c1-1451">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1451">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="e62c1-1452">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1452">Added support for experiments.</span></span> <span data-ttu-id="e62c1-1453">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1453">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="e62c1-1454">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1454">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="e62c1-1455">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1455">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="e62c1-1456">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1456">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="e62c1-1457">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1457">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="e62c1-1458">[BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1458">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="e62c1-1459">[BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1459">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="e62c1-1460">[BREAKING CHANGE] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1460">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="e62c1-1461">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1461">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="e62c1-1462">[BREAKING CHANGE] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1462">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="e62c1-1463">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1463">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="e62c1-1464">[BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1464">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="e62c1-1465">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1465">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="e62c1-1466">[BREAKING CHANGE] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1466">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="e62c1-1467">[BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1467">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="e62c1-1468">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1468">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="e62c1-1469">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1469">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="e62c1-1470">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1470">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="e62c1-1471">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1471">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="e62c1-1472">Karten</span><span class="sxs-lookup"><span data-stu-id="e62c1-1472">Maps</span></span>

* <span data-ttu-id="e62c1-1473">[BREAKING CHANGE] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1473">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1474">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1474">Network</span></span>

* <span data-ttu-id="e62c1-1475">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="e62c1-1475">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="e62c1-1476">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1476">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="e62c1-1477">#6502</span><span class="sxs-lookup"><span data-stu-id="e62c1-1477">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="e62c1-1478">Reservations</span><span class="sxs-lookup"><span data-stu-id="e62c1-1478">Reservations</span></span>

* <span data-ttu-id="e62c1-1479">[BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1479">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="e62c1-1480">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1480">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="e62c1-1481">[BREAKING CHANGE] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1481">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="e62c1-1482">[BREAKING CHANGE] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1482">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="e62c1-1483">[BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1483">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="e62c1-1484">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1484">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-1485">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-1485">Role</span></span>

* <span data-ttu-id="e62c1-1486">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1486">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-1487">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-1487">SQL</span></span>

* <span data-ttu-id="e62c1-1488">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1488">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1489">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1489">Storage</span></span>

* <span data-ttu-id="e62c1-1490">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1490">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1491">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1491">VM</span></span>

* <span data-ttu-id="e62c1-1492">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="e62c1-1492">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="e62c1-1493">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1493">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="e62c1-1494">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-1494">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e62c1-1495">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1495">June 13, 2018</span></span>

<span data-ttu-id="e62c1-1496">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="e62c1-1496">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1497">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1497">Core</span></span>

* <span data-ttu-id="e62c1-1498">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="e62c1-1498">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e62c1-1499">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1499">June 13, 2018</span></span>

<span data-ttu-id="e62c1-1500">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="e62c1-1500">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="e62c1-1501">AKS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1501">AKS</span></span>

* <span data-ttu-id="e62c1-1502">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1502">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="e62c1-1503">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1503">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="e62c1-1504">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1504">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="e62c1-1505">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1505">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="e62c1-1506">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1506">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1507">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1507">AppService</span></span>

* <span data-ttu-id="e62c1-1508">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1508">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e62c1-1509">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1509">June 5, 2018</span></span>

<span data-ttu-id="e62c1-1510">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="e62c1-1510">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-1511">Interactive</span><span class="sxs-lookup"><span data-stu-id="e62c1-1511">Interactive</span></span>

* <span data-ttu-id="e62c1-1512">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1512">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e62c1-1513">5\. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1513">June 5, 2018</span></span>

<span data-ttu-id="e62c1-1514">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="e62c1-1514">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1515">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1515">Core</span></span>

* <span data-ttu-id="e62c1-1516">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1516">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="e62c1-1517">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="e62c1-1517">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-1518">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1518">ACR</span></span>

* <span data-ttu-id="e62c1-1519">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1519">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="e62c1-1520">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1520">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="e62c1-1521">AKS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1521">AKS</span></span>

* <span data-ttu-id="e62c1-1522">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1522">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-1523">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-1523">Batch</span></span>

* <span data-ttu-id="e62c1-1524">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="e62c1-1524">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="e62c1-1525">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-1525">IOT</span></span>

* <span data-ttu-id="e62c1-1526">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1526">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1527">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1527">Network</span></span>

* <span data-ttu-id="e62c1-1528">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1528">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="e62c1-1529">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="e62c1-1529">Policy Insights</span></span>

* <span data-ttu-id="e62c1-1530">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e62c1-1530">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="e62c1-1531">ARM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1531">ARM</span></span>

* <span data-ttu-id="e62c1-1532">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1532">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-1533">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-1533">SQL</span></span>

* <span data-ttu-id="e62c1-1534">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1534">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="e62c1-1535">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1535">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="e62c1-1536">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1536">Storage</span></span>

* <span data-ttu-id="e62c1-1537">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="e62c1-1537">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1538">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1538">VM</span></span>

* <span data-ttu-id="e62c1-1539">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1539">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="e62c1-1540">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1540">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="e62c1-1541">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1541">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="e62c1-1542">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1542">May 22, 2018</span></span>

<span data-ttu-id="e62c1-1543">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="e62c1-1543">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1544">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1544">Core</span></span>

* <span data-ttu-id="e62c1-1545">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1545">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1546">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1546">ACS</span></span>

* <span data-ttu-id="e62c1-1547">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1547">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="e62c1-1548">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1548">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1549">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1549">AppService</span></span>

* <span data-ttu-id="e62c1-1550">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="e62c1-1550">Improved generic update commands</span></span>
* <span data-ttu-id="e62c1-1551">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1551">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-1552">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1552">Container</span></span>

* <span data-ttu-id="e62c1-1553">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1553">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="e62c1-1554">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1554">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e62c1-1555">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e62c1-1555">Extension</span></span>

* <span data-ttu-id="e62c1-1556">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1556">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-1557">Interactive</span><span class="sxs-lookup"><span data-stu-id="e62c1-1557">Interactive</span></span>

* <span data-ttu-id="e62c1-1558">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-1558">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="e62c1-1559">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="e62c1-1559">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="e62c1-1560">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e62c1-1560">KeyVault</span></span>

* <span data-ttu-id="e62c1-1561">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1561">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1562">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1562">Network</span></span>

* <span data-ttu-id="e62c1-1563">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="e62c1-1563">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="e62c1-1564">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="e62c1-1564">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-1565">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-1565">SQL</span></span>

* <span data-ttu-id="e62c1-1566">[BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1566">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="e62c1-1567">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1567">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="e62c1-1568">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1568">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="e62c1-1569">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="e62c1-1569">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="e62c1-1570">[BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1570">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="e62c1-1571">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1571">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="e62c1-1572">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1572">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="e62c1-1573">`edition`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1573">`edition`.</span></span> <span data-ttu-id="e62c1-1574">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1574">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="e62c1-1575">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1575">`elasticPoolName`.</span></span> <span data-ttu-id="e62c1-1576">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1576">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="e62c1-1577">[BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1577">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="e62c1-1578">`edition`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1578">`edition`.</span></span> <span data-ttu-id="e62c1-1579">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1579">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="e62c1-1580">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1580">`dtu`.</span></span> <span data-ttu-id="e62c1-1581">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1581">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="e62c1-1582">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1582">`databaseDtuMin`.</span></span> <span data-ttu-id="e62c1-1583">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1583">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="e62c1-1584">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1584">`databaseDtuMax`.</span></span> <span data-ttu-id="e62c1-1585">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1585">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="e62c1-1586">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1586">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="e62c1-1587">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1587">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1588">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1588">Storage</span></span>

* <span data-ttu-id="e62c1-1589">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1589">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="e62c1-1590">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1590">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1591">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1591">VM</span></span>

* <span data-ttu-id="e62c1-1592">[BREAKING CHANGE] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1592">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="e62c1-1593">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1593">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="e62c1-1594">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1594">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="e62c1-1595">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1595">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="e62c1-1596">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1596">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="e62c1-1597">7\. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1597">May 7, 2018</span></span>

<span data-ttu-id="e62c1-1598">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="e62c1-1598">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1599">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1599">Core</span></span>

* <span data-ttu-id="e62c1-1600">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1600">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="e62c1-1601">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1601">Added limited support for positional arguments</span></span>
* <span data-ttu-id="e62c1-1602">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="e62c1-1602">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="e62c1-1603">#5591</span><span class="sxs-lookup"><span data-stu-id="e62c1-1603">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="e62c1-1604">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1604">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="e62c1-1605">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1605">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="e62c1-1606">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="e62c1-1606">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="e62c1-1607">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1607">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="e62c1-1608">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1608">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-1609">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1609">ACR</span></span>

* <span data-ttu-id="e62c1-1610">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1610">Added ACR Build commands</span></span>
* <span data-ttu-id="e62c1-1611">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1611">Improved resource not found error messages</span></span>
* <span data-ttu-id="e62c1-1612">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="e62c1-1612">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="e62c1-1613">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1613">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="e62c1-1614">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1614">Improved repository commands error messages</span></span>
* <span data-ttu-id="e62c1-1615">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1615">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1616">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1616">ACS</span></span>

* <span data-ttu-id="e62c1-1617">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1617">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="e62c1-1618">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1618">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="e62c1-1619">AMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1619">AMS</span></span>

* <span data-ttu-id="e62c1-1620">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1620">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1621">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1621">Appservice</span></span>

* <span data-ttu-id="e62c1-1622">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1622">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="e62c1-1623">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1623">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="e62c1-1624">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1624">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="e62c1-1625">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1625">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e62c1-1626">Batch KI</span><span class="sxs-lookup"><span data-stu-id="e62c1-1626">Batch AI</span></span>

* <span data-ttu-id="e62c1-1627">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1627">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e62c1-1628">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e62c1-1628">Cognitive Services</span></span>

* <span data-ttu-id="e62c1-1629">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="e62c1-1629">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="e62c1-1630">Nutzung</span><span class="sxs-lookup"><span data-stu-id="e62c1-1630">Consumption</span></span>

* <span data-ttu-id="e62c1-1631">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1631">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-1632">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1632">Container</span></span>

* <span data-ttu-id="e62c1-1633">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1633">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e62c1-1634">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e62c1-1634">Cosmos DB</span></span>

* <span data-ttu-id="e62c1-1635">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e62c1-1635">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="e62c1-1636">DMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1636">DMS</span></span>

* <span data-ttu-id="e62c1-1637">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1637">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="e62c1-1638">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e62c1-1638">Extension</span></span>

* <span data-ttu-id="e62c1-1639">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1639">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-1640">Interactive</span><span class="sxs-lookup"><span data-stu-id="e62c1-1640">Interactive</span></span>

* <span data-ttu-id="e62c1-1641">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1641">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="e62c1-1642">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="e62c1-1642">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="e62c1-1643">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1643">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="e62c1-1644">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1644">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="e62c1-1645">Labor</span><span class="sxs-lookup"><span data-stu-id="e62c1-1645">Lab</span></span>

* <span data-ttu-id="e62c1-1646">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1646">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1647">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1647">Network</span></span>

* <span data-ttu-id="e62c1-1648">[BREAKING CHANGE] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1648">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="e62c1-1649">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-1649">Profile</span></span>

* <span data-ttu-id="e62c1-1650">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1650">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="e62c1-1651">[BREAKING CHANGE] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1651">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="e62c1-1652">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1652">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="e62c1-1653">Redis</span><span class="sxs-lookup"><span data-stu-id="e62c1-1653">Redis</span></span>

* <span data-ttu-id="e62c1-1654">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1654">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="e62c1-1655">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1655">Deprecated `redis list-all`.</span></span> <span data-ttu-id="e62c1-1656">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1656">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="e62c1-1657">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1657">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="e62c1-1658">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1658">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-1659">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-1659">Role</span></span>

* <span data-ttu-id="e62c1-1660">[BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1660">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1661">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1661">Storage</span></span>

* <span data-ttu-id="e62c1-1662">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1662">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="e62c1-1663">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="e62c1-1663">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="e62c1-1664">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="e62c1-1664">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="e62c1-1665">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1665">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="e62c1-1666">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-1666">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1667">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1667">VM</span></span>

* <span data-ttu-id="e62c1-1668">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1668">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="e62c1-1669">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1669">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="e62c1-1670">[BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1670">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="e62c1-1671">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1671">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="e62c1-1672">[BREAKING CHANGE] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1672">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="e62c1-1673">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1673">Added write accelerator support</span></span>
* <span data-ttu-id="e62c1-1674">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1674">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="e62c1-1675">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1675">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="e62c1-1676">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1676">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="e62c1-1677">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1677">April 10, 2018</span></span>

<span data-ttu-id="e62c1-1678">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="e62c1-1678">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-1679">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1679">ACR</span></span>

* <span data-ttu-id="e62c1-1680">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="e62c1-1680">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1681">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1681">ACS</span></span>

* <span data-ttu-id="e62c1-1682">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1682">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1683">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1683">Appservice</span></span>

* [BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="e62c1-1685">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1685">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="e62c1-1686">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e62c1-1686">BatchAI</span></span>

* <span data-ttu-id="e62c1-1687">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1687">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="e62c1-1688">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="e62c1-1688">Job level mounting</span></span>
  - <span data-ttu-id="e62c1-1689">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="e62c1-1689">Environment variables with secret values</span></span>
  - <span data-ttu-id="e62c1-1690">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="e62c1-1690">Performance counters settings</span></span>
  - <span data-ttu-id="e62c1-1691">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="e62c1-1691">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="e62c1-1692">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="e62c1-1692">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="e62c1-1693">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="e62c1-1693">Usage and limits reporting</span></span>
  - <span data-ttu-id="e62c1-1694">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="e62c1-1694">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="e62c1-1695">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="e62c1-1695">Support for custom images</span></span>
  - <span data-ttu-id="e62c1-1696">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1696">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="e62c1-1697">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="e62c1-1697">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="e62c1-1698">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch KI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1698">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="e62c1-1699">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1699">National clouds are supported</span></span>
* <span data-ttu-id="e62c1-1700">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1700">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="e62c1-1701">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="e62c1-1701">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="e62c1-1702">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch KI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1702">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="e62c1-1703">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1703">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="e62c1-1704">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="e62c1-1704">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="e62c1-1705">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="e62c1-1705">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="e62c1-1706">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="e62c1-1706">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="e62c1-1707">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1707">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="e62c1-1708">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1708">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="e62c1-1709">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1709">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="e62c1-1710">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="e62c1-1710">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="e62c1-1711">[BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1711">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="e62c1-1712">[BREAKING CHANGE] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1712">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="e62c1-1713">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="e62c1-1713">Billing</span></span>

* <span data-ttu-id="e62c1-1714">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1714">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="e62c1-1715">Nutzung</span><span class="sxs-lookup"><span data-stu-id="e62c1-1715">Consumption</span></span>

* <span data-ttu-id="e62c1-1716">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1716">Added `marketplace` commands</span></span>
* <span data-ttu-id="e62c1-1717">[BREAKING CHANGE] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1717">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="e62c1-1718">[BREAKING CHANGE] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1718">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="e62c1-1719">[BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1719">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="e62c1-1720">[BREAKING CHANGE] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1720">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="e62c1-1721">[BREAKING CHANGE] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1721">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-1722">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1722">Container</span></span>

* <span data-ttu-id="e62c1-1723">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1723">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="e62c1-1724">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-1724">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="e62c1-1725">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e62c1-1725">Extension</span></span>

* <span data-ttu-id="e62c1-1726">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1726">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-1727">Interactive</span><span class="sxs-lookup"><span data-stu-id="e62c1-1727">Interactive</span></span>

* <span data-ttu-id="e62c1-1728">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1728">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="e62c1-1729">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1729">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="e62c1-1730">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1730">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1731">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1731">Network</span></span>

* <span data-ttu-id="e62c1-1732">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1732">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="e62c1-1733">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1733">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="e62c1-1734">#4910</span><span class="sxs-lookup"><span data-stu-id="e62c1-1734">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="e62c1-1735">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1735">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="e62c1-1736">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1736">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="e62c1-1737">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1737">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="e62c1-1738">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1738">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="e62c1-1739">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1739">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="e62c1-1740">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-1740">Profile</span></span>

* <span data-ttu-id="e62c1-1741">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1741">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="e62c1-1742">[BREAKING CHANGE] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1742">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="e62c1-1743">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1743">RDBMS</span></span>

* <span data-ttu-id="e62c1-1744">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1744">Added `georestore` command</span></span>
* <span data-ttu-id="e62c1-1745">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1745">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-1746">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-1746">Resource</span></span>

* <span data-ttu-id="e62c1-1747">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1747">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="e62c1-1748">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1748">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-1749">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-1749">SQL</span></span>

* <span data-ttu-id="e62c1-1750">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1750">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1751">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1751">Storage</span></span>

* <span data-ttu-id="e62c1-1752">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1752">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1753">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1753">VM</span></span>

* <span data-ttu-id="e62c1-1754">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1754">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="e62c1-1755">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1755">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="e62c1-1757">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1757">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="e62c1-1758">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1758">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="e62c1-1759">#5718</span><span class="sxs-lookup"><span data-stu-id="e62c1-1759">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="e62c1-1760">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1760">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="e62c1-1761">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1761">March 27, 2018</span></span>

<span data-ttu-id="e62c1-1762">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="e62c1-1762">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1763">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1763">Core</span></span>

* <span data-ttu-id="e62c1-1764">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="e62c1-1764">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1765">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1765">ACS</span></span>

* <span data-ttu-id="e62c1-1766">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e62c1-1766">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1767">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1767">Appservice</span></span>

* <span data-ttu-id="e62c1-1768">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1768">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="e62c1-1769">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1769">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e62c1-1770">Backup</span><span class="sxs-lookup"><span data-stu-id="e62c1-1770">Backup</span></span>

* <span data-ttu-id="e62c1-1771">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1771">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="e62c1-1772">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1772">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="e62c1-1773">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1773">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="e62c1-1774">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1774">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-1775">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1775">Container</span></span>

* <span data-ttu-id="e62c1-1776">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1776">Added `container exec` command.</span></span> <span data-ttu-id="e62c1-1777">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="e62c1-1777">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="e62c1-1778">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="e62c1-1778">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e62c1-1779">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e62c1-1779">Extension</span></span>

* <span data-ttu-id="e62c1-1780">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="e62c1-1780">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="e62c1-1781">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1781">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="e62c1-1782">[BREAKING CHANGE] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1782">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-1783">Interactive</span><span class="sxs-lookup"><span data-stu-id="e62c1-1783">Interactive</span></span>

* <span data-ttu-id="e62c1-1784">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1784">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="e62c1-1785">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1785">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="e62c1-1786">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="e62c1-1786">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="e62c1-1787">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="e62c1-1787">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="e62c1-1788">Labor</span><span class="sxs-lookup"><span data-stu-id="e62c1-1788">Lab</span></span>

* <span data-ttu-id="e62c1-1789">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1789">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-1790">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1790">Monitor</span></span>

* <span data-ttu-id="e62c1-1791">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="e62c1-1791">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="e62c1-1792">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken</span><span class="sxs-lookup"><span data-stu-id="e62c1-1792">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="e62c1-1793">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="e62c1-1793">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1794">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1794">Network</span></span>

* <span data-ttu-id="e62c1-1795">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1795">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="e62c1-1796">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-1796">Profile</span></span>

* <span data-ttu-id="e62c1-1797">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1797">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e62c1-1798">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1798">RDBMS</span></span>

* <span data-ttu-id="e62c1-1799">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1799">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-1800">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-1800">Resource</span></span>

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="e62c1-1802">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-1802">Role</span></span>

* <span data-ttu-id="e62c1-1803">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1803">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="e62c1-1804">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1804">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="e62c1-1805">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1805">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="e62c1-1806">[BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1806">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="e62c1-1807">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1807">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1808">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1808">Storage</span></span>

* <span data-ttu-id="e62c1-1809">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1809">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="e62c1-1810">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1810">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1811">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1811">VM</span></span>

* <span data-ttu-id="e62c1-1812">Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1812">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="e62c1-1813">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1813">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="e62c1-1814">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1814">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="e62c1-1815">[BREAKING CHANGE] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1815">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="e62c1-1816">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1816">March 13, 2018</span></span>

<span data-ttu-id="e62c1-1817">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="e62c1-1817">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-1818">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-1818">ACR</span></span>

* <span data-ttu-id="e62c1-1819">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1819">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="e62c1-1820">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1820">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="e62c1-1821">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1821">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1822">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1822">ACS</span></span>

* <span data-ttu-id="e62c1-1823">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1823">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="e62c1-1824">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1824">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="e62c1-1825">Advisor</span><span class="sxs-lookup"><span data-stu-id="e62c1-1825">Advisor</span></span>

* <span data-ttu-id="e62c1-1826">[BREAKING CHANGE] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1826">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="e62c1-1827">[BREAKING CHANGE] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1827">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="e62c1-1828">[BREAKING CHANGE] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1828">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="e62c1-1829">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1829">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="e62c1-1830">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1830">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1831">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1831">Appservice</span></span>

* <span data-ttu-id="e62c1-1832">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1832">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="e62c1-1833">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1833">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="e62c1-1834">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="e62c1-1834">Eventhubs</span></span>

* <span data-ttu-id="e62c1-1835">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e62c1-1835">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="e62c1-1836">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e62c1-1836">Extension</span></span>

* <span data-ttu-id="e62c1-1837">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="e62c1-1837">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-1838">Interactive</span><span class="sxs-lookup"><span data-stu-id="e62c1-1838">Interactive</span></span>

* <span data-ttu-id="e62c1-1839">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="e62c1-1839">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="e62c1-1840">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1840">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="e62c1-1841">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-1841">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="e62c1-1842">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1842">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-1843">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1843">Monitor</span></span>

* <span data-ttu-id="e62c1-1844">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1844">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="e62c1-1845">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1845">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="e62c1-1846">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1846">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="e62c1-1847">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1847">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1848">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1848">Network</span></span>

* <span data-ttu-id="e62c1-1849">[BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1849">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="e62c1-1850">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1850">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="e62c1-1851">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1851">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="e62c1-1852">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1852">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="e62c1-1853">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-1853">Profile</span></span>

* <span data-ttu-id="e62c1-1854">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1854">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="e62c1-1855">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1855">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e62c1-1856">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1856">RDBMS</span></span>

* <span data-ttu-id="e62c1-1857">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1857">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="e62c1-1858">Service Bus</span><span class="sxs-lookup"><span data-stu-id="e62c1-1858">Service Bus</span></span>

* <span data-ttu-id="e62c1-1859">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e62c1-1859">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1860">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1860">Storage</span></span>

* <span data-ttu-id="e62c1-1861">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1861">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="e62c1-1862">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus</span><span class="sxs-lookup"><span data-stu-id="e62c1-1862">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1863">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1863">VM</span></span>

* <span data-ttu-id="e62c1-1864">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1864">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="e62c1-1865">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1865">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="e62c1-1866">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1866">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="e62c1-1867">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1867">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="e62c1-1868">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1868">February 27, 2018</span></span>

<span data-ttu-id="e62c1-1869">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="e62c1-1869">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1870">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1870">Core</span></span>

* <span data-ttu-id="e62c1-1871">[#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew</span><span class="sxs-lookup"><span data-stu-id="e62c1-1871">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="e62c1-1872">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1872">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="e62c1-1873">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1873">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1874">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1874">ACS</span></span>

* <span data-ttu-id="e62c1-1875">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1875">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="e62c1-1876">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="e62c1-1876">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="e62c1-1877">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1877">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="e62c1-1878">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1878">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1879">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1879">Appservice</span></span>

* <span data-ttu-id="e62c1-1880">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="e62c1-1880">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="e62c1-1881">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1881">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e62c1-1882">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e62c1-1882">Cognitive Services</span></span>

* <span data-ttu-id="e62c1-1883">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1883">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="e62c1-1884">Nutzung</span><span class="sxs-lookup"><span data-stu-id="e62c1-1884">Consumption</span></span>

* <span data-ttu-id="e62c1-1885">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1885">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="e62c1-1886">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1886">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-1887">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1887">Container</span></span>

* <span data-ttu-id="e62c1-1888">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="e62c1-1888">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1889">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1889">Network</span></span>

* <span data-ttu-id="e62c1-1890">[#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="e62c1-1890">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-1891">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-1891">Resource</span></span>

* <span data-ttu-id="e62c1-1892">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="e62c1-1892">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-1893">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-1893">Role</span></span>

* <span data-ttu-id="e62c1-1894">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1894">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-1895">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-1895">SQL</span></span>

* <span data-ttu-id="e62c1-1896">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="e62c1-1896">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1897">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1897">Storage</span></span>

* <span data-ttu-id="e62c1-1898">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="e62c1-1898">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1899">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1899">VM</span></span>

* <span data-ttu-id="e62c1-1900">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1900">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="e62c1-1901">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1901">February 13, 2018</span></span>

<span data-ttu-id="e62c1-1902">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="e62c1-1902">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1903">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1903">Core</span></span>

* <span data-ttu-id="e62c1-1904">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1904">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1905">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1905">ACS</span></span>

* <span data-ttu-id="e62c1-1906">[BREAKING CHANGE] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1906">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="e62c1-1907">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1907">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="e62c1-1908">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1908">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="e62c1-1909">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1909">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="e62c1-1910">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1910">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="e62c1-1911">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1911">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="e62c1-1912">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="e62c1-1912">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="e62c1-1913">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="e62c1-1913">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1914">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1914">Appservice</span></span>

* <span data-ttu-id="e62c1-1915">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="e62c1-1915">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="e62c1-1916">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1916">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="e62c1-1917">CDN</span><span class="sxs-lookup"><span data-stu-id="e62c1-1917">CDN</span></span>

* <span data-ttu-id="e62c1-1918">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1918">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-1919">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-1919">Container</span></span>

* <span data-ttu-id="e62c1-1920">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1920">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="e62c1-1921">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1921">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e62c1-1922">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e62c1-1922">CosmosDB</span></span>

* <span data-ttu-id="e62c1-1923">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1923">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="e62c1-1924">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e62c1-1924">Extension</span></span>

* <span data-ttu-id="e62c1-1925">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1925">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="e62c1-1926">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1926">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="e62c1-1927">Feedback</span><span class="sxs-lookup"><span data-stu-id="e62c1-1927">Feedback</span></span>

* <span data-ttu-id="e62c1-1928">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1928">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-1929">Interactive</span><span class="sxs-lookup"><span data-stu-id="e62c1-1929">Interactive</span></span>

* <span data-ttu-id="e62c1-1930">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-1930">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="e62c1-1931">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1931">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="e62c1-1932">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-1932">IoT</span></span>

* <span data-ttu-id="e62c1-1933">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1933">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e62c1-1934">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1934">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e62c1-1935">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1935">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="e62c1-1936">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1936">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-1937">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1937">Monitor</span></span>

* <span data-ttu-id="e62c1-1938">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1938">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1939">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1939">Network</span></span>

* <span data-ttu-id="e62c1-1940">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1940">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="e62c1-1941">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-1941">Profile</span></span>

* <span data-ttu-id="e62c1-1942">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1942">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-1943">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-1943">Resource</span></span>

* <span data-ttu-id="e62c1-1944">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1944">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-1945">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-1945">Role</span></span>

* <span data-ttu-id="e62c1-1946">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1946">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-1947">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-1947">SQL</span></span>

* <span data-ttu-id="e62c1-1948">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1948">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="e62c1-1949">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1949">Added `sql db rename`</span></span>
* <span data-ttu-id="e62c1-1950">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1950">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1951">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1951">Storage</span></span>

* <span data-ttu-id="e62c1-1952">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1952">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1953">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1953">VM</span></span>

* <span data-ttu-id="e62c1-1954">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1954">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="e62c1-1955">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1955">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="e62c1-1956">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="e62c1-1956">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="e62c1-1957">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-1957">January 31, 2018</span></span>

<span data-ttu-id="e62c1-1958">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="e62c1-1958">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-1959">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-1959">Core</span></span>

* <span data-ttu-id="e62c1-1960">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1960">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="e62c1-1961">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1961">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="e62c1-1962">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1962">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="e62c1-1963">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-1963">Use `--verbose` to see</span></span>
* <span data-ttu-id="e62c1-1964">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1964">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-1965">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-1965">ACS</span></span>

* <span data-ttu-id="e62c1-1966">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1966">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="e62c1-1967">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1967">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-1968">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-1968">Appservice</span></span>

* <span data-ttu-id="e62c1-1969">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="e62c1-1969">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="e62c1-1970">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1970">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="e62c1-1971">CDN</span><span class="sxs-lookup"><span data-stu-id="e62c1-1971">CDN</span></span>

* <span data-ttu-id="e62c1-1972">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1972">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e62c1-1973">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e62c1-1973">CosmosDB</span></span>

* <span data-ttu-id="e62c1-1974">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1974">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-1975">Interactive</span><span class="sxs-lookup"><span data-stu-id="e62c1-1975">Interactive</span></span>

* <span data-ttu-id="e62c1-1976">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1976">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-1977">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-1977">Network</span></span>

* <span data-ttu-id="e62c1-1978">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1978">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="e62c1-1979">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="e62c1-1979">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="e62c1-1980">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1980">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="e62c1-1981">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1981">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="e62c1-1982">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1982">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="e62c1-1983">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="e62c1-1983">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="e62c1-1984">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1984">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="e62c1-1985">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1985">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="e62c1-1986">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-1986">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="e62c1-1987">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1987">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="e62c1-1988">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-1988">Profile</span></span>

* <span data-ttu-id="e62c1-1989">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-1989">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-1990">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-1990">Resource</span></span>

* <span data-ttu-id="e62c1-1991">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1991">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-1992">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-1992">Storage</span></span>

* <span data-ttu-id="e62c1-1993">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-1993">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="e62c1-1994">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1994">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="e62c1-1995">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="e62c1-1995">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="e62c1-1996">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-1996">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="e62c1-1997">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="e62c1-1997">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-1998">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-1998">VM</span></span>

* <span data-ttu-id="e62c1-1999">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-1999">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="e62c1-2000">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="e62c1-2000">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="e62c1-2001">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2001">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="e62c1-2002">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2002">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="e62c1-2003">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="e62c1-2003">January 17, 2018</span></span>

<span data-ttu-id="e62c1-2004">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="e62c1-2004">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-2005">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-2005">ACR</span></span>

* <span data-ttu-id="e62c1-2006">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2006">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="e62c1-2007">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2007">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-2008">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-2008">ACS</span></span>

* <span data-ttu-id="e62c1-2009">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2009">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="e62c1-2010">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2010">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-2011">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-2011">Appservice</span></span>

* <span data-ttu-id="e62c1-2012">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="e62c1-2012">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="e62c1-2013">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2013">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="e62c1-2014">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2014">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="e62c1-2015">Backup</span><span class="sxs-lookup"><span data-stu-id="e62c1-2015">Backup</span></span>

* <span data-ttu-id="e62c1-2016">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2016">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="e62c1-2017">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2017">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="e62c1-2018">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2018">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="e62c1-2019">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="e62c1-2019">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="e62c1-2020">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2020">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-2021">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-2021">Batch</span></span>

* <span data-ttu-id="e62c1-2022">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2022">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="e62c1-2023">Cloud</span><span class="sxs-lookup"><span data-stu-id="e62c1-2023">Cloud</span></span>

* <span data-ttu-id="e62c1-2024">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2024">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="e62c1-2025">Nutzung</span><span class="sxs-lookup"><span data-stu-id="e62c1-2025">Consumption</span></span>

* <span data-ttu-id="e62c1-2026">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2026">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="e62c1-2027">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e62c1-2027">Event Grid</span></span>

* <span data-ttu-id="e62c1-2028">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2028">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e62c1-2029">[BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2029">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e62c1-2030">[BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2030">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="e62c1-2031">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2031">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="e62c1-2032">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2032">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="e62c1-2033">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2033">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="e62c1-2034">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2034">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="e62c1-2035">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2035">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-2036">Interactive</span><span class="sxs-lookup"><span data-stu-id="e62c1-2036">Interactive</span></span>

* <span data-ttu-id="e62c1-2037">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="e62c1-2037">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="e62c1-2038">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2038">Fixed errors on startup</span></span>
* <span data-ttu-id="e62c1-2039">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="e62c1-2039">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="e62c1-2040">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-2040">IoT</span></span>

* <span data-ttu-id="e62c1-2041">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2041">Added support for device provisioning service</span></span>
* <span data-ttu-id="e62c1-2042">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2042">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="e62c1-2043">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-2043">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-2044">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2044">Monitor</span></span>

* <span data-ttu-id="e62c1-2045">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2045">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="e62c1-2046">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2046">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="e62c1-2047">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2047">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-2048">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-2048">Network</span></span>

* <span data-ttu-id="e62c1-2049">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="e62c1-2049">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="e62c1-2050">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2050">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="e62c1-2051">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-2051">Profile</span></span>

* <span data-ttu-id="e62c1-2052">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2052">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-2053">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-2053">Role</span></span>

* <span data-ttu-id="e62c1-2054">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2054">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e62c1-2055">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e62c1-2055">Service Fabric</span></span>

* <span data-ttu-id="e62c1-2056">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2056">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="e62c1-2057">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2057">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-2058">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2058">VM</span></span>

* <span data-ttu-id="e62c1-2059">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2059">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="e62c1-2060">[BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2060">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="e62c1-2061">[BREAKING CHANGE] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="e62c1-2061">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="e62c1-2062">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2062">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="e62c1-2063">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2063">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="e62c1-2064">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2064">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="e62c1-2065">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2065">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="e62c1-2066">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2066">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="e62c1-2067">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2067">December 19, 2017</span></span>

<span data-ttu-id="e62c1-2068">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="e62c1-2068">Version 2.0.23</span></span>

* <span data-ttu-id="e62c1-2069">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2069">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-2070">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-2070">Container</span></span>

* <span data-ttu-id="e62c1-2071">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2071">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-2072">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-2072">Network</span></span>

* <span data-ttu-id="e62c1-2073">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2073">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="e62c1-2074">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2074">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-2075">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-2075">Storage</span></span>

* <span data-ttu-id="e62c1-2076">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2076">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-2077">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2077">VM</span></span>

* <span data-ttu-id="e62c1-2078">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2078">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="e62c1-2079">5\. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2079">December 5, 2017</span></span>

<span data-ttu-id="e62c1-2080">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="e62c1-2080">Version 2.0.22</span></span>

* <span data-ttu-id="e62c1-2081">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2081">Removed `az component` commands.</span></span> <span data-ttu-id="e62c1-2082">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2082">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-2083">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-2083">Core</span></span>
* <span data-ttu-id="e62c1-2084">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2084">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="e62c1-2085">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-2085">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-2086">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-2086">ACS</span></span>

* <span data-ttu-id="e62c1-2087">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2087">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="e62c1-2088">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2088">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="e62c1-2089">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="e62c1-2089">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="e62c1-2090">Advisor</span><span class="sxs-lookup"><span data-stu-id="e62c1-2090">Advisor</span></span>

* <span data-ttu-id="e62c1-2091">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e62c1-2091">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-2092">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-2092">Appservice</span></span>

* <span data-ttu-id="e62c1-2093">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2093">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="e62c1-2094">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2094">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="e62c1-2095">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2095">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="e62c1-2096">Nutzung</span><span class="sxs-lookup"><span data-stu-id="e62c1-2096">Consumption</span></span>

* <span data-ttu-id="e62c1-2097">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2097">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-2098">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-2098">Container</span></span>

* <span data-ttu-id="e62c1-2099">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="e62c1-2099">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-2100">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2100">Monitor</span></span>

* <span data-ttu-id="e62c1-2101">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2101">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-2102">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-2102">Resource</span></span>

* <span data-ttu-id="e62c1-2103">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2103">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-2104">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-2104">Role</span></span>

* <span data-ttu-id="e62c1-2105">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2105">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="e62c1-2106">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2106">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="e62c1-2107">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2107">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-2108">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-2108">SQL</span></span>

* <span data-ttu-id="e62c1-2109">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2109">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="e62c1-2110">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2110">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-2111">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2111">VM</span></span>

* <span data-ttu-id="e62c1-2112">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2112">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="e62c1-2113">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2113">November 14, 2017</span></span>

<span data-ttu-id="e62c1-2114">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="e62c1-2114">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-2115">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-2115">ACR</span></span>

* <span data-ttu-id="e62c1-2116">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2116">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="e62c1-2117">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-2117">ACS</span></span>

* <span data-ttu-id="e62c1-2118">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2118">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="e62c1-2119">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="e62c1-2119">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="e62c1-2120">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2120">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="e62c1-2121">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2121">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="e62c1-2122">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2122">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-2123">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-2123">Appservice</span></span>

* <span data-ttu-id="e62c1-2124">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2124">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="e62c1-2125">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2125">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="e62c1-2126">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2126">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="e62c1-2127">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2127">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="e62c1-2128">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2128">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="e62c1-2129">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2129">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-2130">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-2130">Batch</span></span>

* <span data-ttu-id="e62c1-2131">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-2131">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="e62c1-2132">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e62c1-2132">Batchai</span></span>

* <span data-ttu-id="e62c1-2133">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2133">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="e62c1-2134">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2134">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="e62c1-2135">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2135">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="e62c1-2136">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2136">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="e62c1-2137">Cloud</span><span class="sxs-lookup"><span data-stu-id="e62c1-2137">Cloud</span></span>

* <span data-ttu-id="e62c1-2138">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="e62c1-2138">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-2139">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-2139">Container</span></span>

* <span data-ttu-id="e62c1-2140">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2140">Added support to open multiple ports</span></span>
* <span data-ttu-id="e62c1-2141">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2141">Added container group restart policy</span></span>
* <span data-ttu-id="e62c1-2142">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2142">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="e62c1-2143">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2143">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e62c1-2144">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e62c1-2144">Data Lake Analytics</span></span>

* <span data-ttu-id="e62c1-2145">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="e62c1-2145">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e62c1-2146">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e62c1-2146">Data Lake Store</span></span>

* <span data-ttu-id="e62c1-2147">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="e62c1-2147">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="e62c1-2148">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e62c1-2148">Extension</span></span>

* <span data-ttu-id="e62c1-2149">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2149">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="e62c1-2150">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2150">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="e62c1-2151">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-2151">IoT</span></span>

* <span data-ttu-id="e62c1-2152">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2152">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-2153">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2153">Monitor</span></span>

* <span data-ttu-id="e62c1-2154">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2154">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-2155">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-2155">Network</span></span>

* <span data-ttu-id="e62c1-2156">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2156">Added support for CAA DNS records</span></span>
* <span data-ttu-id="e62c1-2157">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="e62c1-2157">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="e62c1-2158">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="e62c1-2158">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="e62c1-2159">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-2159">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="e62c1-2160">Reservations</span><span class="sxs-lookup"><span data-stu-id="e62c1-2160">Reservations</span></span>

* <span data-ttu-id="e62c1-2161">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="e62c1-2161">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-2162">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-2162">Resource</span></span>

* <span data-ttu-id="e62c1-2163">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2163">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-2164">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-2164">SQL</span></span>

* <span data-ttu-id="e62c1-2165">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2165">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-2166">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-2166">Storage</span></span>

* <span data-ttu-id="e62c1-2167">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-2167">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="e62c1-2168">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="e62c1-2168">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="e62c1-2169">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="e62c1-2169">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="e62c1-2170">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2170">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="e62c1-2171">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2171">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="e62c1-2172">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2172">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="e62c1-2173">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-2173">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-2174">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2174">VM</span></span>

* <span data-ttu-id="e62c1-2175">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="e62c1-2175">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="e62c1-2176">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2176">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="e62c1-2177">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="e62c1-2177">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="e62c1-2178">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2178">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="e62c1-2179">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2179">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="e62c1-2180">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2180">October 24, 2017</span></span>

<span data-ttu-id="e62c1-2181">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="e62c1-2181">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-2182">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-2182">Core</span></span>

* <span data-ttu-id="e62c1-2183">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="e62c1-2183">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-2184">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-2184">ACR</span></span>

* <span data-ttu-id="e62c1-2185">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2185">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="e62c1-2186">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2186">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="e62c1-2187">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2187">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-2188">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-2188">ACS</span></span>

* <span data-ttu-id="e62c1-2189">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2189">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="e62c1-2190">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2190">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-2191">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-2191">Appservice</span></span>

* <span data-ttu-id="e62c1-2192">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="e62c1-2192">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="e62c1-2193">Komponente</span><span class="sxs-lookup"><span data-stu-id="e62c1-2193">Component</span></span>

* <span data-ttu-id="e62c1-2194">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2194">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-2195">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2195">Monitor</span></span>

* <span data-ttu-id="e62c1-2196">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2196">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-2197">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-2197">Resource</span></span>

* <span data-ttu-id="e62c1-2198">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2198">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="e62c1-2199">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="e62c1-2199">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-2200">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2200">VM</span></span>

* <span data-ttu-id="e62c1-2201">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2201">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="e62c1-2202">9\. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2202">October 9, 2017</span></span>

<span data-ttu-id="e62c1-2203">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="e62c1-2203">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-2204">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-2204">Core</span></span>

* <span data-ttu-id="e62c1-2205">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2205">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-2206">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-2206">Appservice</span></span>

* <span data-ttu-id="e62c1-2207">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2207">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-2208">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-2208">Batch</span></span>

* <span data-ttu-id="e62c1-2209">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="e62c1-2209">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="e62c1-2210">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2210">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="e62c1-2211">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2211">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="e62c1-2212">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2212">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="e62c1-2213">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e62c1-2213">Batchai</span></span>

* <span data-ttu-id="e62c1-2214">Erste Version des Batch KI-Moduls</span><span class="sxs-lookup"><span data-stu-id="e62c1-2214">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e62c1-2215">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e62c1-2215">Keyvault</span></span>

* <span data-ttu-id="e62c1-2216">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2216">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="e62c1-2217">(#4448)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2217">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="e62c1-2218">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-2218">Network</span></span>

* <span data-ttu-id="e62c1-2219">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2219">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="e62c1-2220">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2220">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-2221">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-2221">Resource</span></span>

* <span data-ttu-id="e62c1-2222">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2222">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="e62c1-2223">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2223">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="e62c1-2224">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2224">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="e62c1-2225">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2225">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-2226">Sql</span><span class="sxs-lookup"><span data-stu-id="e62c1-2226">Sql</span></span>

* <span data-ttu-id="e62c1-2227">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2227">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="e62c1-2228">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2228">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="e62c1-2229">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2229">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-2230">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-2230">Storage</span></span>

* <span data-ttu-id="e62c1-2231">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2231">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-2232">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2232">Vm</span></span>

* <span data-ttu-id="e62c1-2233">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="e62c1-2233">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="e62c1-2234">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2234">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="e62c1-2235">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2235">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="e62c1-2236">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2236">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="e62c1-2237">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2237">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="e62c1-2238">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2238">September 22, 2017</span></span>

<span data-ttu-id="e62c1-2239">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="e62c1-2239">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-2240">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-2240">Resource</span></span>

* <span data-ttu-id="e62c1-2241">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2241">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="e62c1-2242">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2242">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="e62c1-2243">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2243">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="e62c1-2244">[BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2244">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-2245">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-2245">Network</span></span>

* <span data-ttu-id="e62c1-2246">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2246">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="e62c1-2247">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2247">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="e62c1-2248">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2248">Added `asg` application security group commands</span></span>
* <span data-ttu-id="e62c1-2249">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2249">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="e62c1-2250">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2250">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e62c1-2251">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2251">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="e62c1-2252">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2252">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-2253">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-2253">Storage</span></span>

* <span data-ttu-id="e62c1-2254">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="e62c1-2254">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e62c1-2255">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="e62c1-2255">Eventgrid</span></span>

* <span data-ttu-id="e62c1-2256">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2256">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-2257">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-2257">SQL</span></span>

* <span data-ttu-id="e62c1-2258">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2258">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="e62c1-2259">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2259">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="e62c1-2260">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2260">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="e62c1-2261">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e62c1-2261">Keyvault</span></span>

* <span data-ttu-id="e62c1-2262">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2262">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-2263">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2263">VM</span></span>

* <span data-ttu-id="e62c1-2264">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2264">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="e62c1-2265">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="e62c1-2265">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="e62c1-2266">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2266">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="e62c1-2267">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2267">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="e62c1-2268">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2268">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="e62c1-2269">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2269">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-2270">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-2270">ACS</span></span>

* <span data-ttu-id="e62c1-2271">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2271">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-2272">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-2272">Appservice</span></span>

* <span data-ttu-id="e62c1-2273">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2273">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e62c1-2274">Backup</span><span class="sxs-lookup"><span data-stu-id="e62c1-2274">Backup</span></span>

* <span data-ttu-id="e62c1-2275">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="e62c1-2275">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="e62c1-2276">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2276">September 11, 2017</span></span>

<span data-ttu-id="e62c1-2277">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="e62c1-2277">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="e62c1-2278">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-2278">Core</span></span>

* <span data-ttu-id="e62c1-2279">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2279">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="e62c1-2280">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="e62c1-2280">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-2281">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-2281">Acs</span></span>

* <span data-ttu-id="e62c1-2282">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2282">Added `acs list-locations` command</span></span>
* <span data-ttu-id="e62c1-2283">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2283">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-2284">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-2284">Appservice</span></span>

* <span data-ttu-id="e62c1-2285">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="e62c1-2285">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="e62c1-2286">CDN</span><span class="sxs-lookup"><span data-stu-id="e62c1-2286">CDN</span></span>

* <span data-ttu-id="e62c1-2287">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2287">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="e62c1-2288">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="e62c1-2288">Extension</span></span>

* <span data-ttu-id="e62c1-2289">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e62c1-2289">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="e62c1-2290">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e62c1-2290">Keyvault</span></span>

* <span data-ttu-id="e62c1-2291">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="e62c1-2291">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-2292">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-2292">Network</span></span>

* <span data-ttu-id="e62c1-2293">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2293">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e62c1-2294">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2294">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="e62c1-2295">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2295">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="e62c1-2296">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2296">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e62c1-2297">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2297">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-2298">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-2298">Resource</span></span>

* <span data-ttu-id="e62c1-2299">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2299">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="e62c1-2300">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2300">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="e62c1-2301">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2301">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="e62c1-2302">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="e62c1-2302">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-2303">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-2303">SQL</span></span>

* <span data-ttu-id="e62c1-2304">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2304">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-2305">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2305">VM</span></span>

* <span data-ttu-id="e62c1-2306">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-2306">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="e62c1-2307">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="e62c1-2307">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="e62c1-2308">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2308">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="e62c1-2309">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2309">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="e62c1-2310">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2310">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="e62c1-2311">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2311">August 31, 2017</span></span>

<span data-ttu-id="e62c1-2312">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="e62c1-2312">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="e62c1-2313">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e62c1-2313">Keyvault</span></span>

* <span data-ttu-id="e62c1-2314">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2314">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="e62c1-2315">Sf</span><span class="sxs-lookup"><span data-stu-id="e62c1-2315">Sf</span></span>

* <span data-ttu-id="e62c1-2316">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2316">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-2317">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-2317">Storage</span></span>

* <span data-ttu-id="e62c1-2318">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2318">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="e62c1-2319">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="e62c1-2319">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="e62c1-2320">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2320">August 28, 2017</span></span>

<span data-ttu-id="e62c1-2321">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="e62c1-2321">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="e62c1-2322">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2322">CLI</span></span>

* <span data-ttu-id="e62c1-2323">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2323">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-2324">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-2324">ACS</span></span>

* <span data-ttu-id="e62c1-2325">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2325">Corrected preview regions</span></span>
* <span data-ttu-id="e62c1-2326">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2326">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="e62c1-2327">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2327">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-2328">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-2328">Appservice</span></span>

* <span data-ttu-id="e62c1-2329">[BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2329">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="e62c1-2330">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2330">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="e62c1-2331">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="e62c1-2331">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="e62c1-2332">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="e62c1-2332">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="e62c1-2333">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2333">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="e62c1-2334">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-2334">IoT</span></span>

* <span data-ttu-id="e62c1-2335">#3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="e62c1-2335">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-2336">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-2336">Network</span></span>

* <span data-ttu-id="e62c1-2337">[BREAKING CHANGE] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2337">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e62c1-2338">[BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2338">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="e62c1-2339">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2339">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e62c1-2340">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2340">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e62c1-2341">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2341">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="e62c1-2342">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-2342">Profile</span></span>

* <span data-ttu-id="e62c1-2343">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="e62c1-2343">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e62c1-2344">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e62c1-2344">Service Fabric</span></span>

* <span data-ttu-id="e62c1-2345">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="e62c1-2345">Preview release</span></span>
* <span data-ttu-id="e62c1-2346">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="e62c1-2346">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="e62c1-2347">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2347">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="e62c1-2348">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2348">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-2349">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-2349">Storage</span></span>

* <span data-ttu-id="e62c1-2350">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="e62c1-2350">Enabled setting blob tier</span></span>
* <span data-ttu-id="e62c1-2351">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2351">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="e62c1-2352">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2352">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="e62c1-2353">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="e62c1-2353">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="e62c1-2354">[BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2354">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="e62c1-2355">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2355">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-2356">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2356">VM</span></span>

* <span data-ttu-id="e62c1-2357">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-2357">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="e62c1-2358">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-2358">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="e62c1-2359">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2359">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="e62c1-2360">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="e62c1-2360">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="e62c1-2361">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2361">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="e62c1-2362">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="e62c1-2362">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="e62c1-2363">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2363">August 15, 2017</span></span>

<span data-ttu-id="e62c1-2364">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="e62c1-2364">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-2365">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-2365">ACS</span></span>

* <span data-ttu-id="e62c1-2366">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2366">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-2367">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-2367">Appservice</span></span>

* <span data-ttu-id="e62c1-2368">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2368">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="e62c1-2369">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e62c1-2369">Event Grid</span></span>

* <span data-ttu-id="e62c1-2370">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2370">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="e62c1-2371">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2371">August 11, 2017</span></span>

<span data-ttu-id="e62c1-2372">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="e62c1-2372">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-2373">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-2373">ACS</span></span>

* <span data-ttu-id="e62c1-2374">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2374">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-2375">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-2375">Batch</span></span>

* <span data-ttu-id="e62c1-2376">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2376">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="e62c1-2377">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2377">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="e62c1-2378">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2378">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="e62c1-2379">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="e62c1-2379">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="e62c1-2380">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="e62c1-2380">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="e62c1-2381">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2381">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="e62c1-2382">Komponente</span><span class="sxs-lookup"><span data-stu-id="e62c1-2382">Component</span></span>

* <span data-ttu-id="e62c1-2383">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2383">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="e62c1-2384">Container</span><span class="sxs-lookup"><span data-stu-id="e62c1-2384">Container</span></span>

* <span data-ttu-id="e62c1-2385">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="e62c1-2385">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="e62c1-2386">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e62c1-2386">Data Lake Store</span></span>

* <span data-ttu-id="e62c1-2387">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="e62c1-2387">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="e62c1-2388">Event Grid</span><span class="sxs-lookup"><span data-stu-id="e62c1-2388">Event Grid</span></span>

* <span data-ttu-id="e62c1-2389">Erste Version</span><span class="sxs-lookup"><span data-stu-id="e62c1-2389">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-2390">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-2390">Network</span></span>

* <span data-ttu-id="e62c1-2391">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-2391">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="e62c1-2392">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-2392">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="e62c1-2393">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="e62c1-2393">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="e62c1-2394">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2394">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="e62c1-2395">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-2395">Profile</span></span>

* <span data-ttu-id="e62c1-2396">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="e62c1-2396">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-2397">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-2397">Storage</span></span>

* <span data-ttu-id="e62c1-2398">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="e62c1-2398">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-2399">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2399">VM</span></span>

* <span data-ttu-id="e62c1-2400">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="e62c1-2400">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="e62c1-2401">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="e62c1-2401">Exposed `list-skus` command</span></span>
* <span data-ttu-id="e62c1-2402">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2402">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="e62c1-2403">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="e62c1-2403">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="e62c1-2404">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2404">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="e62c1-2405">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2405">July 28, 2017</span></span>

<span data-ttu-id="e62c1-2406">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="e62c1-2406">Version 2.0.12</span></span>

* <span data-ttu-id="e62c1-2407">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2407">Added container commands</span></span>
* <span data-ttu-id="e62c1-2408">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2408">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="e62c1-2409">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-2409">Core</span></span>

* <span data-ttu-id="e62c1-2410">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="e62c1-2410">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="e62c1-2411">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2411">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="e62c1-2412">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="e62c1-2412">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="e62c1-2413">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2413">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="e62c1-2414">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="e62c1-2414">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="e62c1-2415">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2415">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="e62c1-2416">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2416">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e62c1-2417">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2417">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="e62c1-2418">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2418">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="e62c1-2419">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-2419">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="e62c1-2420">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="e62c1-2420">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="e62c1-2421">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2421">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="e62c1-2422">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2422">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="e62c1-2423">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2423">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="e62c1-2424">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e62c1-2424">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="e62c1-2425">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2425">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="e62c1-2426">ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-2426">ACR</span></span>

* <span data-ttu-id="e62c1-2427">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2427">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="e62c1-2428">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2428">Support SKU update for managed registries</span></span>
* <span data-ttu-id="e62c1-2429">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2429">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="e62c1-2430">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2430">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="e62c1-2431">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2431">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="e62c1-2432">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2432">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-2433">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-2433">ACS</span></span>

* <span data-ttu-id="e62c1-2434">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="e62c1-2434">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-2435">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-2435">Appservice</span></span>

* <span data-ttu-id="e62c1-2436">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="e62c1-2436">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="e62c1-2437">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="e62c1-2437">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="e62c1-2438">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2438">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="e62c1-2439">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2439">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="e62c1-2440">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2440">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="e62c1-2441">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2441">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="e62c1-2442">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2442">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="e62c1-2443">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2443">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="e62c1-2444">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2444">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="e62c1-2445">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2445">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="e62c1-2446">Batch</span><span class="sxs-lookup"><span data-stu-id="e62c1-2446">Batch</span></span>

* <span data-ttu-id="e62c1-2447">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2447">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="e62c1-2448">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2448">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="e62c1-2449">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2449">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="e62c1-2450">CDN</span><span class="sxs-lookup"><span data-stu-id="e62c1-2450">CDN</span></span>

* <span data-ttu-id="e62c1-2451">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-2451">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="e62c1-2452">Cloud</span><span class="sxs-lookup"><span data-stu-id="e62c1-2452">Cloud</span></span>

* <span data-ttu-id="e62c1-2453">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2453">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="e62c1-2454">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="e62c1-2454">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="e62c1-2455">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2455">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="e62c1-2456">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="e62c1-2456">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="e62c1-2457">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="e62c1-2457">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e62c1-2458">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e62c1-2458">CosmosDB</span></span>

* <span data-ttu-id="e62c1-2459">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2459">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="e62c1-2460">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2460">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e62c1-2461">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e62c1-2461">Data Lake Analytics</span></span>

* <span data-ttu-id="e62c1-2462">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2462">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="e62c1-2463">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2463">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="e62c1-2464">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2464">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e62c1-2465">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e62c1-2465">Data Lake Store</span></span>

* <span data-ttu-id="e62c1-2466">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2466">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="e62c1-2467">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="e62c1-2467">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="e62c1-2468">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2468">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="e62c1-2469">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2469">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="e62c1-2470">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="e62c1-2470">Interactive</span></span>

* <span data-ttu-id="e62c1-2471">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2471">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="e62c1-2472">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2472">Increased test coverage</span></span>
* <span data-ttu-id="e62c1-2473">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-2473">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="e62c1-2474">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2474">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="e62c1-2475">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2475">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="e62c1-2476">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2476">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="e62c1-2477">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2477">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e62c1-2478">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2478">Added `--progress` flag</span></span>
* <span data-ttu-id="e62c1-2479">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2479">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="e62c1-2480">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2480">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="e62c1-2481">IoT</span><span class="sxs-lookup"><span data-stu-id="e62c1-2481">IoT</span></span>

* <span data-ttu-id="e62c1-2482">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="e62c1-2482">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="e62c1-2483">(3934)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2483">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="e62c1-2484">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="e62c1-2484">Key vault</span></span>

* <span data-ttu-id="e62c1-2485">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="e62c1-2485">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="e62c1-2486">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2486">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="e62c1-2487">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2487">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e62c1-2488">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2488">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e62c1-2489">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2489">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="e62c1-2490">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2490">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="e62c1-2491">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2491">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="e62c1-2492">(3307)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2492">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="e62c1-2493">Labor</span><span class="sxs-lookup"><span data-stu-id="e62c1-2493">Lab</span></span>

* <span data-ttu-id="e62c1-2494">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2494">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="e62c1-2495">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2495">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-2496">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2496">Monitor</span></span>

* <span data-ttu-id="e62c1-2497">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2497">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="e62c1-2498">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2498">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="e62c1-2499">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2499">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="e62c1-2500">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2500">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="e62c1-2501">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2501">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="e62c1-2502">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="e62c1-2502">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="e62c1-2503">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2503">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="e62c1-2504">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="e62c1-2504">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="e62c1-2505">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="e62c1-2505">`location` no longer required</span></span>
  * <span data-ttu-id="e62c1-2506">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="e62c1-2506">Add name and ID support for target</span></span>
  * <span data-ttu-id="e62c1-2507">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2507">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="e62c1-2508">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2508">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="e62c1-2509">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2509">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="e62c1-2510">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="e62c1-2510">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="e62c1-2511">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2511">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="e62c1-2512">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2512">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-2513">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-2513">Network</span></span>

* <span data-ttu-id="e62c1-2514">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2514">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="e62c1-2515">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2515">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="e62c1-2516">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="e62c1-2516">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="e62c1-2517">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="e62c1-2517">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="e62c1-2518">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-2518">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="e62c1-2519">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2519">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="e62c1-2520">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2520">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="e62c1-2521">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2521">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="e62c1-2522">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2522">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="e62c1-2523">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2523">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="e62c1-2524">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2524">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="e62c1-2525">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2525">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="e62c1-2526">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2526">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="e62c1-2527">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2527">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="e62c1-2528">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2528">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="e62c1-2529">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2529">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="e62c1-2530">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers</span><span class="sxs-lookup"><span data-stu-id="e62c1-2530">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="e62c1-2531">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-2531">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="e62c1-2532">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2532">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="e62c1-2533">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2533">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="e62c1-2534">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="e62c1-2534">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="e62c1-2535">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2535">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="e62c1-2536">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2536">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="e62c1-2537">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2537">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="e62c1-2538">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2538">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="e62c1-2539">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2539">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="e62c1-2540">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2540">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="e62c1-2541">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-2541">Profile</span></span>

* <span data-ttu-id="e62c1-2542">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="e62c1-2542">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="e62c1-2543">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="e62c1-2543">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="e62c1-2544">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="e62c1-2544">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="e62c1-2545">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2545">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="e62c1-2546">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="e62c1-2546">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="e62c1-2547">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e62c1-2547">RDBMS</span></span>

* <span data-ttu-id="e62c1-2548">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2548">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="e62c1-2549">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2549">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="e62c1-2550">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2550">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="e62c1-2551">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2551">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-2552">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-2552">Resource</span></span>

* <span data-ttu-id="e62c1-2553">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2553">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="e62c1-2554">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="e62c1-2554">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="e62c1-2555">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-2555">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="e62c1-2556">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2556">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="e62c1-2557">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2557">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="e62c1-2558">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-2558">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="e62c1-2559">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2559">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="e62c1-2560">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2560">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-2561">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-2561">Role</span></span>

* <span data-ttu-id="e62c1-2562">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2562">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="e62c1-2563">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2563">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="e62c1-2564">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="e62c1-2564">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="e62c1-2565">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2565">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="e62c1-2566">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2566">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e62c1-2567">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e62c1-2567">Service Fabric</span></span>
* <span data-ttu-id="e62c1-2568">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2568">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="e62c1-2569">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2569">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="e62c1-2570">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2570">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-2571">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-2571">SQL</span></span>

* <span data-ttu-id="e62c1-2572">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2572">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="e62c1-2573">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2573">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="e62c1-2574">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2574">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-2575">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-2575">Storage</span></span>

* <span data-ttu-id="e62c1-2576">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2576">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="e62c1-2577">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="e62c1-2577">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="e62c1-2578">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2578">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="e62c1-2579">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2579">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="e62c1-2580">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2580">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="e62c1-2581">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2581">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-2582">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2582">VM</span></span>

* <span data-ttu-id="e62c1-2583">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="e62c1-2583">Support configuring nsg</span></span>
* <span data-ttu-id="e62c1-2584">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-2584">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="e62c1-2585">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="e62c1-2585">Support managed service identities</span></span>
* <span data-ttu-id="e62c1-2586">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="e62c1-2586">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="e62c1-2587">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2587">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="e62c1-2588">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2588">May 10, 2017</span></span>

<span data-ttu-id="e62c1-2589">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="e62c1-2589">Version 2.0.6</span></span>

* <span data-ttu-id="e62c1-2590">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="e62c1-2590">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="e62c1-2591">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2591">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="e62c1-2592">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="e62c1-2592">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="e62c1-2593">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="e62c1-2593">Include Cognitive Services module</span></span>
* <span data-ttu-id="e62c1-2594">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="e62c1-2594">Include Service Fabric module</span></span>
* <span data-ttu-id="e62c1-2595">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2595">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="e62c1-2596">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="e62c1-2596">Add support for CDN commands</span></span>
* <span data-ttu-id="e62c1-2597">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="e62c1-2597">Remove Container module</span></span>
* <span data-ttu-id="e62c1-2598">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2598">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="e62c1-2599">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2599">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="e62c1-2600">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-2600">Core</span></span>

* <span data-ttu-id="e62c1-2601">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="e62c1-2601">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="e62c1-2602">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2602">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="e62c1-2603">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2603">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="e62c1-2604">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2604">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="e62c1-2605">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2605">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="e62c1-2606">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2606">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="e62c1-2607">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2607">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="e62c1-2608">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2608">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="e62c1-2609">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2609">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="e62c1-2610">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="e62c1-2610">core: Improved performance</span></span>
* <span data-ttu-id="e62c1-2611">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2611">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="e62c1-2612">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-2612">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-2613">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-2613">ACS</span></span>

* <span data-ttu-id="e62c1-2614">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e62c1-2614">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="e62c1-2615">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="e62c1-2615">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="e62c1-2616">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2616">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="e62c1-2617">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2617">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-2618">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-2618">AppService</span></span>

* <span data-ttu-id="e62c1-2619">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2619">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="e62c1-2620">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="e62c1-2620">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="e62c1-2621">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2621">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="e62c1-2622">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="e62c1-2622">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="e62c1-2623">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="e62c1-2623">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="e62c1-2624">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2624">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="e62c1-2625">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="e62c1-2625">support slot swap with preview</span></span>
* <span data-ttu-id="e62c1-2626">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2626">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="e62c1-2627">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2627">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e62c1-2628">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e62c1-2628">CosmosDB</span></span>

* <span data-ttu-id="e62c1-2629">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="e62c1-2629">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="e62c1-2630">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="e62c1-2630">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="e62c1-2631">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="e62c1-2631">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="e62c1-2632">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="e62c1-2632">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e62c1-2633">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e62c1-2633">Data Lake Analytics</span></span>

* <span data-ttu-id="e62c1-2634">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="e62c1-2634">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="e62c1-2635">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="e62c1-2635">Add support for new catalog item type: package.</span></span> <span data-ttu-id="e62c1-2636">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2636">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="e62c1-2637">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="e62c1-2637">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="e62c1-2638">Table</span><span class="sxs-lookup"><span data-stu-id="e62c1-2638">Table</span></span>
  * <span data-ttu-id="e62c1-2639">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="e62c1-2639">Table valued function</span></span>
  * <span data-ttu-id="e62c1-2640">Sicht</span><span class="sxs-lookup"><span data-stu-id="e62c1-2640">View</span></span>
  * <span data-ttu-id="e62c1-2641">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2641">Table Statistics.</span></span> <span data-ttu-id="e62c1-2642">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2642">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e62c1-2643">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e62c1-2643">Data Lake Store</span></span>

* <span data-ttu-id="e62c1-2644">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-2644">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="e62c1-2645">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2645">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="e62c1-2646">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="e62c1-2646">missed help for access show.</span></span> <span data-ttu-id="e62c1-2647">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="e62c1-2647">adding it.</span></span> <span data-ttu-id="e62c1-2648">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2648">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="e62c1-2649">Suchen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2649">Find</span></span>

* <span data-ttu-id="e62c1-2650">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="e62c1-2650">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="e62c1-2651">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e62c1-2651">KeyVault</span></span>

* <span data-ttu-id="e62c1-2652">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2652">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="e62c1-2653">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="e62c1-2653">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="e62c1-2654">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="e62c1-2654">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="e62c1-2655">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="e62c1-2655">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="e62c1-2656">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2656">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="e62c1-2657">Labor</span><span class="sxs-lookup"><span data-stu-id="e62c1-2657">Lab</span></span>

* <span data-ttu-id="e62c1-2658">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="e62c1-2658">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="e62c1-2659">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="e62c1-2659">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="e62c1-2660">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="e62c1-2660">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="e62c1-2661">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="e62c1-2661">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="e62c1-2662">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="e62c1-2662">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="e62c1-2663">Überwachen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2663">Monitor</span></span>

* <span data-ttu-id="e62c1-2664">Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2664">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="e62c1-2665">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2665">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="e62c1-2666">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-2666">Network</span></span>

* <span data-ttu-id="e62c1-2667">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="e62c1-2667">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="e62c1-2668">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2668">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="e62c1-2669">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="e62c1-2669">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="e62c1-2670">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2670">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="e62c1-2671">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="e62c1-2671">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="e62c1-2672">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="e62c1-2672">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="e62c1-2673">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2673">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="e62c1-2674">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2674">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="e62c1-2675">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2675">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="e62c1-2676">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="e62c1-2676">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="e62c1-2677">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2677">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="e62c1-2678">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2678">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="e62c1-2679">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="e62c1-2679">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="e62c1-2680">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="e62c1-2680">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="e62c1-2681">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="e62c1-2681">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="e62c1-2682">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2682">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="e62c1-2683">Profil</span><span class="sxs-lookup"><span data-stu-id="e62c1-2683">Profile</span></span>

* <span data-ttu-id="e62c1-2684">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2684">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="e62c1-2685">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2685">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="e62c1-2686">Redis</span><span class="sxs-lookup"><span data-stu-id="e62c1-2686">Redis</span></span>

* <span data-ttu-id="e62c1-2687">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-2687">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="e62c1-2688">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="e62c1-2688">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="e62c1-2689">Resource</span><span class="sxs-lookup"><span data-stu-id="e62c1-2689">Resource</span></span>

* <span data-ttu-id="e62c1-2690">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2690">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="e62c1-2691">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2691">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="e62c1-2692">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2692">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="e62c1-2693">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="e62c1-2693">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="e62c1-2694">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2694">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="e62c1-2695">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="e62c1-2695">Add docs for az lock update.</span></span> <span data-ttu-id="e62c1-2696">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2696">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="e62c1-2697">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="e62c1-2697">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="e62c1-2698">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2698">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="e62c1-2699">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="e62c1-2699">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="e62c1-2700">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2700">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="e62c1-2701">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2701">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="e62c1-2702">Role</span><span class="sxs-lookup"><span data-stu-id="e62c1-2702">Role</span></span>

* <span data-ttu-id="e62c1-2703">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2703">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="e62c1-2704">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2704">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="e62c1-2705">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2705">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="e62c1-2706">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="e62c1-2706">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="e62c1-2707">SQL</span><span class="sxs-lookup"><span data-stu-id="e62c1-2707">SQL</span></span>

* <span data-ttu-id="e62c1-2708">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="e62c1-2708">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="e62c1-2709">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2709">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="e62c1-2710">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-2710">Storage</span></span>

* <span data-ttu-id="e62c1-2711">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2711">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="e62c1-2712">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="e62c1-2712">Add support for incremental blob copy</span></span>
* <span data-ttu-id="e62c1-2713">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="e62c1-2713">Add support for large block blob upload</span></span>
* <span data-ttu-id="e62c1-2714">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="e62c1-2714">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-2715">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2715">VM</span></span>

* <span data-ttu-id="e62c1-2716">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="e62c1-2716">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="e62c1-2717">Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="e62c1-2717">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="e62c1-2718">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="e62c1-2718">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="e62c1-2719">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="e62c1-2719">az vm/vmss disk</span></span>
  3. <span data-ttu-id="e62c1-2720">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2720">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="e62c1-2721">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="e62c1-2721">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="e62c1-2722">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2722">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="e62c1-2723">3\. April 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2723">April 3, 2017</span></span>

<span data-ttu-id="e62c1-2724">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="e62c1-2724">Version 2.0.2</span></span>

<span data-ttu-id="e62c1-2725">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2725">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="e62c1-2726">Core</span><span class="sxs-lookup"><span data-stu-id="e62c1-2726">Core</span></span>

* <span data-ttu-id="e62c1-2727">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="e62c1-2727">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="e62c1-2728">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2728">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="e62c1-2729">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2729">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="e62c1-2730">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2730">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e62c1-2731">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2731">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="e62c1-2732">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="e62c1-2732">Add prompting for missing template parameters.</span></span> <span data-ttu-id="e62c1-2733">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2733">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="e62c1-2734">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2734">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="e62c1-2735">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="e62c1-2735">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="e62c1-2736">ACS</span><span class="sxs-lookup"><span data-stu-id="e62c1-2736">ACS</span></span>

* <span data-ttu-id="e62c1-2737">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2737">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="e62c1-2738">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="e62c1-2738">Add support for ssh key password prompting.</span></span> <span data-ttu-id="e62c1-2739">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2739">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="e62c1-2740">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="e62c1-2740">Add support for windows clusters.</span></span> <span data-ttu-id="e62c1-2741">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2741">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="e62c1-2742">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="e62c1-2742">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="e62c1-2743">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2743">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="e62c1-2744">AppService</span><span class="sxs-lookup"><span data-stu-id="e62c1-2744">AppService</span></span>

* <span data-ttu-id="e62c1-2745">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2745">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="e62c1-2746">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2746">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="e62c1-2747">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2747">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="e62c1-2748">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2748">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="e62c1-2749">DataLake</span><span class="sxs-lookup"><span data-stu-id="e62c1-2749">DataLake</span></span>

* <span data-ttu-id="e62c1-2750">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="e62c1-2750">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="e62c1-2751">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="e62c1-2751">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="e62c1-2752">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="e62c1-2752">DocuemntDB</span></span>

* <span data-ttu-id="e62c1-2753">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2753">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="e62c1-2754">VM</span><span class="sxs-lookup"><span data-stu-id="e62c1-2754">VM</span></span>

* <span data-ttu-id="e62c1-2755">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2755">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="e62c1-2756">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2756">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="e62c1-2757">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2757">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="e62c1-2758">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2758">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e62c1-2759">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2759">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="e62c1-2760">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2760">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="e62c1-2761">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="e62c1-2761">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="e62c1-2762">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="e62c1-2762">February 27, 2017</span></span>

<span data-ttu-id="e62c1-2763">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="e62c1-2763">Version 2.0.0</span></span>

<span data-ttu-id="e62c1-2764">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="e62c1-2764">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="e62c1-2765">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2765">Container Service (acs)</span></span>
- <span data-ttu-id="e62c1-2766">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2766">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="e62c1-2767">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="e62c1-2767">Networking</span></span>
- <span data-ttu-id="e62c1-2768">Storage</span><span class="sxs-lookup"><span data-stu-id="e62c1-2768">Storage</span></span>

<span data-ttu-id="e62c1-2769">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2769">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="e62c1-2770">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2770">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="e62c1-2771">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2771">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="e62c1-2772">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="e62c1-2772">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="e62c1-2773">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="e62c1-2773">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="e62c1-2774">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="e62c1-2774">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="e62c1-2775">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2775">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="e62c1-2776">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="e62c1-2776">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="e62c1-2777">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="e62c1-2777">Provide feedback from the command line with the `az feedback` command</span></span>


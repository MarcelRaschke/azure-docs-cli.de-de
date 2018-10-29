---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/23/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 65e34ab6014c47ae92a6d4bae8cdc30d4a1413dc
ms.sourcegitcommit: aec89531c938781b4724f43b5bb4b878e106a26a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/23/2018
ms.locfileid: "49952484"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="60bb3-103">Versionshinweise für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="60bb3-103">Azure CLI release notes</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="60bb3-104">23. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-104">October 23, 2018</span></span>

<span data-ttu-id="60bb3-105">Version 2.0.49</span><span class="sxs-lookup"><span data-stu-id="60bb3-105">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-106">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-106">Core</span></span>
* <span data-ttu-id="60bb3-107">Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte</span><span class="sxs-lookup"><span data-stu-id="60bb3-107">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="60bb3-108">Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden</span><span class="sxs-lookup"><span data-stu-id="60bb3-108">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-109">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-109">ACR</span></span>
* <span data-ttu-id="60bb3-110">Problem mit der ACR Build-Codierung in Python2 behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-110">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="60bb3-111">CDN</span><span class="sxs-lookup"><span data-stu-id="60bb3-111">CDN</span></span>
* <span data-ttu-id="60bb3-112">[WICHTIGE ÄNDERUNG] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist.</span><span class="sxs-lookup"><span data-stu-id="60bb3-112">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="60bb3-113">Er wird jetzt vom Dienst festgelegt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-113">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-114">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-114">Container</span></span>
* <span data-ttu-id="60bb3-115">`Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-115">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="60bb3-116">Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-116">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="60bb3-117">Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="60bb3-117">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="60bb3-118">`--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen</span><span class="sxs-lookup"><span data-stu-id="60bb3-118">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="60bb3-119">`--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen</span><span class="sxs-lookup"><span data-stu-id="60bb3-119">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="60bb3-120">Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-120">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="60bb3-121">Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-121">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="60bb3-122">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="60bb3-122">CosmosDB</span></span>
* <span data-ttu-id="60bb3-123">Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-123">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="60bb3-124">Interactive</span><span class="sxs-lookup"><span data-stu-id="60bb3-124">Interactive</span></span>
* <span data-ttu-id="60bb3-125">Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-125">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="60bb3-126">IoT Central</span><span class="sxs-lookup"><span data-stu-id="60bb3-126">IoT Central</span></span>
* <span data-ttu-id="60bb3-127">Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-127">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="60bb3-128">[WICHTIGE ÄNDERUNG] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="60bb3-128">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="60bb3-129">Überwachen</span><span class="sxs-lookup"><span data-stu-id="60bb3-129">Monitor</span></span>
* <span data-ttu-id="60bb3-130">Änderungen an `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="60bb3-130">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="60bb3-131">Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-131">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="60bb3-132">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-132">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="60bb3-133">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="60bb3-133">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="60bb3-134">`--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-134">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="60bb3-135">`--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="60bb3-135">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="60bb3-136">Änderungen an `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="60bb3-136">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="60bb3-137">`--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-137">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="60bb3-138">Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="60bb3-138">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="60bb3-139">Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-139">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-140">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-140">Network</span></span>
* <span data-ttu-id="60bb3-141">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="60bb3-141">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="60bb3-142">`--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="60bb3-142">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="60bb3-143">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="60bb3-143">ServiceBus</span></span>
* <span data-ttu-id="60bb3-144">Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="60bb3-144">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-145">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-145">SQL</span></span>
* <span data-ttu-id="60bb3-146">`sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-146">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-147">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-147">Storage</span></span>
* <span data-ttu-id="60bb3-148">Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen</span><span class="sxs-lookup"><span data-stu-id="60bb3-148">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="60bb3-149">`--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-149">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-150">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-150">VM</span></span>
* <span data-ttu-id="60bb3-151">Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen</span><span class="sxs-lookup"><span data-stu-id="60bb3-151">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="60bb3-152">Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-152">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="60bb3-153">Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-153">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="60bb3-154">16. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-154">October 16, 2018</span></span>

<span data-ttu-id="60bb3-155">Version 2.0.48</span><span class="sxs-lookup"><span data-stu-id="60bb3-155">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-156">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-156">VM</span></span>
* <span data-ttu-id="60bb3-157">SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat</span><span class="sxs-lookup"><span data-stu-id="60bb3-157">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="60bb3-158">9. Oktober 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-158">October 9, 2018</span></span>

<span data-ttu-id="60bb3-159">Version 2.0.47</span><span class="sxs-lookup"><span data-stu-id="60bb3-159">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-160">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-160">Core</span></span>
* <span data-ttu-id="60bb3-161">Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“</span><span class="sxs-lookup"><span data-stu-id="60bb3-161">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-162">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-162">ACR</span></span>
* <span data-ttu-id="60bb3-163">Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-163">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-164">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-164">ACS</span></span>
* <span data-ttu-id="60bb3-165">`aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1</span><span class="sxs-lookup"><span data-stu-id="60bb3-165">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="60bb3-166">Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert</span><span class="sxs-lookup"><span data-stu-id="60bb3-166">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="60bb3-167">`aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-167">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="60bb3-168">Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind</span><span class="sxs-lookup"><span data-stu-id="60bb3-168">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-169">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-169">Container</span></span>
* <span data-ttu-id="60bb3-170">`functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-170">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="60bb3-171">[VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-171">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="60bb3-172">Event Hub</span><span class="sxs-lookup"><span data-stu-id="60bb3-172">Event Hub</span></span>
* <span data-ttu-id="60bb3-173">Befehl `eventhub update` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-173">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="60bb3-174">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="60bb3-174">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="60bb3-175">Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="60bb3-175">Extensions</span></span>
* <span data-ttu-id="60bb3-176">Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-176">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="60bb3-177">HDInsight</span><span class="sxs-lookup"><span data-stu-id="60bb3-177">HDInsight</span></span>
* <span data-ttu-id="60bb3-178">Erste Version</span><span class="sxs-lookup"><span data-stu-id="60bb3-178">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="60bb3-179">IoT</span><span class="sxs-lookup"><span data-stu-id="60bb3-179">IoT</span></span>
* <span data-ttu-id="60bb3-180">Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-180">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="60bb3-181">KeyVault</span><span class="sxs-lookup"><span data-stu-id="60bb3-181">KeyVault</span></span>
* <span data-ttu-id="60bb3-182">Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind</span><span class="sxs-lookup"><span data-stu-id="60bb3-182">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-183">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-183">Network</span></span>
* <span data-ttu-id="60bb3-184">`network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat.</span><span class="sxs-lookup"><span data-stu-id="60bb3-184">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="60bb3-185">Siehe Nr. 6052</span><span class="sxs-lookup"><span data-stu-id="60bb3-185">See #6052</span></span>
* <span data-ttu-id="60bb3-186">`--remote-vnet-id` für `network vnet peering create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="60bb3-186">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="60bb3-187">`--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-187">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="60bb3-188">Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-188">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="60bb3-189">Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-189">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="60bb3-190">Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="60bb3-190">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="60bb3-191">`--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-191">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="60bb3-192">Rolle</span><span class="sxs-lookup"><span data-stu-id="60bb3-192">Role</span></span>
* <span data-ttu-id="60bb3-193">Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-193">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="60bb3-194">Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-194">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="60bb3-195">Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren</span><span class="sxs-lookup"><span data-stu-id="60bb3-195">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="60bb3-196">`ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-196">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="60bb3-197">Service Bus</span><span class="sxs-lookup"><span data-stu-id="60bb3-197">Service Bus</span></span>
* <span data-ttu-id="60bb3-198">[WICHTIGE ÄNDERUNG] `list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="60bb3-198">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-199">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-199">VM</span></span>
* <span data-ttu-id="60bb3-200">Leeres `accessSas`-Feld in `disk grant-access` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-200">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="60bb3-201">`vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-201">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="60bb3-202">Aktualisierungsbefehle für `sig` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-202">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="60bb3-203">`--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-203">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="60bb3-204">`vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-204">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="60bb3-205">`[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-205">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="60bb3-206">21. September 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-206">September 21, 2018</span></span>

<span data-ttu-id="60bb3-207">Version 2.0.46</span><span class="sxs-lookup"><span data-stu-id="60bb3-207">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-208">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-208">ACR</span></span>
* <span data-ttu-id="60bb3-209">ACR-Aufgabenbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-209">Added ACR Task commands</span></span>
* <span data-ttu-id="60bb3-210">Befehl für die Schnellausführung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-210">Added quick run command</span></span>
* <span data-ttu-id="60bb3-211">`build-task`-Befehlsgruppe als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-211">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="60bb3-212">`helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="60bb3-212">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="60bb3-213">Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-213">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="60bb3-214">Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-214">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-215">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-215">ACS</span></span>
* <span data-ttu-id="60bb3-216">Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-216">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="60bb3-217">Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-217">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-218">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-218">AppService</span></span>

* <span data-ttu-id="60bb3-219">Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)</span><span class="sxs-lookup"><span data-stu-id="60bb3-219">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="60bb3-220">„az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-220">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="60bb3-221">Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-221">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="60bb3-222">Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-222">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="60bb3-223">Batch</span><span class="sxs-lookup"><span data-stu-id="60bb3-223">Batch</span></span>
* <span data-ttu-id="60bb3-224">Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="60bb3-224">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="60bb3-225">Dokumentation akzeptierter `--json-file`-Formate aktualisiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-225">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="60bb3-226">`--max-tasks-per-node-option` zu `batch pool create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-226">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="60bb3-227">Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-227">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="60bb3-228">Batch AI</span><span class="sxs-lookup"><span data-stu-id="60bb3-228">Batch AI</span></span> 
* <span data-ttu-id="60bb3-229">Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-229">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="60bb3-230">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="60bb3-230">Cognitive Services</span></span>
* <span data-ttu-id="60bb3-231">Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-231">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="60bb3-232">Befehl `cognitiveservices account list-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-232">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="60bb3-233">Befehl `cognitiveservices account list-kinds` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-233">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="60bb3-234">Befehl `cognitiveservices account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-234">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="60bb3-235">`cognitiveservices list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-235">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="60bb3-236">`--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)</span><span class="sxs-lookup"><span data-stu-id="60bb3-236">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-237">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-237">Container</span></span>
* <span data-ttu-id="60bb3-238">Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-238">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="60bb3-239">`--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-239">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="60bb3-240">`--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="60bb3-240">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="60bb3-241">Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-241">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="60bb3-242">Data Lake</span><span class="sxs-lookup"><span data-stu-id="60bb3-242">Datalake</span></span>
* <span data-ttu-id="60bb3-243">Befehle für VNET-Regeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-243">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="60bb3-244">Interaktive Shell</span><span class="sxs-lookup"><span data-stu-id="60bb3-244">Interactive Shell</span></span>
* <span data-ttu-id="60bb3-245">Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-245">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="60bb3-246">Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-246">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="60bb3-247">IoT</span><span class="sxs-lookup"><span data-stu-id="60bb3-247">IoT</span></span>
* <span data-ttu-id="60bb3-248">Routingunterstützung für IoT Hubs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-248">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="60bb3-249">Key Vault</span><span class="sxs-lookup"><span data-stu-id="60bb3-249">Key Vault</span></span>
* <span data-ttu-id="60bb3-250">Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-250">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-251">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-251">Network</span></span>
* <span data-ttu-id="60bb3-252">Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="60bb3-252">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="60bb3-253">Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="60bb3-253">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="60bb3-254">Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="60bb3-254">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="60bb3-255">`--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen</span><span class="sxs-lookup"><span data-stu-id="60bb3-255">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="60bb3-256">`--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-256">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="60bb3-257">`--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-257">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="60bb3-258">Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="60bb3-258">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="60bb3-259">Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls</span><span class="sxs-lookup"><span data-stu-id="60bb3-259">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="60bb3-260">Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-260">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="60bb3-261">`network express-route create/update`: Flag `--allow-global-reach` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-261">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="60bb3-262">`network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-262">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="60bb3-263">Befehl `network vnet subnet list-available-delegations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-263">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="60bb3-264">`network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-264">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="60bb3-265">`network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="60bb3-265">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="60bb3-266">`dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-266">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="60bb3-267">Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen</span><span class="sxs-lookup"><span data-stu-id="60bb3-267">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="60bb3-268">`network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-268">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="60bb3-269">Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-269">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="60bb3-270">RDBMS</span><span class="sxs-lookup"><span data-stu-id="60bb3-270">RDBMS</span></span>
* <span data-ttu-id="60bb3-271">Unterstützung für den MariaDB-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-271">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="60bb3-272">Reservierung</span><span class="sxs-lookup"><span data-stu-id="60bb3-272">Reservation</span></span>
* <span data-ttu-id="60bb3-273">Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-273">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="60bb3-274">Namenseigenschaft im Patchmodell hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-274">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="60bb3-275">App-Verwaltung</span><span class="sxs-lookup"><span data-stu-id="60bb3-275">Manage App</span></span>
* <span data-ttu-id="60bb3-276">Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte</span><span class="sxs-lookup"><span data-stu-id="60bb3-276">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="60bb3-277">Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken</span><span class="sxs-lookup"><span data-stu-id="60bb3-277">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="60bb3-278">Rolle</span><span class="sxs-lookup"><span data-stu-id="60bb3-278">Role</span></span>
* <span data-ttu-id="60bb3-279">Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-279">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="60bb3-280">SignalR</span><span class="sxs-lookup"><span data-stu-id="60bb3-280">SignalR</span></span>
* <span data-ttu-id="60bb3-281">Erste Version</span><span class="sxs-lookup"><span data-stu-id="60bb3-281">First release</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-282">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-282">Storage</span></span>
* <span data-ttu-id="60bb3-283">Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-283">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="60bb3-284">`storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-284">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-285">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-285">VM</span></span>
* <span data-ttu-id="60bb3-286">Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)</span><span class="sxs-lookup"><span data-stu-id="60bb3-286">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="60bb3-287">Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-287">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="60bb3-288">28. August 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-288">August 28, 2018</span></span>

<span data-ttu-id="60bb3-289">Version 2.0.45</span><span class="sxs-lookup"><span data-stu-id="60bb3-289">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-290">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-290">Core</span></span>

* <span data-ttu-id="60bb3-291">Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="60bb3-291">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="60bb3-292">Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-292">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-293">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-293">ACR</span></span>

* <span data-ttu-id="60bb3-294">Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-294">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="60bb3-295">Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen</span><span class="sxs-lookup"><span data-stu-id="60bb3-295">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-296">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-296">ACS</span></span>

* <span data-ttu-id="60bb3-297">`aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden</span><span class="sxs-lookup"><span data-stu-id="60bb3-297">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="60bb3-298">`aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen</span><span class="sxs-lookup"><span data-stu-id="60bb3-298">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-299">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-299">AppService</span></span>

* <span data-ttu-id="60bb3-300">Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-300">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="60bb3-301">ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-301">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="60bb3-302">`[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="60bb3-302">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="60bb3-303">Backup</span><span class="sxs-lookup"><span data-stu-id="60bb3-303">Backup</span></span>

* <span data-ttu-id="60bb3-304">`backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="60bb3-304">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="60bb3-305">Botdienst</span><span class="sxs-lookup"><span data-stu-id="60bb3-305">Bot Service</span></span>

* <span data-ttu-id="60bb3-306">Anfängliches Release der Botdienst-CLI</span><span class="sxs-lookup"><span data-stu-id="60bb3-306">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="60bb3-307">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="60bb3-307">Cognitive Services</span></span>

* <span data-ttu-id="60bb3-308">Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-308">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="60bb3-309">IoT</span><span class="sxs-lookup"><span data-stu-id="60bb3-309">IoT</span></span>

* <span data-ttu-id="60bb3-310">Problem mit dem Zuweisen verknüpfter Hubs behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-310">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="60bb3-311">Überwachen</span><span class="sxs-lookup"><span data-stu-id="60bb3-311">Monitor</span></span>

* <span data-ttu-id="60bb3-312">`monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-312">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="60bb3-313">`monitor alert`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-313">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-314">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-314">Network</span></span>

* <span data-ttu-id="60bb3-315">`network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="60bb3-315">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-316">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-316">Resource</span></span>

* <span data-ttu-id="60bb3-317">`provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="60bb3-317">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-318">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-318">Storage</span></span>

* <span data-ttu-id="60bb3-319">`storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="60bb3-319">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-320">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-320">VM</span></span>

* <span data-ttu-id="60bb3-321">`vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden</span><span class="sxs-lookup"><span data-stu-id="60bb3-321">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="60bb3-322">`--storage-caching` für `vm create` eingestellt</span><span class="sxs-lookup"><span data-stu-id="60bb3-322">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="60bb3-323">14. August 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-323">Auguest 14, 2018</span></span>

<span data-ttu-id="60bb3-324">Version 2.0.44</span><span class="sxs-lookup"><span data-stu-id="60bb3-324">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-325">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-325">Core</span></span>

* <span data-ttu-id="60bb3-326">Numerische Anzeige in `table`-Ausgabe korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-326">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="60bb3-327">YAML-Ausgabeformat hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-327">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="60bb3-328">Telemetrie</span><span class="sxs-lookup"><span data-stu-id="60bb3-328">Telemetry</span></span>

* <span data-ttu-id="60bb3-329">Verbesserte Berichterstellung für Telemetriedaten</span><span class="sxs-lookup"><span data-stu-id="60bb3-329">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-330">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-330">ACR</span></span>

* <span data-ttu-id="60bb3-331">Befehle vom Typ `content-trust policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-331">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="60bb3-332">Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde</span><span class="sxs-lookup"><span data-stu-id="60bb3-332">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-333">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-333">ACS</span></span>

* <span data-ttu-id="60bb3-334">`az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-334">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="60bb3-335">`az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren</span><span class="sxs-lookup"><span data-stu-id="60bb3-335">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="60bb3-336">Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe</span><span class="sxs-lookup"><span data-stu-id="60bb3-336">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="60bb3-337">Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-337">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="60bb3-338">Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-338">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="60bb3-339">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-339">AppService</span></span>

* <span data-ttu-id="60bb3-340">Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte</span><span class="sxs-lookup"><span data-stu-id="60bb3-340">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="60bb3-341">Absturz bei ZIP-Bereitstellung behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-341">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="60bb3-342">Batch AI</span><span class="sxs-lookup"><span data-stu-id="60bb3-342">BatchAI</span></span>

* <span data-ttu-id="60bb3-343">Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-343">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="60bb3-344">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-344">Container</span></span>

* <span data-ttu-id="60bb3-345">`--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-345">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="60bb3-346">IoT</span><span class="sxs-lookup"><span data-stu-id="60bb3-346">IoT</span></span>

* <span data-ttu-id="60bb3-347">[WICHTIGE ÄNDERUNG] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-347">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="60bb3-348">Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen</span><span class="sxs-lookup"><span data-stu-id="60bb3-348">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="60bb3-349">Iot Central</span><span class="sxs-lookup"><span data-stu-id="60bb3-349">Iot Central</span></span>

* <span data-ttu-id="60bb3-350">Erstes Release des IoT Central-Moduls</span><span class="sxs-lookup"><span data-stu-id="60bb3-350">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="60bb3-351">KeyVault</span><span class="sxs-lookup"><span data-stu-id="60bb3-351">KeyVault</span></span>


* <span data-ttu-id="60bb3-352">Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-352">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="60bb3-353">Befehle für Netzwerkregeln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-353">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="60bb3-354">Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-354">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="60bb3-355">Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-355">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="60bb3-356">Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-356">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="60bb3-357">Relay</span><span class="sxs-lookup"><span data-stu-id="60bb3-357">Relay</span></span>

* <span data-ttu-id="60bb3-358">Erste Version</span><span class="sxs-lookup"><span data-stu-id="60bb3-358">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-359">Sql</span><span class="sxs-lookup"><span data-stu-id="60bb3-359">Sql</span></span>

* <span data-ttu-id="60bb3-360">Befehle vom Typ `sql failover-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-360">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-361">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-361">Storage</span></span>

* <span data-ttu-id="60bb3-362">[WICHTIGE ÄNDERUNG] `storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region</span><span class="sxs-lookup"><span data-stu-id="60bb3-362">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="60bb3-363">Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-363">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="60bb3-364">Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-364">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="60bb3-365">`[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-365">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="60bb3-366">`blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen</span><span class="sxs-lookup"><span data-stu-id="60bb3-366">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-367">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-367">VM</span></span>

* <span data-ttu-id="60bb3-368">Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-368">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="60bb3-369">31. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-369">July 31, 2018</span></span>

<span data-ttu-id="60bb3-370">Version 2.0.43</span><span class="sxs-lookup"><span data-stu-id="60bb3-370">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-371">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-371">ACR</span></span>

* <span data-ttu-id="60bb3-372">Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-372">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="60bb3-373">Befehl `acr build-task update-build` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-373">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-374">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-374">ACS</span></span>

* <span data-ttu-id="60bb3-375">Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-375">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="60bb3-376">Batch</span><span class="sxs-lookup"><span data-stu-id="60bb3-376">Batch</span></span>

* <span data-ttu-id="60bb3-377">Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="60bb3-377">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-378">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-378">Container</span></span>

* <span data-ttu-id="60bb3-379">Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-379">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-380">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-380">Network</span></span>

* <span data-ttu-id="60bb3-381">DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-381">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="60bb3-382">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-382">Resource</span></span>

* <span data-ttu-id="60bb3-383">`--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen</span><span class="sxs-lookup"><span data-stu-id="60bb3-383">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="60bb3-384">Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte</span><span class="sxs-lookup"><span data-stu-id="60bb3-384">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="60bb3-385">Rolle</span><span class="sxs-lookup"><span data-stu-id="60bb3-385">Role</span></span>

* <span data-ttu-id="60bb3-386">Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-386">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="60bb3-387">Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="60bb3-387">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="60bb3-388">Suchen,</span><span class="sxs-lookup"><span data-stu-id="60bb3-388">Search</span></span>

* <span data-ttu-id="60bb3-389">Befehle für Azure Search-Dienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-389">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="60bb3-390">Service Bus</span><span class="sxs-lookup"><span data-stu-id="60bb3-390">Service Bus</span></span>

* <span data-ttu-id="60bb3-391">Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren</span><span class="sxs-lookup"><span data-stu-id="60bb3-391">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="60bb3-392">Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-392">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="60bb3-393">`--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`</span><span class="sxs-lookup"><span data-stu-id="60bb3-393">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="60bb3-394">`--dead-letter-on-filter-exceptions` in `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="60bb3-394">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-395">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-395">Storage</span></span>

* <span data-ttu-id="60bb3-396">Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-396">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="60bb3-397">`show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde</span><span class="sxs-lookup"><span data-stu-id="60bb3-397">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-398">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-398">VM</span></span>

* <span data-ttu-id="60bb3-399">Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-399">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="60bb3-400">Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-400">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="60bb3-401">Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-401">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="60bb3-402">[WICHTIGE ÄNDERUNG] `[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.</span><span class="sxs-lookup"><span data-stu-id="60bb3-402">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="60bb3-403">18. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-403">July 18, 2018</span></span>

<span data-ttu-id="60bb3-404">Version 2.0.42</span><span class="sxs-lookup"><span data-stu-id="60bb3-404">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-405">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-405">Core</span></span>

* <span data-ttu-id="60bb3-406">Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-406">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="60bb3-407">`--force-string`-Flag für alle generischen Updatebefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-407">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="60bb3-408">[WICHTIGE ÄNDERUNG] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt</span><span class="sxs-lookup"><span data-stu-id="60bb3-408">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-409">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-409">ACR</span></span>

* <span data-ttu-id="60bb3-410">[WICHTIGE ÄNDERUNG] „--no-push“ in Befehl „acr build“ in reines Flag geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-410">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="60bb3-411">Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-411">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="60bb3-412">`--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="60bb3-412">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="60bb3-413">Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-413">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-414">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-414">ACS</span></span>

* <span data-ttu-id="60bb3-415">`az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-415">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-416">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-416">AppService</span></span>

* <span data-ttu-id="60bb3-417">Unterstützung für PremiumV2-SKUs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-417">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="60bb3-418">Batch</span><span class="sxs-lookup"><span data-stu-id="60bb3-418">Batch</span></span>

* <span data-ttu-id="60bb3-419">Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus</span><span class="sxs-lookup"><span data-stu-id="60bb3-419">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="60bb3-420">JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-420">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="60bb3-421">Batch AI</span><span class="sxs-lookup"><span data-stu-id="60bb3-421">Batch AI</span></span>

* <span data-ttu-id="60bb3-422">Befehl `az batchai job exec` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-422">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-423">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-423">Container</span></span>

* <span data-ttu-id="60bb3-424">Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-424">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="60bb3-425">Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-425">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-426">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-426">Network</span></span>

* <span data-ttu-id="60bb3-427">Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-427">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="60bb3-428">`network nic wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-428">Added `network nic wait`</span></span>
* <span data-ttu-id="60bb3-429">`--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-429">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="60bb3-430">`--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen</span><span class="sxs-lookup"><span data-stu-id="60bb3-430">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="60bb3-431">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-431">Resource</span></span>

* <span data-ttu-id="60bb3-432">Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-432">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="60bb3-433">Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-433">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="60bb3-434">Befehl `deployment wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-434">Added `deployment wait` command</span></span>
* <span data-ttu-id="60bb3-435">Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-435">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-436">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-436">SQL</span></span>

* <span data-ttu-id="60bb3-437">Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-437">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="60bb3-438">Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig</span><span class="sxs-lookup"><span data-stu-id="60bb3-438">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="60bb3-439">Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-439">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-440">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-440">Storage</span></span>

* <span data-ttu-id="60bb3-441">`pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-441">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-442">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-442">VM</span></span>

* <span data-ttu-id="60bb3-443">[WICHTIGE ÄNDERUNG] `vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-443">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="60bb3-444">Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-444">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="60bb3-445">`vm extension wait` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-445">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="60bb3-446">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-446">July 3, 2018</span></span>

<span data-ttu-id="60bb3-447">Version 2.0.41</span><span class="sxs-lookup"><span data-stu-id="60bb3-447">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="60bb3-448">AKS</span><span class="sxs-lookup"><span data-stu-id="60bb3-448">AKS</span></span>

* <span data-ttu-id="60bb3-449">Überwachung geändert, sodass Abonnement-ID verwendet wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-449">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="60bb3-450">3. Juli 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-450">July 3, 2018</span></span>

<span data-ttu-id="60bb3-451">Version 2.0.40</span><span class="sxs-lookup"><span data-stu-id="60bb3-451">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-452">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-452">Core</span></span>

* <span data-ttu-id="60bb3-453">Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-453">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-454">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-454">ACR</span></span>

* <span data-ttu-id="60bb3-455">Abruf-Buildstatus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-455">Added polling build status</span></span>
* <span data-ttu-id="60bb3-456">Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-456">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="60bb3-457">Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-457">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-458">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-458">ACS</span></span>

* <span data-ttu-id="60bb3-459">[WICHTIGE ÄNDERUNG] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes</span><span class="sxs-lookup"><span data-stu-id="60bb3-459">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="60bb3-460">Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-460">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="60bb3-461">Optionen für Befehl `aks browse` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="60bb3-461">Updated options for `aks browse` command.</span></span> <span data-ttu-id="60bb3-462">Unterstützung für `--listen-port` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-462">Added `--listen-port` support</span></span>
* <span data-ttu-id="60bb3-463">Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="60bb3-463">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="60bb3-464">Verwenden von „virtual-kubelet-for-aks-latest.tgz“</span><span class="sxs-lookup"><span data-stu-id="60bb3-464">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="60bb3-465">Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-465">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-466">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-466">AppService</span></span>

* <span data-ttu-id="60bb3-467">Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-467">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="60bb3-468">`preview`-Tag für Identitätsfunktion entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-468">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="60bb3-469">Backup</span><span class="sxs-lookup"><span data-stu-id="60bb3-469">Backup</span></span>

* <span data-ttu-id="60bb3-470">Moduldefinition aktualisiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-470">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="60bb3-471">Batch AI</span><span class="sxs-lookup"><span data-stu-id="60bb3-471">BatchAI</span></span>

* <span data-ttu-id="60bb3-472">Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-472">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="60bb3-473">Cloud</span><span class="sxs-lookup"><span data-stu-id="60bb3-473">Cloud</span></span>

* <span data-ttu-id="60bb3-474">Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-474">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-475">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-475">Container</span></span>

* <span data-ttu-id="60bb3-476">`container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-476">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="60bb3-477">Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-477">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="60bb3-478">Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-478">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="60bb3-479">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="60bb3-479">Extension</span></span>

* <span data-ttu-id="60bb3-480">`extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden</span><span class="sxs-lookup"><span data-stu-id="60bb3-480">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-481">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-481">Network</span></span>

* <span data-ttu-id="60bb3-482">Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="60bb3-482">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="60bb3-483">Rdbms</span><span class="sxs-lookup"><span data-stu-id="60bb3-483">Rdbms</span></span>

* <span data-ttu-id="60bb3-484">Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-484">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-485">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-485">Resource</span></span>

* <span data-ttu-id="60bb3-486">Neue Vorgangsgruppe `deployment` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-486">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-487">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-487">VM</span></span>

* <span data-ttu-id="60bb3-488">Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-488">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="60bb3-489">25. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-489">June 25, 2018</span></span>

<span data-ttu-id="60bb3-490">Version 2.0.39</span><span class="sxs-lookup"><span data-stu-id="60bb3-490">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="60bb3-491">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="60bb3-491">CLI</span></span>

* <span data-ttu-id="60bb3-492">Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben</span><span class="sxs-lookup"><span data-stu-id="60bb3-492">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="60bb3-493">19. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-493">June 19, 2018</span></span>

<span data-ttu-id="60bb3-494">Version 2.0.38</span><span class="sxs-lookup"><span data-stu-id="60bb3-494">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-495">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-495">Core</span></span>

* <span data-ttu-id="60bb3-496">Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-496">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-497">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-497">ACR</span></span>

* <span data-ttu-id="60bb3-498">`azure-storage-blob` als Abhängigkeit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-498">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="60bb3-499">CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden</span><span class="sxs-lookup"><span data-stu-id="60bb3-499">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-500">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-500">ACS</span></span>

* <span data-ttu-id="60bb3-501">Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="60bb3-501">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="60bb3-502">Unterstützung für `--update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-502">Added `--update` support</span></span>
* <span data-ttu-id="60bb3-503">`aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-503">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="60bb3-504">Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="60bb3-504">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="60bb3-505">Befehlsfehler `acs browse` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-505">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="60bb3-506">`--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt</span><span class="sxs-lookup"><span data-stu-id="60bb3-506">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="60bb3-507">Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-507">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="60bb3-508">Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-508">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-509">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-509">AppService</span></span>

* <span data-ttu-id="60bb3-510">Unterstützung für neuere Versionen von „urllib“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-510">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="60bb3-511">Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-511">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="60bb3-512">Batch</span><span class="sxs-lookup"><span data-stu-id="60bb3-512">Batch</span></span>

* <span data-ttu-id="60bb3-513">`azure-batch-extensions`-Abhängigkeit entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-513">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="60bb3-514">Batch AI</span><span class="sxs-lookup"><span data-stu-id="60bb3-514">Batch AI</span></span>

* <span data-ttu-id="60bb3-515">Unterstützung für Arbeitsbereiche wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-515">Added support for workspaces.</span></span> <span data-ttu-id="60bb3-516">Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.</span><span class="sxs-lookup"><span data-stu-id="60bb3-516">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="60bb3-517">Unterstützung für Experimente wurde hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-517">Added support for experiments.</span></span> <span data-ttu-id="60bb3-518">Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.</span><span class="sxs-lookup"><span data-stu-id="60bb3-518">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="60bb3-519">Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="60bb3-519">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="60bb3-520">Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-520">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="60bb3-521">Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.</span><span class="sxs-lookup"><span data-stu-id="60bb3-521">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="60bb3-522">Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-522">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="60bb3-523">[WICHTIGE ÄNDERUNG] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="60bb3-523">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="60bb3-524">[WICHTIGE ÄNDERUNG] Aufträge müssen unter Experimenten erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="60bb3-524">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="60bb3-525">[WICHTIGE ÄNDERUNG] `--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-525">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="60bb3-526">Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.</span><span class="sxs-lookup"><span data-stu-id="60bb3-526">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="60bb3-527">[WICHTIGE ÄNDERUNG] `--cluster-resource-group` wurde aus dem Befehl `job create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-527">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="60bb3-528">Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.</span><span class="sxs-lookup"><span data-stu-id="60bb3-528">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="60bb3-529">[WICHTIGE ÄNDERUNG] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-529">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="60bb3-530">„Location“ ist jetzt ein Attribut eines Arbeitsbereichs.</span><span class="sxs-lookup"><span data-stu-id="60bb3-530">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="60bb3-531">[WICHTIGE ÄNDERUNG] `--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-531">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="60bb3-532">[WICHTIGE ÄNDERUNG] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:</span><span class="sxs-lookup"><span data-stu-id="60bb3-532">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="60bb3-533">[`--config`, `-c`] in [`--config-file`, `-f`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-533">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="60bb3-534">[`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-534">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="60bb3-535">[`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-535">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="60bb3-536">[`--job`, `-n`] in [`--job`, `-j`] umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-536">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="60bb3-537">Karten</span><span class="sxs-lookup"><span data-stu-id="60bb3-537">Maps</span></span>

* <span data-ttu-id="60bb3-538">[WICHTIGE ÄNDERUNG] `maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.</span><span class="sxs-lookup"><span data-stu-id="60bb3-538">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-539">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-539">Network</span></span>

* <span data-ttu-id="60bb3-540">Unterstützung für `https` zu `network lb probe create` hinzugefügt ([#6571](https://github.com/Azure/azure-cli/issues/6571))</span><span class="sxs-lookup"><span data-stu-id="60bb3-540">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="60bb3-541">Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde.</span><span class="sxs-lookup"><span data-stu-id="60bb3-541">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="60bb3-542">#6502</span><span class="sxs-lookup"><span data-stu-id="60bb3-542">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="60bb3-543">Reservations</span><span class="sxs-lookup"><span data-stu-id="60bb3-543">Reservations</span></span>

* <span data-ttu-id="60bb3-544">[WICHTIGE ÄNDERUNG] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-544">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="60bb3-545">Parameter `Location` zu `reservations catalog show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-545">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="60bb3-546">[WICHTIGE ÄNDERUNG] `kind` aus `ReservationProperties` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-546">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="60bb3-547">[WICHTIGE ÄNDERUNG] `capabilities` wurde in `Catalog` in `sku_properties` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-547">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="60bb3-548">[WICHTIGE ÄNDERUNG] Eigenschaften `size` und `tier` aus `Catalog` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-548">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="60bb3-549">Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-549">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="60bb3-550">Rolle</span><span class="sxs-lookup"><span data-stu-id="60bb3-550">Role</span></span>

* <span data-ttu-id="60bb3-551">Fehlerbehandlung verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-551">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-552">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-552">SQL</span></span>

* <span data-ttu-id="60bb3-553">Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-553">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-554">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-554">Storage</span></span>

* <span data-ttu-id="60bb3-555">Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-555">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-556">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-556">VM</span></span>

* <span data-ttu-id="60bb3-557">Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`</span><span class="sxs-lookup"><span data-stu-id="60bb3-557">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="60bb3-558">Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-558">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="60bb3-559">`--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde</span><span class="sxs-lookup"><span data-stu-id="60bb3-559">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="60bb3-560">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-560">June 13, 2018</span></span>

<span data-ttu-id="60bb3-561">Version 2.0.37</span><span class="sxs-lookup"><span data-stu-id="60bb3-561">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-562">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-562">Core</span></span>

* <span data-ttu-id="60bb3-563">Verbesserte interaktive Telemetrie</span><span class="sxs-lookup"><span data-stu-id="60bb3-563">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="60bb3-564">13. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-564">June 13, 2018</span></span>

<span data-ttu-id="60bb3-565">Version 2.0.36</span><span class="sxs-lookup"><span data-stu-id="60bb3-565">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="60bb3-566">AKS</span><span class="sxs-lookup"><span data-stu-id="60bb3-566">AKS</span></span>

* <span data-ttu-id="60bb3-567">Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-567">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="60bb3-568">Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-568">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="60bb3-569">Argument `--no-ssh-key` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-569">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="60bb3-570">Argument `--enable-rbac` zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-570">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="60bb3-571">[VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-571">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-572">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-572">AppService</span></span>

* <span data-ttu-id="60bb3-573">Problem mit inkompatiblen urllib-Versionen behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-573">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="60bb3-574">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-574">June 5, 2018</span></span>

<span data-ttu-id="60bb3-575">Version 2.0.35</span><span class="sxs-lookup"><span data-stu-id="60bb3-575">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="60bb3-576">Interactive</span><span class="sxs-lookup"><span data-stu-id="60bb3-576">Interactive</span></span>

* <span data-ttu-id="60bb3-577">Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-577">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="60bb3-578">5. Juni 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-578">June 5, 2018</span></span>

<span data-ttu-id="60bb3-579">Version 2.0.34</span><span class="sxs-lookup"><span data-stu-id="60bb3-579">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-580">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-580">Core</span></span>

* <span data-ttu-id="60bb3-581">Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-581">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="60bb3-582">Verbesserte Zuverlässigkeit bei Telemetrieuploads</span><span class="sxs-lookup"><span data-stu-id="60bb3-582">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-583">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-583">ACR</span></span>

* <span data-ttu-id="60bb3-584">Unterstützung für VSTS als Remotequellort hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-584">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="60bb3-585">Befehl `acr import` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-585">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="60bb3-586">AKS</span><span class="sxs-lookup"><span data-stu-id="60bb3-586">AKS</span></span>

* <span data-ttu-id="60bb3-587">`aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="60bb3-587">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="60bb3-588">Batch</span><span class="sxs-lookup"><span data-stu-id="60bb3-588">Batch</span></span>

* <span data-ttu-id="60bb3-589">Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="60bb3-589">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="60bb3-590">IoT</span><span class="sxs-lookup"><span data-stu-id="60bb3-590">IOT</span></span>

* <span data-ttu-id="60bb3-591">Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-591">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-592">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-592">Network</span></span>

* <span data-ttu-id="60bb3-593">`network vnet peering` wurde verbessert.</span><span class="sxs-lookup"><span data-stu-id="60bb3-593">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="60bb3-594">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="60bb3-594">Policy Insights</span></span>

* <span data-ttu-id="60bb3-595">Erste Version</span><span class="sxs-lookup"><span data-stu-id="60bb3-595">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="60bb3-596">ARM</span><span class="sxs-lookup"><span data-stu-id="60bb3-596">ARM</span></span>

* <span data-ttu-id="60bb3-597">Befehle vom Typ `account management-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-597">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-598">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-598">SQL</span></span>

* <span data-ttu-id="60bb3-599">Neue Befehle für verwaltete Instanzen hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="60bb3-599">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="60bb3-600">Neue Befehle für verwaltete Datenbanken hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="60bb3-600">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="60bb3-601">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-601">Storage</span></span>

* <span data-ttu-id="60bb3-602">Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)</span><span class="sxs-lookup"><span data-stu-id="60bb3-602">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-603">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-603">VM</span></span>

* <span data-ttu-id="60bb3-604">`vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="60bb3-604">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="60bb3-605">Option `--accelerated-networking` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-605">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="60bb3-606">`--tags` zu `identity create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-606">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="60bb3-607">22. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-607">May 22, 2018</span></span>

<span data-ttu-id="60bb3-608">Version 2.0.33</span><span class="sxs-lookup"><span data-stu-id="60bb3-608">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-609">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-609">Core</span></span>

* <span data-ttu-id="60bb3-610">Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-610">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-611">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-611">ACS</span></span>

* <span data-ttu-id="60bb3-612">Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-612">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="60bb3-613">Tippfehler in Hilfemeldung korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-613">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-614">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-614">AppService</span></span>

* <span data-ttu-id="60bb3-615">Verbesserte generische Aktualisierungsbefehle</span><span class="sxs-lookup"><span data-stu-id="60bb3-615">Improved generic update commands</span></span>
* <span data-ttu-id="60bb3-616">Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-616">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-617">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-617">Container</span></span>

* <span data-ttu-id="60bb3-618">Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-618">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="60bb3-619">Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-619">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="60bb3-620">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="60bb3-620">Extension</span></span>

* <span data-ttu-id="60bb3-621">Verbesserte Entfernung von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="60bb3-621">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="60bb3-622">Interactive</span><span class="sxs-lookup"><span data-stu-id="60bb3-622">Interactive</span></span>

* <span data-ttu-id="60bb3-623">Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren</span><span class="sxs-lookup"><span data-stu-id="60bb3-623">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="60bb3-624">Verbesserte Verarbeitung beschädigter Hilfscaches</span><span class="sxs-lookup"><span data-stu-id="60bb3-624">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="60bb3-625">KeyVault</span><span class="sxs-lookup"><span data-stu-id="60bb3-625">KeyVault</span></span>

* <span data-ttu-id="60bb3-626">keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="60bb3-626">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-627">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-627">Network</span></span>

* <span data-ttu-id="60bb3-628">Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))</span><span class="sxs-lookup"><span data-stu-id="60bb3-628">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="60bb3-629">Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))</span><span class="sxs-lookup"><span data-stu-id="60bb3-629">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-630">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-630">SQL</span></span>

* <span data-ttu-id="60bb3-631">[WICHTIGE ÄNDERUNG] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:</span><span class="sxs-lookup"><span data-stu-id="60bb3-631">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="60bb3-632">Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-632">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="60bb3-633">Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-633">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="60bb3-634">Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)</span><span class="sxs-lookup"><span data-stu-id="60bb3-634">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="60bb3-635">[WICHTIGE ÄNDERUNG] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="60bb3-635">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="60bb3-636">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-636">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="60bb3-637">Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.</span><span class="sxs-lookup"><span data-stu-id="60bb3-637">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="60bb3-638">`edition`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-638">`edition`.</span></span> <span data-ttu-id="60bb3-639">Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.</span><span class="sxs-lookup"><span data-stu-id="60bb3-639">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="60bb3-640">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-640">`elasticPoolName`.</span></span> <span data-ttu-id="60bb3-641">Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.</span><span class="sxs-lookup"><span data-stu-id="60bb3-641">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="60bb3-642">[WICHTIGE ÄNDERUNG] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:</span><span class="sxs-lookup"><span data-stu-id="60bb3-642">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="60bb3-643">`edition`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-643">`edition`.</span></span> <span data-ttu-id="60bb3-644">Verwenden Sie zum Aktualisieren den Parameter `--edition`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-644">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="60bb3-645">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-645">`dtu`.</span></span> <span data-ttu-id="60bb3-646">Verwenden Sie zum Aktualisieren den Parameter `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-646">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="60bb3-647">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-647">`databaseDtuMin`.</span></span> <span data-ttu-id="60bb3-648">Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-648">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="60bb3-649">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-649">`databaseDtuMax`.</span></span> <span data-ttu-id="60bb3-650">Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-650">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="60bb3-651">Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-651">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="60bb3-652">Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-652">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-653">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-653">Storage</span></span>

* <span data-ttu-id="60bb3-654">Vervollständigung für das Argument `--account-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-654">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="60bb3-655">Problem mit `storage entity query` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-655">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-656">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-656">VM</span></span>

* <span data-ttu-id="60bb3-657">[WICHTIGE ÄNDERUNG] `--write-accelerator` aus `vm create` entfernt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-657">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="60bb3-658">Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.</span><span class="sxs-lookup"><span data-stu-id="60bb3-658">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="60bb3-659">Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-659">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="60bb3-660">`--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-660">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="60bb3-661">`--license-type` zu `[vm|vmss] update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-661">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="60bb3-662">7. Mai 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-662">May 7, 2018</span></span>

<span data-ttu-id="60bb3-663">Version 2.0.32</span><span class="sxs-lookup"><span data-stu-id="60bb3-663">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-664">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-664">Core</span></span>

* <span data-ttu-id="60bb3-665">Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.</span><span class="sxs-lookup"><span data-stu-id="60bb3-665">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="60bb3-666">Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-666">Added limited support for positional arguments</span></span>
* <span data-ttu-id="60bb3-667">Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="60bb3-667">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="60bb3-668">#5591</span><span class="sxs-lookup"><span data-stu-id="60bb3-668">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="60bb3-669">Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-669">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="60bb3-670">Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage</span><span class="sxs-lookup"><span data-stu-id="60bb3-670">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="60bb3-671">Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten</span><span class="sxs-lookup"><span data-stu-id="60bb3-671">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="60bb3-672">Fehler bei der Eingabe von `az ''` behandelt</span><span class="sxs-lookup"><span data-stu-id="60bb3-672">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="60bb3-673">Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-673">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-674">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-674">ACR</span></span>

* <span data-ttu-id="60bb3-675">ACR Build-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-675">Added ACR Build commands</span></span>
* <span data-ttu-id="60bb3-676">Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-676">Improved resource not found error messages</span></span>
* <span data-ttu-id="60bb3-677">Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="60bb3-677">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="60bb3-678">ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-678">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="60bb3-679">Fehlermeldungen zu Repositorybefehlen optimiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-679">Improved repository commands error messages</span></span>
* <span data-ttu-id="60bb3-680">Tabellenspalten und -reihenfolge aktualisiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-680">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-681">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-681">ACS</span></span>

* <span data-ttu-id="60bb3-682">Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-682">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="60bb3-683">Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-683">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="60bb3-684">AMS</span><span class="sxs-lookup"><span data-stu-id="60bb3-684">AMS</span></span>

* <span data-ttu-id="60bb3-685">Erste Version: Verwalten von Azure Media Services-Ressourcen</span><span class="sxs-lookup"><span data-stu-id="60bb3-685">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-686">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-686">Appservice</span></span>

* <span data-ttu-id="60bb3-687">Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.</span><span class="sxs-lookup"><span data-stu-id="60bb3-687">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="60bb3-688">`--runtime-version` aus `webapp auth update` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-688">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="60bb3-689">Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-689">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="60bb3-690">Unterstützung für mehrere Container hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-690">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="60bb3-691">Batch AI</span><span class="sxs-lookup"><span data-stu-id="60bb3-691">Batch AI</span></span>

* <span data-ttu-id="60bb3-692">`batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.</span><span class="sxs-lookup"><span data-stu-id="60bb3-692">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="60bb3-693">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="60bb3-693">Cognitive Services</span></span>

* <span data-ttu-id="60bb3-694">Tippfehler im Beispiel für `cognitiveservices account create` korrigiert ([#5603](https://github.com/Azure/azure-cli/issues/5603))</span><span class="sxs-lookup"><span data-stu-id="60bb3-694">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="60bb3-695">Nutzung</span><span class="sxs-lookup"><span data-stu-id="60bb3-695">Consumption</span></span>

* <span data-ttu-id="60bb3-696">Neue Befehle für Budget-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-696">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-697">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-697">Container</span></span>

* <span data-ttu-id="60bb3-698">`--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="60bb3-698">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="60bb3-699">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="60bb3-699">Cosmos DB</span></span>

* <span data-ttu-id="60bb3-700">VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="60bb3-700">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="60bb3-701">DMS</span><span class="sxs-lookup"><span data-stu-id="60bb3-701">DMS</span></span>

* <span data-ttu-id="60bb3-702">Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-702">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="60bb3-703">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="60bb3-703">Extension</span></span>

* <span data-ttu-id="60bb3-704">Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-704">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="60bb3-705">Interactive</span><span class="sxs-lookup"><span data-stu-id="60bb3-705">Interactive</span></span>

* <span data-ttu-id="60bb3-706">Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.</span><span class="sxs-lookup"><span data-stu-id="60bb3-706">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="60bb3-707">Benutzerfreundlichere Ausgabe bei der Eingabe von '\'</span><span class="sxs-lookup"><span data-stu-id="60bb3-707">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="60bb3-708">Abschlüsse für Parameter ohne Hilfe korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-708">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="60bb3-709">Beschreibungen für Befehlsgruppen korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-709">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="60bb3-710">Labor</span><span class="sxs-lookup"><span data-stu-id="60bb3-710">Lab</span></span>

* <span data-ttu-id="60bb3-711">Regressionen aus Knack-Umwandlung korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-711">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-712">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-712">Network</span></span>

* <span data-ttu-id="60bb3-713">[WICHTIGE ÄNDERUNG] Parameter `--ids` entfernt für:</span><span class="sxs-lookup"><span data-stu-id="60bb3-713">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="60bb3-714">Profil</span><span class="sxs-lookup"><span data-stu-id="60bb3-714">Profile</span></span>

* <span data-ttu-id="60bb3-715">Quellerkennung für `disk create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-715">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="60bb3-716">[WICHTIGE ÄNDERUNG] `--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden</span><span class="sxs-lookup"><span data-stu-id="60bb3-716">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="60bb3-717">Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-717">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="60bb3-718">Redis</span><span class="sxs-lookup"><span data-stu-id="60bb3-718">Redis</span></span>

* <span data-ttu-id="60bb3-719">`redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-719">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="60bb3-720">`redis list-all` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-720">Deprecated `redis list-all`.</span></span> <span data-ttu-id="60bb3-721">Diese Funktion wurde in `redis list` integriert.</span><span class="sxs-lookup"><span data-stu-id="60bb3-721">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="60bb3-722">`redis import-method` wurde durch `redis import` ersetzt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-722">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="60bb3-723">Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-723">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="60bb3-724">Rolle</span><span class="sxs-lookup"><span data-stu-id="60bb3-724">Role</span></span>

* <span data-ttu-id="60bb3-725">[WICHTIGE ÄNDERUNG] Veralteter Befehl `ad sp reset-credentials` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-725">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-726">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-726">Storage</span></span>

* <span data-ttu-id="60bb3-727">Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden</span><span class="sxs-lookup"><span data-stu-id="60bb3-727">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="60bb3-728">Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads</span><span class="sxs-lookup"><span data-stu-id="60bb3-728">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="60bb3-729">Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln</span><span class="sxs-lookup"><span data-stu-id="60bb3-729">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="60bb3-730">Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt</span><span class="sxs-lookup"><span data-stu-id="60bb3-730">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="60bb3-731">`storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren</span><span class="sxs-lookup"><span data-stu-id="60bb3-731">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-732">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-732">VM</span></span>

* <span data-ttu-id="60bb3-733">Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-733">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="60bb3-734">Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-734">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="60bb3-735">[WICHTIGE ÄNDERUNG] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.</span><span class="sxs-lookup"><span data-stu-id="60bb3-735">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="60bb3-736">Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-736">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="60bb3-737">[WICHTIGE ÄNDERUNG] `--ids` entfernt aus:</span><span class="sxs-lookup"><span data-stu-id="60bb3-737">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="60bb3-738">Unterstützung für Schreibbeschleunigung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-738">Added write accelerator support</span></span>
* <span data-ttu-id="60bb3-739">`vmss perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-739">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="60bb3-740">`vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen</span><span class="sxs-lookup"><span data-stu-id="60bb3-740">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="60bb3-741">`vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen</span><span class="sxs-lookup"><span data-stu-id="60bb3-741">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="60bb3-742">10. April 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-742">April 10, 2018</span></span>

<span data-ttu-id="60bb3-743">Version 2.0.31</span><span class="sxs-lookup"><span data-stu-id="60bb3-743">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-744">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-744">ACR</span></span>

* <span data-ttu-id="60bb3-745">Verbesserte Fehlerbehandlung für wincred-Fallback</span><span class="sxs-lookup"><span data-stu-id="60bb3-745">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-746">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-746">ACS</span></span>

* <span data-ttu-id="60bb3-747">Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-747">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-748">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-748">Appservice</span></span>

* [WICHTIGE ÄNDERUNG]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="60bb3-750">Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-750">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="60bb3-751">Batch AI</span><span class="sxs-lookup"><span data-stu-id="60bb3-751">BatchAI</span></span>

* <span data-ttu-id="60bb3-752">Unterstützung für API 2018-03-01 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-752">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="60bb3-753">Bereitstellung auf Auftragsebene</span><span class="sxs-lookup"><span data-stu-id="60bb3-753">Job level mounting</span></span>
  - <span data-ttu-id="60bb3-754">Umgebungsvariablen mit Geheimniswerten</span><span class="sxs-lookup"><span data-stu-id="60bb3-754">Environment variables with secret values</span></span>
  - <span data-ttu-id="60bb3-755">Einstellungen von Leistungsindikatoren</span><span class="sxs-lookup"><span data-stu-id="60bb3-755">Performance counters settings</span></span>
  - <span data-ttu-id="60bb3-756">Berichtstellung für auftragsspezifisches Pfadsegment</span><span class="sxs-lookup"><span data-stu-id="60bb3-756">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="60bb3-757">Unterstützung für Unterordner in Listendateien-API</span><span class="sxs-lookup"><span data-stu-id="60bb3-757">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="60bb3-758">Berichterstellung zur Nutzung und zu Grenzwerten</span><span class="sxs-lookup"><span data-stu-id="60bb3-758">Usage and limits reporting</span></span>
  - <span data-ttu-id="60bb3-759">Zulassen der Angabe des Cachetyps für NFS-Server</span><span class="sxs-lookup"><span data-stu-id="60bb3-759">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="60bb3-760">Unterstützung für benutzerdefinierte Images</span><span class="sxs-lookup"><span data-stu-id="60bb3-760">Support for custom images</span></span>
  - <span data-ttu-id="60bb3-761">Unterstützung für pyTorch-Toolkit hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-761">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="60bb3-762">Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet</span><span class="sxs-lookup"><span data-stu-id="60bb3-762">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="60bb3-763">Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch AI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden</span><span class="sxs-lookup"><span data-stu-id="60bb3-763">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="60bb3-764">Nationale Clouds werden unterstützt</span><span class="sxs-lookup"><span data-stu-id="60bb3-764">National clouds are supported</span></span>
* <span data-ttu-id="60bb3-765">Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="60bb3-765">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="60bb3-766">Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images</span><span class="sxs-lookup"><span data-stu-id="60bb3-766">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="60bb3-767">Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch AI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-767">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="60bb3-768">Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="60bb3-768">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="60bb3-769">Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).</span><span class="sxs-lookup"><span data-stu-id="60bb3-769">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="60bb3-770">Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)</span><span class="sxs-lookup"><span data-stu-id="60bb3-770">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="60bb3-771">Verbesserte `table`-Ausgabe für `show`-Vorgänge</span><span class="sxs-lookup"><span data-stu-id="60bb3-771">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="60bb3-772">Option `--use-auto-storage` für die Clustererstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-772">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="60bb3-773">Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.</span><span class="sxs-lookup"><span data-stu-id="60bb3-773">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="60bb3-774">`--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-774">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="60bb3-775">Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile</span><span class="sxs-lookup"><span data-stu-id="60bb3-775">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="60bb3-776">[WICHTIGE ÄNDERUNG] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-776">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="60bb3-777">[WICHTIGE ÄNDERUNG] `--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen</span><span class="sxs-lookup"><span data-stu-id="60bb3-777">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="60bb3-778">Abrechnung</span><span class="sxs-lookup"><span data-stu-id="60bb3-778">Billing</span></span>

* <span data-ttu-id="60bb3-779">Registrierungskontobefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-779">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="60bb3-780">Nutzung</span><span class="sxs-lookup"><span data-stu-id="60bb3-780">Consumption</span></span>

* <span data-ttu-id="60bb3-781">Befehle vom Typ `marketplace` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-781">Added `marketplace` commands</span></span>
* <span data-ttu-id="60bb3-782">[WICHTIGE ÄNDERUNG] `reservations summaries` in `reservation summary` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-782">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="60bb3-783">[WICHTIGE ÄNDERUNG] `reservations details` in `reservation detail` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-783">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="60bb3-784">[WICHTIGE ÄNDERUNG] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-784">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="60bb3-785">[WICHTIGE ÄNDERUNG] `--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-785">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="60bb3-786">[WICHTIGE ÄNDERUNG] `--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-786">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-787">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-787">Container</span></span>

* <span data-ttu-id="60bb3-788">Git-Repository-Parameter `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path` für die Volumebereitstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-788">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="60bb3-789">[#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde</span><span class="sxs-lookup"><span data-stu-id="60bb3-789">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="60bb3-790">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="60bb3-790">Extension</span></span>

* <span data-ttu-id="60bb3-791">Meldung für Distributionsüberprüfung in Debugebene geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-791">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="60bb3-792">Interactive</span><span class="sxs-lookup"><span data-stu-id="60bb3-792">Interactive</span></span>

* <span data-ttu-id="60bb3-793">Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen</span><span class="sxs-lookup"><span data-stu-id="60bb3-793">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="60bb3-794">Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-794">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="60bb3-795">Abschluss für `--ids`-Parameter hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-795">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-796">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-796">Network</span></span>

* <span data-ttu-id="60bb3-797">[#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden</span><span class="sxs-lookup"><span data-stu-id="60bb3-797">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="60bb3-798">Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-798">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="60bb3-799">#4910</span><span class="sxs-lookup"><span data-stu-id="60bb3-799">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="60bb3-800">`ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-800">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="60bb3-801">Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="60bb3-801">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="60bb3-802">Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-802">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="60bb3-803">Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-803">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="60bb3-804">Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-804">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="60bb3-805">Profil</span><span class="sxs-lookup"><span data-stu-id="60bb3-805">Profile</span></span>

* <span data-ttu-id="60bb3-806">Unterstützung für klassische Azure-Konten in `account list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-806">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="60bb3-807">[WICHTIGE ÄNDERUNG] `--msi` & `--msi-port`-Argumente entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-807">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="60bb3-808">RDBMS</span><span class="sxs-lookup"><span data-stu-id="60bb3-808">RDBMS</span></span>

* <span data-ttu-id="60bb3-809">Befehl `georestore` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-809">Added `georestore` command</span></span>
* <span data-ttu-id="60bb3-810">Speichergrößenbeschränkung aus Befehl `create` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-810">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-811">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-811">Resource</span></span>

* <span data-ttu-id="60bb3-812">Unterstützung für `--metadata` zu `policy definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-812">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="60bb3-813">Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-813">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-814">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-814">SQL</span></span>

* <span data-ttu-id="60bb3-815">`sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-815">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-816">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-816">Storage</span></span>

* <span data-ttu-id="60bb3-817">Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-817">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-818">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-818">VM</span></span>

* <span data-ttu-id="60bb3-819">Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-819">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="60bb3-820">`vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-820">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [WICHTIGE ÄNDERUNG]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="60bb3-822">Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-822">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="60bb3-823">Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann.</span><span class="sxs-lookup"><span data-stu-id="60bb3-823">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="60bb3-824">#5718</span><span class="sxs-lookup"><span data-stu-id="60bb3-824">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="60bb3-825">Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist</span><span class="sxs-lookup"><span data-stu-id="60bb3-825">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="60bb3-826">27. März 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-826">March 27, 2018</span></span>

<span data-ttu-id="60bb3-827">Version 2.0.30</span><span class="sxs-lookup"><span data-stu-id="60bb3-827">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-828">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-828">Core</span></span>

* <span data-ttu-id="60bb3-829">Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="60bb3-829">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-830">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-830">ACS</span></span>

* <span data-ttu-id="60bb3-831">Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="60bb3-831">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-832">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-832">Appservice</span></span>

* <span data-ttu-id="60bb3-833">Unterstützung nur von HTTPS zu `webapp update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-833">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="60bb3-834">Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-834">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="60bb3-835">Backup</span><span class="sxs-lookup"><span data-stu-id="60bb3-835">Backup</span></span>

* <span data-ttu-id="60bb3-836">Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-836">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="60bb3-837">Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.</span><span class="sxs-lookup"><span data-stu-id="60bb3-837">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="60bb3-838">Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:</span><span class="sxs-lookup"><span data-stu-id="60bb3-838">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="60bb3-839">`--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.</span><span class="sxs-lookup"><span data-stu-id="60bb3-839">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-840">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-840">Container</span></span>

* <span data-ttu-id="60bb3-841">Befehl `container exec` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-841">Added `container exec` command.</span></span> <span data-ttu-id="60bb3-842">Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe</span><span class="sxs-lookup"><span data-stu-id="60bb3-842">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="60bb3-843">Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe</span><span class="sxs-lookup"><span data-stu-id="60bb3-843">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="60bb3-844">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="60bb3-844">Extension</span></span>

* <span data-ttu-id="60bb3-845">Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet</span><span class="sxs-lookup"><span data-stu-id="60bb3-845">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="60bb3-846">`extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="60bb3-846">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="60bb3-847">[WICHTIGE ÄNDERUNG] `extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="60bb3-847">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="60bb3-848">Interactive</span><span class="sxs-lookup"><span data-stu-id="60bb3-848">Interactive</span></span>

* <span data-ttu-id="60bb3-849">Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="60bb3-849">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="60bb3-850">Fehler bei der Verwendung des Parameters `--style` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-850">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="60bb3-851">Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)</span><span class="sxs-lookup"><span data-stu-id="60bb3-851">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="60bb3-852">Verbesserte Unterstützung der Vervollständigung</span><span class="sxs-lookup"><span data-stu-id="60bb3-852">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="60bb3-853">Labor</span><span class="sxs-lookup"><span data-stu-id="60bb3-853">Lab</span></span>

* <span data-ttu-id="60bb3-854">Probleme mit Befehl `create environment` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-854">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="60bb3-855">Überwachen</span><span class="sxs-lookup"><span data-stu-id="60bb3-855">Monitor</span></span>

* <span data-ttu-id="60bb3-856">Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="60bb3-856">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="60bb3-857">[#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken.</span><span class="sxs-lookup"><span data-stu-id="60bb3-857">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="60bb3-858">Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt ([#5785](https://github.com/Azure/azure-cli/issues/5785))</span><span class="sxs-lookup"><span data-stu-id="60bb3-858">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-859">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-859">Network</span></span>

* <span data-ttu-id="60bb3-860">Unterstützung für private DNS-Zonen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-860">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="60bb3-861">Profil</span><span class="sxs-lookup"><span data-stu-id="60bb3-861">Profile</span></span>

* <span data-ttu-id="60bb3-862">Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-862">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="60bb3-863">RDBMS</span><span class="sxs-lookup"><span data-stu-id="60bb3-863">RDBMS</span></span>

* <span data-ttu-id="60bb3-864">GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-864">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-865">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-865">Resource</span></span>

* [WICHTIGE ÄNDERUNG]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="60bb3-867">Rolle</span><span class="sxs-lookup"><span data-stu-id="60bb3-867">Role</span></span>

* <span data-ttu-id="60bb3-868">Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-868">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="60bb3-869">`rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="60bb3-869">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="60bb3-870">Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-870">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="60bb3-871">[WICHTIGE ÄNDERUNG] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-871">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="60bb3-872">Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-872">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-873">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-873">Storage</span></span>

* <span data-ttu-id="60bb3-874">Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-874">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="60bb3-875">[#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursachten</span><span class="sxs-lookup"><span data-stu-id="60bb3-875">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-876">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-876">VM</span></span>

* <span data-ttu-id="60bb3-877">Warnung für anstehende wichtige Änderungen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-877">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="60bb3-878">Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-878">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="60bb3-879">Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden</span><span class="sxs-lookup"><span data-stu-id="60bb3-879">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="60bb3-880">[WICHTIGE ÄNDERUNG] `vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="60bb3-880">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="60bb3-881">13. März 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-881">March 13, 2018</span></span>

<span data-ttu-id="60bb3-882">Version 2.0.29</span><span class="sxs-lookup"><span data-stu-id="60bb3-882">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-883">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-883">ACR</span></span>

* <span data-ttu-id="60bb3-884">Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-884">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="60bb3-885">Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-885">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="60bb3-886">Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-886">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-887">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-887">ACS</span></span>

* <span data-ttu-id="60bb3-888">Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-888">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="60bb3-889">`kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-889">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="60bb3-890">Advisor</span><span class="sxs-lookup"><span data-stu-id="60bb3-890">Advisor</span></span>

* <span data-ttu-id="60bb3-891">[WICHTIGE ÄNDERUNG] `advisor configuration get` in `advisor configuration list` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-891">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="60bb3-892">[WICHTIGE ÄNDERUNG] `advisor configuration set` in `advisor configuration update` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-892">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="60bb3-893">[WICHTIGE ÄNDERUNG] `advisor recommendation generate` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-893">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="60bb3-894">Parameter `--refresh` zu `advisor recommendation list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-894">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="60bb3-895">Befehl `advisor recommendation show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-895">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-896">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-896">Appservice</span></span>

* <span data-ttu-id="60bb3-897">`[webapp|functionapp] assign-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-897">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="60bb3-898">Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-898">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="60bb3-899">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="60bb3-899">Eventhubs</span></span>

* <span data-ttu-id="60bb3-900">Erste Version</span><span class="sxs-lookup"><span data-stu-id="60bb3-900">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="60bb3-901">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="60bb3-901">Extension</span></span>

* <span data-ttu-id="60bb3-902">Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann</span><span class="sxs-lookup"><span data-stu-id="60bb3-902">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="60bb3-903">Interactive</span><span class="sxs-lookup"><span data-stu-id="60bb3-903">Interactive</span></span>

* <span data-ttu-id="60bb3-904">[#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten</span><span class="sxs-lookup"><span data-stu-id="60bb3-904">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="60bb3-905">[#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt</span><span class="sxs-lookup"><span data-stu-id="60bb3-905">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="60bb3-906">[#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse nicht angezeigt, wenn beim Laden der Befehlstabelle Ausnahme auftrat</span><span class="sxs-lookup"><span data-stu-id="60bb3-906">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="60bb3-907">Statusanzeige für lang ausgeführte Vorgänge korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-907">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="60bb3-908">Überwachen</span><span class="sxs-lookup"><span data-stu-id="60bb3-908">Monitor</span></span>

* <span data-ttu-id="60bb3-909">`monitor autoscale-settings`-Befehle als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-909">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="60bb3-910">Befehle vom Typ `monitor autoscale` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-910">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="60bb3-911">Befehle vom Typ `monitor autoscale profile` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-911">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="60bb3-912">Befehle vom Typ `monitor autoscale rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-912">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-913">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-913">Network</span></span>

* <span data-ttu-id="60bb3-914">[WICHTIGE ÄNDERUNG] Parameter `--tags` aus `route-filter rule create` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-914">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="60bb3-915">Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:</span><span class="sxs-lookup"><span data-stu-id="60bb3-915">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="60bb3-916">`network watcher connection-monitor`-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-916">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="60bb3-917">Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-917">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="60bb3-918">Profil</span><span class="sxs-lookup"><span data-stu-id="60bb3-918">Profile</span></span>

* <span data-ttu-id="60bb3-919">Parameter `--msi` für `az login` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-919">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="60bb3-920">Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-920">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="60bb3-921">RDBMS</span><span class="sxs-lookup"><span data-stu-id="60bb3-921">RDBMS</span></span>

* <span data-ttu-id="60bb3-922">[VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-922">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="60bb3-923">Service Bus</span><span class="sxs-lookup"><span data-stu-id="60bb3-923">Service Bus</span></span>

* <span data-ttu-id="60bb3-924">Erste Version</span><span class="sxs-lookup"><span data-stu-id="60bb3-924">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-925">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-925">Storage</span></span>

* <span data-ttu-id="60bb3-926">[#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.</span><span class="sxs-lookup"><span data-stu-id="60bb3-926">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="60bb3-927">[#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: `storage blob [delete-batch|download-batch|upload-batch]`-Batchbefehle lösen bei Vorbedingungsfehlern keinen Fehler mehr aus.</span><span class="sxs-lookup"><span data-stu-id="60bb3-927">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-928">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-928">VM</span></span>

* <span data-ttu-id="60bb3-929">`[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.</span><span class="sxs-lookup"><span data-stu-id="60bb3-929">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="60bb3-930">`[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-930">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="60bb3-931">Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-931">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="60bb3-932">Standardpriorität in `vmss create` auf „Keine“ geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-932">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="60bb3-933">27. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-933">February 27, 2018</span></span>

<span data-ttu-id="60bb3-934">Version 2.0.28</span><span class="sxs-lookup"><span data-stu-id="60bb3-934">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-935">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-935">Core</span></span>

* <span data-ttu-id="60bb3-936">[5184](https://github.com/Azure/azure-cli/issues/5184) (Problem beim Installieren von Homebrew) behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-936">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="60bb3-937">Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-937">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="60bb3-938">HTTP-Protokollierung zu `--debug` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-938">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-939">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-939">ACS</span></span>

* <span data-ttu-id="60bb3-940">Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-940">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="60bb3-941">Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe</span><span class="sxs-lookup"><span data-stu-id="60bb3-941">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="60bb3-942">Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-942">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="60bb3-943">Veraltungshinweis aus `aks get-versions` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-943">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-944">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-944">Appservice</span></span>

* <span data-ttu-id="60bb3-945">Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="60bb3-945">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="60bb3-946">[5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.</span><span class="sxs-lookup"><span data-stu-id="60bb3-946">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="60bb3-947">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="60bb3-947">Cognitive Services</span></span>

* <span data-ttu-id="60bb3-948">Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-948">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="60bb3-949">Nutzung</span><span class="sxs-lookup"><span data-stu-id="60bb3-949">Consumption</span></span>

* <span data-ttu-id="60bb3-950">Neue Befehle für PriceSheet-API hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-950">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="60bb3-951">Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-951">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-952">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-952">Container</span></span>

* <span data-ttu-id="60bb3-953">Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können</span><span class="sxs-lookup"><span data-stu-id="60bb3-953">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-954">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-954">Network</span></span>

* <span data-ttu-id="60bb3-955">[5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="60bb3-955">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-956">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-956">Resource</span></span>

* <span data-ttu-id="60bb3-957">`group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war</span><span class="sxs-lookup"><span data-stu-id="60bb3-957">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="60bb3-958">Rolle</span><span class="sxs-lookup"><span data-stu-id="60bb3-958">Role</span></span>

* <span data-ttu-id="60bb3-959">`role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="60bb3-959">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-960">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-960">SQL</span></span>

* <span data-ttu-id="60bb3-961">Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)</span><span class="sxs-lookup"><span data-stu-id="60bb3-961">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-962">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-962">Storage</span></span>

* <span data-ttu-id="60bb3-963">Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht</span><span class="sxs-lookup"><span data-stu-id="60bb3-963">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-964">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-964">VM</span></span>

* <span data-ttu-id="60bb3-965">Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-965">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="60bb3-966">13. Februar 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-966">February 13, 2018</span></span>

<span data-ttu-id="60bb3-967">Version 2.0.27</span><span class="sxs-lookup"><span data-stu-id="60bb3-967">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-968">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-968">Core</span></span>

* <span data-ttu-id="60bb3-969">Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-969">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-970">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-970">ACS</span></span>

* <span data-ttu-id="60bb3-971">[WICHTIGE ÄNDERUNG] `aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-971">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="60bb3-972">`aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-972">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="60bb3-973">Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-973">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="60bb3-974">Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-974">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="60bb3-975">Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-975">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="60bb3-976">Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-976">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="60bb3-977">`aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln</span><span class="sxs-lookup"><span data-stu-id="60bb3-977">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="60bb3-978">Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern</span><span class="sxs-lookup"><span data-stu-id="60bb3-978">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-979">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-979">Appservice</span></span>

* <span data-ttu-id="60bb3-980">Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte</span><span class="sxs-lookup"><span data-stu-id="60bb3-980">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="60bb3-981">Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-981">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="60bb3-982">CDN</span><span class="sxs-lookup"><span data-stu-id="60bb3-982">CDN</span></span>

* <span data-ttu-id="60bb3-983">Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-983">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-984">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-984">Container</span></span>

* <span data-ttu-id="60bb3-985">Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-985">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="60bb3-986">Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-986">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="60bb3-987">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="60bb3-987">CosmosDB</span></span>

* <span data-ttu-id="60bb3-988">Unterstützung für Einstellungsfunktionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-988">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="60bb3-989">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="60bb3-989">Extension</span></span>

* <span data-ttu-id="60bb3-990">Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-990">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="60bb3-991">Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-991">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="60bb3-992">Feedback</span><span class="sxs-lookup"><span data-stu-id="60bb3-992">Feedback</span></span>

* <span data-ttu-id="60bb3-993">Erweiterungsinformationen zu Telemetriedaten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-993">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="60bb3-994">Interactive</span><span class="sxs-lookup"><span data-stu-id="60bb3-994">Interactive</span></span>

* <span data-ttu-id="60bb3-995">Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-995">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="60bb3-996">Regression mit fehlenden Parametervervollständigungen korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-996">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="60bb3-997">IoT</span><span class="sxs-lookup"><span data-stu-id="60bb3-997">IoT</span></span>

* <span data-ttu-id="60bb3-998">Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="60bb3-998">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="60bb3-999">Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt</span><span class="sxs-lookup"><span data-stu-id="60bb3-999">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="60bb3-1000">Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1000">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="60bb3-1001">`iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1001">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="60bb3-1002">Überwachen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1002">Monitor</span></span>

* <span data-ttu-id="60bb3-1003">Befehl `az monitor log-profiles create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1003">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-1004">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1004">Network</span></span>

* <span data-ttu-id="60bb3-1005">Option `--tags` für folgende Befehle korrigiert:</span><span class="sxs-lookup"><span data-stu-id="60bb3-1005">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="60bb3-1006">Profil</span><span class="sxs-lookup"><span data-stu-id="60bb3-1006">Profile</span></span>

* <span data-ttu-id="60bb3-1007">`az login` im interaktiven Modus aktiviert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1007">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-1008">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-1008">Resource</span></span>

* <span data-ttu-id="60bb3-1009">`feature show` wieder hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1009">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="60bb3-1010">Rolle</span><span class="sxs-lookup"><span data-stu-id="60bb3-1010">Role</span></span>

* <span data-ttu-id="60bb3-1011">Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1011">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-1012">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-1012">SQL</span></span>

* <span data-ttu-id="60bb3-1013">Befehle vom Typ `sql server dns-alias` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1013">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="60bb3-1014">`sql db rename` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1014">Added `sql db rename`</span></span>
* <span data-ttu-id="60bb3-1015">Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1015">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-1016">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-1016">Storage</span></span>

* <span data-ttu-id="60bb3-1017">Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1017">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1018">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1018">VM</span></span>

* <span data-ttu-id="60bb3-1019">Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1019">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="60bb3-1020">Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1020">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="60bb3-1021">`vm boot-diagnostics get-boot-log` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1021">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="60bb3-1022">31. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-1022">January 31, 2018</span></span>

<span data-ttu-id="60bb3-1023">Version 2.0.26</span><span class="sxs-lookup"><span data-stu-id="60bb3-1023">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-1024">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-1024">Core</span></span>

* <span data-ttu-id="60bb3-1025">Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1025">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="60bb3-1026">Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1026">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="60bb3-1027">Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1027">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="60bb3-1028">`--verbose` zum Anzeigen verwenden.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1028">Use `--verbose` to see</span></span>
* <span data-ttu-id="60bb3-1029">Statusanzeige für Wait-Befehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1029">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-1030">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1030">ACS</span></span>

* <span data-ttu-id="60bb3-1031">Argument `--disable-browser` erläutert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1031">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="60bb3-1032">Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1032">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-1033">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-1033">Appservice</span></span>

* <span data-ttu-id="60bb3-1034">`webapp log [tail|download]` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1034">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="60bb3-1035">Überprüfung `kind` für Web-Apps und Funktionen entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1035">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="60bb3-1036">CDN</span><span class="sxs-lookup"><span data-stu-id="60bb3-1036">CDN</span></span>

* <span data-ttu-id="60bb3-1037">Problem mit fehlendem Client für `cdn custom-domain create` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1037">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="60bb3-1038">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="60bb3-1038">CosmosDB</span></span>

* <span data-ttu-id="60bb3-1039">Parameterbeschreibung für Failoverrichtlinien korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1039">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="60bb3-1040">Interactive</span><span class="sxs-lookup"><span data-stu-id="60bb3-1040">Interactive</span></span>

* <span data-ttu-id="60bb3-1041">Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1041">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-1042">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1042">Network</span></span>

* <span data-ttu-id="60bb3-1043">Schutz für `--cert-password` zu `application-gateway create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1043">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="60bb3-1044">Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete</span><span class="sxs-lookup"><span data-stu-id="60bb3-1044">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="60bb3-1045">Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1045">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="60bb3-1046">Problem mit fehlendem Client für `asg create` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1046">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="60bb3-1047">Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1047">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="60bb3-1048">Folgende Probleme mit `dns zone export` behoben:</span><span class="sxs-lookup"><span data-stu-id="60bb3-1048">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="60bb3-1049">Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1049">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="60bb3-1050">Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1050">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="60bb3-1051">Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1051">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="60bb3-1052">Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1052">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="60bb3-1053">Profil</span><span class="sxs-lookup"><span data-stu-id="60bb3-1053">Profile</span></span>

* <span data-ttu-id="60bb3-1054">`get-access-token` zur Verwendung auf einer VM mit Identität korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1054">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-1055">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-1055">Resource</span></span>

* <span data-ttu-id="60bb3-1056">Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1056">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-1057">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-1057">Storage</span></span>

* <span data-ttu-id="60bb3-1058">Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1058">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="60bb3-1059">Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1059">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="60bb3-1060">Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="60bb3-1060">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="60bb3-1061">Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1061">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="60bb3-1062">Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1062">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1063">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1063">VM</span></span>

* <span data-ttu-id="60bb3-1064">Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1064">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="60bb3-1065">`[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können</span><span class="sxs-lookup"><span data-stu-id="60bb3-1065">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="60bb3-1066">[VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1066">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="60bb3-1067">Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1067">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="60bb3-1068">17. Januar 2018</span><span class="sxs-lookup"><span data-stu-id="60bb3-1068">January 17, 2018</span></span>

<span data-ttu-id="60bb3-1069">Version 2.0.25</span><span class="sxs-lookup"><span data-stu-id="60bb3-1069">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-1070">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-1070">ACR</span></span>

* <span data-ttu-id="60bb3-1071">Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1071">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="60bb3-1072">Registrierungsprotokolle aktiviert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1072">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-1073">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1073">ACS</span></span>

* <span data-ttu-id="60bb3-1074">Befehl `get-credentials` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1074">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="60bb3-1075">SPN-Rollenanforderung entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1075">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-1076">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-1076">Appservice</span></span>

* <span data-ttu-id="60bb3-1077">Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war</span><span class="sxs-lookup"><span data-stu-id="60bb3-1077">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="60bb3-1078">Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1078">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="60bb3-1079">Slotunterstützung für `log tail` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1079">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="60bb3-1080">Backup</span><span class="sxs-lookup"><span data-stu-id="60bb3-1080">Backup</span></span>

* <span data-ttu-id="60bb3-1081">Option `--container-name` von `backup item list` geändert (ist jetzt optional)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1081">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="60bb3-1082">Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1082">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="60bb3-1083">Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1083">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="60bb3-1084">Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat</span><span class="sxs-lookup"><span data-stu-id="60bb3-1084">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="60bb3-1085">`backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1085">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="60bb3-1086">Batch</span><span class="sxs-lookup"><span data-stu-id="60bb3-1086">Batch</span></span>

* <span data-ttu-id="60bb3-1087">`batch login` geändert, um Authentifizierungsdetails zurückzugeben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1087">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="60bb3-1088">Cloud</span><span class="sxs-lookup"><span data-stu-id="60bb3-1088">Cloud</span></span>

* <span data-ttu-id="60bb3-1089">Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1089">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="60bb3-1090">Nutzung</span><span class="sxs-lookup"><span data-stu-id="60bb3-1090">Consumption</span></span>

* <span data-ttu-id="60bb3-1091">Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1091">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="60bb3-1092">Event Grid</span><span class="sxs-lookup"><span data-stu-id="60bb3-1092">Event Grid</span></span>

* <span data-ttu-id="60bb3-1093">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1093">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="60bb3-1094">[WICHTIGE ÄNDERUNG] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1094">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="60bb3-1095">[WICHTIGE ÄNDERUNG] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1095">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="60bb3-1096">Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1096">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="60bb3-1097">Befehl `eventgrid topic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1097">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="60bb3-1098">Befehl `eventgrid event-subscription update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1098">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="60bb3-1099">Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1099">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="60bb3-1100">Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1100">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="60bb3-1101">Interactive</span><span class="sxs-lookup"><span data-stu-id="60bb3-1101">Interactive</span></span>

* <span data-ttu-id="60bb3-1102">Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="60bb3-1102">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="60bb3-1103">Fehler beim Start behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1103">Fixed errors on startup</span></span>
* <span data-ttu-id="60bb3-1104">Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1104">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="60bb3-1105">IoT</span><span class="sxs-lookup"><span data-stu-id="60bb3-1105">IoT</span></span>

* <span data-ttu-id="60bb3-1106">Unterstützung für Gerätebereitstellungsdienst hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1106">Added support for device provisioning service</span></span>
* <span data-ttu-id="60bb3-1107">Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1107">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="60bb3-1108">IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren</span><span class="sxs-lookup"><span data-stu-id="60bb3-1108">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="60bb3-1109">Überwachen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1109">Monitor</span></span>

* <span data-ttu-id="60bb3-1110">Unterstützung mehrerer Diagnoseeinstellung hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1110">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="60bb3-1111">Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1111">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="60bb3-1112">Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1112">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-1113">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1113">Network</span></span>

* <span data-ttu-id="60bb3-1114">Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat</span><span class="sxs-lookup"><span data-stu-id="60bb3-1114">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="60bb3-1115">Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1115">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="60bb3-1116">Profil</span><span class="sxs-lookup"><span data-stu-id="60bb3-1116">Profile</span></span>

* <span data-ttu-id="60bb3-1117">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1117">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="60bb3-1118">Rolle</span><span class="sxs-lookup"><span data-stu-id="60bb3-1118">Role</span></span>

* <span data-ttu-id="60bb3-1119">Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1119">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="60bb3-1120">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="60bb3-1120">Service Fabric</span></span>

* <span data-ttu-id="60bb3-1121">Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1121">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="60bb3-1122">Problem mit fehlendem Client für verschiedene Befehle behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1122">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1123">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1123">VM</span></span>

* <span data-ttu-id="60bb3-1124">[VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1124">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="60bb3-1125">[WICHTIGE ÄNDERUNG] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1125">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="60bb3-1126">[WICHTIGE ÄNDERUNG] `externalIdentities` in `userAssignedIdentities` geändert für EMSI</span><span class="sxs-lookup"><span data-stu-id="60bb3-1126">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="60bb3-1127">[VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1127">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="60bb3-1128">Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1128">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="60bb3-1129">Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1129">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="60bb3-1130">Fehlerbedingte Probleme mit `[vm|vmss] create` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1130">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="60bb3-1131">Übermäßige Ressourcenverwendung durch `vm image list --all` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1131">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="60bb3-1132">19. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1132">December 19, 2017</span></span>

<span data-ttu-id="60bb3-1133">Version 2.0.23</span><span class="sxs-lookup"><span data-stu-id="60bb3-1133">Version 2.0.23</span></span>

* <span data-ttu-id="60bb3-1134">Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1134">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-1135">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-1135">Container</span></span>

* <span data-ttu-id="60bb3-1136">Falsche Reihenfolge der Parameter für Containerprotokolle behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1136">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-1137">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1137">Network</span></span>

* <span data-ttu-id="60bb3-1138">Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1138">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="60bb3-1139">Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1139">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-1140">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-1140">Storage</span></span>

* <span data-ttu-id="60bb3-1141">Unterstützung für Storage V2 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1141">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1142">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1142">VM</span></span>

* <span data-ttu-id="60bb3-1143">[VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1143">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="60bb3-1144">5. Dezember 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1144">December 5, 2017</span></span>

<span data-ttu-id="60bb3-1145">Version 2.0.22</span><span class="sxs-lookup"><span data-stu-id="60bb3-1145">Version 2.0.22</span></span>

* <span data-ttu-id="60bb3-1146">`az component`-Befehle wurden entfernt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1146">Removed `az component` commands.</span></span> <span data-ttu-id="60bb3-1147">Verwenden Sie stattdessen `az extension`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1147">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-1148">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-1148">Core</span></span>
* <span data-ttu-id="60bb3-1149">Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1149">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="60bb3-1150">Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1150">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1151">ACS</span></span>

* <span data-ttu-id="60bb3-1152">Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1152">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="60bb3-1153">Verbesserte Fehlerberichterstellung für `acs create`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1153">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="60bb3-1154">Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad</span><span class="sxs-lookup"><span data-stu-id="60bb3-1154">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="60bb3-1155">Advisor</span><span class="sxs-lookup"><span data-stu-id="60bb3-1155">Advisor</span></span>

* <span data-ttu-id="60bb3-1156">Erste Version</span><span class="sxs-lookup"><span data-stu-id="60bb3-1156">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-1157">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-1157">Appservice</span></span>

* <span data-ttu-id="60bb3-1158">Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1158">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="60bb3-1159">`webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1159">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="60bb3-1160">Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1160">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="60bb3-1161">Nutzung</span><span class="sxs-lookup"><span data-stu-id="60bb3-1161">Consumption</span></span>

* <span data-ttu-id="60bb3-1162">Unterstützung für API-Version 2017-11-30 hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1162">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-1163">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-1163">Container</span></span>

* <span data-ttu-id="60bb3-1164">Feste Regression für Standardports</span><span class="sxs-lookup"><span data-stu-id="60bb3-1164">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="60bb3-1165">Überwachen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1165">Monitor</span></span>

* <span data-ttu-id="60bb3-1166">Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1166">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-1167">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-1167">Resource</span></span>

* <span data-ttu-id="60bb3-1168">Argument `--include-response-body` zu `resource show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1168">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="60bb3-1169">Rolle</span><span class="sxs-lookup"><span data-stu-id="60bb3-1169">Role</span></span>

* <span data-ttu-id="60bb3-1170">Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1170">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="60bb3-1171">Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1171">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="60bb3-1172">Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1172">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-1173">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-1173">SQL</span></span>

* <span data-ttu-id="60bb3-1174">Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1174">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="60bb3-1175">Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1175">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1176">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1176">VM</span></span>

* <span data-ttu-id="60bb3-1177">Zoneninformationen zu `az vm list-skus` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1177">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="60bb3-1178">14. November 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1178">November 14, 2017</span></span>

<span data-ttu-id="60bb3-1179">Version 2.0.21</span><span class="sxs-lookup"><span data-stu-id="60bb3-1179">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-1180">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-1180">ACR</span></span>

* <span data-ttu-id="60bb3-1181">Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1181">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="60bb3-1182">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1182">ACS</span></span>

* <span data-ttu-id="60bb3-1183">Formulierung in AKS von „Agent“ in „Knoten“ geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1183">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="60bb3-1184">Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet</span><span class="sxs-lookup"><span data-stu-id="60bb3-1184">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="60bb3-1185">VM-Standardgröße für AKS in `Standard_D1_v2` geändert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1185">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="60bb3-1186">`az aks browse` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1186">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="60bb3-1187">`az aks get-credentials` für Windows korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1187">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-1188">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-1188">Appservice</span></span>

* <span data-ttu-id="60bb3-1189">Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1189">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="60bb3-1190">Option `--docker-container-logging` zu `az webapp log config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1190">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="60bb3-1191">Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1191">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="60bb3-1192">Fehlermeldungen für `deployment user set` verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1192">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="60bb3-1193">Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1193">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="60bb3-1194">`list-locations` (feststehend)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1194">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="60bb3-1195">Batch</span><span class="sxs-lookup"><span data-stu-id="60bb3-1195">Batch</span></span>

* <span data-ttu-id="60bb3-1196">Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-1196">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="60bb3-1197">BatchAI</span><span class="sxs-lookup"><span data-stu-id="60bb3-1197">Batchai</span></span>

* <span data-ttu-id="60bb3-1198">Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1198">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="60bb3-1199">Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1199">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="60bb3-1200">Dokumentation für `job list-files` und `job stream-file` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1200">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="60bb3-1201">Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1201">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="60bb3-1202">Cloud</span><span class="sxs-lookup"><span data-stu-id="60bb3-1202">Cloud</span></span>

* <span data-ttu-id="60bb3-1203">`cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern</span><span class="sxs-lookup"><span data-stu-id="60bb3-1203">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-1204">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-1204">Container</span></span>

* <span data-ttu-id="60bb3-1205">Unterstützung für das Öffnen mehrerer Ports hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1205">Added support to open multiple ports</span></span>
* <span data-ttu-id="60bb3-1206">Neustartrichtlinie für Containergruppen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1206">Added container group restart policy</span></span>
* <span data-ttu-id="60bb3-1207">Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1207">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="60bb3-1208">Hilfedokumente aktualisiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1208">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="60bb3-1209">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="60bb3-1209">Data Lake Analytics</span></span>

* <span data-ttu-id="60bb3-1210">`[job|account] list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1210">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="60bb3-1211">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="60bb3-1211">Data Lake Store</span></span>

* <span data-ttu-id="60bb3-1212">`account list` geändert, um präzisere Informationen zu erhalten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1212">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="60bb3-1213">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="60bb3-1213">Extension</span></span>

* <span data-ttu-id="60bb3-1214">`extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1214">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="60bb3-1215">`--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1215">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="60bb3-1216">IoT</span><span class="sxs-lookup"><span data-stu-id="60bb3-1216">IoT</span></span>

* <span data-ttu-id="60bb3-1217">Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1217">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="60bb3-1218">Überwachen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1218">Monitor</span></span>

* <span data-ttu-id="60bb3-1219">Befehle vom Typ `activity-log alert` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1219">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-1220">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1220">Network</span></span>

* <span data-ttu-id="60bb3-1221">Unterstützung für CAA-DNS-Einträge hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1221">Added support for CAA DNS records</span></span>
* <span data-ttu-id="60bb3-1222">Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1222">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="60bb3-1223">Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="60bb3-1223">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="60bb3-1224">Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1224">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="60bb3-1225">Reservations</span><span class="sxs-lookup"><span data-stu-id="60bb3-1225">Reservations</span></span>

* <span data-ttu-id="60bb3-1226">Erste Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="60bb3-1226">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-1227">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-1227">Resource</span></span>

* <span data-ttu-id="60bb3-1228">Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1228">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-1229">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-1229">SQL</span></span>

* <span data-ttu-id="60bb3-1230">Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1230">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-1231">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-1231">Storage</span></span>

* <span data-ttu-id="60bb3-1232">`storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-1232">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="60bb3-1233">Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1233">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="60bb3-1234">Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="60bb3-1234">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="60bb3-1235">Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1235">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="60bb3-1236">Problem beim Aktivieren von Metriken mit `storage metrics update` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1236">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="60bb3-1237">Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1237">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="60bb3-1238">Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1238">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1239">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1239">VM</span></span>

* <span data-ttu-id="60bb3-1240">Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat</span><span class="sxs-lookup"><span data-stu-id="60bb3-1240">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="60bb3-1241">`--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1241">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="60bb3-1242">Befehle hinzugefügt: `vm secret `[add|remove|list]</span><span class="sxs-lookup"><span data-stu-id="60bb3-1242">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="60bb3-1243">`vm format-secret` in `vm secret format` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1243">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="60bb3-1244">Argument `--encrypt format` zu `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1244">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="60bb3-1245">24. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1245">October 24, 2017</span></span>

<span data-ttu-id="60bb3-1246">Version 2.0.20</span><span class="sxs-lookup"><span data-stu-id="60bb3-1246">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-1247">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-1247">Core</span></span>

* <span data-ttu-id="60bb3-1248">Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API</span><span class="sxs-lookup"><span data-stu-id="60bb3-1248">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-1249">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-1249">ACR</span></span>

* <span data-ttu-id="60bb3-1250">Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1250">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="60bb3-1251">SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1251">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="60bb3-1252">Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1252">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-1253">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1253">ACS</span></span>

* <span data-ttu-id="60bb3-1254">[VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1254">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="60bb3-1255">Problem mit `get-credentials` in Kubernetes behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1255">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-1256">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-1256">Appservice</span></span>

* <span data-ttu-id="60bb3-1257">Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren</span><span class="sxs-lookup"><span data-stu-id="60bb3-1257">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="60bb3-1258">Komponente</span><span class="sxs-lookup"><span data-stu-id="60bb3-1258">Component</span></span>

* <span data-ttu-id="60bb3-1259">Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1259">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="60bb3-1260">Überwachen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1260">Monitor</span></span>

* <span data-ttu-id="60bb3-1261">Befehle vom Typ `action-group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1261">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-1262">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-1262">Resource</span></span>

* <span data-ttu-id="60bb3-1263">Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1263">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="60bb3-1264">Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann</span><span class="sxs-lookup"><span data-stu-id="60bb3-1264">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1265">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1265">VM</span></span>

* <span data-ttu-id="60bb3-1266">Argument `--accelerated-networking` zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1266">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="60bb3-1267">9. Oktober 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1267">October 9, 2017</span></span>

<span data-ttu-id="60bb3-1268">Version 2.0.19</span><span class="sxs-lookup"><span data-stu-id="60bb3-1268">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-1269">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-1269">Core</span></span>

* <span data-ttu-id="60bb3-1270">Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1270">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-1271">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-1271">Appservice</span></span>

* <span data-ttu-id="60bb3-1272">Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1272">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="60bb3-1273">Batch</span><span class="sxs-lookup"><span data-stu-id="60bb3-1273">Batch</span></span>

* <span data-ttu-id="60bb3-1274">Aktualisierung auf Batch SDK 4.0.0</span><span class="sxs-lookup"><span data-stu-id="60bb3-1274">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="60bb3-1275">Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1275">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="60bb3-1276">Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1276">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="60bb3-1277">Batch-Unterstützung aus dem Komponentenmodell entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1277">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="60bb3-1278">BatchAI</span><span class="sxs-lookup"><span data-stu-id="60bb3-1278">Batchai</span></span>

* <span data-ttu-id="60bb3-1279">Erste Version des Batch AI-Moduls</span><span class="sxs-lookup"><span data-stu-id="60bb3-1279">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="60bb3-1280">KeyVault</span><span class="sxs-lookup"><span data-stu-id="60bb3-1280">Keyvault</span></span>

* <span data-ttu-id="60bb3-1281">Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1281">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="60bb3-1282">(#4448)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1282">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="60bb3-1283">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1283">Network</span></span>

* <span data-ttu-id="60bb3-1284">Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1284">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="60bb3-1285">`traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1285">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-1286">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-1286">Resource</span></span>

* <span data-ttu-id="60bb3-1287">Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1287">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="60bb3-1288">Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1288">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="60bb3-1289">Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1289">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="60bb3-1290">Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1290">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-1291">Sql</span><span class="sxs-lookup"><span data-stu-id="60bb3-1291">Sql</span></span>

* <span data-ttu-id="60bb3-1292">Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1292">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="60bb3-1293">Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1293">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="60bb3-1294">`db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1294">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-1295">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-1295">Storage</span></span>

* <span data-ttu-id="60bb3-1296">Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1296">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1297">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1297">Vm</span></span>

* <span data-ttu-id="60bb3-1298">Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte</span><span class="sxs-lookup"><span data-stu-id="60bb3-1298">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="60bb3-1299">[VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1299">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="60bb3-1300">Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1300">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="60bb3-1301">Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1301">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="60bb3-1302">Parameter `--license-type` für Windows zu `vmss create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1302">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="60bb3-1303">22. September 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1303">September 22, 2017</span></span>

<span data-ttu-id="60bb3-1304">Version 2.0.18</span><span class="sxs-lookup"><span data-stu-id="60bb3-1304">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-1305">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-1305">Resource</span></span>

* <span data-ttu-id="60bb3-1306">Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1306">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="60bb3-1307">Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1307">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="60bb3-1308">Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1308">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="60bb3-1309">[WICHTIGE ÄNDERUNG] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1309">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-1310">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1310">Network</span></span>

* <span data-ttu-id="60bb3-1311">Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1311">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="60bb3-1312">Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1312">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="60bb3-1313">Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1313">Added `asg` application security group commands</span></span>
* <span data-ttu-id="60bb3-1314">Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1314">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="60bb3-1315">Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1315">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="60bb3-1316">Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1316">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="60bb3-1317">Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1317">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-1318">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-1318">Storage</span></span>

* <span data-ttu-id="60bb3-1319">Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="60bb3-1319">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="60bb3-1320">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="60bb3-1320">Eventgrid</span></span>

* <span data-ttu-id="60bb3-1321">Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1321">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-1322">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-1322">SQL</span></span>

* <span data-ttu-id="60bb3-1323">`sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1323">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="60bb3-1324">Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1324">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="60bb3-1325">Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1325">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="60bb3-1326">KeyVault</span><span class="sxs-lookup"><span data-stu-id="60bb3-1326">Keyvault</span></span>

* <span data-ttu-id="60bb3-1327">Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1327">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1328">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1328">VM</span></span>

* <span data-ttu-id="60bb3-1329">Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1329">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="60bb3-1330">Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="60bb3-1330">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="60bb3-1331">Argument `--asgs` zu `vm create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1331">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="60bb3-1332">Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1332">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="60bb3-1333">[VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1333">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="60bb3-1334">Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1334">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-1335">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1335">ACS</span></span>

* <span data-ttu-id="60bb3-1336">[VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1336">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-1337">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-1337">Appservice</span></span>

* <span data-ttu-id="60bb3-1338">Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1338">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="60bb3-1339">Backup</span><span class="sxs-lookup"><span data-stu-id="60bb3-1339">Backup</span></span>

* <span data-ttu-id="60bb3-1340">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="60bb3-1340">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="60bb3-1341">11. September 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1341">September 11, 2017</span></span>

<span data-ttu-id="60bb3-1342">Version 2.0.17</span><span class="sxs-lookup"><span data-stu-id="60bb3-1342">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="60bb3-1343">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-1343">Core</span></span>

* <span data-ttu-id="60bb3-1344">Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1344">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="60bb3-1345">Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat</span><span class="sxs-lookup"><span data-stu-id="60bb3-1345">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-1346">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1346">Acs</span></span>

* <span data-ttu-id="60bb3-1347">Befehl `acs list-locations` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1347">Added `acs list-locations` command</span></span>
* <span data-ttu-id="60bb3-1348">`ssh-key-file` wird mit dem erwarteten Standardwert versehen.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1348">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-1349">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-1349">Appservice</span></span>

* <span data-ttu-id="60bb3-1350">Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs</span><span class="sxs-lookup"><span data-stu-id="60bb3-1350">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="60bb3-1351">CDN</span><span class="sxs-lookup"><span data-stu-id="60bb3-1351">CDN</span></span>

* <span data-ttu-id="60bb3-1352">Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1352">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="60bb3-1353">Durchwahl</span><span class="sxs-lookup"><span data-stu-id="60bb3-1353">Extension</span></span>

* <span data-ttu-id="60bb3-1354">Erste Version</span><span class="sxs-lookup"><span data-stu-id="60bb3-1354">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="60bb3-1355">KeyVault</span><span class="sxs-lookup"><span data-stu-id="60bb3-1355">Keyvault</span></span>

* <span data-ttu-id="60bb3-1356">Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste</span><span class="sxs-lookup"><span data-stu-id="60bb3-1356">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-1357">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1357">Network</span></span>

* <span data-ttu-id="60bb3-1358">`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1358">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="60bb3-1359">Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1359">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="60bb3-1360">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1360">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="60bb3-1361">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1361">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="60bb3-1362">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1362">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-1363">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-1363">Resource</span></span>

* <span data-ttu-id="60bb3-1364">Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1364">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="60bb3-1365">Übergabe von Parameterwerten für `policy assignment create` zulassen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1365">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="60bb3-1366">Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1366">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="60bb3-1367">Inkrementierte API-Version</span><span class="sxs-lookup"><span data-stu-id="60bb3-1367">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-1368">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-1368">SQL</span></span>

* <span data-ttu-id="60bb3-1369">Befehle vom Typ `sql server vnet-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1369">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1370">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1370">VM</span></span>

* <span data-ttu-id="60bb3-1371">Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-1371">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="60bb3-1372">Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1372">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="60bb3-1373">`subscription` aus der Ausgabe von `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1373">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="60bb3-1374">Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1374">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="60bb3-1375">Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1375">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="60bb3-1376">31. August 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1376">August 31, 2017</span></span>

<span data-ttu-id="60bb3-1377">Version 2.0.16</span><span class="sxs-lookup"><span data-stu-id="60bb3-1377">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="60bb3-1378">KeyVault</span><span class="sxs-lookup"><span data-stu-id="60bb3-1378">Keyvault</span></span>

* <span data-ttu-id="60bb3-1379">Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1379">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="60bb3-1380">Sf</span><span class="sxs-lookup"><span data-stu-id="60bb3-1380">Sf</span></span>

* <span data-ttu-id="60bb3-1381">Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1381">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-1382">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-1382">Storage</span></span>

* <span data-ttu-id="60bb3-1383">Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1383">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="60bb3-1384">Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind</span><span class="sxs-lookup"><span data-stu-id="60bb3-1384">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="60bb3-1385">28. August 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1385">August 28, 2017</span></span>

<span data-ttu-id="60bb3-1386">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="60bb3-1386">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="60bb3-1387">Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1387">CLI</span></span>

* <span data-ttu-id="60bb3-1388">Rechtlichen Hinweis zu `--version` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1388">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-1389">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1389">ACS</span></span>

* <span data-ttu-id="60bb3-1390">Vorschauregionen korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1390">Corrected preview regions</span></span>
* <span data-ttu-id="60bb3-1391">Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1391">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="60bb3-1392">ACS-Befehlsausgabe optimiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1392">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-1393">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-1393">Appservice</span></span>

* <span data-ttu-id="60bb3-1394">[WICHTIGE ÄNDERUNG] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1394">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="60bb3-1395">Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1395">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="60bb3-1396">`az webapp log show` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="60bb3-1396">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="60bb3-1397">Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1397">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="60bb3-1398">Behoben: Korrekte Erkennung der Sloteinstellungen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1398">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="60bb3-1399">IoT</span><span class="sxs-lookup"><span data-stu-id="60bb3-1399">IoT</span></span>

* <span data-ttu-id="60bb3-1400">Behoben (3934): Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="60bb3-1400">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-1401">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1401">Network</span></span>

* <span data-ttu-id="60bb3-1402">[WICHTIGE ÄNDERUNG] `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1402">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="60bb3-1403">[WICHTIGE ÄNDERUNG] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1403">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="60bb3-1404">Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1404">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="60bb3-1405">Unterstützung für SKU zu `lb create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1405">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="60bb3-1406">Unterstützung für SKU zu `public-ip create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1406">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="60bb3-1407">Profil</span><span class="sxs-lookup"><span data-stu-id="60bb3-1407">Profile</span></span>

* <span data-ttu-id="60bb3-1408">`--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="60bb3-1408">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="60bb3-1409">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="60bb3-1409">Service Fabric</span></span>

* <span data-ttu-id="60bb3-1410">Vorschauversion</span><span class="sxs-lookup"><span data-stu-id="60bb3-1410">Preview release</span></span>
* <span data-ttu-id="60bb3-1411">Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht</span><span class="sxs-lookup"><span data-stu-id="60bb3-1411">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="60bb3-1412">Kennwortanforderung für Benutzer trotz Parameterübergabe behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1412">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="60bb3-1413">Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1413">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-1414">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-1414">Storage</span></span>

* <span data-ttu-id="60bb3-1415">Festlegen des Blobtarifs ermöglicht</span><span class="sxs-lookup"><span data-stu-id="60bb3-1415">Enabled setting blob tier</span></span>
* <span data-ttu-id="60bb3-1416">Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1416">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="60bb3-1417">Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1417">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="60bb3-1418">Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht</span><span class="sxs-lookup"><span data-stu-id="60bb3-1418">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="60bb3-1419">[WICHTIGE ÄNDERUNG] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1419">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="60bb3-1420">Behoben (4220): `az storage account update encryption` – Syntaxkonflikt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1420">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1421">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1421">VM</span></span>

* <span data-ttu-id="60bb3-1422">Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1422">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="60bb3-1423">Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="60bb3-1423">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="60bb3-1424">Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1424">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="60bb3-1425">Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1425">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="60bb3-1426">Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1426">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="60bb3-1427">Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="60bb3-1427">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="60bb3-1428">15. August 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1428">August 15, 2017</span></span>

<span data-ttu-id="60bb3-1429">Version 2.0.14</span><span class="sxs-lookup"><span data-stu-id="60bb3-1429">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-1430">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1430">ACS</span></span>

* <span data-ttu-id="60bb3-1431">sshMaster0-Portnummer für Kubernetes korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1431">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-1432">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-1432">Appservice</span></span>

* <span data-ttu-id="60bb3-1433">Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1433">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="60bb3-1434">Event Grid</span><span class="sxs-lookup"><span data-stu-id="60bb3-1434">Event Grid</span></span>

* <span data-ttu-id="60bb3-1435">SDK-Abhängigkeiten hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1435">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="60bb3-1436">11. August 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1436">August 11, 2017</span></span>

<span data-ttu-id="60bb3-1437">Version 2.0.13</span><span class="sxs-lookup"><span data-stu-id="60bb3-1437">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-1438">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1438">ACS</span></span>

* <span data-ttu-id="60bb3-1439">Weitere Vorschauregionen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1439">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="60bb3-1440">Batch</span><span class="sxs-lookup"><span data-stu-id="60bb3-1440">Batch</span></span>

* <span data-ttu-id="60bb3-1441">Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1441">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="60bb3-1442">Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1442">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="60bb3-1443">Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1443">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="60bb3-1444">Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“</span><span class="sxs-lookup"><span data-stu-id="60bb3-1444">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="60bb3-1445">Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag</span><span class="sxs-lookup"><span data-stu-id="60bb3-1445">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="60bb3-1446">Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1446">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="60bb3-1447">Komponente</span><span class="sxs-lookup"><span data-stu-id="60bb3-1447">Component</span></span>

* <span data-ttu-id="60bb3-1448">Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1448">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="60bb3-1449">Container</span><span class="sxs-lookup"><span data-stu-id="60bb3-1449">Container</span></span>

* <span data-ttu-id="60bb3-1450">`create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war</span><span class="sxs-lookup"><span data-stu-id="60bb3-1450">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="60bb3-1451">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="60bb3-1451">Data Lake Store</span></span>

* <span data-ttu-id="60bb3-1452">Fortschrittsüberwachung ermöglicht</span><span class="sxs-lookup"><span data-stu-id="60bb3-1452">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="60bb3-1453">Event Grid</span><span class="sxs-lookup"><span data-stu-id="60bb3-1453">Event Grid</span></span>

* <span data-ttu-id="60bb3-1454">Erste Version</span><span class="sxs-lookup"><span data-stu-id="60bb3-1454">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-1455">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1455">Network</span></span>

* <span data-ttu-id="60bb3-1456">`lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht ordnungsgemäß aufgelöst wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1456">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="60bb3-1457">`application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde</span><span class="sxs-lookup"><span data-stu-id="60bb3-1457">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="60bb3-1458">`application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte</span><span class="sxs-lookup"><span data-stu-id="60bb3-1458">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="60bb3-1459">Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1459">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="60bb3-1460">Profil</span><span class="sxs-lookup"><span data-stu-id="60bb3-1460">Profile</span></span>

* <span data-ttu-id="60bb3-1461">`account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren</span><span class="sxs-lookup"><span data-stu-id="60bb3-1461">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-1462">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-1462">Storage</span></span>

* <span data-ttu-id="60bb3-1463">Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht</span><span class="sxs-lookup"><span data-stu-id="60bb3-1463">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1464">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1464">VM</span></span>

* <span data-ttu-id="60bb3-1465">`availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="60bb3-1465">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="60bb3-1466">Befehl `list-skus` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="60bb3-1466">Exposed `list-skus` command</span></span>
* <span data-ttu-id="60bb3-1467">Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1467">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="60bb3-1468">Anwenden von Speicher-SKU beim Anfügen von Datenträgern</span><span class="sxs-lookup"><span data-stu-id="60bb3-1468">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="60bb3-1469">Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1469">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="60bb3-1470">28. Juli 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1470">July 28, 2017</span></span>

<span data-ttu-id="60bb3-1471">Version 2.0.12</span><span class="sxs-lookup"><span data-stu-id="60bb3-1471">Version 2.0.12</span></span>

* <span data-ttu-id="60bb3-1472">Containerbefehle hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1472">Added container commands</span></span>
* <span data-ttu-id="60bb3-1473">Abrechnungs- und Nutzungsmodule hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1473">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="60bb3-1474">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-1474">Core</span></span>

* <span data-ttu-id="60bb3-1475">Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1475">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="60bb3-1476">Ausnahmen beim Bereitstellungsfortschritt behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1476">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="60bb3-1477">Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients</span><span class="sxs-lookup"><span data-stu-id="60bb3-1477">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="60bb3-1478">Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1478">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="60bb3-1479">Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung</span><span class="sxs-lookup"><span data-stu-id="60bb3-1479">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="60bb3-1480">Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1480">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="60bb3-1481">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1481">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="60bb3-1482">Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1482">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="60bb3-1483">Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1483">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="60bb3-1484">Erstellung von Abonnementclients mit richtigem SDK-Profil</span><span class="sxs-lookup"><span data-stu-id="60bb3-1484">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="60bb3-1485">Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner</span><span class="sxs-lookup"><span data-stu-id="60bb3-1485">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="60bb3-1486">Idempotenz für VM-/VMSS-Erstellung behoben (3586)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1486">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="60bb3-1487">Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1487">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="60bb3-1488">Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1488">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="60bb3-1489">Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack</span><span class="sxs-lookup"><span data-stu-id="60bb3-1489">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="60bb3-1490">Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1490">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="60bb3-1491">ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-1491">ACR</span></span>

* <span data-ttu-id="60bb3-1492">Befehl `show-usage` für verwaltete Registrierungen hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1492">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="60bb3-1493">Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1493">Support SKU update for managed registries</span></span>
* <span data-ttu-id="60bb3-1494">Verwaltete Registrierungen mit verwalteter SKU hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1494">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="60bb3-1495">Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1495">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="60bb3-1496">AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1496">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="60bb3-1497">Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1497">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-1498">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1498">ACS</span></span>

* <span data-ttu-id="60bb3-1499">Unterstützung der API-Version 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="60bb3-1499">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-1500">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-1500">Appservice</span></span>

* <span data-ttu-id="60bb3-1501">Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat</span><span class="sxs-lookup"><span data-stu-id="60bb3-1501">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="60bb3-1502">Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR</span><span class="sxs-lookup"><span data-stu-id="60bb3-1502">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="60bb3-1503">Entfernung aller Befehle unter `appservice web`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1503">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="60bb3-1504">Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1504">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="60bb3-1505">Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1505">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="60bb3-1506">Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1506">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="60bb3-1507">Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1507">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="60bb3-1508">Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1508">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="60bb3-1509">Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1509">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="60bb3-1510">Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1510">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="60bb3-1511">Batch</span><span class="sxs-lookup"><span data-stu-id="60bb3-1511">Batch</span></span>

* <span data-ttu-id="60bb3-1512">Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1512">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="60bb3-1513">`pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1513">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="60bb3-1514">`pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1514">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="60bb3-1515">CDN</span><span class="sxs-lookup"><span data-stu-id="60bb3-1515">CDN</span></span>

* <span data-ttu-id="60bb3-1516">Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-1516">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="60bb3-1517">Cloud</span><span class="sxs-lookup"><span data-stu-id="60bb3-1517">Cloud</span></span>

* <span data-ttu-id="60bb3-1518">API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1518">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="60bb3-1519">Katalogendpunkt nicht erforderlich</span><span class="sxs-lookup"><span data-stu-id="60bb3-1519">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="60bb3-1520">Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1520">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="60bb3-1521">Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können</span><span class="sxs-lookup"><span data-stu-id="60bb3-1521">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="60bb3-1522">`endpoint_vm_image_alias_doc` verfügbar gemacht</span><span class="sxs-lookup"><span data-stu-id="60bb3-1522">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="60bb3-1523">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="60bb3-1523">CosmosDB</span></span>

* <span data-ttu-id="60bb3-1524">Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1524">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="60bb3-1525">Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1525">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="60bb3-1526">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="60bb3-1526">Data Lake Analytics</span></span>

* <span data-ttu-id="60bb3-1527">Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1527">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="60bb3-1528">`dla job pipeline show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1528">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="60bb3-1529">`dla job recurrence list` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1529">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="60bb3-1530">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="60bb3-1530">Data Lake Store</span></span>

* <span data-ttu-id="60bb3-1531">Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1531">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="60bb3-1532">Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln</span><span class="sxs-lookup"><span data-stu-id="60bb3-1532">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="60bb3-1533">Befehl `dls enable-key-vault` hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1533">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="60bb3-1534">Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1534">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="60bb3-1535">Interaktiv</span><span class="sxs-lookup"><span data-stu-id="60bb3-1535">Interactive</span></span>

* <span data-ttu-id="60bb3-1536">Startzeit durch Verwendung zwischengespeicherter Befehle verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1536">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="60bb3-1537">Testabdeckung verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1537">Increased test coverage</span></span>
* <span data-ttu-id="60bb3-1538">?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-1538">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="60bb3-1539">Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1539">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="60bb3-1540">`--version` als Parameter für den interaktiven Modus zugelassen (3645)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1540">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="60bb3-1541">Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1541">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="60bb3-1542">Statusmeldung für Vorlagenbereitstellungen (3510)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1542">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="60bb3-1543">Flag `--progress` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1543">Added `--progress` flag</span></span>
* <span data-ttu-id="60bb3-1544">`--debug` und `--verbose` aus Abschlüssen entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1544">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="60bb3-1545">`interactive` aus Abschlüssen entfernt (3324)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1545">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="60bb3-1546">IoT</span><span class="sxs-lookup"><span data-stu-id="60bb3-1546">IoT</span></span>

* <span data-ttu-id="60bb3-1547">Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien</span><span class="sxs-lookup"><span data-stu-id="60bb3-1547">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="60bb3-1548">(3934)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1548">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="60bb3-1549">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="60bb3-1549">Key vault</span></span>

* <span data-ttu-id="60bb3-1550">Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:</span><span class="sxs-lookup"><span data-stu-id="60bb3-1550">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="60bb3-1551">`keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1551">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="60bb3-1552">`keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1552">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="60bb3-1553">`keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1553">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="60bb3-1554">`keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1554">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="60bb3-1555">Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1555">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="60bb3-1556">Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1556">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="60bb3-1557">(3307)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1557">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="60bb3-1558">Labor</span><span class="sxs-lookup"><span data-stu-id="60bb3-1558">Lab</span></span>

* <span data-ttu-id="60bb3-1559">Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1559">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="60bb3-1560">Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1560">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="60bb3-1561">Überwachen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1561">Monitor</span></span>

* <span data-ttu-id="60bb3-1562">Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1562">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="60bb3-1563">`monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1563">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="60bb3-1564">`monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1564">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="60bb3-1565">`monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1565">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="60bb3-1566">`monitor alert-rules` in `monitor alert` umbenannt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1566">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="60bb3-1567">`monitor alert create` geändert:</span><span class="sxs-lookup"><span data-stu-id="60bb3-1567">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="60bb3-1568">Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1568">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="60bb3-1569">Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung</span><span class="sxs-lookup"><span data-stu-id="60bb3-1569">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="60bb3-1570">`location` nicht mehr erforderlich</span><span class="sxs-lookup"><span data-stu-id="60bb3-1570">`location` no longer required</span></span>
  * <span data-ttu-id="60bb3-1571">Hinzufügung von Namen- und ID-Unterstützung für Ziel</span><span class="sxs-lookup"><span data-stu-id="60bb3-1571">Add name and ID support for target</span></span>
  * <span data-ttu-id="60bb3-1572">Entfernung von `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1572">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="60bb3-1573">Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1573">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="60bb3-1574">`description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1574">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="60bb3-1575">Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats</span><span class="sxs-lookup"><span data-stu-id="60bb3-1575">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="60bb3-1576">Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1576">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="60bb3-1577">Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1577">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-1578">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1578">Network</span></span>

* <span data-ttu-id="60bb3-1579">Befehl `list-private-access-services` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1579">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="60bb3-1580">Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1580">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="60bb3-1581">Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte</span><span class="sxs-lookup"><span data-stu-id="60bb3-1581">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="60bb3-1582">Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte</span><span class="sxs-lookup"><span data-stu-id="60bb3-1582">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="60bb3-1583">Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-1583">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="60bb3-1584">Befehle vom Typ `application-gateway redirect-config` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1584">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="60bb3-1585">Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1585">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="60bb3-1586">Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1586">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="60bb3-1587">Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1587">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="60bb3-1588">Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1588">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="60bb3-1589">Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1589">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="60bb3-1590">Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1590">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="60bb3-1591">Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1591">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="60bb3-1592">Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1592">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="60bb3-1593">Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1593">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="60bb3-1594">Argument `--internal-dns-name-suffix` von `nic create` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1594">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="60bb3-1595">Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Unterstützung für „--dns-servers“ hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1595">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="60bb3-1596">Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde</span><span class="sxs-lookup"><span data-stu-id="60bb3-1596">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="60bb3-1597">Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1597">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="60bb3-1598">Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1598">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="60bb3-1599">Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1599">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="60bb3-1600">Fehler mit Standardlogik von `network watcher show-topology` korrigiert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1600">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="60bb3-1601">Ausgabeformatierung für `network list-usages` verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1601">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="60bb3-1602">Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1602">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="60bb3-1603">Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1603">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="60bb3-1604">Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1604">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="60bb3-1605">Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1605">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="60bb3-1606">Profil</span><span class="sxs-lookup"><span data-stu-id="60bb3-1606">Profile</span></span>

* <span data-ttu-id="60bb3-1607">Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität</span><span class="sxs-lookup"><span data-stu-id="60bb3-1607">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="60bb3-1608">Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat</span><span class="sxs-lookup"><span data-stu-id="60bb3-1608">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="60bb3-1609">Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“</span><span class="sxs-lookup"><span data-stu-id="60bb3-1609">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="60bb3-1610">Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1610">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="60bb3-1611">Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements</span><span class="sxs-lookup"><span data-stu-id="60bb3-1611">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="60bb3-1612">RDBMS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1612">RDBMS</span></span>

* <span data-ttu-id="60bb3-1613">Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1613">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="60bb3-1614">Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1614">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="60bb3-1615">Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1615">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="60bb3-1616">MySQL- und PostgreSQL-Hilfe korrigiert (3369)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1616">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-1617">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-1617">Resource</span></span>

* <span data-ttu-id="60bb3-1618">Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1618">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="60bb3-1619">Analyse der Syntax `--parameters KEY=VALUE` verbessert</span><span class="sxs-lookup"><span data-stu-id="60bb3-1619">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="60bb3-1620">Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1620">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="60bb3-1621">Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1621">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="60bb3-1622">Einige Analyse- und Fehlermeldungen korrigiert (3584)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1622">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="60bb3-1623">Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1623">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="60bb3-1624">Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1624">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="60bb3-1625">Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1625">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="60bb3-1626">Rolle</span><span class="sxs-lookup"><span data-stu-id="60bb3-1626">Role</span></span>

* <span data-ttu-id="60bb3-1627">Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1627">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="60bb3-1628">Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1628">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="60bb3-1629">Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente</span><span class="sxs-lookup"><span data-stu-id="60bb3-1629">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="60bb3-1630">Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1630">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="60bb3-1631">Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1631">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="60bb3-1632">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="60bb3-1632">Service Fabric</span></span>
* <span data-ttu-id="60bb3-1633">Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1633">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="60bb3-1634">Tests für Service Fabric-Befehle hinzugefügt (3424)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1634">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="60bb3-1635">Zahlreiche Service Fabric-Befehle korrigiert (3234)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1635">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-1636">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-1636">SQL</span></span>

* <span data-ttu-id="60bb3-1637">Fehlerhaften Parameter `--identity` für `sql server create` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1637">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="60bb3-1638">Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1638">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="60bb3-1639">Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1639">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-1640">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-1640">Storage</span></span>

* <span data-ttu-id="60bb3-1641">Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1641">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="60bb3-1642">Erstellung eines reinen HTTPS-Speicherkontos ermöglicht</span><span class="sxs-lookup"><span data-stu-id="60bb3-1642">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="60bb3-1643">Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1643">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="60bb3-1644">Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1644">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="60bb3-1645">Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1645">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="60bb3-1646">Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1646">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1647">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1647">VM</span></span>

* <span data-ttu-id="60bb3-1648">Unterstützung der NSG-Konfiguration</span><span class="sxs-lookup"><span data-stu-id="60bb3-1648">Support configuring nsg</span></span>
* <span data-ttu-id="60bb3-1649">Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde</span><span class="sxs-lookup"><span data-stu-id="60bb3-1649">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="60bb3-1650">Unterstützung verwalteter Dienstidentitäten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1650">Support managed service identities</span></span>
* <span data-ttu-id="60bb3-1651">Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte</span><span class="sxs-lookup"><span data-stu-id="60bb3-1651">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="60bb3-1652">Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1652">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="60bb3-1653">10. Mai 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1653">May 10, 2017</span></span>

<span data-ttu-id="60bb3-1654">Version 2.0.6</span><span class="sxs-lookup"><span data-stu-id="60bb3-1654">Version 2.0.6</span></span>

* <span data-ttu-id="60bb3-1655">Umbenennen von „documentdb“ in „cosmosdb“</span><span class="sxs-lookup"><span data-stu-id="60bb3-1655">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="60bb3-1656">Hinzufügen von rdbms (mysql, postgres)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1656">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="60bb3-1657">Einbeziehen der Data Lake Analytics- und Data Lake Store-Module</span><span class="sxs-lookup"><span data-stu-id="60bb3-1657">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="60bb3-1658">Einbeziehen des Cognitive Services-Moduls</span><span class="sxs-lookup"><span data-stu-id="60bb3-1658">Include Cognitive Services module</span></span>
* <span data-ttu-id="60bb3-1659">Einbeziehen des Service Fabric-Moduls</span><span class="sxs-lookup"><span data-stu-id="60bb3-1659">Include Service Fabric module</span></span>
* <span data-ttu-id="60bb3-1660">Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1660">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="60bb3-1661">Hinzufügen von Unterstützung für CDN-Befehle</span><span class="sxs-lookup"><span data-stu-id="60bb3-1661">Add support for CDN commands</span></span>
* <span data-ttu-id="60bb3-1662">Entfernen des Containermoduls</span><span class="sxs-lookup"><span data-stu-id="60bb3-1662">Remove Container module</span></span>
* <span data-ttu-id="60bb3-1663">Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1663">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="60bb3-1664">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1664">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="60bb3-1665">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-1665">Core</span></span>

* <span data-ttu-id="60bb3-1666">Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung</span><span class="sxs-lookup"><span data-stu-id="60bb3-1666">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="60bb3-1667">Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1667">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="60bb3-1668">Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1668">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="60bb3-1669">Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1669">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="60bb3-1670">Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1670">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="60bb3-1671">Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1671">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="60bb3-1672">Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1672">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="60bb3-1673">Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1673">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="60bb3-1674">Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1674">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="60bb3-1675">Core: Verbesserte Leistung</span><span class="sxs-lookup"><span data-stu-id="60bb3-1675">core: Improved performance</span></span>
* <span data-ttu-id="60bb3-1676">Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1676">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="60bb3-1677">Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-1677">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-1678">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1678">ACS</span></span>

* <span data-ttu-id="60bb3-1679">Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="60bb3-1679">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="60bb3-1680">Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung</span><span class="sxs-lookup"><span data-stu-id="60bb3-1680">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="60bb3-1681">Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1681">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="60bb3-1682">Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1682">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-1683">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-1683">AppService</span></span>

* <span data-ttu-id="60bb3-1684">functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1684">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="60bb3-1685">Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“</span><span class="sxs-lookup"><span data-stu-id="60bb3-1685">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="60bb3-1686">Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1686">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="60bb3-1687">Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps</span><span class="sxs-lookup"><span data-stu-id="60bb3-1687">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="60bb3-1688">Verfügbarmachen von „webapp list-runtimes“</span><span class="sxs-lookup"><span data-stu-id="60bb3-1688">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="60bb3-1689">Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1689">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="60bb3-1690">Unterstützen des Slottauschs mit Vorschau</span><span class="sxs-lookup"><span data-stu-id="60bb3-1690">support slot swap with preview</span></span>
* <span data-ttu-id="60bb3-1691">Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1691">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="60bb3-1692">Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1692">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="60bb3-1693">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="60bb3-1693">CosmosDB</span></span>

* <span data-ttu-id="60bb3-1694">Umbenennen des documentdb-Moduls in cosmosdb</span><span class="sxs-lookup"><span data-stu-id="60bb3-1694">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="60bb3-1695">Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung</span><span class="sxs-lookup"><span data-stu-id="60bb3-1695">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="60bb3-1696">Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1696">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="60bb3-1697">Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie</span><span class="sxs-lookup"><span data-stu-id="60bb3-1697">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="60bb3-1698">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="60bb3-1698">Data Lake Analytics</span></span>

* <span data-ttu-id="60bb3-1699">Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst</span><span class="sxs-lookup"><span data-stu-id="60bb3-1699">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="60bb3-1700">Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“</span><span class="sxs-lookup"><span data-stu-id="60bb3-1700">Add support for new catalog item type: package.</span></span> <span data-ttu-id="60bb3-1701">Zugriff über: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1701">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="60bb3-1702">Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):</span><span class="sxs-lookup"><span data-stu-id="60bb3-1702">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="60bb3-1703">Table</span><span class="sxs-lookup"><span data-stu-id="60bb3-1703">Table</span></span>
  * <span data-ttu-id="60bb3-1704">Tabellenwertfunktion</span><span class="sxs-lookup"><span data-stu-id="60bb3-1704">Table valued function</span></span>
  * <span data-ttu-id="60bb3-1705">Sicht</span><span class="sxs-lookup"><span data-stu-id="60bb3-1705">View</span></span>
  * <span data-ttu-id="60bb3-1706">Tabellenstatistiken.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1706">Table Statistics.</span></span> <span data-ttu-id="60bb3-1707">Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1707">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="60bb3-1708">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="60bb3-1708">Data Lake Store</span></span>

* <span data-ttu-id="60bb3-1709">Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-1709">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="60bb3-1710">Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1710">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="60bb3-1711">Fehlende Hilfe für Zugriffsanzeige</span><span class="sxs-lookup"><span data-stu-id="60bb3-1711">missed help for access show.</span></span> <span data-ttu-id="60bb3-1712">hinzugefügt</span><span class="sxs-lookup"><span data-stu-id="60bb3-1712">adding it.</span></span> <span data-ttu-id="60bb3-1713">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1713">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="60bb3-1714">Suchen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1714">Find</span></span>

* <span data-ttu-id="60bb3-1715">Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex</span><span class="sxs-lookup"><span data-stu-id="60bb3-1715">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="60bb3-1716">KeyVault</span><span class="sxs-lookup"><span data-stu-id="60bb3-1716">KeyVault</span></span>

* <span data-ttu-id="60bb3-1717">BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1717">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="60bb3-1718">BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1718">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="60bb3-1719">Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben</span><span class="sxs-lookup"><span data-stu-id="60bb3-1719">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="60bb3-1720">Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht</span><span class="sxs-lookup"><span data-stu-id="60bb3-1720">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="60bb3-1721">Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1721">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="60bb3-1722">Labor</span><span class="sxs-lookup"><span data-stu-id="60bb3-1722">Lab</span></span>

* <span data-ttu-id="60bb3-1723">Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung</span><span class="sxs-lookup"><span data-stu-id="60bb3-1723">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="60bb3-1724">Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor</span><span class="sxs-lookup"><span data-stu-id="60bb3-1724">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="60bb3-1725">Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern</span><span class="sxs-lookup"><span data-stu-id="60bb3-1725">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="60bb3-1726">Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors</span><span class="sxs-lookup"><span data-stu-id="60bb3-1726">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="60bb3-1727">Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor</span><span class="sxs-lookup"><span data-stu-id="60bb3-1727">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="60bb3-1728">Überwachen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1728">Monitor</span></span>

* <span data-ttu-id="60bb3-1729">Programmfehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1729">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="60bb3-1730">Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1730">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="60bb3-1731">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1731">Network</span></span>

* <span data-ttu-id="60bb3-1732">Hinzufügen des `network watcher test-connectivity`-Befehls</span><span class="sxs-lookup"><span data-stu-id="60bb3-1732">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="60bb3-1733">Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1733">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="60bb3-1734">Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich</span><span class="sxs-lookup"><span data-stu-id="60bb3-1734">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="60bb3-1735">Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1735">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="60bb3-1736">Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln</span><span class="sxs-lookup"><span data-stu-id="60bb3-1736">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="60bb3-1737">Hinzufügen von Unterstützung für geografisches TrafficManager-Routing</span><span class="sxs-lookup"><span data-stu-id="60bb3-1737">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="60bb3-1738">Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1738">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="60bb3-1739">Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1739">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="60bb3-1740">Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1740">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="60bb3-1741">Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways</span><span class="sxs-lookup"><span data-stu-id="60bb3-1741">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="60bb3-1742">Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1742">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="60bb3-1743">BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1743">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="60bb3-1744">Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde</span><span class="sxs-lookup"><span data-stu-id="60bb3-1744">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="60bb3-1745">Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden</span><span class="sxs-lookup"><span data-stu-id="60bb3-1745">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="60bb3-1746">Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte</span><span class="sxs-lookup"><span data-stu-id="60bb3-1746">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="60bb3-1747">Hinzufügen von Network Watcher-Vorschaubefehlen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1747">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="60bb3-1748">Profil</span><span class="sxs-lookup"><span data-stu-id="60bb3-1748">Profile</span></span>

* <span data-ttu-id="60bb3-1749">Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1749">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="60bb3-1750">Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1750">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="60bb3-1751">Redis</span><span class="sxs-lookup"><span data-stu-id="60bb3-1751">Redis</span></span>

* <span data-ttu-id="60bb3-1752">Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-1752">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="60bb3-1753">Verwerfen des Befehls „update-settings“</span><span class="sxs-lookup"><span data-stu-id="60bb3-1753">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="60bb3-1754">Ressource</span><span class="sxs-lookup"><span data-stu-id="60bb3-1754">Resource</span></span>

* <span data-ttu-id="60bb3-1755">Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1755">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="60bb3-1756">Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1756">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="60bb3-1757">Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1757">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="60bb3-1758">Korrigieren der Ressourcenanalyse und der API-Versionssuche</span><span class="sxs-lookup"><span data-stu-id="60bb3-1758">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="60bb3-1759">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1759">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="60bb3-1760">Hinzufügen von Dokumenten für „az lock update“</span><span class="sxs-lookup"><span data-stu-id="60bb3-1760">Add docs for az lock update.</span></span> <span data-ttu-id="60bb3-1761">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1761">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="60bb3-1762">Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1762">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="60bb3-1763">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1763">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="60bb3-1764">[Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen</span><span class="sxs-lookup"><span data-stu-id="60bb3-1764">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="60bb3-1765">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1765">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="60bb3-1766">Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1766">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="60bb3-1767">Rolle</span><span class="sxs-lookup"><span data-stu-id="60bb3-1767">Role</span></span>

* <span data-ttu-id="60bb3-1768">create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1768">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="60bb3-1769">RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1769">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="60bb3-1770">Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1770">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="60bb3-1771">create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird</span><span class="sxs-lookup"><span data-stu-id="60bb3-1771">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="60bb3-1772">SQL</span><span class="sxs-lookup"><span data-stu-id="60bb3-1772">SQL</span></span>

* <span data-ttu-id="60bb3-1773">Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“</span><span class="sxs-lookup"><span data-stu-id="60bb3-1773">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="60bb3-1774">SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1774">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="60bb3-1775">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-1775">Storage</span></span>

* <span data-ttu-id="60bb3-1776">Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1776">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="60bb3-1777">Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs</span><span class="sxs-lookup"><span data-stu-id="60bb3-1777">Add support for incremental blob copy</span></span>
* <span data-ttu-id="60bb3-1778">Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs</span><span class="sxs-lookup"><span data-stu-id="60bb3-1778">Add support for large block blob upload</span></span>
* <span data-ttu-id="60bb3-1779">Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist</span><span class="sxs-lookup"><span data-stu-id="60bb3-1779">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1780">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1780">VM</span></span>

* <span data-ttu-id="60bb3-1781">avail-set: Festlegen der UD- und FD-Domänenanzahl als optional</span><span class="sxs-lookup"><span data-stu-id="60bb3-1781">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="60bb3-1782">Hinweis zu VM-Befehlen in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:</span><span class="sxs-lookup"><span data-stu-id="60bb3-1782">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="60bb3-1783">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="60bb3-1783">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="60bb3-1784">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1784">az vm/vmss disk</span></span>
  3. <span data-ttu-id="60bb3-1785">Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1785">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="60bb3-1786">vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren</span><span class="sxs-lookup"><span data-stu-id="60bb3-1786">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="60bb3-1787">vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1787">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="60bb3-1788">3. April 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1788">April 3, 2017</span></span>

<span data-ttu-id="60bb3-1789">Version 2.0.2</span><span class="sxs-lookup"><span data-stu-id="60bb3-1789">Version 2.0.2</span></span>

<span data-ttu-id="60bb3-1790">In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1790">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="60bb3-1791">Core</span><span class="sxs-lookup"><span data-stu-id="60bb3-1791">Core</span></span>

* <span data-ttu-id="60bb3-1792">Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste</span><span class="sxs-lookup"><span data-stu-id="60bb3-1792">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="60bb3-1793">Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1793">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="60bb3-1794">Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1794">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="60bb3-1795">Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1795">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="60bb3-1796">Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1796">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="60bb3-1797">Hinzufügen der Meldung zu fehlenden Vorlagenparametern</span><span class="sxs-lookup"><span data-stu-id="60bb3-1797">Add prompting for missing template parameters.</span></span> <span data-ttu-id="60bb3-1798">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1798">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="60bb3-1799">Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1799">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="60bb3-1800">Unterstützen der Anmeldung an einem bestimmten Mandanten</span><span class="sxs-lookup"><span data-stu-id="60bb3-1800">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="60bb3-1801">ACS</span><span class="sxs-lookup"><span data-stu-id="60bb3-1801">ACS</span></span>

* <span data-ttu-id="60bb3-1802">[ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1802">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="60bb3-1803">Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel</span><span class="sxs-lookup"><span data-stu-id="60bb3-1803">Add support for ssh key password prompting.</span></span> <span data-ttu-id="60bb3-1804">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1804">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="60bb3-1805">Hinzufügen von Unterstützung für Windows-Cluster</span><span class="sxs-lookup"><span data-stu-id="60bb3-1805">Add support for windows clusters.</span></span> <span data-ttu-id="60bb3-1806">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1806">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="60bb3-1807">Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“</span><span class="sxs-lookup"><span data-stu-id="60bb3-1807">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="60bb3-1808">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1808">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="60bb3-1809">AppService</span><span class="sxs-lookup"><span data-stu-id="60bb3-1809">AppService</span></span>

* <span data-ttu-id="60bb3-1810">appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1810">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="60bb3-1811">appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1811">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="60bb3-1812">appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1812">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="60bb3-1813">AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1813">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="60bb3-1814">DataLake</span><span class="sxs-lookup"><span data-stu-id="60bb3-1814">DataLake</span></span>

* <span data-ttu-id="60bb3-1815">Erste Version des Data Lake Analytics-Moduls</span><span class="sxs-lookup"><span data-stu-id="60bb3-1815">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="60bb3-1816">Erste Version des Data Lake Store-Moduls</span><span class="sxs-lookup"><span data-stu-id="60bb3-1816">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="60bb3-1817">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="60bb3-1817">DocuemntDB</span></span>

* <span data-ttu-id="60bb3-1818">DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1818">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="60bb3-1819">VM</span><span class="sxs-lookup"><span data-stu-id="60bb3-1819">VM</span></span>

* <span data-ttu-id="60bb3-1820">[Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1820">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="60bb3-1821">[VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1821">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="60bb3-1822">VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1822">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="60bb3-1823">Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1823">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="60bb3-1824">VM-Skalierungsgruppe: Unterstützung von „\*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1824">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="60bb3-1825">Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1825">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="60bb3-1826">Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="60bb3-1826">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="60bb3-1827">27. Februar 2017</span><span class="sxs-lookup"><span data-stu-id="60bb3-1827">February 27, 2017</span></span>

<span data-ttu-id="60bb3-1828">Version 2.0.0</span><span class="sxs-lookup"><span data-stu-id="60bb3-1828">Version 2.0.0</span></span>

<span data-ttu-id="60bb3-1829">Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:</span><span class="sxs-lookup"><span data-stu-id="60bb3-1829">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="60bb3-1830">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1830">Container Service (acs)</span></span>
- <span data-ttu-id="60bb3-1831">Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1831">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="60bb3-1832">Netzwerk</span><span class="sxs-lookup"><span data-stu-id="60bb3-1832">Networking</span></span>
- <span data-ttu-id="60bb3-1833">Speicher</span><span class="sxs-lookup"><span data-stu-id="60bb3-1833">Storage</span></span>

<span data-ttu-id="60bb3-1834">Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1834">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="60bb3-1835">Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1835">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="60bb3-1836">Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1836">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="60bb3-1837">Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.</span><span class="sxs-lookup"><span data-stu-id="60bb3-1837">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="60bb3-1838">Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="60bb3-1838">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="60bb3-1839">Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:</span><span class="sxs-lookup"><span data-stu-id="60bb3-1839">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="60bb3-1840">Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1840">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="60bb3-1841">Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="60bb3-1841">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="60bb3-1842">Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`</span><span class="sxs-lookup"><span data-stu-id="60bb3-1842">Provide feedback from the command line with the `az feedback` command</span></span>


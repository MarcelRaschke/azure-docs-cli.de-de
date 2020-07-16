---
title: Versionshinweise für die Azure CLI
description: Enthält Informationen zu den aktuellen Updates der Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 07/14/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: cf9c4e1a86b3315d45a7533f67b731ee2f3d6bc0
ms.sourcegitcommit: 857d0f19fd87d37d134efdf0dda0e7003260938b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/14/2020
ms.locfileid: "86308677"
---
# <a name="azure-cli-release-notes"></a>Versionshinweise für die Azure CLI

# <a name="current-release-notes"></a>[Aktuelle Versionshinweise](#tab/azure-cli)

## <a name="july-14-2020"></a>14. Juli 2020

Version 2.9.0

### <a name="acr"></a>ACR

* Verarbeiten des Protokollartefaktlinks aus der Registrierung zum Streamen von Protokollen
* Helm2-Befehle als veraltet kennzeichnen

### <a name="aks"></a>AKS

* `az aks create`: Argument „--enable-aad“ hinzufügen
* `az aks update`: Argument „--enable-aad“ hinzufügen

### <a name="apim"></a>APIM

* Allgemeine Befehle vom Typ „az apim api“ hinzugefügt

### <a name="appconfig"></a>AppConfig

* Beispiel für die Verwendung von „--fields“ in AppConfig-Revision hinzufügen

### <a name="appservice"></a>AppService

* `az functionapp create`: Unterstützung für Java 11 und PowerShell 7 hinzugefügt. Unterstützung für Stapel-API hinzugefügt.
* Behebung von Nr. 14208: Erstellen einer App mit mehreren Containern erzeugt einen Fehler
* Korrektur von „az webapp create“ – hartcodierte Laufzeitstapel verwenden

### <a name="arm"></a>ARM

* `az resource tag`: Behebung des Problems beim Taggen von Ressourcen mit dem Ressourcentyp `Microsoft.ContainerInstance/containerGroups`

### <a name="compute"></a>Compute

* Datenträgerversion aktualisieren 2020-05-01, Compute 2020-06-01
* Doppelte Verschlüsselung des Datenträgerverschlüsselungssatzes
* `az vmss update`: Unterstützung für das Angeben eines mandantenübergreifendes Image.
* `az sig image-version create`: Unterstützung für das Angeben eines mandantenübergreifendes Image.
* vm/vmss create: Verschlüsselung von Cache und Daten während der Übertragung für (Betriebssystem-)Datenträger und temporäre Datenträger für VM und VMSS
* Vorgang „simulate-eviction“ für VM und VMSS hinzufügen

### <a name="cosmosdb"></a>CosmosDB

* Aktuelle Features: Autoscale, IpRules, EnableFreeTier und EnableAnalyticalStorage

### <a name="eventgrid"></a>EventGrid

* CLI-Unterstützung für 2020-04-01-preview hinzufügen und Previewfunktionen mit „is_Preview=True“ kennzeichnen

### <a name="find"></a>Suchen

* Behebung von Nr. 14094 „az find“: Abfragen schlagen fehl, wenn nicht angemeldet und Telemetrie deaktiviert

### <a name="hdinsight"></a>HDInsight

* Zwei Befehle zur Unterstützung der Neustartfunktion für HDInsight-Knoten hinzufügen

### <a name="monitor"></a>Überwachen

* Vorschaukennzeichnung für Befehle unter Log Analytics-Arbeitsbereich entfernen
* `az monitor diagnostic-settings subscription`: Diagnoseeinstellungen für Abonnement unterstützen
* `az monitor metrics`: „,“ und „|“ in Metrikname unterstützen
* `az monitor log-analytics workspace data-export`: Log Analytics-Datenexport unterstützen

### <a name="network"></a>Netzwerk

* `az network application-gateway frontend-ip update`: Parameter „--public-ip-address“ als veraltet markieren
* „azure-mgmt-network“ auf 11.0.0 aktualisieren
* `az network express-route gateway connection`: Routingkonfiguration unterstützen
* `az network virtual-appliance`: Virtuelle Azure-Netzwerkgerät unterstützen.
* Application Gateway-Unterstützung der Funktion für private Links

### <a name="policyinsights"></a>PolicyInsights

* `az policy state`: Befehl „trigger-scan“ zu Auswertungen der Compliance von Auslöserrichtinien hinzufügen
* `az policy state list`: Versionen von Richtlinienentitäten in jedem Compliancedatensatz verfügbar machen

### <a name="profile"></a>Profil

* `az account get-access-token`: „expiresOn“ für verwaltete Identität anzeigen

### <a name="rdbms"></a>RDBMS

* TLS-Mindestversion unterstützen
* Infrastrukturverschlüsselung für Azure Postgres und MySQL hinzufügen

### <a name="security"></a>Sicherheit

* Befehl „allowed_connections“ hinzufügen
* Befehle für adaptive Netzwerkhärtung hinzufügen
* Befehle vom Typ „adaptive_application_controls“ hinzufügen
* Hinzufügen von „az security iot-solution“/„iot-alerts“/„iot-recommendations“/„iot-analytics“ REST zu Azure CLI
* CLI für Einhaltung gesetzlicher Bestimmungen hinzufügen

### <a name="signalr"></a>SignalR

* Features einschließlich der Verwaltung privater Endpunktverbindungen, Netzwerkregeln und Upstream hinzufügen

### <a name="sql"></a>SQL

* `az sql mi create`, `az sql mi update`: Parameter `--tags` zur Unterstützung von Ressourcenkennzeichnung hinzufügen
* `az sql mi failover`: Failover vom primären oder sekundären Punkt unterstützen

### <a name="storage"></a>Storage

* `az storage account create/update`: „--allow-blob-public-access“ hinzufügen, um den öffentlichen Zugriff für Blob und Container zuzulassen oder zu unterbinden
* `az storage account create/update`: `--min-tls-version` hinzufügen, um das Festlegen der TLS-Mindestversion für Anforderungen an den Speicher zu unterstützen.
* Token-Anmeldeinformationen zum Einchecken entfernen
* Namen des Speicherkontos in Beispielen korrigieren

### <a name="webapp"></a>Webapp

* Fehlerbehebung: „az webapp log deployment show -“ gibt Bereitstellungsprotokolle anstatt von Protokollmetadaten zurück
* Fehlerbehebung: „az webapp vnet-integration“ hinzufügen – Fehlerbehandlung korrigieren bei ungültigem VNET-Namen, VNET-Ressourcen-ID unterstützen

## <a name="june-23-2020"></a>23. Juni 2020

Version 2.8.0

### <a name="acr"></a>ACR

* Unterstützung für Deaktivierung des Regionsendpunkts/Routings hinzugefügt
* [BREAKING CHANGE] `az acr login --expose-token` akzeptiert Benutzername und Kennwort nicht.

### <a name="acs"></a>ACS

* Privater Cluster und API „2019-10-27-preview“ entfernt

### <a name="aks"></a>AKS

* Unterstützung: Ja, für „az aks upgrade“
* „Änderung der Standard-VM-SKU in Standard_D2s_v3 (Nr. 13541)“ wiederhergestellt
* „az aks update --uptime-sla“ hinzugefügt
* Tippfehler im Befehl „az aks update“ korrigiert
* Änderung, um einen Agentpool mit 0 Knoten zu unterstützen und die manuelle Skalierung für einen Pool mit CAS-Aktivierung zu blockieren
* Tippfehler in VirtualMachineScaleSets korrigiert und Verweise auf Kubernetes-Versionen aktualisiert

### <a name="ams"></a>AMS

* ÄNDERUNG: Hilfetext für Parameter „--expiry“

### <a name="appservice"></a>AppService

* `az webapp log deployment show`: Anzeigen des aktuellen Bereitstellungsprotokolls oder der Bereitstellungsprotokolle einer bestimmten Bereitstellung, wenn die Bereitstellungs-ID angegeben ist
* `az webapp log deployment list`: Liste der verfügbaren Bereitstellungsprotokolle
* Behebung: Oberflächenfehler bei Angabe eines ungültigen Web-App-Namens
* Nr. 13261 korrigiert: „az webapp list-runtimes“ nutzt eine statische Liste, bis die neue API für verfügbare Stapel zur Verfügung steht
* `az appservice ase create`: Erstellungsproblem behoben (Nr. 13361)
* `az appservice ase list-addresses`: SDK-Änderung korrigiert (Nr. 13140)
* Web-App-/Sloterstellung für Windows-Container korrigiert
* `az webapp auth update`: Optionaler Parameter zum Aktualisieren der Laufzeitversion hinzugefügt
* Unterstützung für das Auflisten, Löschen, Genehmigen und Ablehnen der Verbindung mit privatem Endpunkt für eine Web-App in der CLI
* Behebung Nr. 13888: Unterstützung für Static Web Apps hinzugefügt: Befehle zum Abrufen, Auflisten und Erstellen
* Fehlermeldungen für die SSH-Tunnelverbindung verbessert

### <a name="arm"></a>ARM

* `az tag`: Beispiele für „-h“ hinzugefügt
* `az deployment group/sub what-if`: Parameter „--exclude-change-types/-x“ hinzugefügt
* `az deployment group/sub/mg/tenant create`: Parameter „--what-if-exclude-change-types/-x“ hinzugefügt
* `az deployment group/sub/mg/tenant validate`: Anzeigen von Fehlermeldungen in einem besseren Format
* `az group export`: Neue Parameter `--skip-resource-name-params` und `--skip-all-params` hinzugefügt, um das Überspringen der Parametrisierung zu unterstützen
* API „az feature unregister“ hinzugefügt

### <a name="aro"></a>ARO

* „Public“/„Private“ zu Parametern zur Unterstützung bei Eingangs-/APIServer-Sichtbarkeit hinzugefügt

### <a name="batch"></a>Batch

* `az batch account create`: Neuer Parameter `--public-network-access` hinzugefügt
* `az batch account create`: Neuer Parameter `--identity-type` hinzugefügt
* `az batch account set`: Neuer Parameter `--identity-type` hinzugefügt
* [BREAKING CHANGE] az batch pool create: Bei der Erstellung eines Pools mithilfe eines benutzerdefinierten Images kann die Eigenschaft „--image“ nun ausschließlich auf ein Shared Image Gallery-Image verweisen.
* [BREAKING CHANGE] az batch pool create: Bei der Erstellung eines Pools mit der Option „--json-file“ und Angabe einer Netzwerkkonfiguration (networkConfiguration) wurde die Eigenschaft „publicIPs“ in die neue Eigenschaft „publicIPAddressConfiguration“ verschoben. Diese neue Eigenschaft unterstützt außerdem die neue Eigenschaft „ipAddressProvisioningType“. Diese gibt an, wie der Pool IP-Adressen und die Eigenschaft „publicIPs“ zuordnen muss, um die Konfiguration einer Liste mit PublicIP-Ressourcen zu ermöglichen, die bei der Festlegung von „ipAddressProvisioningType“ auf „UserManaged“ verwendet werden sollen.
* `az network private-link-resource`: Unterstützung für die Microsoft.Batch-Ressource „batchAccount“ hinzugefügt
* `az network private-endpoint-connection`: Unterstützung für die Microsoft.Batch-Ressource „batchAccount“ hinzugefügt

### <a name="cdn"></a>CDN

* `az cdn custom-domain enable-https`: Unterstützung für BYOC hinzugefügt
* `az cdn custom-domain enable-https`: Aktivierung von benutzerdefiniertem HTTPS mit CDN-verwalteten Zertifikaten für die SKUs Standard_Verizon und Standard_Microsoft korrigiert

### <a name="cognitive-services"></a>Cognitive Services

* [BREAKING CHANGE] `az cognitiveservices account` besitzt nun eine einheitliche Struktur für alle Befehle.
* `az cognitiveservices account identity`: Identitätsverwaltung für Cognitive Services hinzugefügt

### <a name="compute"></a>Compute

* `az image builder`: API-Version auf 2020-02-14 aktualisiert
* `az image builder create`: `--identity` zur Unterstützung der Identitätskonfiguration hinzugefügt
* `az image builder customizer add`: Unterstützung für Windows Update-Anpassung
* Neuer Befehl `az image builder cancel`
* Anzeigen einer Warnung, wenn ein Benutzer eine VMSS bereitstellt, die an eine bestimmte (und nicht an die neueste) Imageversion angeheftet ist

### <a name="cosmos-db"></a>Cosmos DB

* `az cosmosdb`: Befehl „exists“ zu Datenbank- und Containergruppen hinzugefügt
* Zulassen der Erstellung fester Sammlungen

### <a name="eventhub"></a>EventHub

* `az eventhubs namespace create` : Parameter für verwaltete Identität hinzugefügt

### <a name="extension"></a>Durchwahl

* „--version“ hinzugefügt, um die Installation über eine bestimmte Version zu unterstützen
* CLI-Erweiterungen dürfen nun Pakete im Namespace „azure“ enthalten.

### <a name="iot-hub"></a>IoT Hub

* [BREAKING CHANGE] az iot hub job: Veraltete job-Befehle entfernt

### <a name="keyvault"></a>KeyVault

* `az keyvault key import`: Unterstützt das Importieren aus Zeichenfolgen über zwei neue Parameter.
* Unterstützung der Ver- und Entschlüsselung von Zeichenfolgen/Bytes mit gespeicherten Schlüsseln

### <a name="monitor"></a>Überwachen

* Unterstützung für „no wait“ bei der Clustererstellung
* `az monitor log-analytics workspace saved-search`: Unterstützung neuer Befehle für gespeicherte Suche

### <a name="network"></a>Netzwerk

* `az network application-gateway address-pool update`: Hilfenachricht optimiert und Beispiele hinzugefügt
* `az network vnet create`: Unterstützung für das Argument „--nsg“
* `az network lb address-pool`: Unterstützung für das Erstellen eines Back-End-Pools des Lastenausgleichs mit Back-End-Adresse
* `az network application-gateway address-pool`: Korrektur für das Argument „--add“

### <a name="rbac"></a>RBAC

* `az ad sp create-for-rabc`: Unterstützung von Namen mit Leerzeichen, Schrägstrich und umgekehrtem Schrägstrich
* `az ad sp create-for-rbac`: Fehlermeldung optimiert, die angezeigt wird, wenn Benutzer einen ungültigen Bereich angeben

### <a name="security"></a>Sicherheit

* Befehle für Sicherheitsbewertungen hinzugefügt

### <a name="sql"></a>SQL

* `az sql db ltr-policy/ltr-backup`: Aktualisieren/Anzeigen der Richtlinie zur langfristigen Aufbewahrung, Anzeigen/Löschen von Sicherungen zur langfristigen Aufbewahrung, Wiederherstellen von Sicherungen zur langfristigen Aufbewahrung

### <a name="storage"></a>Storage

* Authentifizierungsproblem behoben, um das Abrufen eines Tokens für „--subscription“ zu unterstützen
* `az storage remove`: Problem Nr. 13459 behoben, um eine Ausnahme bei einem Vorgangsfehler auszulösen
* Probleme Nr. 13012, 13632 und 13657 behoben, um nicht verwendete Argumente für Befehle im Zusammenhang mit „generate-sas“ zu entfernen
* `az storage logging update`: Überprüfung für Protokollierungsversion hinzugefügt
* `az storage blob show`: Weitere Eigenschaften für Blob mit Track 2 SDK hinzugefügt
* Behebung Nr. 13708: Warnmeldung für Anmeldeinformationen optimiert
* `az storage share-rm create/update`: Unterstützung für NFS-Protokoll und Root-Squash hinzugefügt
* `az storage account create`: Unterstützung für doppelte Verschlüsselung hinzugefügt
* [BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: „--expiry“ und „--permissions“ als erforderlich festgelegt
* `az storage blob set-tier`: Migration zu Track 2, um das Festlegen der Aktivierungspriorität zu unterstützen

## <a name="june-02-2020"></a>2\. Juni 2020

Version 2.7.0

### <a name="acr"></a>ACR

* Tippfehler in einer Fehlermeldung der Tokenerstellung korrigiert

### <a name="aks"></a>AKS

* Standard-VM-SKU in „Standard_D2s_v3“ geändert
* Erstellung der Rollenzuweisung für MSI-Cluster plus benutzerdefiniertes Subnetz korrigiert

### <a name="appservice"></a>AppService

* Fehlerbehebung Nr. 12739: Von „az appservice list-locations“ werden einige ungültige Standorte zurückgegeben.

### <a name="arm"></a>ARM

* `az deployment`: Fehlerbehebung Nr. 13159 der fehlerhaften JSON-Meldung nach dem Entfernen von Kommentaren und nach dem Komprimieren
* `az resource tag`: Fehlerbehebung Nr. 13255 für das Markieren von Ressourcen mit dem Ressourcentyp `Microsoft.ContainerRegistry/registries/webhooks`
* Beispiele für das Ressourcenmodul verbessert

### <a name="aro"></a>ARO

* CLIError in das richtige Flag für „--worker-vm-disk-size-gb“ geändert

### <a name="eventhub"></a>EventHub

* Fehlerbehebung Nr. 12406: „intervalInSeconds“ wird von Argument „--capture-interval“ nicht aktualisiert.

### <a name="hdinsight"></a>HDInsight

* „get_json_object“ in „shell_safe_json_parse“ geändert

### <a name="monitor"></a>Überwachen

* `az monitor metrics alert`: Verschiedene Hilfemeldungen optimiert
* `az monitor diagnostic-settings create`: Unterstützung für das Argument „--export-to-resource-specific“
* Unterstützung für die Wiederherstellung von LA-Arbeitsbereichen

### <a name="network"></a>Netzwerk

* `az network dns zone`: Unterstützung des Bindestrichs (-)
* `az network vpn-connection ipsec-policy`: „--sa-lifetime“ und „--sa-max-size“ im Beispiel in höhere Werte geändert
* Netzwerk auf 2020-04-01 aktualisiert
* `az network private-endpoint-connection`: Unterstützung von Event Grid
* `az network express-route list-route-tables`: Fehler behoben, der dazu führte, dass Routen nicht als Tabelle aufgeführt werden konnten

### <a name="packaging"></a>Verpackung

* Ubuntu-Paket (Focal) hinzugefügt

### <a name="rbac"></a>RBAC

* `az ad sp credential reset`: Erstellung von Anmeldeinformationen geändert, um problematische Sonderzeichen zu vermeiden

### <a name="redis"></a>Redis

* Fehlerbehebung Nr. 13529: Dokumentation des Parameters „enable_non_ssl_port“ geändert

### <a name="storage"></a>Storage

* `az storage copy`: Parameter `--follow-symlinks` zur Unterstützung von symbolischen Verknüpfungen hinzugefügt
* Lokaler Kontext für Speicherkonto aktiviert
* `az storage logging`: Fehlerbehebung Nr. 11969: Fehlermeldung optimiert

## <a name="may-19-2020"></a>19. Mai 2020

Version 2.6.0

### <a name="acr"></a>ACR

* Standardtimeout von fünf Minuten für jede an ACR gesendete Anforderung hinzugefügt
* Unterstützung für das Deaktivieren des Zugriffs auf das öffentliche Netzwerk
* `az acr token create`: Argument „--days“ verfügbar gemacht
* `az acr import`: Akzeptiert Werte für das Argument „--source“, bei denen der Servername einen Anmeldenamen enthält (mittels clientseitiger Korrektur)

### <a name="acs"></a>ACS

* Fehlerbehebung: Felderbereinigung für Felder entfernt, die nicht mehr vorhanden sind

### <a name="aks"></a>AKS

* Hilfekontext des Befehls „uptime-sla“ aktualisiert
* Bereichsüberprüfung für die Aktualisierung der Mindestanzahl für die Autoskalierung entfernt
* Hotfix, der bewirkt, dass bei der CLI kein Fehler auftritt, wenn der Benutzer nur das Windows-Kennwort angibt

### <a name="ams"></a>AMS

* `az ams transform create`: Funktion zum Erstellen einer Transformation mit einer FaceDetector-Voreinstellung hinzugefügt
* `az ams content-key-policy create` : Funktion zum Erstellen einer FairPlay-Inhaltsschlüsselrichtlinie mit einer Konfiguration für die Offlinemiete hinzugefügt

### <a name="appconfig"></a>AppConfig

* Fehlerbehebung für die Schlüsselauflistungswerte mit Feldern

### <a name="appservice"></a>AppService

* `az functionapp create`: AzureWebJobsDashboard wird nur festgelegt, wenn AppInsights deaktiviert ist
* Fehlerbehebung Nr. 10664: VNET-Integration – Standortüberprüfungsfehler und Fehlerbehebung Nr. 13257: Fehler bei „az webapp up“, wenn eine Ressourcengruppe erstellt werden muss
* `az webapp|functionapp config ssl import`: Ressourcengruppenübergreifende Suche des Schlüsseltresors im Abonnement und verbesserte Hilfe und Beispiele
* Lokaler Kontext für App Service integriert

### <a name="arm"></a>ARM

* `az deployment`: Problem behoben, das dazu führte, dass templateLink beim Bereitstellen oder Überprüfen von „template-uri“ nicht zurückgegeben wurde
* `az deployment`: Problem behoben, das dazu führte, dass speziell codierte Zeichen von der Bereitstellung/Überprüfung nicht unterstützt wurden
* `az deployment sub/group what-if`: Arrayausrichtung und Fehlerbehandlung korrigiert
* `az deployment operation`: Veraltete Informationen angepasst

### <a name="aro"></a>ARO

* Beispiele zu folgenden Befehlen hinzugefügt: az aro create, list, list-credentials, show, delete
* Funktion „generate_random_id“ hinzugefügt

### <a name="backup"></a>Backup

* FriendlyName im Befehl zum Aktivieren des Schutzes für AzureFileShare zulässig
* Korrektur im IaasVM-Befehl „restore-disks“
* BackupManagementType „MAB“ zum Befehl zum Auflisten der Elemente hinzugefügt
* Unterstützung für die Wiederholung des Richtlinienupdates für fehlerhafte Elemente hinzugefügt
* Funktion zum Fortsetzen des Schutzes für virtuelle Azure-Computer hinzugefügt
* Unterstützung zum Angeben der Ressourcengruppe zum Speichern von instantRP beim Erstellen oder Ändern der Richtlinie hinzugefügt

### <a name="ci"></a>CI

* Unterstützung für flake8 3.8.0

### <a name="compute"></a>Compute

* Neuer Befehl: az vm auto-shutdown
* `az vm list-skus`: Verhalten von „--zone“aktualisiert. Jetzt werden alle SKU-Typen zurückgegeben.

### <a name="core"></a>Core

* Aktivierungsstatus aus dem lokalen Kontext für globale Benutzerebene aktualisiert

### <a name="extension"></a>Durchwahl

* `az extension add`: „--system“ hinzugefügt, um die Installation von Erweiterungen in einem Systempfad zu ermöglichen
* Unterstützung für „.egg-info“ zum Speichern der Metadaten für die Radtyperweiterung

### <a name="iot"></a>IoT

* `az iot`: Nachricht des IoT-Befehlsmoduls mit dem Hinweis auf die Erweiterung für die erste Ausführung aktualisiert, sodass sie anstelle der veralteten ID die korrekte moderne ID (`azure-iot`) enthält

### <a name="iot-hub"></a>IoT Hub

* Unterstützung für API- und Netzwerkisolationsbefehle für 2020-03-01

### <a name="netappfiles"></a>NetAppFiles

* `az volume create`: „snapshot-id“ als Parameter zum Erstellen eines Volumes hinzugefügt. Ermöglicht Benutzern das Erstellen eines Volumes auf der Grundlage einer vorhandenen Momentaufnahme.

### <a name="network"></a>Netzwerk

* TTL-Wert korrigiert, der für „dns add-record“ unbeabsichtigt geändert wurde
* `az network public-ip create`: Kunden über einen bevorstehenden Breaking Change informiert
* Unterstützung von generischen Befehlen für Private Link-Szenario
* `az network private-endpoint-connection`: Unterstützung für MySQL-, Postgre- und MariaDB-Typen
* `az network private-endpoint-connection`: Unterstützung von CosmosDB-Typen
* `az network private-endpoint`: „--group-ids“ und Umleitung an „--group-id“ als veraltet gekennzeichnet

### <a name="output"></a>Output

* Anzeigen der Updateanweisung bei der Suche, beim Feedback und in „--help“

### <a name="packaging"></a>Verpackung

* Erstellen von MSI-/Homebrew-Paketen mit Abhängigkeiten, die aus „requirements.txt“ aufgelöst werden

### <a name="rbac"></a>RBAC

* `az ad sp credential reset`: Erstellung unsicherer Anmeldeinformationen korrigiert

### <a name="storage"></a>Storage

* `az storage account file-service-properties update/show`: Unterstützung für Dateieigenschaften für Speicherkonto hinzugefügt
* `az storage container create`: Fehlerbehebung Nr. 13373 durch Hinzufügen eines Validierungssteuerelements für öffentlichen Zugriff
* Unterstützung für ADLS Gen2 (track2) hinzugefügt
* `az storage blob sync`: Unterstützung für `--connection-string`
* `az storage blob sync`: Falsche Fehlermeldung korrigiert, die angezeigt wird, wenn der Installationsspeicherort von „azcopy“ nicht gefunden wird

## <a name="april-30-2020"></a>30. April 2020

Version 2.5.1

### <a name="acr"></a>ACR

* `az acr check-health`: „DOCKER_PULL_ERROR“ unter Windows behoben

### <a name="compute"></a>Compute

* `az vm list-ip-addresses`: Fehlerbehandlung
* Fehler behoben, der bei der VM-Erstellung auftrat, wenn „endpoint_vm_image_alias_doc“ im Cloudprofil nicht festgelegt war
* `az vmss create`: „--os-disk-size-gb“ hinzugefügt

### <a name="cosmos-db"></a>Cosmos DB

* `az cosmosdb create/update`: Unterstützung für „--enable-public-network“ hinzugefügt

### <a name="extension"></a>Durchwahl

* Laden der falschen Metadaten für die Radtyperweiterung korrigiert

### <a name="packaging"></a>Verpackung

* Az-Skript für Git Bash/Cygwin unter Windows hinzugefügt

### <a name="sql"></a>SQL

* `az sql instance-pool`: Befehlsgruppe für Instanzpools hinzugefügt

### <a name="storage"></a>Storage

* Paket „azure-multiapi-storage“ auf 0.3.0 aktualisiert
* Unterstützung von GZRS für Speicherkontoerstellung und -aktualisierung
* `az storage account failover`: Unterstützung für das Failover von GRS/GZRS-Speicherkonten hinzugefügt
* `az storage blob upload`: Parameter „--encryption-scope“ hinzugefügt, um die Angabe von Informationen zum Verschlüsselungsbereich zu unterstützen

## <a name="april-28-2020"></a>28. April 2020

Version 2.5.0

### <a name="acs"></a>ACS

* [BREAKING CHANGE] az openshift create: Parameter „--vnet-peer“ entfernt
* `az openshift create`: Flags zur Unterstützung des privaten Clusters hinzugefügt
* `az openshift`: Upgrade auf API-Version `2019-10-27-preview`
* `az openshift`: Befehl `update` hinzugefügt

### <a name="aks"></a>AKS

* `az aks create`: Unterstützung für Windows hinzugefügt

### <a name="appservice"></a>AppService

* `az webapp deployment source config-zip`: Energiesparmodus nach „request.get()“ entfernt

### <a name="arm"></a>ARM

* Was-wäre-wenn-Befehle für Vorlagenbereitstellung hinzugefügt

### <a name="aro"></a>ARO

* `az aro`: Tabellenausgabe korrigiert

### <a name="ci"></a>CI

* pytest integriert und nose für Automatisierungstest als veraltet gekennzeichnet

### <a name="compute"></a>Compute

* `az vmss disk detach`: Datenträgerfehler „NoneType“ behoben
* `az vm availability-set list`: Unterstützung zum Anzeigen der VM-Liste
* `az vm list-skus`: Anzeigeproblem des Tabellenformats behoben

### <a name="keyvault"></a>KeyVault

* Neuer Parameter `--enable-rbac-authorization` bei Erstellung oder Aktualisierung hinzugefügt

### <a name="monitor"></a>Überwachen

* Unterstützung der CMK-Features für LA-Cluster
* `az monitor log-analytics workspace linked-storage`: Unterstützung für BYOS-Features

### <a name="network"></a>Netzwerk

* `az network security-partner`: Unterstützung des Sicherheitspartneranbieters

### <a name="privatedns"></a>PrivateDNS

* Funktion in privater DNS-Zone zum Importieren der Exportzonendatei hinzugefügt

## <a name="april-21-2020"></a>21. April 2020

Version 2.4.0

### <a name="acr"></a>ACR

* `az acr run --cmd`: Deaktivieren der Arbeitsverzeichnisaußerkraftsetzung
* Unterstützung dedizierter Datenendpunkte

### <a name="aks"></a>AKS

* `az aks list -o table` sollte „privateFqdn“ als FQDN für private Cluster anzeigen
* „--uptime-sla“ hinzugefügt
* containerservice-Paket aktualisiert
* Unterstützung für öffentliche IP-Adressen für Knoten hinzugefügt
* Tippfehler im help-Befehl korrigiert

### <a name="appconfig"></a>AppConfig

* Schlüsseltresorverweis für die Befehle „kv list“ und „kv export“ aufgelöst
* Fehlerbehebung für die Werte für das Auflisten von Schlüsseln

### <a name="appservice"></a>AppService

* `az functionapp create`: Vorgehensweise zum Festlegen von „linuxFxVersion“ für Linux-Funktions-Apps (.NET) geändert. Dadurch sollte der Fehler behoben sein, der die Erstellung von Linux-Verbrauchs-Apps (.NET) verhindert hat.
* [BREAKING CHANGE] `az webapp create`: Korrektur vorgenommen, um vorhandene App-Einstellungen (AppSettings) für „az webapp create“ beizubehalten
* [BREAKING CHANGE] `az webapp up`: Korrektur vorgenommen, um bei Verwendung des Flags „-g“ eine RG für den Befehl „az webapp up“ zu erstellen
* [BREAKING CHANGE] `az webapp config`: Korrektur vorgenommen, um Werte für Nicht-JSON-Ausgaben mit „az webapp config connection-string list“ anzuzeigen

### <a name="arm"></a>ARM

* `az deployment create/validate`: Parameter `--no-prompt` hinzugefügt, um das Überspringen der Eingabeaufforderung für fehlende Parameter für die ARM-Vorlage zu unterstützen
* `az deployment group/mg/sub/tenant validate`: Unterstützung von Kommentaren in der Bereitstellungsparameterdatei
* `az deployment`: `is_preview` für Parameter `--handle-extended-json-format` entfernt
* `az deployment group/mg/sub/tenant cancel`: Unterstützung für den Abbruch der Bereitstellung für ARM-Vorlagen
* `az deployment group/mg/sub/tenant validate`: Fehlermeldung bei einem Fehler der Bereitstellungsüberprüfung verbessert
* `az deployment-scripts`: Neue Befehle für DeploymentScripts hinzugefügt
* `az resource tag`: Parameter `--is-incremental` hinzugefügt, um das inkrementelle Hinzufügen von Tags zur Ressource zu unterstützen

### <a name="aro"></a>ARO

* `az aro`:  ARO-Befehlsmodul von Azure RedHat OpenShift V4 hinzugefügt

### <a name="batch"></a>Batch

* Batch-API aktualisiert

### <a name="compute"></a>Compute

* `az sig image-version create`: Speicherkontotyp „Premium_LRS“ hinzugefügt
* `az vmss update`: Problem behoben, das beim Aktualisieren der Beendigungsbenachrichtigung auftrat
* `az vm/vmss create`: Unterstützung für spezialisierte Imageversion hinzugefügt
* SIG-API-Version 2019-12-01
* `az sig image-version create`: „--target-region-encryption“ hinzugefügt
* Fehler bei Serientestausführung behoben, der auf die Duplizierung des Schlüsseltresornamens im globalen In-Memory-Cache zurückzuführen war.

### <a name="cosmosdb"></a>CosmosDB

* Unterstützung für `az cosmosdb private-link-resource/private-endpoint-connection`

### <a name="iot-central"></a>IoT Central

* `az iotcentral` als veraltet gekennzeichnet
* Befehlsmodul `az iot central` hinzugefügt

### <a name="monitor"></a>Überwachen

* Unterstützung eines Private Link-Szenarios für die Überwachung
* Falsche Simulationsmethode in „test_monitor_general_operations.py“ korrigiert

### <a name="network"></a>Netzwerk

* SKU für den Befehl zur Aktualisierung der öffentlichen IP-Adresse als veraltet gekennzeichnet
* `az network private-endpoint`: Unterstützung für private DNS-Zonengruppe
* Feature für lokalen Kontext für VNET-/Subnetzparameter aktiviert
* Falsches Verwendungsbeispiel in „test_nw_flow_log_delete“ korrigiert

### <a name="packaging"></a>Verpackung

* Unterstützung für Ubuntu-/Disco-Paket eingestellt

### <a name="rbac"></a>RBAC

* `az ad app create/update`: Unterstützung von „--optional-claims“ als Parameter

### <a name="rdbms"></a>RDBMS

* Azure Active Directory-Administratorbefehle für PostgreSQL und MySQL hinzugefügt

### <a name="service-fabric"></a>Service Fabric

* Fehlerbehebung Nr. 12891: `az sf application update --application-parameters` entfernt alte Parameter, die nicht in der Anforderung enthalten sind.
* Fehlerbehebung Nr. 12470: az sf create cluster: Fehler im Zusammenhang mit der Dauerhaftigkeit und Zuverlässigkeit von Updates sowie im Zusammenhang mit der codebasierten Suche der VMSS unter Angabe eines bestimmten Knotentypnamens behoben

### <a name="sql"></a>SQL

* `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel` hinzugefügt
* `az sql midb`: Aktualisieren/Anzeigen der Richtlinie zur langfristigen Aufbewahrung, Anzeigen/Löschen von Sicherungen zur langfristigen Aufbewahrung, Wiederherstellen von Sicherungen zur langfristigen Aufbewahrung

### <a name="storage"></a>Storage

* „azure-mgmt-storage“ auf 9.0.0 aktualisiert
* `az storage logging off`: Unterstützung für das Ausschalten der Protokollierung für ein Speicherkonto
* `az storage account update`: Automatische Rotation von Schlüsseln für CMK aktiviert
* `az storage account encryption-scope create/update/list/show`: Unterstützung zum Anpassen des Verschlüsselungsbereichs hinzugefügt
* `az storage container create`: „--default-encryption-scope“ und „--deny-encryption-scope-override“ hinzugefügt, um den Verschlüsselungsbereich für die Containerebene festzulegen

### <a name="survey"></a>Umfrage

* Switch zum Deaktivieren des Umfragelinks hinzugefügt

## <a name="april-01-2020"></a>01. April 2020

Version 2.3.1

### <a name="acr"></a>ACR

* Falsche Version von „azure-mgmt-containerregistry“ für Linux korrigiert

### <a name="profile"></a>Profil

* az login: Anmeldefehler behoben, der auftrat, wenn nicht das Cloudprofil `latest` verwendet wurde

## <a name="march-31-2020"></a>31. März 2020

Version 2.3.0

### <a name="acr"></a>ACR

* „az acr task update“: NULL-Zeiger-Ausnahme
* `az acr import`: Hilfe und Fehlermeldung geändert, um die Verwendung von „--source“ und „--registry“ zu verdeutlichen
* Überprüfung für das Argument „registry_name“ hinzugefügt
* `az acr login`: Vorschauflag für „--expose-token“ entfernt
* [BREAKING CHANGE] Branch-Parameter „az acr task create/update“ entfernt
* „az acr task update“: Kunde kann nun Kontext, Git-Token und/oder Trigger einzeln aktualisieren
* „az acr agentpool“: Neues Feature

### <a name="aks"></a>AKS

* „apiServerAccessProfile“ bei der Aktualisierung von „--api-server-authorized-ip-ranges“ korrigiert
* aks update: Überschreibung ausgehender IP-Adressen mit Eingabewerten bei der Aktualisierung
* Keine SPN-Erstellung für MSI-Cluster sowie Unterstützung der Anfügung von ACR an MSI-Cluster

### <a name="ams"></a>AMS

* Fix 12469: Hinzufügen von „content-key-policy“ für Fairplay aufgrund von Problemen mit dem Parameter „ask“ nicht erfolgreich

### <a name="appconfig"></a>AppConfig

* „--skip-keyvault“ für „kv export“ hinzugefügt

### <a name="appservice"></a>AppService

* Fix 12509: Tag für „az webapp up“ standardmäßig entfernt
* az functionapp create: Hilfemenü für „--runtime-version“ aktualisiert und Warnung hinzugefügt, wenn der Benutzer „--runtime-version“ für .NET angibt
* az functionapp create: Methode zum Festlegen von „javaVersion“ für Windows-Funktions-Apps aktualisiert

### <a name="arm"></a>ARM

* az deployment create/validate: Standardmäßige Verwendung von „--handle-extended-json-format“
* az lock create: Beispiele für die Erstellung einer Unterressource in der Hilfedokumentation hinzugefügt
* az deployment {group/mg/sub/tenant} list: Unterstützung der provisioningState-Filterung
* az deployment: Analysefehler für Kommentar unter letztem Argument behoben

### <a name="backup"></a>Backup

* Mehrere Dateiwiederherstellungsfunktionen hinzugefügt
* Unterstützung der ausschließlichen Sicherung von Betriebssystemdatenträgern hinzugefügt
* Parameter „restore-as-unmanaged-disk“ für die Angabe einer nicht verwalteten Wiederherstellung hinzugefügt

### <a name="compute"></a>Compute

* az vm create: Option „NONE“ von „--nsg-rule“ hinzugefügt
* az vmss create/update: Vorschautag für automatische VMSS-Reparaturen entfernt
* az vm update: Unterstützung von „--workspace“
* Fehler im VirtualMachineScaleSetExtension-Initialisierungscode behoben
* Upgrade der VMAccessAgent-Version auf 2.4 durchgeführt
* az vmss set-orchestration-service-state: Unterstützung zum Festlegen des Orchestrierungdienstzustands für VMSS
* Upgrade der Datenträger-API-Version auf 2019-11-01 durchgeführt
* az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun

### <a name="cosmos-db"></a>Cosmos DB

* Fehlende Option „--type“ für Veraltungsumleitungen korrigiert

### <a name="docker"></a>Docker

* Update auf Alpine 3.11 und Python 3.6.10 durchgeführt

### <a name="extension"></a>Durchwahl

* Laden von Erweiterungen im Systempfad mittels Paketen ermöglicht

### <a name="hdinsight"></a>HDInsight

* (az hdinsight create:) Unterstützung der Angabe der unterstützten TLS-Mindestversion durch Kunden unter Verwendung des Parameters `--minimal-tls-version`. Zulässiger Wert: 1.0,1.1,1.2

### <a name="iot"></a>IoT

* Codebesitzer hinzugefügt
* az iot hub create: Standard-SKU von F1 in S1 geändert
* iot hub: Unterstützung von „IotHub“ im Profil „2019-03-01-hybrid“

### <a name="iotcentral"></a>IoTCentral

* Fehlerdetails sowie Standardanwendungsvorlage und Aufforderungsmeldung aktualisiert

### <a name="keyvault"></a>KeyVault

* Unterstützung von Zertifikatsicherung/-wiederherstellung
* keyvault create/update: Unterstützung von „--retention-days“
* Keine Anzeige von verwalteten Schlüsseln/Geheimnissen bei der Auflistung mehr
* az keyvault create: Unterstützung von `--network-acls`, `--network-acls-ips` und `--network-acls-vnets` zur Angabe von Netzwerkregeln bei der Tresorerstellung

### <a name="lock"></a>Sperre

* Fehlerbehebung für „az lock delete“: „az lock delete“ funktioniert für „Microsoft.DocumentDB“ nicht.

### <a name="monitor"></a>Überwachen

* az monitor clone: Unterstützung des Klonens von Metrikregeln zwischen Ressourcen
* Fix IcM179210086: Erstellung einer benutzerdefinierten Metrikwarnung für die Application Insights-Metrik nicht möglich

### <a name="netappfiles"></a>NetAppFiles

* az volume create: Datenschutzvolumes zum Hinzufügen von Replikationsvorgängen zugelassen: Genehmigen, Aussetzen, Fortsetzen, Status, Entfernen

### <a name="network"></a>Netzwerk

* az network application-gateway waf-policy managed-rule rule-set add: Unterstützung von „ Microsoft_BotManagerRuleSet“
* network watcher flow-log show: Falsche Veraltungsinformationen behoben
* Unterstützung von Hostnamen im Application Gateway-Listener
* az network nat gateway: Unterstützung der Erstellung einer leeren Ressource ohne öffentliche IP-Adresse oder Präfix für öffentliche IP-Adressen
* Unterstützung der VPN-Gateway-Generierung
* Unterstützung von `--if-none-match` in `az network dns record-set {} add-record`

### <a name="packaging"></a>Verpackung

* Unterstützung von Python 3.5 eingestellt

### <a name="profile"></a>Profil

* az login: Warnung für MFA-Fehler

### <a name="rdbms"></a>RDBMS

* Befehle zur Verwaltung von Verschlüsselungsschlüsseln für Serverdaten für PostgreSQL und MySQL hinzugefügt

## <a name="march-10-2020"></a>10. März 2020

Version 2.2.0

### <a name="acr"></a>ACR

* Fix: `az acr login` löst fälschlicherweise Fehler aus
* Neuer Befehl `az acr helm install-cli` hinzugefügt
* Privater Link und CMK-Unterstützung hinzugefügt
* Befehl „private-link-resource list“ hinzugefügt

### <a name="aks"></a>AKS

* Durchsuchen von AKS in Cloud-Shell korrigiert
* az aks: NoneType-Fehler beim Überwachen von „addon“ und „agentpool“ behoben
* „--nodepool-tags“ zum Knotenpool beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt
* „--tags“ beim Hinzufügen oder Aktualisieren eines Knotenpool in einem Cluster hinzugefügt
* aks create: `--enable-private-cluster` hinzugefügt
* „--nodepool-labels“ beim Erstellen von Azure-Kubernetes-Clustern hinzugefügt
* „--labels“ beim Hinzufügen eines neuen Knotenpools zu einem Azure-Kubernetes-Cluster hinzugefügt
* Fehlender Schrägstrich (/) in der Dashboard-URL hinzugefügt
* Unterstützung der Erstellung von AKS-Clustern, sodass verwaltete Identitäten möglich sind
* az aks: Überprüfen, ob das Netzwerk-Plug-In entweder „azure“ oder „kubenet“ ist
* az aks: Unterstützung für AAD-Sitzungsschlüssel hinzugefügt
* [BREAKING CHANGE] az aks: Unterstützung von MSI-Änderungen für GF und BF für omsagent (Containerüberwachung)(#1)
* az aks use-dev-spaces: Endpunkt-Typoption zum Befehl „use-dev-spaces“, hinzugefügt, um den auf einem Azure Dev Spaces-Controller erstellten Endpunkt anzupassen

### <a name="appconfig"></a>AppConfig

* Verwendung von „kv set“ entsperrt, um Schlüsseltresorverweis und -funktion hinzuzufügen …

### <a name="appservice"></a>AppService

* az webapp create : Beheben eines Problems beim Ausführen des Befehls mit „--runtime“
* az functionapp deployment source config-zip: Fehlermeldung hinzugefügt, wenn der Ressourcengruppen- oder Funktionsname ungültig oder nicht vorhanden ist
* functionapp create: Warnmeldung korrigiert, die derzeit mit `functionapp create` angezeigt wird und ein `--functions_version`-Flag angibt, aber irrtümlich ein `_` anstelle eines `-` im Flagnamen verwendet
* az functionapp create: Es wurde aktualisiert, wie linuxFxVersion und der Containerimagename für Linux-Funktions-Apps festgelegt werden.
* az functionapp deployment source config-zip: Problems behoben, das durch die Racebedingung für die Änderung von App-Einstellungen während der ZIP-Bereitstellung verursacht wird und während der Bereitstellung 5xx-Fehler ausgibt
* Fix #5720946: „az webapp backup“ legt Namen nicht fest

### <a name="arm"></a>ARM

* az resource: Beispiele für das Ressourcenmodul verbessert
* az policy assignment list: Unterstützung für das Auflisten von Richtlinienzuweisungen im Verwaltungsgruppenbereich
* `az deployment group` und `az deployment operation group` für Vorlagenbereitstellung in Ressourcengruppen hinzugefügt Dies ist ein Duplikat von `az group deployment` und `az group deployment operation`.
* `az deployment sub` und `az deployment operation sub` für Vorlagenbereitstellung im Abonnementbereich hinzugefügt Dies ist ein Duplikat von `az deployment` und `az deployment operation`.
* `az deployment mg` und `az deployment operation mg` für Vorlagenbereitstellung in Verwaltungsgruppen hinzugefügt
* `az deployment tenant` und `az deployment operation tenant` für Vorlagenbereitstellung im Mandantenbereich hinzugefügt
* az policy assignment create: Beschreibung zu Parameter `--location` hinzugefügt
* az group deployment create: Parameter `--aux-tenants` zur mandantenübergreifenden Unterstützung hinzugefügt

### <a name="cdn"></a>CDN

* CDN-WAF-Befehle hinzugefügt

### <a name="compute"></a>Compute

* az sig image-version: „--data-snapshot-luns“ hinzugefügt
* az ppg show: „--colocation-status“ hinzugefügt, um das Abrufen des Zusammenstellungsstatus aller Ressourcen in der Näherungsplatzierungsgruppe zu ermöglichen
* az vmss create/update: Unterstützung automatischer Reparaturen
* [BREAKING CHANGE] az image template: „template“ in „builder“ umbenannt
* az image builder create: „--image-template“ hinzugefügt

### <a name="cosmos-db"></a>Cosmos DB

* Gespeicherte Prozedur „Add Sql“, udf- und trigger-Cmdlets hinzugefügt
* az cosmosdb create: „--key-uri“ hinzugefügt, um das Hinzufügen von Schlüsseltresor-Verschlüsselungsinformationen zu unterstützen

### <a name="keyvault"></a>KeyVault

* keyvault create: „soft-delete“ standardmäßig aktiviert

### <a name="monitor"></a>Überwachen

* az monitor metrics alert create: Unterstützung von `~` in `--condition`

### <a name="network"></a>Netzwerk

* az network application-gateway rewrite-rule create: Unterstützung der URL-Konfiguration
* az network dns zone import: Bei „--zone-name“ wird die Groß-/Kleinschreibung künftig nicht mehr beachtet.
* az network private-endpoint/private-link-service: Vorschaubezeichnung entfernt
* az network bastion: Unterstützung von „bastion“
* az network vnet list-available-ips: Unterstützung für das Auflisten verfügbarer IPs in einem VNET
* az network watcher flow-log create/list/delete/update: neue Befehle hinzugefügt, um Watcher-Datenflussprotokolle zu verwalten und „--location“ zur expliziten Identifizierung von Watcher verfügbar zu machen
* az network watcher flow-log configure: veraltet
* az network watcher flow-log show: Unterstützung von „--location“ und „--name“, um ein ARM-formatiertes Ergebnis zu erhalten; alte formatierte Ausgabe als veraltet markiert

### <a name="policy"></a>Richtlinie

* az policy assignment create: Fehler behoben, dass automatisch generierter Name der Richtlinienzuweisung den Grenzwert überschreitet

### <a name="rbac"></a>RBAC

* az ad group show: Problem behoben, dass „--group“-Wert als regulärer Ausdruck behandelt wurde

### <a name="rdbms"></a>RDBMS

* SDK-Version von „azure-mgmt-rdbms“ auf 2.0.0 festgelegt
* az postgres private-endpoint-connection: Verwalten von Verbindungen mit privatem Postgres-Endpunkt
* az postgres private-link-resource: Verwalten von privaten Postgres-Linkressourcen
* az mysql private-endpoint-connection: Verwalten von Verbindungen mit privatem MySQL-Endpunkt
* az mysql private-link-resource: Verwalten von privaten MySQL-Linkressourcen
* az mariadb private-endpoint-connection: Verwalten von Verbindungen mit privatem MariaDB-Endpunkt
* az mariadb private-link-resource: Verwalten von privaten MariaDB-Linkressourcen
* Aktualisieren von Tests von privaten RDBMS-Endpunkten

### <a name="sql"></a>SQL

* Sql midb: list-deleted, show-deleted, update-retention, show-retention hinzugefügt
* (sql server create:) Optionales Flag „Enable“/„Disable“ für public-network-access zu „sql server create“ hinzugefügt
* (sql server update): kundenorientierte Änderung vorgenommen
* Eigenschaft „minimal_tls_version“ für MI und SQL-Datenbank hinzugefügt

### <a name="storage"></a>Storage

* az storage blob delete-batch: Flag `--dryrun` mit Fehlverhalten
* az storage account network-rule hinzugefügt (Fehlerbehebung): Hinzufügen von Vorgängen muss idempotent sein
* az storage account create/update: Unterstützung für Routingpräferenz hinzugefügt
* „azure-mgmt-storage“ auf Version 8.0.0 aktualisiert
* az storage container immutability create: Parameter „--allow-protected-append-write“ hinzugefügt
* az storage account private-link-resource list: Unterstützung zum Auflisten privater Linkressourcen für Speicherkonto hinzugefügt
* az storage account private-endpoint-connection approve/reject/show/delete: Unterstützung der Verwaltung von Verbindungen mit privaten Endpunkten
* az storage account blob-service-properties update: „--enable-restore-policy“ und „--restore-days“ hinzugefügt
* az storage blob restore: Unterstützung für die Wiederherstellung von Blobbereichen hinzugefügt

## <a name="february-18-2020"></a>18. Februar 2020

Version 2.1.0

### <a name="acr"></a>ACR

* Neues Argument `--expose-token` für `az acr login` hinzugefügt
* Falsche Ausgabe für `az acr task identity show -n Name -r Registry -o table` korrigiert
* az acr login: Auslösen von „CLIError“, wenn vom Docker-Befehl Fehler zurückgegeben werden

### <a name="acs"></a>ACS

* aks create/update: Validierung für `--vnet-subnet-id` hinzugefügt

### <a name="aladdin"></a>Aladdin

* Analysieren der generierten Beispiele in „_help.py“ der Befehle

### <a name="ams"></a>AMS

* az ams ist jetzt allgemein verfügbar.

### <a name="appconfig"></a>AppConfig

* Hilfenachricht überarbeitet, um nicht unterstützte Schlüssel-/Bezeichnungsfilter auszuschließen
* Vorschautag für die meisten Befehle entfernt (mit Ausnahme der Flags für verwaltete Identitäten und Features)
* Kundenseitig verwalteter Schlüssel beim Aktualisieren der Speicher hinzugefügt

### <a name="appservice"></a>AppService

* az webapp list-runtimes: Fehler bei „list-runtimes“ behoben
* „az webapp|functionapp config ssl create“ hinzugefügt
* Unterstützung für v3-Funktions-Apps und Node 12

### <a name="arm"></a>ARM

* az policy assignment create: Fehlermeldung korrigiert, die angezeigt wird, wenn der Parameter `--policy` ungültig ist
* az group deployment create: Fehler „stat: path too long for Windows" korrigiert, der angezeigt wird, wenn eine zu große Datei vom Typ „parameters.json“ verwendet wird

### <a name="backup"></a>Backup

* Korrektur des Wiederherstellungsflows auf Elementebene am ursprünglichen Speicherort
* Unterstützung von „Als Dateien wiederherstellen“ für SQL- und SAP-Datenbanken hinzugefügt

### <a name="compute"></a>Compute

* vm/vmss/availability-set update: „--ppg“ hinzugefügt, um die Aktualisierung von „ProximityPlacementGroup“ zu ermöglichen
* vmss create: „--data-disk-iops“ und „--data-disk-mbps“ hinzugefügt
* az vm host: Vorschautag für `vm host` und `vm host group` entfernt
* [BREAKING CHANGE] Behebung Nr. 10728: `az vm create`: Automatisches Erstellen des Subnetzes, wenn das VNET angegeben wird und das Subnetz nicht vorhanden ist
* Erhöhen der Stabilität von „vm image list“

### <a name="eventhub"></a>Eventhub

* Azure Stack-Unterstützung für Profil „2019-03-01-hybrid“

### <a name="keyvault"></a>KeyVault

* az keyvault key create: neuer Wert `import` für Parameter `--ops` hinzugefügt
* az keyvault key list-versions: Unterstützung des Parameters `--id` für die Angabe von Schlüsseln
* Unterstützung für Verbindungen mit privaten Endpunkten

### <a name="network"></a>Netzwerk

* Geändert in „azure-mgmt-network 9.0.0“
* az network private-link-service update/create: Unterstützung von „--enable-proxy-protocol“
* Feature für Version 2 von Verbindungsmonitor hinzugefügt

### <a name="packaging"></a>Verpackung

* [BREAKING CHANGE] Unterstützung für Python 2.7 eingestellt

### <a name="profile"></a>Profil

* Vorschau: Neue Attribute `homeTenantId` und `managedByTenants` zu Abonnementkonten hinzugefügt. Führen Sie `az login` erneut aus, damit die Änderungen wirksam werden.
* az login: Eine Warnung wird angezeigt, wenn ein Abonnement von mehren Mandanten aufgeführt wird und der erste als Standard festgelegt wird. Fügen Sie `--tenant` in `az login` ein, um beim Zugreifen auf dieses Abonnement einen bestimmten Mandanten auszuwählen.

### <a name="role"></a>Role

* az role assignment create: Problem behoben, das beim Zuweisen einer Rolle zu einem Dienstprinzipal nach Anzeigename einen Fehler vom Typ „HTTP 400“ verursachte

### <a name="sql"></a>SQL

* Cmdlet `az sql mi update` der verwalteten SQL-Instanz mit zwei neuen Parametern aktualisiert: tier und family

### <a name="storage"></a>Storage

* [BREAKING CHANGE] `az storage account create`: Art des Standardspeicherkontos in StorageV2 geändert

## <a name="february-04-2020"></a>04. Februar 2020

Version 2.0.81

### <a name="acs"></a>ACS

* Unterstützung für das Festlegen zugeordneter Ausgangsports und Leerlauftimeouts für Load Balancer Standard hinzugefügt
* Aktualisierung auf API-Version 2019-11-01

### <a name="acr"></a>ACR

* [BREAKING CHANGE] `az acr delete` löst eine Eingabeaufforderung aus.
* [BREAKING CHANGE] „az acr task delete“ löst eine Eingabeaufforderung aus.
* Neue Befehlsgruppe „az acr taskrun show/list/delete“ für die Aufgabenausführungsverwaltung hinzugefügt

### <a name="aks"></a>AKS

* Jeder Cluster erhält einen separaten Dienstprinzipal zur Verbesserung der Isolation.

### <a name="appconfig"></a>AppConfig

* Unterstützung für den Import/Export von KeyVault-Verweisen in/aus AppService
* Unterstützung für den Import/Export aller Bezeichnungen in appconfig und aus appconfig
* Überprüfen der Schlüssel- und Featurenamen vor dem Festlegen und Importieren
* Verfügbarmachen der SKU-Änderung für den Konfigurationsspeicher
* Befehlsgruppe für die verwaltete Identität hinzugefügt

### <a name="appservice"></a>AppService

* Azure Stack: Oberflächenbefehle im Profil „2019-03-01-hybrid“
* functionapp: Funktion zum Erstellen von Java-Funktions-Apps in Linux hinzugefügt

### <a name="arm"></a>ARM

* Behebung von Problem Nr. 10246: `az resource tag` stürzt ab, wenn der übergebene Parameter `--ids` der Ressourcengruppen-ID entspricht.
* Behebung von Problem Nr. 11658: Der Befehl `az group export` unterstützt die Parameter `--query` und `--output` nicht.
* Behebung von Problem Nr. 10279: Der Exitcode von `az group deployment validate` ist 0, wenn bei der Überprüfung ein Fehler auftritt.
* Behebung von Problem Nr. 9916: Fehlermeldung des Konflikts zwischen Tag und anderen Filterbedingungen für Befehl `az resource list` verbessert
* Neuer Parameter `--managed-by` hinzugefügt, um das Hinzufügen der Informationen vom Typ „managedBy“ für Befehl `az group create` zu unterstützen

### <a name="azure-red-hat-openshift"></a>Azure Red Hat OpenShift

* Untergruppe `monitor` hinzugefügt, um Log Analytics-Überwachung im Azure Red Hat OpenShift-Cluster zu unterstützen

### <a name="botservice"></a>BotService

* Behebung von Problem Nr. 11697: `az bot create` ist nicht idempotent.
* Tests zur Namenskorrektur geändert, sodass sie nur im Livemodus ausgeführt werden

### <a name="cdn"></a>CDN

* Unterstützung für das rulesEngine-Feature hinzugefügt
* Neue Befehlsgruppe „cdn endpoint rule“ zum Verwalten von Regeln hinzugefügt
* azure-mgmt-cdn-Version auf 4.0.0 aktualisiert, um API-Version 2019-04-15 zu verwenden

### <a name="deployment-manager"></a>Bereitstellungs-Manager

* Auflistungsvorgang für alle Ressourcen hinzugefügt
* Schrittressource für neuen Schritttyp optimiert
* Paket „azure-mgmt-deploymentmanager“ zur Verwendung von Version 0.2.0 aktualisiert

### <a name="iot"></a>IoT

* Befehle vom Typ „IoT hub Job“ als veraltet gekennzeichnet

### <a name="iot-central"></a>IoT Central

* Unterstützung der App-Erstellung/-Aktualisierung mit neuem SKU-Namen ST0, ST1, ST2

### <a name="key-vault"></a>Key Vault

* Neuer Befehl `az keyvault key download` zum Herunterladen von Schlüsseln hinzugefügt

### <a name="misc"></a>Sonstiges

* Behebung Nr. 6371: Unterstützung für die Vervollständigung von Dateinamen und Umgebungsvariablen in Bash

### <a name="network"></a>Netzwerk

* Behebung Nr. 2092: az network dns record-set add/remove: Warnung hinzugefügt, wenn Datensatzgruppe nicht gefunden wurde. In Zukunft wird ein zusätzliches Argument unterstützt, um diese automatische Erstellung zu bestätigen.

### <a name="policy"></a>Richtlinie

* Neuer Befehl `az policy metadata` hinzugefügt, um umfangreiche Richtlinienmetadatenressourcen abzurufen
* `az policy remediation create`: Geben Sie mit dem Parameter `--resource-discovery-mode` an, ob die Konformität vor der Wartung neu bewertet werden soll.

### <a name="profile"></a>Profil

* `az account get-access-token`: Parameter `--tenant` hinzugefügt, um das Token für den Mandanten direkt abzurufen. Es muss kein Abonnement angegeben werden.

### <a name="rbac"></a>RBAC

* [BREAKING CHANGE] Behebung Nr. 11883: `az role assignment create`: Bei leerem Bereich wird ein Fehler ausgegeben.

### <a name="security"></a>Sicherheit

* Neue Befehle `az atp show` und `az atp update` hinzugefügt, um erweiterte Einstellungen für den Bedrohungsschutz für Speicherkonten anzuzeigen und zu verwalten

### <a name="sql"></a>SQL

* `sql dw create`: Parameter `--zone-redundant` und `--read-replica-count` als veraltet gekennzeichnet. Diese Parameter gelten nicht für Datawarehouse.
* [BREAKING CHANGE] `az sql db create`: „WideWorldImportersStd“ und „WideWorldImportersFull“ als dokumentierte zulässige Werte für „az sql db create --sample-name“ entfernt. Diese Beispieldatenbanken führen immer zu einem Fehler bei der Erstellung.
* Neue Befehle `sql db classification show/list/update/delete` und `sql db classification recommendation list/enable/disable` zur Verwaltung von Vertraulichkeitsklassifizierungen für SQL-Datenbanken hinzugefügt
* `az sql db audit-policy`: Behebung für leere Überwachungsaktionen und -gruppen

### <a name="storage"></a>Storage

* Neue Befehlsgruppe `az storage share-rm` hinzugefügt, um den Ressourcenanbieter „Microsoft.Storage“ für Verwaltungsvorgänge der Azure-Dateifreigabe zu verwenden
* Behebung für Problem Nr. 11415: Berechtigungsfehler für `az storage blob update`
* Integration von Azcopy 10.3.3 und Unterstützung von Win32
* `az storage copy`: Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt
* `az storage remove`: Parameter `--inlcude` und `--exclude` in Parameter `--include-path`, `--include-pattern`, `--exclude-path` und`--exclude-pattern` geändert
* `az storage sync`: Parameter `--include-pattern`, `--exclude-path` und`--exclude-pattern` hinzugefügt

### <a name="servicefabric"></a>ServiceFabric

* Neue Befehle zum Verwalten von Anwendung und Diensten hinzugefügt

## <a name="january-13-2020"></a>13. Januar 2020

Version 2.0.80

### <a name="compute"></a>Compute

* Datenträgeraktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt
* Momentaufnahmeerstellung/-aktualisierung: „--disk-encryption-set“ und „--encryption-type“ hinzugefügt

### <a name="storage"></a>Storage

* „azure-mgmt-storage“ auf Version 7.1.0 aktualisiert
* `az storage account create`: `--encryption-key-type-for-table` und `--encryption-key-type-for-queue` zur Unterstützung des Tabellen- und Warteschlangenverschlüsselungsdiensts hinzugefügt

## <a name="january-07-2020"></a>7\. Januar 2020

Version 2.0.79

### <a name="acr"></a>ACR

* [BREAKING CHANGE] Parameter „--os“ für „acr build“, „acr task create/update“, „acr run“ und „acr pack“ wurde entfernt. Verwenden Sie stattdessen „--platform“.

### <a name="appconfig"></a>AppConfig

* Unterstützung für das Importieren/Exportieren von Featureflags hinzugefügt
* Neuer Befehl „az appconfig kv set-keyvault“ für das Erstellen einer KeyVault-Referenz hinzugefügt
* Unterstützung verschiedener Benennungskonventionen beim Exportieren von Featureflags in eine Datei

### <a name="appservice"></a>AppService

* Behebung von Problem Nr. 7154: Aktualisierung der Dokumentation für Befehl „<>“, sodass Backticks anstelle von einfachen Anführungszeichen verwendet werden.
* Behebung von Problem Nr. 11287: „webapp up“: Für die mit „up“ erstellte App muss standardmäßig SSL aktiviert sein.
* Behebung von Problem Nr. 11592: Flag „az webapp up“ für statische HTML-Websites hinzugefügt

### <a name="arm"></a>ARM

* Behebung `az resource tag`: Recovery Services-Tresor-Tags können nicht aktualisiert werden.

### <a name="backup"></a>Backup

* Neuer Befehl „backup protection undelete“ hinzugefügt, um die Funktion zum vorläufigen Löschen für IaasVM-Workloads zu aktivieren
* Neuer Parameter „--soft-delete-feature-state“ hinzugefügt, um den Befehl „backup-properties“ festzulegen
* Unterstützung für den Ausschluss von Datenträgern für IaasVM-Workload hinzugefügt

### <a name="compute"></a>Compute

* Fehler `vm create` in Azure Stack-Profil behoben.
* vm monitor metrics tail/list-definitions: Unterstützung einer Abfragemetrik und von Listendefinitionen für eine VM.
* Neue Aktion des Befehls zum erneuten Anwenden für „az vm“ hinzugefügt

### <a name="hdinsight"></a>HDInsight

* Unterstützung für das Erstellen eines Kafka-Clusters mit Kafka-REST-Proxy
* „azure-mgmt-hdinsight“ auf 1.3.0 aktualisiert

### <a name="misc"></a>Verschiedenes:

* Vorschaubefehl `az version show` hinzugefügt, um die Versionen der Azure CLI-Module und Erweiterungen standardmäßig im JSON-Format oder im mit „--output“ konfigurierten Format anzuzeigen

### <a name="event-hubs"></a>Event Hubs

* [BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus „az eventhubs eventhub update“ und „az eventhubs eventhub create“ entfernt. Diese Option ist für Event Hub-Entitäten nicht gültig.

### <a name="service-bus"></a>Service Bus

* [BREAKING CHANGE] Statusoption „ReceiveDisabled“ aus Befehlen „az servicebus topic create“, „az servicebus topic update“, „az servicebus queue create“ und „az servicebus queue update“ entfernt. Diese Option ist für Service Bus-Themen und -Warteschlangen nicht gültig.

### <a name="rbac"></a>RBAC

* Behebung Nr. 11712: `az ad app/sp show` gibt nicht den Exitcode 3 zurück, wenn die Anwendung oder der Dienstprinzipal nicht vorhanden ist.

### <a name="storage"></a>Storage

* `az storage account create`: Vorschaukennzeichnung für Parameter „--enable-hierarchical-namespace“ entfernt
* azure-mgmt-storage-Version auf 7.0.0 aktualisiert, um API-Version 2019-06-01 zu verwenden
* Neue Parameter `--enable-delete-retention` und `--delete-retention-days` hinzugefügt, um die Verwaltung der Aufbewahrungsrichtlinie für Löschen für „blob-service-properties“ von Speicherkonten zu unterstützen.

## <a name="december-17-2019"></a>17. Dezember 2019

2.0.78

### <a name="acr"></a>ACR

* Unterstützung für lokalen Kontext in „acr task run“

### <a name="acs"></a>ACS

* [BREAKING CHANGE] az openshift create: `--workspace-resource-id` in `--workspace-id` umbenannt.

### <a name="ams"></a>AMS

* Befehle zum Anzeigen aktualisiert, sodass 3 zurückgegeben wird, wenn die Ressource nicht gefunden wurde

### <a name="appconfig"></a>AppConfig

* Fehler beim Anhängen der API-Version an die Anforderungs-URL korrigiert. Die vorhandene Lösung funktioniert nicht mit Paginierung.
* Unterstützung für die Anzeige von weiteren Sprachen neben Englisch hinzugefügt, da der Back-End-Dienst Unicode für die Globalisierung unterstützt.

### <a name="appservice"></a>AppService

* Problem Nr. 11217 behoben: Web-App: „az webapp config ssl upload“ muss Slot-Parameter unterstützen.
* Problem Nr. 10965 behoben: Error: Der Name darf nicht leer sein. Entfernen anhand von „ip_address“ und „subnet“ zulassen
* Unterstützung des Imports von Zertifikaten aus Key Vault hinzugefügt `az webapp config ssl import`

### <a name="arm"></a>ARM

* Paket „azure-mgmt-resource“ auf die Verwendung von 6.0.0 aktualisiert
* Mandantenübergreifende Unterstützung für Befehl `az group deployment create` durch Hinzufügen des neuen Parameters `--aux-subs`
* Neuer Parameter `--metadata` hinzugefügt, um das Hinzufügen von Metadateninformationen für Richtliniensatzdefinitionen zu unterstützen

### <a name="backup"></a>Backup

* Unterstützung der Sicherung für SQL- und SAP Hana-Workloads hinzugefügt.

### <a name="botservice"></a>BotService

* [Breaking Change] Flag „--version“ aus Vorschaubefehl „az bot create“ entfernt. Nur v4-SDK-Bots werden unterstützt.
* Überprüfung der Namensverfügbarkeit für „az bot create“ hinzugefügt.
* Unterstützung für das Aktualisieren der Symbol-URL für einen Bot über „az bot update“ hinzugefügt.
* Unterstützung für das Aktualisieren eines Direct Line-Kanals über „az bot directline update“ hinzugefügt.
* Unterstützung für Flag „--enable-enhanced-auth“ zu „az bot directline create“ hinzugefügt.
* Die folgenden Befehlsgruppen sind allgemein verfügbar und befinden sich nicht in der Vorschau: „az bot authsetting“.
* Die folgenden Befehle in „az bot“ sind allgemein verfügbar und befinden sich nicht in der Vorschau: „create“, „prepare-deploy“, „show“, „delete“, „update“.
* „az bot prepare-deploy“ korrigiert, indem der Wert voon „--proj-file-path“ in Kleinschreibung geändert wurde (z. B. „Test.csproj“ in „test.csproj“).

### <a name="compute"></a>Compute

* vmss create/update: „--scale-in-policy“ hinzugefügt, womit entschieden wird, welche virtuellen Computer beim horizontalen Herunterskalieren einer VM-Skalierungsgruppe zum Entfernen ausgewählt werden.
* vm/vmss update: „--priority“ hinzugefügt.
* vm/vmss update: „--max-price“ hinzugefügt.
* Befehlsgruppe „disk-encryption-set“ hinzugefügt (create, show, update, delete, list).
* disk create: „--encryption-type“ und „--disk-encryption-set“ hinzugefügt.
* vm/vmss create: „--os-disk-encryption-set“ und „--data-disk-encryption-sets“ hinzugefügt.

### <a name="core"></a>Core

* Unterstützung für Python 3.4 entfernt
* Plug-In für HaTS-Umfrage in mehreren Befehlen

### <a name="dls"></a>DLS

* ADLS-SDK-Version aktualisiert (0.0.48).

### <a name="install"></a>Installieren

* Installationsskript unterstützt Python 3.8

### <a name="iot"></a>IoT

* [BREAKING CHANGE] Parameter „--failover-region“ aus „manual-failover“ entfernt. Das Failover erfolgt jetzt in eine zugewiesene, geografisch gekoppelte sekundäre Region.

### <a name="key-vault"></a>Key Vault

* Nr. 8095 behoben: `az keyvault storage remove`: Hilfemeldung verbessert
* Nr. 8921 behoben: `az keyvault key/secret/certificate list/list-deleted/list-versions`: Validierungsfehler in Parameter `--maxresults` behoben
* Nr. 10512 behoben: `az keyvault set-policy`: Fehlermeldung verbessert, wenn weder `--object-id`, `--spn` noch `--upn` angegeben ist
* Nr. 10846 behoben: `az keyvault secret show-deleted`: Wenn `--id` angegeben ist, ist `--name/-n` nicht erforderlich.
* Nr. 11084 behoben: `az keyvault secret download`: Hilfemeldung von Parameter `--encoding` verbessert

### <a name="network"></a>Netzwerk

* az network application-gateway probe: Unterstützung für Option „--port“ hinzugefügt, um einen Port zum Prüfen von Back-End-Servern beim Erstellen und Aktualisieren anzugeben
* az network application-gateway url-path-map create/update: Fehlerbehebung für `--waf-policy`
* az network application-gateway: Unterstützung für `--rewrite-rule-set` hinzugefügt
* az network list-service-aliases: Unterstützung für Listendienstaliase hinzugefügt, die für Dienstendpunktrichtlinien verwendet werden können
* az network dns zone import: Unterstützung für „.@“ in Datensatzname hinzugefügt

### <a name="packaging"></a>Verpackung

* Back-Edge-Builds für PIP-Installation hinzugefügt
* Ubuntu-Eoan-Paket hinzugefügt

### <a name="policy"></a>Richtlinie

* Unterstützung für Version 2019-09-01 der Richtlinien-API hinzugefügt
* az policy set-definition: Unterstützung der Gruppierung innerhalb von Richtliniensatzdefinitionen mit `--definition-groups`-Parameter hinzugefügt

### <a name="redis"></a>Redis

* Vorschauparameter `--replicas-per-master` zu Befehl `az redis create`hinzugefügt
* „azure-mgmt-redis“ von 6.0.0 auf 7.0.0rc1 aktualisiert

### <a name="servicefabric"></a>ServiceFabric

* Hinzufügen von Logik in Knotentyp korrigiert, einschließlich Nr. 10963: Beim Hinzufügen eines neuen Knotentyps mit Dauerhaftigkeitsstufe „Gold“ wird immer ein CLI-Fehler ausgegeben.
* ServiceFabricNodeVmExt-Version in Erstellungsvorlage auf 1.1 aktualisiert

### <a name="sql"></a>SQL

* Parameter „--read-scale“ und „--read-replicas“ zu Befehlen „sql db create“ und „sql db update“ hinzugefügt, um Leseskalierungsverwaltung zu unterstützen.

### <a name="storage"></a>Storage

* Allgemein verfügbares Release – Eigenschaft „Large File Shares“ für Befehle „storage account create“ und „storage account update“
* Allgemein verfügbares Release – Unterstützung von SAS-Token für die Benutzerdelegierung
* Neue Befehle `az storage account blob-service-properties show` und `az storage account blob-service-properties update --enable-change-feed` hinzugefügt, um Blob-Diensteigenschaften für das Speicherkonto zu verwalten.
* [BEVORSTEHENDER BREAKING CHANGE] `az storage copy`: Das Zeichen `*` wird nicht mehr als Platzhalter in der URL, es werden jedoch die neuen Parameter „--include-pattern“ und „--exclude-pattern“ mit Unterstützung des Platzhalters `*` hinzugefügt.
* Problem Nr. 11043 behoben: Unterstützung für das Entfernen des gesamten Containers/der gesamten Freigabe in `az storage remove` Befehl hinzugefügt

## <a name="november-26-2019"></a>26. November 2019

Version 2.0.77

### <a name="acr"></a>ACR

* Parameter `--branch` in „acr task create/update“ als veraltet markiert

### <a name="azure-red-hat-openshift"></a>Azure Red Hat OpenShift

* `--workspace-resource-id`-Flag hinzugefügt, um die Erstellung eines Azure Red Hat OpenShift-Clusters mit Überwachung zuzulassen
* `monitor_profile`-Flag hinzugefügt, um einen Azure Red Hat OpenShift-Clusters mit Überwachung zu erstellen

### <a name="aks"></a>AKS

* Unterstützung des Rotationsvorgangs für Clusterzertifikate mithilfe von für Cluster Zertifikat Rotation mit „az aks rotate-certs“ hinzugefügt.

### <a name="appconfig"></a>AppConfig

* Unterstützung für die Verwendung von „:“ für `as az appconfig kv import`-Trennzeichen hinzugefügt
* Problem beim Auflisten von Schlüsselwerten mit mehreren Bezeichnungen, einschließlich NULL-Bezeichnung, behoben. 
* Verwaltungsebenen-SDK, „azure-mgmt-appconfiguration“, auf Version 0.3.0 aktualisiert. 

### <a name="appservice"></a>AppService

* Problem Nr. 11100 behoben AttributeError für „az webapp up“ beim Erstellen eines Dienstplans
* az webapp up: Erzwingen der Erstellung oder Bereitstellung auf einer Website für unterstützte Sprachen, es werden keine Standardeinstellungen verwendet.
* Unterstützung für App Service-Umgebung hinzugefügt: az appservice ase show | list | list-addresses | list-plans | create | update | delete

### <a name="backup"></a>Backup

* Problem in Az-Sicherungsrichtlinie „list-associated-items“ behoben. Optionaler Parameter „BackupManagementType“ hinzugefügt.

### <a name="compute"></a>Compute

* API-Version von Compute, Datenträger, Momentaufnahmen auf 2019-07-01 aktualisiert
* vmss create: Verbesserung für – Orchestrierungsmodus
* sig image-definition create: „--os-state“ hinzugefügt, um die Angabe zu ermöglichen, ob die unter diesem Image erstellten virtuellen Computer „generalisiert“ oder „spezialisiert“ sind
* sig image-definition create: „--hyper-v-generation“ hinzugefügt, um die Angabe der Hypervisorgeneration zu ermöglichen
* sig image-version create: Unterstützung für „--os-snapshot“ und „--data-snapshots“ hinzugefügt
* image create: „--data-disk-caching“ hinzugefügt, um die Angabe der Zwischenspeicherungseinstellung von Datenträger zu ermöflichen
* Upgrade des Python-Compute-SDK auf 10.0.0
* vm/vmss create: „Spot“ zu Aufzählungseigenschaft „Priority“ hinzugefügt
* [Breaking Change] Parameter „--max-billing“ für sowohl VM als auch VMSS in „--max-price“ umbenannt, um die Konsistenz mit Swagger- und PowerShell-Cmdlets sicherzustellen
* vm monitor log show: Unterstützung für das Abfragen von Protokollen über verknüpften Protokollanalyse-Arbeitsbereich hinzugefügt.

### <a name="iot"></a>IoT

* Behebung Nr. 2531: Argumente für Benutzerfreundlichkeit für Hub-Update hinzugefügt.
* Behebung Nr. 8323: Fehlende Parameter zum Erstellen eines benutzerdefinierten Speicherendpunkts hinzugefügt.
* Regressionsfehler behoben: Die Änderungen wurden rückgängig gemacht, sodass der standardmäßige Speicherendpunkt überschrieben wurde.

### <a name="key-vault"></a>Key Vault

* Nr. 11121 behoben: Bei der Verwendung von `az keyvault certificate list` erfordert die Übergabe von `--include-pending` jetzt nicht mehr den Wert `true` oder `false`.

### <a name="netappfiles"></a>NetAppFiles

* Upgrade von „azure-mgmt-netapp“ auf Version 0.7.0, die einige zusätzliche Volumeeigenschaften enthält, die bevorstehenden Replikationsvorgängen zugeordnet sind

### <a name="network"></a>Netzwerk

* application-gateway waf-config: veraltet
* application-gateway waf-policy: Untergruppe „managed-rules“ zur Verwaltung von verwalteten Regelsätzen und Ausschlussregeln hinzugefügt
* application-gateway waf-policy: Untergruppe „policy-setting“ zur Verwaltung der globalen Konfiguration von „waf-policy“ hinzugefügt
* [BREAKING CHANGE] application-gateway waf-policy: Untergruppenregel in „custom-rule“ umbenannt
* application-gateway http-listener: „--firewall-policy“ beim Erstellen hinzugefügt
* application-gateway url-path-map rule: „--firewall-policy“ beim Erstellen hinzugefügt

### <a name="packaging"></a>Verpackung

* Az-Wrapper in Python neu geschrieben
* Unterstützung für Python 3.8 hinzugefügt
* Für RPM-Paket in Python 3 geändert

### <a name="profile"></a>Profil

* Fehler beim Ausführen von `az login -u {} -p {}` mit Microsoft-Konto entfernt
* `SSLError` beim Ausführen von `az login` hinter einem Proxy mit einem selbstsignierten Stammzertifikat entfernt
* Nr. 10578 behoben: `az login` hängt, wenn mehrere Instanzen gleichzeitig unter Windows oder WSL gestartet werden.
* Nr. 11059 behoben: `az login --allow-no-subscriptions` schlägt fehl, wenn Abonnements im Mandanten vorhanden sind.
* Nr. 11238 behoben: Nach dem Umbenennen eines Abonnements führt die Anmeldung mit MSI dazu, dass das gleiche Abonnement zweimal angezeigt wird.

### <a name="rbac"></a>RBAC

* Nr. 10996 behoben: Fehler für `--force-change-password-next-login` in `az ad user update` entfernt, wenn `--password` nicht angegeben ist

### <a name="redis"></a>Redis

* Nr. 2902 behoben: Festlegen von Speicherkonfigurationen beim Aktualisieren des Basic-SKU-Cache vermeiden

### <a name="reservations"></a>Reservations

* SDK-Version auf 0.6.0 aktualisiert
* Abrechnungsplandetails nach dem Aufrufen von „Get-Gatalogs“ hinzugefügt
* Neuer Befehl `az reservations reservation-order calculate` zum Berechnen des Preises für eine Reservierung hinzugefügt
* Neuer Befehl `az reservations reservation-order purchase` zum Erwerb einer neuen Reservierung hinzugefügt

### <a name="rest"></a>REST
* `az rest` in allgemeine Verfügbarkeit geändert

### <a name="sql"></a>SQL

* „azure-mgmt-sql“ auf Version 0.15.0 aktualisiert.

### <a name="storage"></a>Storage

* storage account create: „--enable-hierarchical-namespace“ hinzugefügt, um Dateisystemsemantik in Blobdienst zu unterstützen.
* Ausnahme ohne Zusammenhang aus Fehlermeldung entfernt
* Probleme mit falscher Fehlermeldung „Sie verfügen nicht über die erforderlichen Berechtigungen zum Ausführen dieses Vorgangs“ behoben. bei Blockierung durch Netzwerkregeln oder bei „AuthenticationFailed“.

## <a name="november-4-2019"></a>4\. November 2019

Version 2.0.76

### <a name="acr"></a>ACR

* Vorschauparameter `--pack-image-tag` wurde dem Befehl `az acr pack build` hinzugefügt.
* Unterstützung der Aktivierung der Überwachung beim Erstellen einer Registrierung hinzugefügt
* Unterstützung von RBAC mit Repositoryumfang hinzugefügt

### <a name="aks"></a>AKS

* `--enable-cluster-autoscaler`, `--min-count` und `--max-count` wurden dem Befehl `az aks create` hinzugefügt, sodass die automatische Clusterskalierung für den Knotenpool aktiviert ist.
* Die obigen Flags sowie `--update-cluster-autoscaler` und `--disable-cluster-autoscaler` wurden dem Befehl `az aks update` hinzugefügt, sodass Updates der automatischen Clusterskalierung zulässig sind.

### <a name="appconfig"></a>AppConfig

* Befehlsgruppe der AppConfig-Funktion zum Verwalten von in einer App Configuration-Instanz gespeicherten Featureflags wurde hinzugefügt.
* Geringfügiger Programmfehler für Befehl „appconfig kv export to file“ wurde behoben. Das Lesen der Zieldateiinhalte wird während des Exports angehalten.

### <a name="appservice"></a>AppService

* `az appservice plan create`: Unterstützung für das Festlegen von „persitescalung“ beim Erstellen eines App-Serviceplans wurde hinzugefügt.
* Ein Problem wurde behoben, aufgrund dessen der Vorgang „webapp config ssl bind“ vorhandene Tags aus der Ressource entfernt hat.
* Flag `--build-remote` wurde für `az functionapp deployment source config-zip` hinzugefügt, um die Remotebuildaktion während der Funktions-App-Bereitstellung zu unterstützen.
* Die Standardknotenversion in Funktions-Apps wurde für Windows in ~ 10 geändert.
* `--runtime-version`-Eigenschaft zu `az functionapp create` hinzugefügt

### <a name="arm"></a>ARM

* `az deployment/group deployment validate`: Parameter `--handle-extended-json-format` wurde hinzugefügt, um bei der Bereitstellung mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen.
* „azure-mgmt-resource“ auf „2019-07-01“ festgelegt

### <a name="backup"></a>Backup

* Unterstützung für AzureFiles-Sicherung hinzugefügt

### <a name="compute"></a>Compute

* `az vm create`: Beim gleichzeitigen Festlegen von beschleunigtem Netzwerkbetrieb und einer vorhandenen NIC wurde eine Warnung hinzugefügt.
* `az vm create`: `--vmss` hinzugefügt, um eine vorhandene VM-Skalierungsgruppe anzugeben, welcher der virtuelle Computer zugewiesen werden soll.
* `az vm/vmss create`: Eine lokale Kopie der Imagealiasdatei wurde hinzugefügt, sodass in einer eingeschränkten Netzwerkumgebung darauf zugegriffen werden kann.
* `az vmss create`: `--orchestration-mode` hinzugefügt, um anzugeben, wie virtuelle Computer von der Skalierungsgruppe verwaltet werden.
* `az vm/vmss update`: `--ultra-ssd-enabled` hinzugefügt, um das Aktualisieren der SSD-Einstellung zuzulassen.
* [BREAKING CHANGE] `az vm extension set`: Ein Fehler wurde behoben, aufgrund dessen Benutzer mit `--ids` keine Erweiterung auf einem virtuellen Computer festlegen konnten.
* Neue Befehle wurden zu `az vm image terms accept/cancel/show` hinzugefügt , um Azure Marketplace-Imagebedingungen zu verwalten.
* VMAccessForLinux auf Version 1.5 aktualisiert

### <a name="cosmosdb"></a>CosmosDB

* [BREAKING CHANGE] `az sql container create`: `--partition-key-path` in erforderlichen Parameter geändert
* [BREAKING CHANGE] `az gremlin graph create`: `--partition-key-path` in erforderlichen Parameter geändert
* `az sql container create`: `--unique-key-policy` und `--conflict-resolution-policy` hinzugefügt
* `az sql container create/update`: Aktualisierung des `--idx`-Standardschemas
* `gremlin graph create`: `--conflict-resolution-policy` hinzugefügt
* `gremlin graph create/update`: Aktualisierung des `--idx`-Standardschemas
* Tippfehler in Hilfemeldung korrigiert
* Datenbank: Informationen zur eingestellten Unterstützung hinzugefügt
* Auflistung: Informationen zur eingestellten Unterstützung hinzugefügt

### <a name="iot"></a>IoT

* Neuer Routingquelltyp hinzugefügt: DigitalTwinChangeEvents
* Fehlende Features in `az iot hub create` behoben

### <a name="key-vault"></a>Key Vault

* Ein unerwarteter Fehler wurde behoben, bei dem keine Zertifikatdatei vorhanden war.
* Funktionsunfähigkeit von `az keyvault recover/purge` behoben

### <a name="netappfiles"></a>NetAppFiles

* „azure-mgmt-netapp“ wurde auf 0.6.0 aktualisiert, um API-Version 2019-07-01 zu verwenden. Diese neue API-Version umfasst:

    - Volumeerstellung `--protocol-types` akzeptiert jetzt „NFSv4.1“ anstelle von „NFSv4“.
    - Die Richtlinie der Volumeexportrichtlinie heißt jetzt „nfsv41“ anstelle von „nfsv4“.
    - Volume `--creation-token` wurde in `--file-path` umbenannt.
    - Das Erstellungsdatum einer Momentaufnahme heißt jetzt einfach „erstellt“.

### <a name="network"></a>Netzwerk

* `az network private-dns link vnet create/update`: Unterstützung für mandantenübergreifende Verknüpfung virtueller Netzwerke.
* [BREAKING CHANGE] `az network vnet subnet list`: `--resource-group` und `--vnet-name` wurden geändert und sind jetzt erforderlich.
* `az network public-ip prefix create`: Unterstützung der Angabe der IP-Adressversion (IPv4, IPv6) bei der Erstellung hinzugefügt
* „azure-mgmt-network“ auf 7.0.0 und „api-version“ auf 2019-09-01 festgelegt
* `az network vrouter`: Unterstützung für neuen virtuellen Dienstrouter und virtuelles Routerpeering hinzugefügt
* `az network express-route gateway connection`: Unterstützung für `--internet-security` wurde hinzugefügt.

### <a name="profile"></a>Profil

* Funktionsunfähigkeit von `az account get-access-token --resource-type ms-graph` behoben
* Warnung aus `az login` entfernt

### <a name="rbac"></a>RBAC

* Funktionsunfähigkeit von `az ad app update --id {} --display-name {}` behoben

### <a name="servicefabric"></a>ServiceFabric

* `az sf cluster create`: Ein Problem wurde behoben, indem die Compute-VMSS von „template.json“ für Service Fabric unter Linux und Windows von Standarddatenträgern auf verwaltete Datenträger umgestellt wurde.

### <a name="sql"></a>SQL

* Die Parameter `--compute-model`, `--auto-pause-delay` und `--min-capacity` wurden hinzugefügt, um CRUD-Vorgänge für das neue SQL-Datenbank-Angebot zu unterstützen: Serverloses Computemodell.

### <a name="storage"></a>Storage

* `az storage account create/update`: Parameter „--enable-files-adds“ und Azure Active Directory-Eigenschaftenargumentgruppe hinzugefügt, um Active Directory Domain-Dienstauthentifizierung für Azure Files zu unterstützen.
* `az storage account keys list/renew` wurde erweitert, um die Auflistung oder erneute Generierung von Kerberos-Schlüsseln des Speicherkontos zu unterstützen.

## <a name="october-15-2019"></a>15. Oktober 2019

Version 2.0.75

### <a name="aks"></a>AKS

* Standardwert `--load-balancer-sku` in `standard` geändert, sofern von der Kubernetes-Version unterstützt
* Standardwert `--vm-set-type` in `virtualmachinescalesets` geändert, sofern von der Kubernetes-Version unterstützt

### <a name="ams"></a>AMS

* [BREAKING CHANGE] Name von `job start` in `job create` geändert
* [BREAKING CHANGE] Parameter `--ask` von `content-key-policy create` geändert, sodass eine hexadezimale Zeichenfolge mit 32 Zeichen anstelle von UTF8 verwendet wird

### <a name="appservice"></a>AppService

* Befehle vom Typ `webapp config access-restriction show|set|add|remove` hinzugefügt
* Bessere Fehlerbehandlung zu `webapp up` hinzugefügt
* Unterstützung für SKU `Isolated` zu `appservice plan update` hinzugefügt

### <a name="arm"></a>ARM

* Parameter `--handle-extended-json-format` zu `deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen

### <a name="compute"></a>Compute

* Parameter `--enable-agent` zu `vm create` hinzugefügt
* `vm create` geändert, um bei der Verwendung von Zonen die SKU „Standard“ für die öffentliche IP-Adresse zu verwenden
* `vm create` geändert, um automatisch einen gültigen Computernamen für eine VM zu erstellen, falls keiner angegeben wurde
* Parameter `--computer-name-prefix` zu `vmss create` hinzugefügt, um das benutzerdefinierte Computernamenspräfix virtueller Computer in VMSS zu unterstützen
* Parameter `--workspace` zu `vm create` hinzugefügt, um automatisch einen Log Analytics-Arbeitsbereich zu aktivieren
* API-Version für Kataloge auf 2019-07-01 aktualisiert

### <a name="core"></a>Core

* Syntaxprüfung für Parameter `--set` im generischen Updatebefehl hinzugefügt

### <a name="iot"></a>IoT

* Problem behoben, bei dem für `iot hub show` der Fehler „Ressource nicht gefunden.“ zurückgegeben wurde

### <a name="monitor"></a>Überwachen

* Unterstützung für CRUD zu `monitor log-analytics workspace` hinzugefügt

### <a name="network"></a>Netzwerk

* Unterstützung für mandantenübergreifende virtuelle Verbindung zu `network private-dns link vnet [create|update]` hinzugefügt
* [BREAKING CHANGE]`network vnet subnet list` geändert, um Parameter `--resource-group` und `--vnet-name` vorauszusetzen

### <a name="sql"></a>SQL

* Befehle zu `sql mi ad-admin` hinzugefügt, die das Festlegen eines AAD-Administrators für verwaltete Instanzen unterstützen

### <a name="storage"></a>Storage

* Parameter `--preserve-s2s-access-tier` zu `storage copy` hinzugefügt, um die Zugriffsebene beim Kopieren von Dienst zu Dienst beizubehalten
* Parameter `--enable-large-file-share` zu `storage account [create|update]` hinzugefügt, um große Dateifreigaben für ein Speicherkonto zu unterstützen

## <a name="september-24-2019"></a>24. September 2019

Version 2.0.74

### <a name="acr"></a>ACR

* Erforderlicher Parameter `--type` zu `acr config retention update` hinzugefügt
* [BREAKING CHANGE] Umbenannter Parameter `--name -n` in `--registry -r ` für Befehlsgruppe `acr config` geändert

### <a name="aks"></a>AKS

* Parameter `--load-balancer-sku` zum Befehl `aks create` hinzugefügt, um die Erstellung von AKS-Clustern mit SLB zu ermöglichen
* Parameter `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` und `--load-balancer-outbound-ip-prefixes` zu den Befehlen `aks [create|update]` hinzugefügt,um die Aktualisierung des Lastenausgleichsprofils eines AKS-Clusters mit SLB zu ermöglichen
* Parameter `--vm-set-type` zum Befehl `aks create` hinzugefügt, um die Angabe von VM-Typen eines AKS-Clusters (vmas oder vmss) zu ermöglichen

### <a name="arm"></a>ARM

* Parameter `--handle-extended-json-format` zum Befehl `group deployment create` hinzugefügt, um mehrere Zeilen und Kommentare in der JSON-Vorlage zu unterstützen

### <a name="compute"></a>Compute

* Parameter `--terminate-notification-time` zu den Befehlen `vmss [create|update]` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen
* Parameter `--enable-terminate-notification` zu den Befehlen `vmss update` hinzugefügt, um die Konfigurierbarkeit der Beendigung geplanter Ereignisse zu unterstützen
* Parameter `--priority,` `--eviction-policy,` `--max-billing` zu `[vm|vmss] create`-Befehlen hinzugefügt
* `disk create` geändert, um die Angabe der genauen Größe des Datenträgeruploads zu ermöglichen
* Unterstützung für inkrementelle Momentaufnahmen für verwaltete Datenträger zu `snapshot create` hinzugefügt

### <a name="cosmos-db"></a>Cosmos DB

* Parameter `--type <key-type>` zum Befehl `cosmosdb keys list` hinzugefügt, um Schlüssel, schreibgeschützte Schlüssel oder Verbindungszeichenfolgen anzuzeigen
* Befehl `cosmosdb keys regenerate` hinzugefügt
* [VERALTET] Befehle `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` und `cosmosdb list-read-only-keys` als veraltet markiert

### <a name="eventgrid"></a>EventGrid

* Endpunkthilfetext korrigiert, um auf den richtigen Parameter zu verweisen

### <a name="key-vault"></a>Key Vault

* Problem behoben, aufgrund dessen die Anmeldung mit einem Mandanten (`login -t`) unter Umständen zu einem Fehler von `keyvault create` führte

### <a name="monitor"></a>Überwachen

* Problem behoben, aufgrund dessen das Zeichen `:` in `--condition` für `monitor metrics alert create` nicht zulässig war

### <a name="policy"></a>Richtlinie

* Unterstützung für Policy-API-Version 2019-06-01 hinzugefügt
* Parameter `--enforcement-mode` zum Befehl `policy assignment create` hinzugefügt

### <a name="storage"></a>Storage

* Parameter `--blob-type` zum Befehl `az storage copy` hinzugefügt

## <a name="september-10-2019"></a>10. September 2019

### <a name="acr"></a>ACR

* Befehlsgruppe `acr config retention` zum Konfigurieren der Aufbewahrungsrichtlinie hinzugefügt

### <a name="aks"></a>AKS

* Unterstützung für die ACR-Integration mit den folgenden Befehlen hinzugefügt:
  * Parameter `--attach-acr` zu `aks [create|update]` hinzugefügt, um einen ACR an einen AKS-Cluster anzufügen
  * Parameter `--detach-acr` zu `aks update` hinzugefügt, um den ACR von einem AKS-Cluster zu trennen

### <a name="arm"></a>ARM

* Zur Verwendung der API-Version 2019-05-10 aktualisiert

### <a name="batch"></a>Batch

* Neue JSON-Konfigurationseinstellungen für `batch pool create` zu `--json-file` hinzugefügt:
  * `MountConfigurations` für Dateisystemeinbindungen hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )
  * Optionale Eigenschaft `publicIPs` in `NetworkConfiguration` für öffentliche IP-Adressen für Pools hinzugefügt (Details siehe https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body )
* Unterstützung für Kataloge mit freigegebenen Images zu `--image` hinzugefügt
* [BREAKING CHANGE] Standardwert von `--start-task-wait-for-success` für `batch pool create` in `true` geändert
* [BREAKING CHANGE] Standardwert von `Scope` für `AutoUserSpecification` geändert, damit immer „Pool“ verwendet wird (vormals `Task` für Windows-Knoten bzw. `Pool` für Linux-Knoten)
  * Dieses Argument kann nur über eine JSON-Konfiguration mit `--json-file` festgelegt werden.

### <a name="hdinsight"></a>HDInsight

* Allgemein verfügbares Release
* [BREAKING CHANGE] Parameter `--workernode-count/-c` von `az hdinsight resize` in erforderlich geändert

### <a name="key-vault"></a>Key Vault

* Problem behoben, aufgrund dessen Subnetze nicht aus Netzwerkregeln gelöscht werden konnten
* Problem behoben, aufgrund dessen doppelte Subnetze und IP-Adressen zu Netzwerkregeln hinzugefügt werden konnten

### <a name="network"></a>Netzwerk

* Parameter `--interval` zu `network watcher flow-log` hinzugefügt, um den Wert für das Intervall der Datenverkehrsanalyse festzulegen
* `network application-gateway identity` zum Verwalten der Gatewayidentität hinzugefügt
* Unterstützung zum Festlegen der Key Vault-ID zu `network application-gateway ssl-cert` hinzugefügt
* `network express-route peering peer-connection [show|list]` hinzugefügt

### <a name="policy"></a>Richtlinie

* Zur Verwendung der API-Version 2019-01-01 aktualisiert

## <a name="august-27-2019"></a>27. August 2019

Version 2.0.72

### <a name="acr"></a>ACR

* [BREAKING CHANGE] Unterstützung für SKU `classic` entfernt

### <a name="api-management"></a>API Management

* [VORSCHAU] Befehlsgruppe `apim` hinzugefügt

### <a name="appservice"></a>AppService

* Problem mit dem Befehl `webapp webjob continuous start` bei Angabe eines Slots behoben
* `webapp up` geändert, um den Ordner `env` zu erkennen und aus der für die Bereitstellung verwendeten Datei zu entfernen

### <a name="keyvault"></a>KeyVault

* Fehler in `keyvault secret set` behoben, aufgrund dessen das Argument `--expires` ignoriert wurde

### <a name="network"></a>Netzwerk

* Unterstützung für IPv6-Adressen zu Argumenten vom Typ `--private-ip-address-version` hinzugefügt
* Neue Befehle vom Typ `network private-endpoint [create|update|list-types]` für die Verwaltung privater Endpunkte hinzugefügt
* Befehlsgruppe `network private-link-service` hinzugefügt
* Argumente `--private-endpoint-network-policies` und `--private-link-service-network-policies` zu `network vnet subnet update` hinzugefügt

### <a name="rbac"></a>RBAC

* Problem mit `ad app update --homepage` behoben, aufgrund dessen die Startseite nicht aktualisiert wurde

### <a name="servicefabric"></a>ServiceFabric

* Unterstützung für Key Vault-Namen mit Groß- und Kleinschreibung hinzugefügt
* Problem bei der Verwendung von Zertifikaten in Key Vault behoben
* Problem bei der Verwendung von PFX-Zertifikatdateien behoben
* Problem mit `sf cluster certificate add` behoben, wenn keine Key Vault-Ressourcengruppe angegeben wurde
* Problem behoben, aufgrund dessen `sf cluster set` nicht funktionierte

### <a name="signalr"></a>SignalR

* Neue Befehle hinzugefügt:
  * `signalr cors`: Verwalten von CORS für SignalR
  * `signalr restart`: Starten eines SignalR-Diensts
  * `signalr update`: Aktualisieren eines SignalR-Diensts
* Argument `--service-mode` zu `signalr create` hinzugefügt

### <a name="storage"></a>Storage

* Befehl `storage account revoke-delegation-keys` hinzugefügt

## <a name="august-13-2019"></a>13. August 2019

Version 2.0.71

### <a name="appservice"></a>AppService

* Problem behoben, aufgrund dessen bei Befehlen vom Typ `webapp webjob continuous` für Slots Fehler auftraten

### <a name="botservice"></a>BotService

* [BREAKING CHANGE] Unterstützung für die Erstellung von Bots der Version 3 entfernt

### <a name="cognitiveservices"></a>CognitiveServices

* Befehle vom Typ `cognitiveservices account network-rule` hinzugefügt

### <a name="cosmos-db"></a>Cosmos DB

* Beim Aktualisieren mehrerer Schreibstandorte wurde eine Warnung entfernt.
* CRUD-Befehle für CosmosDB SQL-, MongoDB-, Cassandra-, Gremlin- und Tabellenressourcen sowie den Ressourcendurchsatz hinzugefügt

### <a name="hdinsight"></a>HDInsight

Dieses Release enthält zahlreiche wichtige Änderungen.

* [BREAKING CHANGE] Parameter für `hdinsight create` umbenannt:
  * `--storage-default-container` in `--storage-container` umbenannt
  * `--storage-default-filesystem` in `--storage-filesystem` umbenannt
* [BREAKING CHANGE] Das Argument `--name` von `application create` wurde so geändert, dass es den Anwendungsnamen anstelle des Clusternamens darstellt.
* Argument `--cluster-name` zu `application create` hinzugefügt, um die alte Funktion `--name` zu ersetzen
* [BREAKING CHANGE] Parameter für `application create` umbenannt:
  * `--application-type` in `--type` umbenannt
  * `--marketplace-identifier` in `--marketplace-id` umbenannt
  * `--https-endpoint-access-mode` in `--access-mode` umbenannt
  * `--https-endpoint-destination-port` in `--destination-port` umbenannt
* [BREAKING CHANGE] Parameter für `application create` entfernt:
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* [WICHTIGE ÄNDERUNG] `--target-instance-count` für `hdinsight resize` in `--workernode-count` umbenannt
* [BREAKING CHANGE] Alle Befehle in der Gruppe `hdinsight script-action` wurden so geändert, dass sie den Parameter `--name` als Namen der Skriptaktion verwenden.
* Argument `--cluster-name` zu allen Befehlen vom Typ `hdinsight script-action` hinzugefügt, um die alte Funktion `--name` zu ersetzen
* [BREAKING CHANGE]`--script-execution-id` für alle Befehle vom Typ `hdinsight script-action` in `--execution-id` umbenannt
* [BREAKING CHANGE]`hdinsight script-action show` in `hdinsight script-action show-execution-details` umbenannt
* [WICHTIGE ÄNDERUNG] Parameter in `hdinsight script-action execute --roles` geändert, sodass sie durch Leerzeichen anstelle von Kommas getrennt sind
* [BREAKING CHANGE] Parameter `--persisted` für `hdinsight script-action list` entfernt
* Der Parameter `hdinsight create --cluster-configurations` wurde so geändert, dass er einen Pfad zu einer lokalen JSON-Datei oder JSON-Zeichenfolge akzeptiert.
* Befehl `hdinsight script-action list-execution-history` hinzugefügt
* `hdinsight monitor enable --workspace` geändert, um die ID oder den Namen eines Log Analytics-Arbeitsbereichs zu akzeptieren
* Argument `hdinsight monitor enable --primary-key` hinzugefügt. Dieses Argument wird benötigt, wenn eine Arbeitsbereichs-ID als Parameter angegeben wird.
* Weitere Beispiele und aktualisierte Beschreibungen für Hilfemeldungen hinzugefügt

### <a name="interactive"></a>Interactive

* Ladefehler behoben

### <a name="kubernetes"></a>Kubernetes

* Änderung, um `https` zu verwenden, wenn der Dashboardcontainerport `https` verwendet

### <a name="network"></a>Netzwerk

* Argument `--yes` hinzugefügt zu `network dns record-set cname delete`

### <a name="profile"></a>Profil

* Argument `--resource-type` zu `account get-access-token` zum Abrufen von Ressourcenzugriffstoken hinzugefügt

### <a name="servicefabric"></a>ServiceFabric

* Alle unterstützten Betriebssystemversionen für „sf cluster create“ hinzugefügt
* Fehler beim Überprüfen des primären Zertifikats behoben

### <a name="storage"></a>Storage

* Befehl `storage copy` hinzugefügt

## <a name="july-30-2019"></a>30. Juli 2019

Version 2.0.70

### <a name="acr"></a>ACR

* Problem #9952 behoben (Regression im Befehl `acr pack build`)
* Standardname des Generatorimages in `acr pack build` entfernt

### <a name="appservice"></a>AppService

* `webapp config ssl` geändert, um eine Meldung anzuzeigen, wenn eine Ressource nicht gefunden wurde
* Problem behoben, aufgrund dessen `functionapp create` den Speicherkontotypen `Standard_RAGRS` nicht akzeptiert hat
* Problem behoben, aufgrund dessen für `webapp up` ein Fehler auftrat, wenn für die Ausführung ältere Python-Versionen verwendet wurden

### <a name="network"></a>Netzwerk

* Ungültiger Parameter `--ids` aus `network nic ip-config add` entfernt (Fehlerbehebungen #9861)
* Fehlerbehebungen #9604. Parameter `--root-certs` zu `network application-gateway http-settings [create|update]` hinzugefügt, um vom Benutzer zugewiesene vertrauenswürdige Stammzertifikate zu unterstützen.
* Argument `--subscription` für `network dns record-set ns create` korrigiert (#9965)

### <a name="rbac"></a>RBAC

* Befehl `user update` hinzugefügt
* [VERALTET]`--upn-or-object-id` in benutzerbezogenen Befehlen als veraltet markiert
    * Verwenden Sie das Ersatzargument `--id`.
* Argument `--id` zu benutzerbezogenen Befehlen hinzugefügt

### <a name="sql"></a>SQL

* Verwaltungsbefehle für Schlüssel verwalteter Instanzen und TDE-Schutzvorrichtung hinzugefügt

### <a name="storage"></a>Storage

* Befehl `storage remove` hinzugefügt
* Problem mit `storage blob update` behoben

### <a name="vm"></a>VM

* `list-skus` wurde geändert, um eine neuere API-Version für die Ausgabe von Zonendetails zu verwenden.
* Standardwert `--single-placement-group` für `vmss create` in `false` geändert
* Möglichkeit zum Auswählen von ZRS-Speicher-SKUs für `[snapshot|disk] create` hinzugefügt
* Neue Befehlsgruppe `vm host` zur Unterstützung dedizierter Hosts hinzugefügt
* Parameter `--host` und `--host-group` für `vm create` hinzugefügt, um den dedizierten VM-Host festzulegen

## <a name="july-16-2019"></a>16. Juli 2019

Version 2.0.69

### <a name="appservice"></a>AppService

* `webapp identity`-Befehle geändert, um eine korrekte Fehlermeldung zurückzugeben, wenn „ResourceGroupName“ oder der App-Name ungültig sind
* `webapp list` korrigiert, sodass der korrekte Wert für „numberOfSites“ zurückgegeben wird, wenn „ResourceGroup“ nicht angegeben wurde
* Nebeneffekte von `appservice plan create` und `webapp create` behoben

### <a name="core"></a>Core

* Problem behoben, aufgrund dessen `--subscription` angezeigt wurde, obwohl nicht anwendbar

### <a name="batch"></a>Batch

* [BREAKING CHANGE]`batch pool node-agent-skus list` durch `batch pool supported-images list` ersetzt
* Unterstützung für Sicherheitsregeln hinzugefügt, die den Netzwerkzugriff auf einen Pool basierend auf dem Quellport des Datenverkehrs blockieren, wenn die Option `--json-file` von `batch pool create network` verwendet wird
* Unterstützung für die Ausführung der Aufgabe im Arbeitsverzeichnis des Containers oder der Batch-Aufgabe hinzugefügt, wenn die Option `--json-file` von `batch task create` verwendet wird
* Fehler in Option `--application-package-references` von `batch pool create` behoben, aufgrund dessen nur Standardeinstellungen möglich waren

### <a name="eventhubs"></a>Event Hubs

* Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt

### <a name="rdbms"></a>RDBMS

* Optionaler Parameter zum Angeben der Replikat-SKU für den Befehl zum Erstellen von Replikaten hinzugefügt
* Problem mit CI-Testfehler bei der Erstellung von MySQL-Replikaten behoben

### <a name="relay"></a>Relay

* Problem mit Hybridverbindung behoben, wenn die Client-Autorisierung deaktiviert ist [#8775](https://github.com/azure/azure-cli/issues/8775)
* Parameter `--requires-transport-security` zu `relay wcfrelay create` hinzugefügt

### <a name="servicebus"></a>ServiceBus

* Validierung für Parameter `--rights` von `authorizationrule`-Befehlen hinzugefügt

### <a name="storage"></a>Storage

* AADDS für Files für Speicherkontoaktualisierung aktiviert
* Problem `storage blob service-properties update --set` behoben

## <a name="july-2-2019"></a>2\. Juli 2019

Version 2.0.68

### <a name="core"></a>Core

* Befehlsmodule sind jetzt in einer einzelnen verteilbaren Python-Komponente zusammengefasst. Die direkte Verwendung zahlreicher Pakete vom Typ `azure-cli-` in PyPI ist daher veraltet.
  Dadurch sollte sich die Installationsgröße reduzieren. Darüber hinaus sollte es nur Benutzer betreffen, die eine direkte Installation über `pip` ausgeführt haben.

### <a name="acr"></a>ACR

* Unterstützung für Trigger mit Timer zu Aufgabe hinzugefügt

### <a name="appservice"></a>AppService

* `functionapp create` wurde so geändert, das Application Insights standardmäßig aktiviert wird.
* [BREAKING CHANGE] Veralteter Befehl `functionapp devops-build` entfernt.
  *  Verwenden Sie stattdessen den neuen Befehl `az functionapp devops-pipeline`.
* Unterstützung des Funktions-App-Plans für Linux-Verbrauch zu `functionapp deployment config-zip` hinzugefügt

### <a name="cosmos-db"></a>Cosmos DB

* Unterstützung für das Deaktivieren von TTL hinzugefügt

### <a name="dls"></a>DLS

* Aktualisierte ADLS-Version (0.0.45)

### <a name="feedback"></a>Feedback

* Wird ein fehlgeschlagener Erweiterungsbefehl gemeldet, versucht `az feedback` nun, über den Index die Projekt-/Repository-URL der Erweiterung im Browser zu öffnen.

### <a name="hdinsight"></a>HDInsight

* [BREAKING CHANGE] Der Befehlsgruppenname `oms` wurde in `monitor` geändert.
* [BREAKING CHANGE]`--http-password/-p` als erforderlicher Parameter festgelegt 
* Vervollständigungen für `--cluster-admin-account` und `cluster-users-group-dns` hinzugefügt 
* Parameter `cluster-users-group-dns` so geändert, dass er erforderlich ist, wenn `—esp` vorhanden ist
* Timeout für alle vorhandenen automatischen Argumentvervollständigungen hinzugefügt
* Timeout für das Transformieren des Ressourcennamens in eine Ressourcen-ID hinzugefügt
* Die automatischen Vervollständigungen wurden so geändert, dass Ressourcen aus einer beliebigen Ressourcengruppe ausgewählt werden. Dabei kann es sich um eine andere Ressourcengruppe als die mit `-g` angegebene Gruppe handeln.
* Unterstützung für die Parameter `--sub-domain-suffix` und `--disable_gateway_auth` im Befehl `hdinsight application create` hinzugefügt

### <a name="managed-services"></a>Verwaltete Dienste

* Befehlsmodul für verwaltete Dienste als Vorschau eingeführt

### <a name="profile"></a>Profil
* Argument `--subscription` für Abmeldebefehl unterdrückt

### <a name="rbac"></a>RBAC

* [BREAKING CHANGE] Argument `--password` für `create-for-rbac` entfernt
* Parameter `--assignee-principal-type` zum Befehl `create` hinzugefügt, um zeitweilige Fehler zu vermeiden, die durch die Replikationswartezeit des AAD-Graph-Servers verursacht werden
* Absturz in `ad signed-in-user` beim Auflisten von in Besitz befindlichen Objekten behoben
* Problem behoben, aufgrund dessen `ad sp` nicht die richtige Anwendung über einen Dienstprinzipal fand

### <a name="rdbms"></a>RDBMS

* Unterstützung für die Replikation für MariaDB hinzugefügt

### <a name="sql"></a>SQL

* Zulässige Werte für `sql db create --sample-name` dokumentiert

### <a name="storage"></a>Storage

* Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage blob generate-sas` hinzugefügt 
* Unterstützung von SAS-Token für die Benutzerdelegierung mit `--as-user` zu `storage container generate-sas` hinzugefügt 

### <a name="vm"></a>VM

* Fehler behoben, aufgrund dessen `vmss create` bei der Ausführung mit `--no-wait` eine Fehlermeldung zurückgab
* Die clientseitige Validierung für `vmss create --single-placement-group` wurde entfernt. Es tritt kein Fehler auf, wenn `--single-placement-group` auf `true` und für `--instance-count` ein größerer Wert als 100 festgelegt wird oder wenn Verfügbarkeitszonen angegeben werden. Diese Validierung wird jedoch dem Computedienst überlassen.
* Problem behoben, aufgrund dessen bei der Verwendung von `--latest` für `[vm|vmss] extension image list` ein Fehler auftrat


## <a name="june-18-2019"></a>18. Juni 2019

Version 2.0.67

### <a name="core"></a>Core

In diesem Release wird das neue [Preview]-Tag eingeführt, um Kunden gegenüber deutlich zu machen, dass sich eine Befehlsgruppe, ein Befehl oder ein Argument in der Vorschauphase befindet. Diese Information war zuvor im Hilfetext oder implizit durch die Versionsnummer des Befehlsmoduls angegeben.
Die Befehlszeilenschnittstelle wird künftig Versionsnummern für einzelne Pakete entfernen. Wenn sich ein Befehl in der Vorschauphase befindet, gilt dies auch für alle seine Argumente. Wenn eine Befehlsgruppe als Vorschau gekennzeichnet ist, befinden sich auch alle Befehle und Argumente in der Vorschauphase.

Infolge dieser Änderung befinden sich in diesem Release verschiedene Befehlsgruppen anscheinend „plötzlich“ in der Vorschauphase. Tatsächlich ist es jedoch so, dass sich die meisten Pakete in der Vorschauphase befanden, in diesem Release jedoch als allgemein verfügbar gelten.

### <a name="acr"></a>ACR
* Befehl „acr check-health“ hinzugefügt
* Verbesserte Fehlerbehandlung für AAD-Token und für das Abrufen externer Befehle

### <a name="acs"></a>ACS
* Veraltete ACS-Befehle werden jetzt in der Hilfeansicht ausgeblendet.

### <a name="ams"></a>AMS
* [BREAKING CHANGE] Änderung, damit ISO 8601-Zeitzeichenfolgen für „archive-window-length“ und „key-frame-interval-duration“ zurückgegeben werden

### <a name="appservice"></a>AppService
* Standortbasiertes Routing für `webapp deleted list` und `webapp deleted restore` hinzugefügt
* Problem behoben, aufgrund dessen in Azure Cloud Shell nicht auf die von einer Web-App protokollierte Ziel-URL („Sie können die App starten unter...“) geklickt werden konnte
* Problem behoben, aufgrund dessen beim Erstellen von Apps bei einigen SKUs ein AlwaysOn-Fehler auftrat
* Vorabüberprüfung zu `[appservice|webapp] create` hinzugefügt
* `[webapp|functionapp] traffic-routing` korrigiert, damit der richtige actionHostName-Wert verwendet wird
* Slotunterstützung zu `functionapp`-Befehlen hinzugefügt

### <a name="batch"></a>Batch
* AAD-Authentifizierungsregression korrigiert, die von übermäßiger Berichterstellung für Authentifizierung mit gemeinsam verwendetem Schlüssel verursacht wurde

### <a name="batchai"></a>Batch AI
* BatchAI-Befehle sind jetzt veraltet und ausgeblendet.

### <a name="botservice"></a>BotService
* Für Befehle, die Version 3 des SDK unterstützen, wurden die Warnmeldungen „Support eingestellt“/„Wartungsmodus“ hinzugefügt

### <a name="cosmosdb"></a>CosmosDB
* [VERALTET] Der Befehl `cosmosdb list-keys` wurde als veraltet gekennzeichnet.
* Befehl `cosmosdb keys list` hinzugefügt, er ersetzt `cosmosdb list-keys`.
* `cosmsodb create/update`: Neues Format für „--location“ hinzugefügt, um das Festlegen der Eigenschaft „isZoneRedundant“ zu ermöglichen Das alte Format wurde als veraltet gekennzeichnet.

### <a name="eventgrid"></a>EventGrid
* `eventgrid domain`-Befehle für CRUD-Vorgänge für Domänen hinzugefügt
* `eventgrid domain topic`-Befehle für CRUD-Vorgänge für Domänenthemen hinzugefügt
* Argument `--odata-query` zu `eventgrid [topic|event-subscription] list` zum Filtern der Ergebnisse mithilfe von OData-Syntax hinzugefügt
* `event-subscription create/update`: „servicebusqueue“ als neue Werte für den Parameter `--endpoint-type` hinzugefügt
* [BREAKING CHANGE] Unterstützung für `--included-event-types All` mit `eventgrid event-subscription [create|update]` entfernt

### <a name="hdinsight"></a>HDInsight
* Unterstützung für den Parameter `--ssh-public-key` im Befehl vom Typ `hdinsight create` hinzugefügt

### <a name="iot"></a>IoT
* Unterstützung für das erneute Generieren von Autorisierungsrichtlinienschlüsseln hinzugefügt
* SDK und Unterstützung für den Bereitstellungsdienst des DigitalTwin-Repositorys hinzugefügt

### <a name="network"></a>Netzwerk
* Zonenunterstützung für NAT Gateway hinzugefügt
* Befehl `network list-service-tags` hinzugefügt
* Problem mit `dns zone import` behoben, aufgrund dessen Benutzer keine A-Platzhaltereinträge importieren konnten
* Problem mit `watcher flow-log configure` behoben, aufgrund dessen die Flowprotokollierung in bestimmten Regionen nicht aktiviert werden konnte

### <a name="resource"></a>Resource
* Befehl `az rest` zum Ausführen von REST-Aufrufen hinzugefügt
* Fehler behoben, der bei Verwendung von `policy assignment list` mit `--scope` auf Ressourcengruppen- oder Abonnementebene auftrat

### <a name="servicebus"></a>ServiceBus
* Problem mit `servicebus topic create --max-size` behoben [Nr. 9319](https://github.com/azure/azure-cli/issues/9319)

### <a name="sql"></a>SQL
* `--location` wurde geändert und ist nun für `sql [server|mi] create` optional. Ohne Angabe wird der Ressourcengruppenstandort verwendet.
* Der Fehler, dass das Objekt „NoneType“ nicht wiederholbar ist, wurde für `sql db list-editions --available` behoben.

### <a name="sqlvm"></a>SQLVm
* [WICHTIGE ÄNDERUNG] `sql vm create` wurde geändert und erfordert nun den Parameter `--license-type`.
* Änderung, um beim Erstellen oder Aktualisieren einer SQL-VM das Festlegen der SQL-Image-SKU zu ermöglichen

### <a name="storage"></a>Storage
* Problem mit fehlendem Kontoschlüssel für `storage container generate-sas` behoben
* Problem mit `storage blob sync` unter Linux behoben

### <a name="vm"></a>VM
* [VORSCHAU] Befehle vom Typ `vm image template` zum Erstellen von VM-Images hinzugefügt

## <a name="june-4-2019"></a>4\. Juni 2019

Version 2.0.66

### <a name="core"></a>Core
* Fehler behoben, aufgrund dessen bei Befehlen ein Fehler auftrat, wenn `--output yaml` mit `--query` verwendet wurde

### <a name="acr"></a>ACR
* Befehlsgruppe „acr pack“ zum Erstellen von Aufgaben zur Schnellerstellung mit Buildpacks hinzugefügt

### <a name="acs"></a>ACS
* Zulassen der Aktivierung/Deaktivierung des AKS-Add-Ons für das Kube-Dashboard
* Ausgeben einer benutzerfreundlichen Nachricht, wenn das Abonnement nicht in der Whitelist zur Verwendung von Azure Red Hat OpenShift enthalten ist

### <a name="batch"></a>Batch
* Bessere Fehlerbehandlung, wenn der Benutzer nicht bei einem Konto angemeldet ist \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]

### <a name="iot"></a>IoT
* Unterstützung für manuelles Failover hinzugefügt

### <a name="network"></a>Netzwerk
* Befehle vom Typ `network application-gateway waf-policy` hinzugefügt, um benutzerdefinierte WAF-Regeln zu unterstützen
* Argumente `--waf-policy` und `--max-capacity` zu `network application-gateway [create|update]` hinzugefügt 

### <a name="resource"></a>Resource
* Verbesserte Fehlermeldungen aus `deployment create`, wenn TTY nicht verfügbar ist

### <a name="role"></a>Role
* Hilfetext aktualisiert

### <a name="compute"></a>Compute
* Unterstützung zu `vm create` für virtuelle Computer aus einem verwalteten Image mit Datenträger-LUNs hinzugefügt, die nicht bei 0 beginnen oder die Nummern überspringen

## <a name="may-21-2019"></a>21. Mai 2019

Version 2.0.65

### <a name="core"></a>Core
* Besseres Feedback für Authentifizierungsfehler hinzugefügt
* Problem behoben, aufgrund dessen die CLI Erweiterungen lädt, die nicht mit der Core-Version kompatibel waren
* Problem beim Starten behoben, wenn `clouds.config` beschädigt ist

### <a name="acr"></a>ACR
* Unterstützung für verwaltete Identitäten zu Aufgaben hinzugefügt

### <a name="acs"></a>ACS
* `openshift create`-Befehl bei der Verwendung mit dem AAD-Kundenclient korrigiert

### <a name="appservice"></a>AppService
* [VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet – wird in der nächsten Version entfernt
* `functionapp devops-pipeline` geändert, um das Buildprotokoll von Azure DevOps im ausführlichen Modus abzurufen
* [BREAKING CHANGE] Flag `--use_local_settings` aus dem Befehl `functionapp devops-pipeline` entfernt – kein Vorgang wurde ausgeführt
* `webapp up` geändert, sodass die JSON-Ausgabe zurückgegeben wird, wenn `--logs` nicht verwendet wird
* Unterstützung hinzugefügt zum Schreiben von Standardressourcen in die lokale Konfiguration für `webapp up`
* Unterstützung zu `webapp up` hinzugefügt für die erneute Bereitstellung einer App ohne Verwendung des `--location`-Arguments
* Problem behoben, bei dem für die ASP-Erstellung der Linux-SKU „Free“ der SKU-Wert „Free“ nicht funktioniert hat

### <a name="botservice"></a>BotService
* Geändert, sodass Groß-/Kleinschreibung für `--lang`-Parameter für Befehle zulässig ist
* Beschreibung für das Befehlsmodul aktualisiert

### <a name="consumption"></a>Nutzung
* Fehlende erforderliche Parameter bei der Ausführung von `consumption usage list --billing-period-name` hinzugefügt

### <a name="iot"></a>IoT
* Unterstützung für das Auflisten aller Schlüssel hinzugefügt

### <a name="network"></a>Netzwerk
* [BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* `--nat-gateway`-Argument zu `network vnet subnet [create|update]` für das Anfügen an ein NAT-Gateway hinzugefügt
* Problem mit `dns zone import` behoben, aufgrund dessen Eintragsnamen keinem Datensatztyp entsprochen haben

### <a name="rdbms"></a>RDBMS
* Postgres- und MySLQ-Unterstützung für die Georeplikation hinzugefügt

### <a name="rbac"></a>RBAC
* Unterstützung für den Verwaltungsgruppenumfang zu `role assignment` hinzugefügt

### <a name="storage"></a>Storage
* `storage blob sync`: Synchronisierungsbefehl für Speicherblob hinzugefügt

### <a name="compute"></a>Compute
* `--computer-name` zu `vm create` zum Festlegen des Computernamens eines virtuellen Computers hinzugefügt
* `--ssh-key-value` umbenannt in `--ssh-key-values` für `[vm|vmss] create`: Jetzt können mehrere öffentliche SSH-Schlüsselwerte oder -pfade akzeptiert werden.
  * __Hinweis__: Dies ist **kein** Breaking Change: `--ssh-key-value` wird korrekt analysiert, da nur eine Übereinstimmung mit `--ssh-key-values` besteht.
* `--type`-Argument von `ppg create` in optionales Argument geändert

## <a name="may-6-2019"></a>6\. Mai 2019

Version 2.0.64

### <a name="acs"></a>ACS
* [BREAKING CHANGE] Flag `--fqdn` aus den `openshift`-Befehlen entfernt
* Geändert, sodass die allgemein verfügbare Azure Red Hat Openshift-API-Version verwendet wird
* Flag `customer-admin-group-id` wurde zu `openshift create` hinzugefügt.
* [ALLGEMEIN VERFÜGBAR] `(PREVIEW)` aus der `aks create`-Option `--network-policy` entfernt

### <a name="appservice"></a>AppService
* [VERALTET] Befehl `functionapp devops-build` als veraltet gekennzeichnet
  * Umbenannt in `functionapp devops-pipeline`
* Fehler beim Abrufen des richtigen Benutzernamens für Cloud Shell behoben, der einen Fehler von `webapp up` verursachte
* Dokumentation von `appservice plan --sku` mit den unterstützten App Service-Plänen aktualisiert
* Optionale Argumente für Ressourcengruppe und Plan zu `webapp up` hinzugefügt
* Unterstützung zur Berücksichtigung der Umgebungsvariablen `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` zu `webapp ssh` hinzugefügt
* Unterstützung für `appserviceplan create` für die kostenlose Linux-SKU hinzugefügt
* `webapp up` geändert, um nach dem Festlegen der App-Einstellung `SCM_DO_BUILD_DURING_DEPLOYMENT=true` zum Verarbeiten des Kudu-Kaltstarts für 30 Sekunden in den Energiesparmodus zu wechseln
* Unterstützung für die `powershell`-Runtime zu `functionapp create` unter Windows hinzugefügt
* Befehl `create-remote-connection` hinzugefügt

### <a name="batch"></a>Batch
* Fehler im Validierungssteuerelement für `--application-package-references`-Optionen korrigiert

### <a name="botservice"></a>Botservice
* [BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass standardmäßig eine leerer Web-App-Bot erstellt wird (d. h. kein Bot wird in App Service bereitgestellt)
* `--echo`-Flag zu `bot create` hinzugefügt, sodass das alte Verhalten mit `-v v4` verwendet wird
* [BREAKING CHANGE] Standardwert von `--version` in `v4` geändert
  * __HINWEIS:__ `bot prepare-publish` verwendet weiterhin den alten Standard.
* [BREAKING CHANGE]`--lang` geändert, sodass der Standard nicht mehr `Csharp` ist. Wenn der Befehl `--lang` erfordert und dies nicht angegeben ist, wird der Befehl nun mit Fehler beendet.
* [BREAKING CHANGE]`--appid`- und `--password`-Argumente für `bot create` in erforderlich geändert, sie können jetzt über `ad app create` erstellt werden.
* `--appid`- und `--password`-Validierung hinzugefügt
* [BREAKING CHANGE]`bot create -v v4` geändert, sodass kein Speicherkonto bzw. keine Application Insights-Instanz erstellt oder verwendet wird
* [BREAKING CHANGE]`bot create -v v3` geändert, sodass eine Region erforderlich ist, in der Application Insights verfügbar ist
* [BREAKING CHANGE]`bot update` geändert, sodass es sich jetzt nur auf spezifische Eigenschaften eines Bots auswirkt
* [BREAKING CHANGE]`--lang`-Flags geändert, sodass `Javascript` anstelle von `Node` akzeptiert wird
* [BREAKING CHANGE]`Node` als zulässiger `--lang`-Wert entfernt.
* [BREAKING CHANGE]`bot create -v v4 -k webapp` geändert, sodass `SCM_DO_BUILD_DURING_DEPLOYMENT` nicht mehr auf TRUE festgelegt ist. Alle Bereitstellungen über Kudu fungieren ihrem Standardverhalten entsprechend.
* `bot download` für Bots ohne `.bot`-Dateien geändert, sodass die sprachspezifische Konfigurationsdatei mit Werten aus den Anwendungseinstellungen für den Bot erstellt wird.
* Unterstützung für `Typescript` zu `bot prepare-deploy` hinzugefügt
* Warnmeldung zu `bot prepare-deploy` für `Javascript`- und `Typescript`-Bots hinzugefügt, wenn `package.json` in `--code-dir` nicht enthalten ist
* `bot prepare-deploy` geändert, sodass bei Erfolg `true` zurückgegeben wird
* Ausführliche Protokollierung zu `bot prepare-deploy` hinzugefügt
* Mehr verfügbare Application Insights-Regionen zu `az bot create -v v3` hinzugefügt

### <a name="configure"></a>Konfigurieren
* Unterstützung für die ordnerbasierte Argument-Standardwertkonfigurationen hinzugefügt

### <a name="eventhubs"></a>Event Hubs
* Befehle vom Typ `namespace network-rule` hinzugefügt
* `--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt

### <a name="network"></a>Netzwerk
* [BREAKING CHANGE]`--cache`-Argument mit `--defer` für `vnet [create|update]` ersetzt 

### <a name="policy-insights"></a>Policy Insights
* Unterstützung für `--expand PolicyEvaluationDetails` hinzugefügt, sodass Richtlinienauswertungsdetails von der Ressource abgefragt werden

### <a name="role"></a>Role
* [VERALTET]: Ausblenden des „--password"-Arguments von `create-for-rbac` geändert; Unterstützung wird im Mai 2019 entfernt

### <a name="service-bus"></a>Service Bus
* Befehle vom Typ `namespace network-rule` hinzugefügt
* `--default-action`-Argument für Netzwerkregeln zu `namespace [create|update]` hinzugefügt
* `topic [create|update]` korrigiert, sodass `--max-size`-Unterstützung für 10-, 20-, 40- und 80-GB-Werte mit Premium-SKU zulässig ist

### <a name="sql"></a>SQL
* Befehle vom Typ `sql virtual-cluster [list|show|delete]` hinzugefügt

### <a name="vm"></a>VM
* `--protect-from-scale-in` und `--protect-from-scale-set-actions` zu `vmss update` hinzugefügt, sodass Aktualisierungen der Schutzrichtlinie von VMSS-VM-Instanzen aktiviert sind
* `--instance-id` zu `vmss update` hinzugefügt, sodass allgemeine Aktualisierungen von VMSS-VM-Instanzen aktiviert sind
* `--instance-id` zu `vmss wait` hinzugefügt
* Neue `ppg`-Befehlsgruppe für die Verwaltung von Näherungsplatzierungsgruppen hinzugefügt
* `--ppg` zu `[vm|vmss] create` und `vm availability-set create` für die Verwaltung von PPGs hinzugefügt
* Parameter `--hyper-v-generation` zu `image create` hinzugefügt

## <a name="april-23-2019"></a>23. April 2019

Version 2.0.63

### <a name="acs"></a>ACS
* `aks get-credentials` zur Anzeige einer Eingabeaufforderung zum Überschreiben doppelter Werte geändert
* `(PREVIEW)` aus Dev Spaces-Befehlen „aks use-dev-spaces“ und „aks remove-dev-spaces“ entfernt

### <a name="ams"></a>AMS
* Fehler bei der Objekt- und Kontofilteraktualisierung behoben

### <a name="appservice"></a>AppService
* Unterstützung für die App Service-Umgebung (App Service Environment, ASE) und Zeitlimit zu `webapp ssh` hinzugefügt
* Unterstützung für die Einrichtung von CI/CD für eine Azure DevOps-Pipeline aus einem GitHub-Repository zu Funktions-Apps hinzugefügt
* `--github-pat`-Argument zu `functionapp devops-build create` hinzugefügt, um persönliche GitHub-Zugriffstoken zu akzeptieren
* `--github-repository`-Argument zu `functionapp devops-build create` hinzugefügt, um das GitHub-Repository mit dem Quellcode einer Funktions-App zu akzeptieren
* Problem behoben, aufgrund dessen bei `az webapp up --logs` ein Fehler auftrat und die .NET Core-Standardversion auf 2.1 aktualisiert wurde
* Unnötige Funktions-App-Einstellungen beim Erstellen einer Funktions-App mit Verbrauchsplan entfernt
* `webapp up` geändert, sodass die ASP-Standardzeichenfolge jetzt eine Zahl am Ende anfügt, um einen neuen ASP basierend auf SKU-Optionen zu erstellen
* `-b` als Option für `webapp up` hinzugefügt, um die App im Browser zu starten
* `webapp deployment source config zip` geändert, um die `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`-Umgebungsvariable zu behandeln

### <a name="deployment-manager"></a>Bereitstellungs-Manager
* [VORSCHAUVERSIPN] Erstellen und Verwalten von Artefakten, die Rollouts unterstützen

### <a name="lab"></a>Labor
* Fehler behoben, der zu einer vorzeitigen Beendigung führen würde

### <a name="network"></a>Netzwerk
* Automatische Delegierung des Namenservers im übergeordneten Element während der Erstellung der untergeordneten Zone zu `dns zone create` hinzugefügt

### <a name="resource"></a>Resource
* [VERALTET]: Argumente `--link-id`, `--target-id` und `--filter-string` von `resource link` als veraltet markiert
  * Verwenden Sie stattdessen die Argumente `--link`, `--target` und `--filter`.
* Problem behoben, aufgrund dessen `resource link [create|update]`-Befehle nicht verwendet werden konnten
* Problem behoben, aufgrund dessen das Löschen anhand einer Ressourcen-ID bei einem Fehler zu einem Absturz führen konnte

### <a name="sql"></a>SQL
* Unterstützung für benutzerdefinierte Zeitzonen auf verwalteten Instanzen hinzugefügt
* Geändert, um die Verwendung des Namens eines Pools für elastische Datenbanken mit `sql db update` zuzulassen
* Unterstützung für `--no-wait` zu `sql server [create|update]` hinzugefügt
* Befehl `sql server wait` hinzugefügt

### <a name="storage"></a>Storage
* Problem mit doppelt codierten SAS-Token in `storage blob generate-sas` behoben

### <a name="vm"></a>VM
* `--skip-shutdown`-Flag zum Ausschalten von VMs ohne Herunterfahren zu `vm|vmss stop` hinzugefügt
* `--storage-account-type`-Argument zum Festlegen des Kontotyps des Veröffentlichungsprofils zu `sig image-version create` hinzugefügt
* `--target-regions`-Argument zu `sig image-version create` hinzugefügt, um das Festlegen von regionsspezifischen Speicherkontotypen zuzulassen

## <a name="april-9-2019"></a>9\. April 2019

### <a name="core"></a>Core
* Problem behoben, aufgrund dessen einige Erweiterungen mit der Version `Unknown` angezeigt wurden und nicht aktualisiert werden konnten

### <a name="acr"></a>ACR
* Unterstützung für die kontextlose Ausführung eines Images hinzugefügt

### <a name="ams"></a>AMS
* [VERALTET]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* Unterstützung für neue Verschlüsselungsparameter in `ams streaming-policy create` hinzugefügt
* Neuer Parameter `--filters` zu `ams streaming-locator create` hinzugefügt

### <a name="appservice"></a>AppService
* Unterstützung für `--logs` zu `webapp up` hinzugefügt
* Probleme bei der Generierung von `azure-pipelines.yml` beim Befehl `functionapp devops-build create` behoben
* Fehlerbehandlung und Indikatoren für `unctionapp devops-build create` verbessert
* [BREAKING CHANGE] Flag `--local-git` für den Befehl `devops-build` entfernt; lokale Git-Erkennung und -Verarbeitung sind zum Erstellen von Azure DevOps-Pipelines obligatorisch
* Unterstützung für das Erstellen von Linux-Functions-Plänen hinzugefügt
* Möglichkeit zum Wechseln eines Plans unter einer Funktions-App mit `functionapp update --plan` hinzugefügt
* Unterstützung für Einstellungen zum Aufskalieren für den Azure Functions-Premium-Plan hinzugefügt

### <a name="cdn"></a>CDN
* Unterstützung hinzugefügt für `Microsoft_Standard` und `Standard_ChinaCdn`

### <a name="feedback"></a>Feedback
* `feedback` zur Anzeige von Metadaten zu den zuletzt ausgeführten Befehlen geändert
* `feedback` geändert, um den Benutzer zur Unterstützung beim Issueerstellungsprozess aufzufordern (durch Öffnen eines Browsers und Verwenden einer Issuevorlage)
* `feedback` geändert, um den Issuetext bei der Ausführung mit „--verbose“ auszugeben

### <a name="monitor"></a>Überwachen
* Problem behoben, aufgrund dessen „Count“ kein zulässiger Wert für `metrics alert [create|update]` war 

### <a name="network"></a>Netzwerk
* Problem behoben, aufgrund dessen das Tabellenformat mit `vnet-gateway list-bgp-peer-status` nicht angezeigt wurde
* Befehle `list-request-headers` und `list-response-headers` zu `application-gateway rewrite-rule` hinzugefügt
* Befehl `list-server-variables` zu `application-gateway rewrite-rule condition` hinzugefügt
* Problem behoben, aufgrund dessen durch das Aktualisieren des Linkstatus für einen ExpressRoute-Port eine Ausnahme vom Typ „unbekanntes Attribut“ ausgelöst wurde: `express-route port update`

### <a name="privatedns"></a>PrivateDNS
* `network private-dns` für private DNS-Zonen hinzugefügt

### <a name="resource"></a>Resource
* Problem mit `deployment create` und `group deployment create` behoben, aufgrund dessen eine Parameterdatei mit leerem Parametersatz nicht verwendet werden konnte

### <a name="role"></a>Role
* `create-for-rbac` korrigiert, um `--years` korrekt zu verarbeiten
* [BREAKING CHANGE]`role assignment delete` geändert, um eine Eingabeaufforderung anzuzeigen, wenn alle Zuweisungen im Abonnement ohne Bedingungen gelöscht werden

### <a name="sql"></a>SQL
* `sql mi [create|update]` mit den Eigenschaften „proxyOverride“ und „publicDataEndpointEnabled“ aktualisiert

### <a name="storage"></a>Storage
* [BREAKING CHANGE] Ergebnis von `storage blob delete` entfernt
* `--full-uri` zu `storage blob generate-sas` hinzugefügt, um den vollständigen URI für das Blob mit SAS zu erstellen
* `--file-snapshot` zu `storage file copy start` hinzugefügt, um die Datei aus der Momentaufnahme zu kopieren
* `storage blob copy cancel` geändert, um anstelle der Ausnahme für „NoPendingCopyOperation“ nur den Fehler anzuzeigen

## <a name="march-26-2019"></a>26. März 2019


### <a name="core"></a>Core
* Probleme mit der Inkompatibilität der Entwicklungserweiterung behoben
* Die Fehlerbehandlung verweist Kunden jetzt auf die Problemseite.

### <a name="cloud"></a>Cloud
* Fehler „Abonnement nicht gefunden“ in `cloud set` behoben

### <a name="acr"></a>ACR
* Redundante Quellen im Imageimport korrigiert
* `--auth-mode` wurde den Befehlen `acr build`, `acr run`, `acr task create` und `acr task update` hinzugefügt.
* Befehlsgruppe „acr task credential“ zum Verwalten von Anmeldeinformationen für eine Aufgabe hinzugefügt
* „--no-wait“ zum Befehl `acr build` hinzugefügt

### <a name="appservice"></a>AppService
* Problem behoben, das dazu führte, dass die Ausführung aus einem leeren Verzeichnis oder ein Szenario mit unbekannten Code von `webapp up` nicht korrekt behandelt wurde
* Problem behoben, aufgrund dessen Slots für `[webapp|functionapp] config ssl bind` nicht verwendet werden konnten

### <a name="bot-service"></a>Bot Service
* `bot prepare-deploy` hinzugefügt, um die Bereitstellung von Bots über `webapp` vorzubereiten
* `bot create --kind registration` geändert, um das Kennwort anzuzeigen, falls kein Kennwort angegeben wurde
* [BREAKING CHANGE]`--endpoint` wurde in `bot create --kind registration` geändert, sodass nun standardmäßig eine leere Zeichenfolge verwendet wird, anstatt eine Angabe zu erfordern.
* `SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt

### <a name="cdn"></a>CDN
* Unterstützung für `--no-wait` zu `cdn endpoint [create|update|start|stop|delete|load|purge]` hinzugefügt  
* [BREAKING CHANGE] Das standardmäßige Zwischenspeicherverhalten für Abfragezeichenfolgen von `cdn endpoint create` wurde geändert. Es wird nicht mehr standardmäßig „IgnoreQueryString“ festgelegt. Er wird jetzt vom Dienst festgelegt.

### <a name="cosmosdb"></a>Cosmosdb
* Unterstützung für `--enable-multiple-write-locations` bei Kontoaktualisierung hinzugefügt
* Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt

### <a name="interactive"></a>Interactive
* Inkompatibilität mit der über azdev installierten interaktiven Erweiterung korrigiert

### <a name="monitor"></a>Überwachen
* Geändert, sodass der Dimensionswert `*` für `monitor metrics alert [create|update]` zulässig ist

### <a name="network"></a>Netzwerk
* Befehlsgruppe `rewrite-rule` zu `application-gateway` hinzugefügt

### <a name="profile"></a>Profil
* Kontounterstützung auf Mandantenebene für verwaltete Dienstidentität zu `login` hinzugefügt

### <a name="postgres"></a>Postgres 
* postgresql-Befehle vom Typ `replica` und Befehl `restart server` hinzugefügt
* Änderungen vorgenommen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen

### <a name="resource"></a>Resource
* Verbesserte Tabellenausgabe für `deployment [create|list|show]`
* Problem mit `deployment [create|validate]` behoben, aufgrund dessen der Typ „secureObject“ nicht erkannt wurde

### <a name="graph"></a>Graph
* Unterstützung für `--end-date` zu `ad [app|sp] credential reset` hinzugefügt
* Unterstützung für das Hinzufügen von Berechtigungen mit `ad app permission add` hinzugefügt
* Fehler mit `ad app permission list` behoben, wenn keine Berechtigungen vorlagen
* Änderung an `ad sp delete` vorgenommen, um das Entfernen einer Rollenzuweisung zu überspringen, wenn das aktuelle Konto kein Abonnement enthält
* `ad app create` geändert, sodass ohne Angabe für `--identifier-uris` standardmäßig eine leere Liste verwendet wird

### <a name="storage"></a>storage
* `--snapshot` zu `storage file download-batch` für den Download von einer Freigabemomentaufnahme hinzugefügt
* Statusanzeige für `storage blob [download-batch|upload-batch]` geändert, damit sie weniger ausführlich dargestellt wird und das aktuelle Blob angibt
* Problem mit `storage account update` behoben, das beim Aktualisieren von Verschlüsselungsparametern auftrat
* Problem behoben, bei dem für `storage blob show` ein Fehler auftrat, wenn oauth (`--auth-mode=login`) verwendet wurde

### <a name="vm"></a>VM
* Befehl `image update` hinzugefügt

## <a name="march-12-2019"></a>12. März 2019

Version 2.0.60

### <a name="core"></a>Core

* Falsche Fehlermeldung in `cloud set` zu nicht gefundenem Abonnement korrigiert

### <a name="acr"></a>ACR

* Redundante Quellen im Imageimport korrigiert

### <a name="acs"></a>ACS

* Änderung vorgenommen, um den Parameter `--listen-address` für `aks browse` zu ignorieren, wenn er nicht von kubectl unterstützt wird 

### <a name="appservice"></a>AppService

* `[webapp|functionapp] deployment list-publishing-credentials` hinzugefügt, um die Kudu-Veröffentlichungs-URL und die entsprechenden Anmeldeinformationen abzurufen
* Fehlerhafte Ausgabeanweisung für `webapp auth update` entfernt
* `functionapp` korrigiert, um das korrekte Image für die Runtime in App Service-Plänen unter Linux festzulegen
* Vorschau-Tag für `webapp up` entfernt und Verbesserungen am Befehl implementiert

### <a name="botservice"></a>Botservice

* `SCM_DO_BUILD_DURING_DEPLOYMENT` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt
* `Microsoft-BotFramework-AppId` und `Microsoft-BotFramework-AppPassword` zu den Anwendungseinstellungen der ARM-Vorlage für Web-App-Bot (v4) hinzugefügt
* Einfache Anführungszeichen aus der Befehlsausgabe von `bot publish` am Ende von `bot create` entfernt
* `bot publish` wurde geändert und ist jetzt asynchron.

### <a name="container"></a>Container

* Argument `--no-wait` zu `container [start|restart]` hinzugefügt

### <a name="eventhub"></a>EventHub

* Flag `--skip-empty-archives` zu `eventhub create|update` hinzugefügt, um leere Archive in der Aufzeichnung zu unterstützen

### <a name="find"></a>Suchen

* Umfangreiches Funktionsupdate

### <a name="hdinsight"></a>HDInsight

* Parameter `--storage-account-managed-identity` zu `hdinsight create` hinzugefügt, um MSI in ADLS Gen2 zu unterstützen

### <a name="network"></a>Netzwerk

* Problem mit `vpn-connection update` behoben, aufgrund dessen die Aktualisierung einer VPN-Verbindung zwischen Gateways in verschiedenen Abonnements fehlschlug

### <a name="rdbms"></a>Rdbms

* Kleinere Korrekturen, um den Standardspeicherort aus der Ressourcengruppe abzurufen, wenn er für die Erstellung von Servern nicht angegeben wurde, und um eine Überprüfung für die Aufbewahrungstage hinzuzufügen

### <a name="role"></a>Role

* `role definition update` wurde korrigiert und nutzt nun die ID, um die Definition korrekt aufzulösen.
* `ad app credential reset` geändert, um die Annahme zu entfernen, dass der Dienstprinzipal der App stets vorhanden ist

### <a name="service-fabric"></a>Service Fabric

* Das Problem, dass `sf cluster list` nicht wiederholbar war, wurde behoben.

## <a name="february-26-2019"></a>26. Februar 2019

Version 2.0.59

### <a name="core"></a>Core

* Problem behoben, aufgrund dessen die Verwendung von `--subscription NAME` in einigen Instanzen eine Ausnahme ausgelöst hat

### <a name="acr"></a>ACR

* Parameter `--target` für die Befehle `acr build`, `acr task create` und `acr task update` hinzugefügt
* Verbesserte Fehlerbehandlung für Runtimebefehle, wenn keine Anmeldung bei Azure besteht

### <a name="acs"></a>ACS

* Option `--listen-address` zu `aks port-forward` hinzugefügt

### <a name="appservice"></a>AppService

* Befehl `functionapp devops-build` hinzugefügt

### <a name="batch"></a>Batch
* [BREAKING CHANGE] Befehl `batch pool upgrade os` entfernt
* [BREAKING CHANGE]`Pacakges`-Eigenschaft aus `Application`-Antworten entfernt
* Befehl `batch application package list` zum Auflisten von Paketen einer Anwendung hinzugefügt
* [BREAKING CHANGE]`--application-id` in allen `batch application`-Befehlen in `--application-name` geändert 
* Argument `--json-file` für Befehle zum Anfordern der unformatierten API-Antwort hinzugefügt
* Validierung aktualisiert, sodass das `https://`-Element automatisch in alle Endpunkte aufgenommen wird, wenn es fehlt

### <a name="cosmosdb"></a>CosmosDB

* Untergruppe `network-rule` mit Befehlen `add`, `remove` und `list` zum Verwalten von VNET-Regeln eines Cosmos DB-Kontos hinzugefügt

### <a name="kusto"></a>Kusto

* [BREAKING CHANGE] Typen `hot_cache_period` und `soft_delete_period` für Datenbank in Format der Zeitspanne nach ISO8601 geändert

### <a name="network"></a>Netzwerk

* Argument `--express-route-gateway-bypass` zu `vpn-connection [create|update]` hinzugefügt
* Befehlsgruppen aus `express-route`-Erweiterungen hinzugefügt
* Befehlsgruppen `express-route gateway` und `express-route port` hinzugefügt
* Argument `--legacy-mode` zu `express-route peering [create|update]` hinzugefügt 
* Argumente `--allow-classic-operations` und `--express-route-port` zu `express-route [create|update]` hinzugefügt
* Argument `--gateway-default-site` zu `vnet-gateway [create|update]` hinzugefügt
* Befehle vom Typ `ipsec-policy` zu `vnet-gateway` hinzugefügt

### <a name="resource"></a>Resource

* Problem mit `deployment create` behoben, aufgrund dessen beim Feld „Typ“ die Groß-/Kleinschreibung beachtet wurde
* Unterstützung für URI-basierte Parameterdatei zu `policy assignment create` hinzugefügt
* Unterstützung für URI-basierte Parameter und Definitionen zu `policy set-definition update` hinzugefügt
* Verarbeitung von Parametern und Regeln für `policy definition update` korrigiert
* Problem mit `resource show/update/delete/tag/invoke-action` behoben, aufgrund dessen bei abonnementübergreifenden IDs die Abonnement-ID nicht ordnungsgemäß berücksichtigt wurde

### <a name="role"></a>Role

* Unterstützung für App-Rollen zu `ad app [create|update]` hinzugefügt

### <a name="vm"></a>VM

* Problem mit `vm create where ` behoben, aufgrund dessen der beschleunigte Netzwerkbetrieb für Ubuntu 18.0 nicht standardmäßig aktiviert war

## <a name="february-12-2019"></a>12. Februar 2019

Version 2.0.58

### <a name="core"></a>Core

* `az --version` zeigt jetzt eine Benachrichtigung an, wenn Sie Pakete haben, für die ein Update verfügbar ist.
* Die Regression, dass `--ids` nicht mehr mit JSON-Ausgaben verwendet werden konnte, wurde behoben.

### <a name="acr"></a>ACR
* [BREAKING CHANGE] Die Befehlsgruppe `acr build-task` wurde entfernt.
* [BREAKING CHANGE] Die Optionen `--tag` und `--manifest` wurden aus `acr repository delete` entfernt.

### <a name="acs"></a>ACS
* Unterstützung für Namen ohne Berücksichtigung von Groß-/Kleinschreibung wurde zu `aks [enable-addons|disable-addons]` hinzugefügt.
* Unterstützung für Azure Active Directory-Aktualisierungsvorgang mithilfe von `aks update-credentials --reset-aad` wurde hinzugefügt.
* Die Information, dass `--output` für `aks get-credentials` ignoriert wird, wurde hinzugefügt.

### <a name="ams"></a>AMS
* Befehle vom Typ `ams streaming-endpoint [start | stop | create | update] wait` hinzugefügt
* Befehle vom Typ `ams live-event [create | start | stop | reset] wait` hinzugefügt

### <a name="appservice"></a>AppService
* Die Möglichkeit zum Erstellen und Konfigurieren von Funktionen mithilfe von ACR-Containern wurde hinzugefügt.
* Unterstützung für das Aktualisieren von Web-App-Konfigurationen über JSON wurde hinzugefügt.
* Die Hilfe für `appservice-plan-update` wurde verbessert.
* Unterstützung für App-Erkenntnisse beim Erstellen von Funktions-Apps wurde hinzugefügt.
* Probleme mit der Web-App SSH wurden behoben.

### <a name="botservice"></a>Botservice
* Die Benutzeroberfläche für `bot publish` wurde verbessert.
* Eine Warnung für Zeitlimit bei der Ausführung von `npm install` während `az bot publish` wurde hinzugefügt.
* Ungültiges char-Element wurde `.` aus `--name` in `az bot create` entfernt.
* Eine Änderung wurde vorgenommen, um die zufällige Zuordnung von Ressourcennamen beim Erstellen von Azure Storage-Instanzen, App Service-Plänen, Funktions-/Web-Apps und Application Insights-Instanzen zu verhindern.
* [VERALTET] Argument `--proj-name` zugunsten von `--proj-file-path` als veraltet markiert
* `az bot publish` wurde geändert, um abgerufene IIS-Bereitstellungsdateien vom Typ „Node.js“ zu entfernen, wenn sie nicht bereits vorhanden waren.
* Das `--keep-node-modules` Argument wurde zu `az bot publish` hinzugefügt, damit der Ordner `node_modules` in App Service nicht gelöscht wird.
* Das Schlüssel-Wert-Paar `"publishCommand"` wurde der Ausgabe von `az bot create` beim Erstellen einer Funktions-App oder eines Web-App-Bots hinzugefügt.
  * Der Wert von `"publishCommand"` ist ein `az bot publish`-Befehl, der bereits die erforderlichen Parameter zum Veröffentlichen des neu erstellten Bots enthält.
* `"WEBSITE_NODE_DEFAULT_VERSION"` in der ARM-Vorlage wurde so aktualisiert, dass v4-SDK-Bots 10.14.1 anstelle von 8.9.4 verwenden.

### <a name="key-vault"></a>Key Vault
* Ein Problem mit `keyvault secret backup` wurde behoben, aufgrund dessen einige Benutzer bei Verwendung von `--id` einen `unexpected_keyword`-Fehler erhielten.

### <a name="monitor"></a>Überwachen
* `monitor metrics alert [create|update]` wurde so geändert, dass der Dimensionswert `*` zulässig ist.

### <a name="network"></a>Netzwerk
* `dns zone export` wurde geändert, um sicherzustellen, dass es sich bei exportierten CNAMEs um FQDNs handelt.
* Parameter `--gateway-name` wurde zu `nic ip-config address-pool [add|remove]` hinzugefügt, um Back-End-Adresspools von Anwendungsgateways zu unterstützen.
* Argumente `--traffic-analytics` und `--workspace` wurden zu `network watcher flow-log configure` hinzugefügt, um Datenverkehrsanalysen über einen Log Analytics-Arbeitsbereich zu unterstützen.
* `--idle-timeout` und `--floating-ip` wurden zu `lb inbound-nat-pool [create|update]` hinzugefügt.

### <a name="policy-insights"></a>Policy Insights
* `policy remediation`-Befehle wurden hinzugefügt, um Korrekturfunktionen der Ressourcenrichtlinie zu unterstützen.

### <a name="rdbms"></a>RDBMS
* Hilfemeldung und Befehlsparameter wurden verbessert.

### <a name="redis"></a>Redis
* Befehle zum Verwalten von „firewall-rules“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.
* Befehle zum Verwalten von „server-link“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.
* Befehle zum Verwalten von „patch-schedule“ (erstellen, aktualisieren, löschen, anzeigen, auflisten) wurden hinzugefügt.
* Unterstützung für Verfügbarkeitszonen und TLS-Mindestversion wurden zu „redis create“ hinzugefügt.
* [BREAKING CHANGE] Befehle `redis update-settings` und `redis list-all` wurden entfernt.
* [BREAKING CHANGE] Parameter für `redis create`: „Mandanteneinstellungen“ werden im Format „Schlüssel[=Wert] nicht akzeptiert.
* [VERALTET] Warnmeldung zur Markierung des Befehls `redis import-method` als veraltet hinzugefügt

### <a name="role"></a>Role
* [BREAKING CHANGE] Befehl `az identity` wurde aus den `vm`-Befehlen hierher verschoben.

### <a name="sql-vm"></a>SQL-VM
* [VERALTET] Argument `--boostrap-acc-pwd` aufgrund eines Tippfehlers als veraltet markiert

### <a name="vm"></a>VM
* `vm list-skus` wurde so geändert, dass `--all` anstelle von `--all true` verwendet werden kann.
* `vmss run-command [invoke | list | show]` hinzugefügt
* Ein Fehler wurde behoben, aufgrund dessen bei der Ausführung von `vmss encryption enable` bisher ein Fehler auftrat.
* [BREAKING CHANGE] Die Befehle vom Typ `az identity` wurden zu `role`-Befehlen verschoben.

## <a name="january-31-2019"></a>31. Januar 2019

Version 2.0.57

### <a name="core"></a>Core

* Hotfix für [Problem 8399](https://github.com/Azure/azure-cli/issues/8399).

## <a name="january-28-2019"></a>28. Januar 2019

Version 2.0.56

### <a name="acr"></a>ACR
* Unterstützung für VNet/IP-Regeln wurde hinzugefügt.

### <a name="acs"></a>ACS
* Virtuelle Knoten (Vorschau) hinzugefügt
* Verwaltete OpenShift-Befehle wurden hinzugefügt.
* Unterstützung für den Dienstprinzipal-Updatevorgang mit `aks update-credentials -reset-service-principal` wurde hinzugefügt.

### <a name="ams"></a>AMS
* [BREAKING CHANGE]`ams asset get-streaming-locators` in `ams asset list-streaming-locators` umbenannt
* [BREAKING CHANGE]`ams streaming-locator get-content-keys` in `ams streaming-locator list-content-keys` umbenannt

### <a name="appservice"></a>AppService
* Unterstützung für App-Erkenntnisse in `functionapp create` wurde hinzugefügt.
* Unterstützung für die Erstellung von App Service-Plänen (einschließlich Elastic Premium) wurde zu Funktions-Apps hinzugefügt.
* Probleme bei einer App-Einstellung mit Elastic Premium-Plänen wurden behoben.

### <a name="container"></a>Container
* Befehl `container start` hinzugefügt
* Eine Änderung wurde vorgenommen, um bei der Containererstellung die Verwendung von Dezimalwerten für die CPU zuzulassen.

### <a name="eventgrid"></a>EventGrid
* Parameter `--deadletter-endpoint` zu `event-subscription [create|update]` hinzugefügt
* „storagequeue“ und „hybridconnection“ wurden als neue Werte für „event-subscription [create|update] --endpoint-type“ hinzugefügt.
* Parameter `--max-delivery-attempts` und `--event-ttl` wurden zu `event-subscription create` hinzugefügt, um die Wiederholungsrichtlinie für Ereignisse anzugeben.
* Eine Warnmeldung wurde zu `event-subscription [create|update]` hinzugefügt, wenn Webhook als Ziel für ein Ereignisabonnement verwendet wird.
* Parameter „source-resource-id“ wurde für alle Befehle im Zusammenhang mit Ereignisabonnements hinzugefügt, und alle anderen Parameter im Zusammenhang mit Quellressourcen wurden als veraltet markiert.

### <a name="hdinsight"></a>HDInsight
* [BREAKING CHANGE] Die Parameter `--virtual-network` und `--subnet-name` wurden aus `hdinsight [application] create` entfernt.
* [BREAKING CHANGE]`hdinsight create --storage-account` wurde so geändert, dass der Name oder die ID eines Speicherkontos anstellen von Blobendpunkten akzeptiert wird.
* Parameter `--vnet-name` und `--subnet-name` zu `hdinsight create` hinzugefügt
* Unterstützung für das Enterprise-Sicherheitspaket und Datenträgerverschlüsselung wurde zu `hdinsight create` hinzugefügt. 
* Befehl `hdinsight rotate-disk-encryption-key` hinzugefügt
* Befehl `hdinsight update` hinzugefügt

### <a name="iot"></a>IoT
* Codierungsformat wurde zu Befehl „routing-endpoint“ hinzugefügt.

### <a name="kusto"></a>Kusto
* Vorschauversion

### <a name="monitor"></a>Überwachen
* ID-Vergleich wurde so geändert, dass Groß-/Kleinschreibung nicht mehr beachtet wird.

### <a name="profile"></a>Profil
* Konto auf Mandantenebene für verwaltete Dienstidentität für `login` wird aktiviert.

### <a name="network"></a>Netzwerk
* Ein Problem mit `express-route update` wurde behoben, aufgrund dessen das Argument `--bandwidth` ignoriert wurde.
* Ein Problem mit `ddos-protection update` wurde behoben, aufgrund dessen das festgelegte Verständnis zu einer Stapelüberwachung führte.

### <a name="resource"></a>Resource
* Unterstützung für die URI-Parameterdatei wurde zu `group deployment create` hinzugefügt.
* Unterstützung für verwaltete Identitäten wurde zu `policy assignment [create|list|show]` hinzugefügt.

### <a name="sql-virtual-machine"></a>Virtueller SQL-Computer
* Vorschauversion

### <a name="storage"></a>Storage
* Eine Lösung wurde so geändert, dass nur Eigenschaften aktualisiert werden, die im selben Objekt geändert werden.
* Nr. 8021 wurde korrigiert, Binärdaten werden bei der Rückgabe in Base64 codiert.

### <a name="vm"></a>VM
* `vm encryption enable` wurde geändert, um den Schlüsseltresor für die Datenträgerverschlüsselung zu überprüfen und sicherzustellen, dass der Schlüsseltresor für die Schlüsselverschlüsselung vorhanden ist.
* Flag `--force` wurde zu `vm encryption enable` hinzugefügt.

## <a name="january-15-2019"></a>15. Januar 2019

Version 2.0.55

### <a name="acr"></a>ACR
* Wurde geändert, um den Push eines nicht vorhandenen Helm-Diagramms zu ermöglichen.
* Wurde geändert, um Laufzeitvorgänge ohne ARM-Anforderungen zu ermöglichen.
* [VERALTET] Parameter `--resource-group` in folgenden Befehlen als veraltet markiert:
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a>ACS
* Unterstützung für neue ACI-Regionen wurde hinzugefügt.

### <a name="appservice"></a>AppService
* Ein Problem beim Hochladen von Zertifikaten für in einer ASE gehostete Apps wurde behoben, aufgrund dessen die AS-RG und die App-RG nicht übereinstimmten.
* `webapp up` wurde geändert, sodass SKU P1V1 als Standard für Linux verwendet wird.
* `[webapp|functionapp] deployment source config-zip` wurde korrigiert, sodass beim Fehlschlagen einer Bereitstellung die richtige Fehlermeldung angezeigt wird. 
* Befehl `webapp ssh` hinzugefügt

### <a name="botservice"></a>Botservice
* Aktualisierungen des Bereitstellungsstatus wurden zu `bot create` hinzugefügt.

### <a name="configure"></a>Konfigurieren
* `none` wurde als konfigurierbares Ausgabeformat hinzugefügt.

### <a name="cosmosdb"></a>CosmosDB
* Unterstützung für das Erstellen einer Datenbank mit gemeinsam genutztem Durchsatz wurde hinzugefügt.

### <a name="hdinsight"></a>HDInsight
* Befehle zum Verwalten von Anwendungen wurden hinzugefügt.
* Befehle zum Verwalten von Skriptaktionen wurden hinzugefügt.
* Befehle zum Verwalten von der Operations Management Suite (OMS) wurden hinzugefügt.
* Unterstützung zum Auflisten der regionalen Nutzung wurde zu `hdinsight list-usage` hinzugefügt.
* [BREAKING CHANGE] Standardclustertyp wurde aus `hdinsight create` entfernt.

### <a name="network"></a>Netzwerk
* Argumente `--custom-headers` und `--status-code-ranges` zu `traffic-manager profile [create|update]` hinzugefügt
* Neue Routingtypen wurden hinzugefügt: Subnetz und MultiValue
* Argumente `--custom-headers` und `--subnets` zu `traffic-manager endpoint [create|update]` hinzugefügt  
* Eine Problem wurde behoben, aufgrund dessen die Angabe von `--vnets ""` für `ddos-protection update` einen Fehler verursacht hat.

### <a name="role"></a>Role
* [VERALTET] Argument `--password` als veraltet markiert für `create-for-rbac`. Verwenden Sie stattdessen sichere, von der CLI generierte Kennwörter.

### <a name="security"></a>Sicherheit
* Erstrelease

### <a name="storage"></a>Storage
* [BREAKING CHANGE] Die Standardanzahl von Ergebnissen wurde für `storage [blob|file|container|share] list` in 5.000 geändert. Verwenden Sie `--num-results *` für das ursprüngliche Verhalten, alle Ergebnisse zurückzugeben.
* Parameter `--marker` zu `storage [blob|file|container|share] list` hinzugefügt
* Ein Protokollmarker für die nächste Seite wurde zur STDERR für `storage [blob|file|container|share] list` hinzugefügt. 
* Der Befehl `storage blob service-properties update` mit Unterstützung für statische Websites wurde hinzugefügt.

### <a name="vm"></a>VM
* `vm [disk|unmanaged-disk]` und `vmss disk` wurden geändert, sodass sie konsistentere Parameter enthalten.
* Unterstützung für mandantenübergreifende Imageverweise wurden zu `[vm|vmss] create` hinzugefügt.
* Fehler bei Standardkonfiguration in `vm diagnostics get-default-config --windows-os` wurde behoben.
* Argument `--provision-after-extensions` wurde zu `vmss extension set` hinzugefügt, um zu definieren, welche Erweiterungen vor dem Festlegen der Erweiterung bereitgestellt werden müssen.
* Argument `--replica-count` wurde zu `sig image-version update` hinzugefügt, um die Standardanzahl für die Replikation festzulegen.
* Fehler bei `image create --source` wurde behoben, aufgrund dessen, der Quellbetriebssystem-Datenträger für einen virtuellen Computer mit dem gleichen Namen gehalten wurde, selbst wenn die vollständige Ressourcen-ID angegeben war.

## <a name="december-20-2018"></a>20. Dezember 2018

Version 2.0.54
### <a name="appservice"></a>AppService
* Problem behoben, bei dem `webapp up` nicht erneut bereitgestellt werden konnte
* Unterstützung für das Auflisten und Wiederherstellen von Web-App-Momentaufnahmen hinzugefügt
* Unterstützung für das Flag `--runtime` zu Windows-Funktions-Apps hinzugefügt

### <a name="iotcentral"></a>IoTCentral
* Fehler bei API-Aufruf für update-Befehl behoben

### <a name="role"></a>Role
* [BREAKING CHANGE]`ad [app|sp] list` geändert, damit standardmäßig nur die ersten 100 Objekte aufgelistet werden

### <a name="sql"></a>SQL
* Unterstützung für die benutzerdefinierte Sortierung auf verwalteten Instanzen hinzugefügt

### <a name="vm"></a>VM
* Parameter `---os-type` zu `disk create` hinzugefügt

## <a name="december-18-2018"></a>18. Dezember 2018

Version 2.0.53
### <a name="acr"></a>ACR
* Unterstützung für Imageimport aus externen Containerregistrierungen hinzugefügt
* Tabellenlayout für Aufgabenliste komprimiert
* Unterstützung für Azure DevOps-URLs hinzugefügt

### <a name="acs"></a>ACS
* Virtuelle Knoten (Vorschau) hinzugefügt
* „(PREVIEW)“ aus AAD-Argumenten für `aks create` entfernt
* [VERALTET]`az acs`-Befehle als veraltet markiert. ACS wird am 31. Januar 2020 eingestellt
* Unterstützung für Netzwerkrichtlinie bei der Erstellung neuer AKS-Cluster hinzugefügt
* Anforderung des Arguments `--nodepool-name` bei nur einem Knotenpool für `aks scale` entfernt

### <a name="appservice"></a>AppService
* Problem behoben, bei dem für `webapp config container` der Parameter `--slot` nicht berücksichtigt wurde

### <a name="botservice"></a>Botservice
* Unterstützung für Analyse von `.bot`-Dateien beim Aufrufen von `bot show` hinzugefügt
* Fehler bei der AppInsights-Bereitstellung behoben
* Leerzeichenfehler bei Dateipfaden behoben
* Kudu-Netzwerkaufrufe reduziert
* Allgemeine Verbesserungen bei Befehlen der Benutzeroberfläche durchgeführt

### <a name="consumption"></a>Nutzung
* Fehler für Budget-API zum Anzeigen von Benachrichtigungen behoben

### <a name="cosmosdb"></a>CosmosDB
* Unterstützung für die Aktualisierung des Kontos von „Singlemaster“ auf „Multimaster“ hinzugefügt

### <a name="maps"></a>Karten
* Unterstützung für SKU „S1“ für `maps account [create|update]` hinzugefügt

### <a name="network"></a>Netzwerk
* Unterstützung für `--format` und `--log-version` für `watcher flow-log configure` hinzugefügt
* Problem mit `dns zone update` behoben, bei dem die Verwendung von "" zum Löschen von Auflösungs- und Registrierungs-VNETs nicht funktionierte

### <a name="resource"></a>Resource
* Verarbeitung des Bereichsparameters für Verwaltungsgruppen in `policy assignment [create|list|delete|show|update]` behoben 
* Neuen Befehl `resource wait` hinzugefügt

### <a name="storage"></a>Storage
*  Möglichkeit zum Aktualisieren der Protokollschemaversion für Speicherdienste in `storage logging update` hinzugefügt

### <a name="vm"></a>VM
* Absturz in `vm identity remove` behoben, der aufgetreten ist, wenn der angegebenen VM keine verwalteten Dienstidentitäten zugewiesen waren

## <a name="december-4-2018"></a>4\. Dezember 2018

Version 2.0.52
### <a name="core"></a>Core
* Unterstützung für mandantenübergreifende Ressourcenbereitstellung für mehrinstanzenfähigen Dienstprinzipal hinzugefügt
* Behebung eines Fehlers, aufgrund dessen IDs, die von einem Befehl mit Ausgabe im TSV-Format weitergeleitet wurden, nicht ordnungsgemäß analysiert wurden

### <a name="appservice"></a>AppService
* [VORSCHAU] Befehl `webapp up` hinzugefügt, der Benutzer beim Erstellen und Bereitstellen von Inhalten in Apps unterstützt
* Behebung eines Fehlers in einer containerbasierten Windows-App, der aufgrund einer Back-End-Änderung auftrat

### <a name="network"></a>Netzwerk
* Argument `--exclusion` zu `application-gateway waf-config set` hinzugefügt, um WAF-Ausschlüsse zu unterstützen

### <a name="role"></a>Role
* Unterstützung für benutzerdefinierte Bezeichner für Kennwortanmeldeinformation hinzugefügt 

### <a name="vm"></a>VM
* [VERALTET] Parameter `vm extension [show|wait] --expand` als veraltet markiert
* Parameter `--force` zu `vm restart` hinzugefügt, um nicht reagierende virtuelle Computer erneut bereitzustellen
* `[vm|vmss] create --authentication-type` geändert, um „all“ zu akzeptieren und einen virtuellen Computer mit Kennwort- und SSH-Authentifizierung zu erstellen
* Parameter `image create --os-disk-caching` hinzugefügt, um die Zwischenspeicherung von Betriebssystemdatenträgern für ein Image festzulegen

## <a name="november-20-2018"></a>20. November 2018

Version 2.0.51
### <a name="core"></a>Core
* MSI-Anmeldung geändert, sodass der Abonnementname nicht in der Identität wiederverwendet wird

### <a name="acr"></a>ACR
* Kontexttoken zum Aufgabenschritt hinzugefügt
* Unterstützung für das Festlegen von Geheimnissen in „acr run“ zum Spiegeln der ACR-Aufgabe hinzugefügt
* Unterstützung für `--top` und `--orderby` für die Befehle `show-tags` und `show-manifests` verbessert

### <a name="appservice"></a>AppService
* Standardtimeout der ZIP-Bereitstellung für das Abrufen des Status auf fünf Minuten erhöht und Timeout-Eigenschaft zum Anpassen dieses Werts hinzugefügt
* Aktualisierung der standardmäßigen `node_version`. Während eines Austauschvorgangs mit zwei Phasen werden bei der Austauschaktion zum Zurücksetzen des Slots alle App-Einstellungen und Verbindungszeichenfolgen beibehalten.
* Clientseitige SKU-Überprüfung für die Erstellung eines Linux-App Service-Plans entfernt
* Behebung eines Fehlers beim Abrufen des ZipDeploy-Status

### <a name="iotcentral"></a>IotCentral
* Verfügbarkeitsprüfung für Unterdomänen beim Erstellen einer IoT Central-Anwendung hinzugefügt

### <a name="keyvault"></a>KeyVault
* Behebung eines Fehlers, aufgrund dessen Fehler mitunter ignoriert wurden

### <a name="network"></a>Netzwerk
* `root-cert`-Unterbefehle zum Behandeln von vertrauenswürdigen Stammzertifikaten zu `application-gateway` hinzugefügt
* Optionen `--min-capacity` und `--custom-error-pages` zu `application-gateway [create|update]` hinzugefügt:
* `--zones` zur Unterstützung von Verfügbarkeitszonen zu `application-gateway create` hinzugefügt 
* Argumente `--file-upload-limit`, `--max-request-body-size` und `--request-body-check` zu `application-gateway waf-config set` hinzugefügt

### <a name="rdbms"></a>Rdbms
* MariaDB-VNET-Befehle hinzugefügt

### <a name="rbac"></a>RBAC
* Problem beim Aktualisieren unveränderlicher Anmeldeinformationen in `ad app update` behoben
* Ausgabewarnungen zur Ankündigung bevorstehender Breaking Changes für `ad [app|sp] list` hinzugefügt 

### <a name="storage"></a>Storage
* Behandlung von Ausnahmefällen für Speicherkopierbefehle verbessert
* Problem behoben, aufgrund dessen `storage blob copy start-batch` bei identischen Ziel- und Quellkonten keine Anmeldeinformationen verwendete
* Fehler bei `storage [blob|file] url` behoben, aufgrund dessen `sas_token` nicht in die URL eingebunden wurde
* Breaking Change-Warnung zu `[blob|container] list` hinzugefügt: In Kürze werden standardmäßig nur die ersten 5.000 Ergebnisse ausgegeben.

### <a name="vm"></a>VM
* Unterstützung für die separate Angabe einer Speicherkonto-SKU für verwaltete Betriebssystemdatenträger und Datenträger zu `[vm|vmss] create --storage-sku` hinzugefügt
* Parameter für den Versionsnamen von `sig image-version` in `--image-version -e` geändert
* `sig image-version`-Argument `--image-version-name` als veraltet markiert und durch `--image-version` ersetzt
* Unterstützung für die Verwendung des lokalen Betriebssystemdatenträgers für `[vm|vmss] create --ephemeral-os-disk` hinzugefügt
* Unterstützung für `--no-wait` zu `snapshot create/update` hinzugefügt
* Befehl `snapshot wait` hinzugefügt
* Unterstützung für die Verwendung von Instanznamen mit `[vm|vmss] extension set --extension-instance-name` hinzugefügt

## <a name="november-6-2018"></a>6\. November 2018

Version 2.0.50

### <a name="core"></a>Core
* Unterstützung für die Dienstprinzipalauthentifizierung (SN und Aussteller) hinzugefügt

### <a name="acr"></a>ACR
* Unterstützung für Commit- und Pull Request-Git-Ereignisse für Aufgabenquellentrigger hinzugefügt
* Auf Verwendung des Standard-Dockerfiles umgestellt, falls im Erstellungsbefehl kein Dockerfile angegeben wurde

### <a name="acs"></a>ACS
* [BREAKING CHANGE]`enable_cloud_console_aks_browse` entfernt, um standardmäßig „az aks browse“ zu aktivieren

### <a name="advisor"></a>Advisor
* Allgemein verfügbares Release

### <a name="ams"></a>AMS
* Neue Befehlsgruppen hinzugefügt:
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* Neue Befehle hinzugefügt:
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* Unterstützung von Verschlüsselungsparametern für `ams streaming-policy create` hinzugefügt
* Für `ams transform output remove` kann jetzt der zu entfernende Ausgabeindex angegeben werden.
* Argumente `--correlation-data` und `--label` zur Befehlsgruppe `ams job` hinzugefügt
* Argumente `--storage-account` und `--container` zur Befehlsgruppe `ams asset` hinzugefügt
* Standardwerte für Ablaufzeit (aktueller Zeitpunkt + 23 Std.) und Berechtigungen (Lesen) im Befehl `ams asset get-sas-url` hinzugefügt 
* [BREAKING CHANGE] Befehl `ams streaming locator` durch `ams streaming-locator` ersetzt
* [BREAKING CHANGE] Argument `--content-keys` von `ams streaming locator` aktualisiert
* [BREAKING CHANGE]`--content-policy-name` im Befehl `ams streaming locator` in `--content-key-policy-name` umbenannt
* [BREAKING CHANGE] Befehl `ams streaming policy` durch `ams streaming-policy` ersetzt
* [BREAKING CHANGE] Das Argument `--preset-names` wurde in der Befehlsgruppe `--preset` durch `ams transform` ersetzt. Ab sofort kann nur noch eine einzelne Ausgabe/Voreinstellung festgelegt werden. (Wenn Sie weitere hinzufügen möchten, müssen Sie `ams transform output add` ausführen.) Darüber hinaus können Sie eine benutzerdefinierte Voreinstellung für den Standard-Encoder (StandardEncoderPreset) festlegen, indem Sie den Pfad an Ihr benutzerdefiniertes JSON-Objekt übergeben.
* [BREAKING CHANGE]`--output-asset-names ` wurde im Befehl `ams job start` in `--output-assets` umbenannt. Ab sofort wird eine durch Leerzeichen getrennte Ressourcenliste im Format „assetName=Bezeichnung“ akzeptiert. Ressourcen ohne Bezeichnung können wie folgt gesendet werden: „assetName=“.

### <a name="appservice"></a>AppService
* Fehler in `az webapp config backup update` behoben, der dazu führte, dass kein Sicherungszeitplan festgelegt werden konnte, wenn noch keiner festgelegt war

### <a name="configure"></a>Konfigurieren
* YAML zu Ausgabeformatoptionen hinzugefügt

### <a name="container"></a>Container
* Auf Anzeige der Identität umgestellt, wenn eine Containergruppe nach YAML exportiert wird

### <a name="eventhub"></a>EventHub
* Flag `--enable-kafka` hinzugefügt, um Kafka in `eventhub namespace [create|update]` zu unterstützen

### <a name="interactive"></a>Interactive
* Interactive installiert nun die Erweiterung `interactive`, um schnellere Updates und schnelleren Support zu ermöglichen

### <a name="monitor"></a>Überwachen
* Unterstützung für Metriknamen mit Schrägstrichen und Punkten zu `--condition` in `monitor metrics alert [create|update]` hinzugefügt

### <a name="network"></a>Netzwerk
* Befehlsnamen vom Typ `network interface-endpoint` zugunsten von `network private-endpoint` als veraltet markiert
* Problem behoben, das dazu führte, dass das Argument `--peer-circuit` in `express-route peering connection create` keine ID akzeptiert
* Problem behoben, das dazu führte, dass `--ip-tags` mit `public-ip create` nicht ordnungsgemäß funktioniert 

### <a name="profile"></a>Profil
* `--use-cert-sn-issuer` zu `az login` hinzugefügt, um Dienstprinzipalanmeldungen mit automatischem Zertifikatrollover zu ermöglichen

### <a name="rdbms"></a>RDBMS
* MySQL-Replikatbefehle hinzugefügt

### <a name="resource"></a>Resource
* Unterstützung für Verwaltungsgruppen und Abonnements zu Befehlen vom Typ `policy definition|set-definition` hinzugefügt

### <a name="role"></a>Role
* Unterstützung für die API-Berechtigungsverwaltung, den angemeldeten Benutzer und die Verwaltung von Anwendungskennwörtern und Zertifikatanmeldeinformationen hinzugefügt
* `ad sp create-for-rbac` geändert, um „displayName“ und Dienstprinzipalname besser unterscheiden zu können
* Unterstützung der Gewährung von Berechtigungen für AAD-Apps hinzugefügt

### <a name="storage"></a>Storage
* Möglichkeit hinzugefügt, allein mit SAS und Endpunkten (ohne Kontoname oder Schlüssel) eine Verbindung mit Speicherdiensten herzustellen, wie unter `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>` beschrieben

### <a name="vm"></a>VM
* Argument `storage-sku` zu `image create` hinzugefügt, um das Festlegen des standardmäßigen Speicherkontotyps für das Image zu ermöglichen
* Fehler für `vm resize` behoben, durch den die Option `--no-wait` einen Absturz des Befehls verursachte
* Tabellenausgabeformat für `vm encryption show` geändert, um den Status anzuzeigen
* `vm secret format` geändert, um JSON/JSONC-Ausgabe erforderlich zu machen. Der Benutzer wird gewarnt, und es wird standardmäßig die JSON-Ausgabe verwendet, wenn ein unzulässiges Ausgabeformat ausgewählt wird.
* Argumentüberprüfung für `vm create --image` verbessert

## <a name="october-23-2018"></a>23. Oktober 2018

Version 2.0.49

### <a name="core"></a>Core
* Problem mit `--ids` behoben, aufgrund dessen `--subscription` Vorrang vor dem Abonnement in `--ids` hatte
* Ausdrückliche Warnungen hinzugefügt, wenn Parameter durch die Verwendung von `--ids` ignoriert würden

### <a name="acr"></a>ACR
* Problem mit der ACR Build-Codierung in Python2 behoben

### <a name="cdn"></a>CDN
* [BREAKING CHANGE] Standardverhalten beim Zwischenspeichern der Abfragezeichenfolge von `cdn endpoint create` so geändert, dass der Standardwert nicht mehr „IgnoreQueryString“ ist. Er wird jetzt vom Dienst festgelegt.

### <a name="container"></a>Container
* `Private` als gültiger Typ für die Übergabe an „--ip-address“ hinzugefügt
* Geändert, sodass nur eine Subnetz-ID für das Einrichten eines virtuellen Netzwerks für die Containergruppe zulässig ist
* Geändert, sodass das Verwenden eines VNET-Namens oder einer Ressourcen-ID zulässig ist, um die Verwendung von VNETs aus verschiedenen Ressourcengruppen zu ermöglichen
* `--assign-identity` hinzugefügt, um einer Containergruppe eine MSI-Identität hinzuzufügen
* `--scope` hinzugefügt, um eine Rollenzuweisung für die vom System zugewiesene MSI-Identität zu erstellen
* Warnung hinzugefügt, wenn eine Containergruppe mit einem Image ohne Prozess mit langer Ausführungszeit erstellt wird
* Probleme mit der Tabellenausgabe für Befehle `list` und `show` behoben

### <a name="cosmosdb"></a>CosmosDB
* Unterstützung für `--enable-multiple-write-locations` zu `cosmosdb create` hinzugefügt

### <a name="interactive"></a>Interactive
* Geändert, um sicherzustellen, dass der Parameter für globales Abonnement in Parametern angezeigt wird

### <a name="iot-central"></a>IoT Central
* Optionen für Vorlagen und Anzeigenamen für die Erstellung von IoT Central-Anwendungen hinzugefügt
* [BREAKING CHANGE] Unterstützung für F1-SKU entfernt; stattdessen ist die S1-SKU zu verwenden.

### <a name="monitor"></a>Überwachen
* Änderungen an `monitor activity-log list`:
  * Unterstützung für das Auflisten aller Ereignisse auf Abonnementebene hinzugefügt
  * `--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt
  * Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen
  * `--namespace` als Alias für veraltete Option `--resource-provider` hinzugefügt
  * `--filters` als veraltet markiert, da vom Dienst ausschließlich Werte mit stark typisierten Optionen unterstützt werden
* Änderungen an `monitor metrics list`:
  * `--offset`-Parameter für das einfachere Erstellen von Zeitabfragen hinzugefügt
  * Validierung für `--start-time` und `--end-time` verbessert, um die Verwendung von mehr ISO8601-Formate und benutzerfreundlicheren datetime-Formaten zu ermöglichen
* Validierung für `--event-hub`- und `--event-hub-rule`-Argumente an `monitor diagnostic-settings create` verbessert

### <a name="network"></a>Netzwerk
* `--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic create` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen
* `--app-gateway-address-pools`- und `--gateway-name`-Argumente zu `nic ip-config create/update` hinzugefügt, um das Hinzufügen von Back-End-Adresspools für Anwendungsgateways zu einer NIC zu unterstützen

### <a name="servicebus"></a>ServiceBus
* Schreibgeschütztes `migration_state`-Element zu „MigrationConfigProperties“ hinzugefügt, um den aktuellen Status der Migration von Service Bus Standard- zu Premium-Namespace anzuzeigen

### <a name="sql"></a>SQL
* `sql failover-group create` und `sql failover-group update` korrigiert, damit die Verwendung einer Richtlinie für manuelles Failover möglich ist

### <a name="storage"></a>Storage
* Formatierung der `az storage cors list`-Ausgabe korrigiert, sodass alle Elemente den richtigen Dienstschlüssel anzeigen
* `--bypass-immutability-policy`-Parameter für das Löschen von durch Unveränderlichkeitsrichtlinien blockierten Containern hinzugefügt

### <a name="vm"></a>VM
* Datenträger-Zwischenspeicherungsmodus `None` für Lv/Lv2-Computerserine in `[vm|vmss] create` erzwungen
* Liste der unterstützten Größen für unterstützenden Netzwerkbeschleuniger für `vm create` aktualisiert
* Stark typisierte Argumente für UltraSSD-IOPS und MBit/s-Konfigurationen für `disk create` hinzugefügt

## <a name="october-16-2018"></a>16. Oktober 2018

Version 2.0.48

### <a name="vm"></a>VM
* SDK-Problem behoben, das ein Fehlschlagen der Homebrew-Installation verursacht hat

## <a name="october-9-2018"></a>9\. Oktober 2018

Version 2.0.47

### <a name="core"></a>Core
* Verbesserte Fehlerbehandlung für Fehler vom Typ „Ungültige Anforderung“

### <a name="acr"></a>ACR
* Unterstützung für ähnliches Tabellenformat wie Helm-Client hinzugefügt

### <a name="acs"></a>ACS
* `aks [create|scale] --nodepool-name` zum Konfigurieren des Knotenpoolnamens hinzugefügt, auf 12 Zeichen gekürzt, Standard: nodepool1 
* Korrektur, bei der auf „scp“ zurückgegriffen wird, wenn Parimiko nicht funktioniert
* `aks create` geändert, sodass `--aad-tenant-id` nicht mehr erforderlich ist
* Verbesserte Zusammenführung von Kubernetes-Anmeldeinformationen, wenn doppelte Einträge vorhanden sind

### <a name="container"></a>Container
* `functionapp create` geändert, sodass das Erstellen eines Linux-Nutzungsplans mit einer bestimmten Runtime unterstützt wird
* [VORSCHAUVERSION] Unterstützung für das Hosten von Web-Apps in Windows-Containern hinzugefügt

### <a name="event-hub"></a>Event Hub
* Befehl `eventhub update` korrigiert
* [BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen

### <a name="extensions"></a>Erweiterungen
* Problem beim Hinzufügen einer Erweiterung behoben, die bereits installiert ist

### <a name="hdinsight"></a>HDInsight
* Erste Veröffentlichung

### <a name="iot"></a>IoT
* Befehl zur Erweiterungsinstallation zu Banner bei der ersten Ausführung hinzugefügt

### <a name="keyvault"></a>KeyVault
* Geändert, sodass Key Vault-Speicherbefehle auf das aktuelle API-Profil beschränkt sind

### <a name="network"></a>Netzwerk
* `network dns zone create` korrigiert: Befehl ist auch erfolgreich, wenn der Benutzer einen Standardspeicherort konfiguriert hat. Siehe Nr. 6052
* `--remote-vnet-id` für `network vnet peering create` eingestellt
* `--remote-vnet` zum `network vnet peering create`-Element hinzugefügt, das einen Namen oder eine ID akzeptiert
* Unterstützung für mehrere Subnetzpräfixe zu `network vnet create` in `--subnet-prefixes` hinzugefügt
* Unterstützung für mehrere Subnetzpräfixe zu `network vnet subnet [create|update]` in `--address-prefixes` hinzugefügt
* Problem mit `network application-gateway create` behoben, das die Erstellung von Gateways mit der SKU `WAF_v2` oder `Standard_v2` verhindert hat
* `--service-endpoint-policy`-Argument für Benutzerfreundlichkeit zu `network vnet subnet update` hinzugefügt

### <a name="role"></a>Role
* Unterstützung für das Auflisten von Azure AD-App-Besitzern in `ad app owner` hinzugefügt
* Unterstützung für das Auflisten von Azure AD-Dienstprinzipalbesitzern in `ad sp owner` hinzugefügt
* Geändert, um sicherzustellen, dass die Erstellungs- und Aktualisierungsbefehle für die Rollendefinition Konfigurationen mit mehreren Berechtigungen akzeptieren
* `ad sp create-for-rbac` geändert, um sicherzustellen, dass der Homepage-URI immer „https“ ist

### <a name="service-bus"></a>Service Bus
* [BREAKING CHANGE]`list`-Befehle geändert, sodass Fehler von Typ „NotFound(404)“ für Ressourcen mit der typische Vorgehensweise behandelt werden, anstatt eine leere Liste anzuzeigen

### <a name="vm"></a>VM
* Leeres `accessSas`-Feld in `disk grant-access` korrigiert
* `vmss create` geändert, sodass ein ausreichend großer Front-End-Portbereich zur Verarbeitung von Überbereitstellung reserviert ist
* Aktualisierungsbefehle für `sig` korrigiert
* `--no-wait`-Unterstützung für die Verwaltung von Imageversionen in `sig` hinzugefügt
* `vm list-ip-addresses` geändert, sodass die Verfügbarkeitszone von öffentlichen IP-Adressen angezeigt wird
* `[vm|vmss] disk attach` geändert, sodass die Standard-LUN eines Datenträgers standardmäßig auf die erste verfügbare Stelle festgelegt wird

## <a name="september-21-2018"></a>21. September 2018

Version 2.0.46

### <a name="acr"></a>ACR
* ACR-Aufgabenbefehle hinzugefügt
* Befehl für die Schnellausführung hinzugefügt
* `build-task`-Befehlsgruppe als veraltet markiert
* `helm`-Befehlsgruppe hinzugefügt, um die Verwaltung von Helm-Diagrammen mit ACR zu unterstützen
* Unterstützung für idempotentes Erstellen für die verwaltete Registrierung hinzugefügt
* Formatfreies Flag für die Anzeige von Buildprotokollen hinzugefügt

### <a name="acs"></a>ACS
* Befehl `install-connector` zum Festlegen des AKS-Master-FQDN geändert
* Erstellen der Rollenzuweisung für „vnet-subnet-id“ (wenn kein Dienstprinzipal angegeben wurde) und „skip-role-assignment“ korrigiert

### <a name="appservice"></a>AppService

* Unterstützung für WebJobs-Vorgangsverwaltung hinzugefügt (kontinuierlich/ausgelöst)
* „az webapp config set“ unterstützt die Eigenschaft „--fts-state“; Unterstützung für „az functionapp config set/show“ hinzugefügt
* Unterstützung für Bring Your Own Storage für Web-Apps hinzugefügt
* Unterstützung für das Auflisten und Wiederherstellen gelöschter Web-Apps hinzugefügt

### <a name="batch"></a>Batch
* Hinzufügen von Aufgaben über `--json-file` geändert, um die AddTaskCollectionParameter-Syntax zu unterstützen
* Dokumentation akzeptierter `--json-file`-Formate aktualisiert
* `--max-tasks-per-node-option` zu `batch pool create` hinzugefügt
* Verhalten von `batch account` geändert, um das aktuell angemeldete Konto anzuzeigen, wenn keine Optionen angegeben wurden

### <a name="batch-ai"></a>Batch KI 
* Fehler bei der automatischen Speicherkontoerstellung im Befehl `batchai cluster create` behoben

### <a name="cognitive-services"></a>Cognitive Services
* Vervollständigung für die Argumente `--sku`, `--kind` und `--location` hinzugefügt
* Befehl `cognitiveservices account list-usage` hinzugefügt
* Befehl `cognitiveservices account list-kinds` hinzugefügt
* Befehl `cognitiveservices account list` hinzugefügt
* `cognitiveservices list` als veraltet markiert
* `--name` geändert (ist jetzt optional für `cognitiveservices account list-skus`)

### <a name="container"></a>Container
* Möglichkeit zum Neustarten und Beenden einer ausgeführten Containergruppe hinzugefügt
* `--network-profile` zum Übergeben eines Netzwerkprofils hinzugefügt
* `--subnet` und `--vnet_name` hinzugefügt, um das Erstellen von Containergruppen in einem VNET zu ermöglichen
* Tabellenausgabe geändert, sodass der Status der Containergruppe angezeigt wird

### <a name="datalake"></a>Data Lake
* Befehle für VNET-Regeln hinzugefügt

### <a name="interactive-shell"></a>Interaktive Shell
* Fehler in Windows behoben, durch den Befehle nicht ordnungsgemäß ausgeführt wurden
* Durch veraltete Objekte verursachtes Problem beim Laden von Befehlen im interaktiven Modus behoben

### <a name="iot"></a>IoT
* Routingunterstützung für IoT Hubs hinzugefügt

### <a name="key-vault"></a>Key Vault
* Key Vault-Schlüsselimport für RSA-Schlüssel korrigiert

### <a name="network"></a>Netzwerk
* Befehle vom Typ `network public-ip prefix` hinzugefügt, um Präfixe von öffentlichen IP-Adressen zu unterstützen
* Befehle vom Typ `network service-endpoint` hinzugefügt, um Dienstendpunktrichtlinien-Features zu unterstützen
* Befehle vom Typ `network lb outbound-rule` hinzugefügt, um die Erstellung von Ausgangsregeln für Load Balancer Standard zu unterstützen
* `--public-ip-prefix` zu `network lb frontend-ip create/update` hinzugefügt, um Front-End-IP-Konfigurationen mit Präfixen von öffentlichen IP-Adressen zu unterstützen
* `--enable-tcp-reset` zu `network lb rule/inbound-nat-rule/inbound-nat-pool create/update` hinzugefügt
* `--disable-outbound-snat` zu `network lb rule create/update` hinzugefügt
* Verwendung von `network watcher flow-log show/configure` mit klassischen NSGs ermöglicht
* Hinzufügen des `network watcher run-configuration-diagnostic`-Befehls
* Befehl `network watcher test-connectivity` korrigiert und Eigenschaften `--method`, `--valid-status-codes` und `--headers` hinzugefügt
* `network express-route create/update`: Flag `--allow-global-reach` hinzugefügt
* `network vnet subnet create/update`: Unterstützung für `--delegation` hinzugefügt
* Befehl `network vnet subnet list-available-delegations` hinzugefügt
* `network traffic-manager profile create/update`: Unterstützung für `--interval`, `--timeout` und `--max-failures` für die Überwachungskonfiguration hinzugefügt; Optionen `--monitor-path`, `--monitor-port` und `--monitor-protocol` zugunsten von `--path`, `--port` und `--protocol` als veraltet markiert
* `network lb frontend-ip create/update`: Logik für das Festlegen der Zuweisungsmethode für private IP-Adressen korrigiert. Bei Angabe einer privaten IP-Adresse ist die Zuweisung statisch. Wird keine private IP-Adresse (oder eine leere Zeichenfolge für die private IP-Adresse) angegeben, erfolgt eine dynamische Zuweisung.
* `dns record-set * create/update`: Unterstützung für `--target-resource` hinzugefügt
* Befehle vom Typ `network interface-endpoint` hinzugefügt, um Schnittstellenendpunkt-Objekte abzufragen
* `network profile show/list/delete` für die partielle Verwaltung von Netzwerkprofilen hinzugefügt
* Befehle vom Typ `network express-route peering connection` für die Verwaltung von Peeringverbindungen zwischen ExpressRoute-Instanzen hinzugefügt

### <a name="rdbms"></a>RDBMS
* Unterstützung für den MariaDB-Dienst hinzugefügt

### <a name="reservation"></a>Reservierung
* Cosmos DB im Enumerationstyp für reservierte Ressourcen hinzugefügt
* Namenseigenschaft im Patchmodell hinzugefügt

### <a name="manage-app"></a>App-Verwaltung
* Fehler in `managedapp create --kind MarketPlace` korrigiert, der zum Absturz der Instanzerstellung einer verwalteten Marketplace-App führte
* Befehle vom Typ `feature` geändert, um sie auf unterstützte Profile zu beschränken

### <a name="role"></a>Role
* Unterstützung für das Auflisten der Gruppenmitgliedschaften des Benutzers hinzugefügt

### <a name="signalr"></a>SignalR
* Erste Version

### <a name="storage"></a>Storage
* Parameter `--auth-mode login` für die Verwendung der Anmeldeinformationen des Benutzers für die Blob- und Warteschlangenautorisierung hinzugefügt
* `storage container immutability-policy/legal-hold` für die Verwaltung von unveränderlichem Speicher hinzugefügt

### <a name="vm"></a>VM
* Problem behoben, das dazu führte, dass die Datei mit dem privaten Schlüssel durch `vm create --generate-ssh-keys` überschrieben wird, wenn die Datei mit dem privaten Schlüssel fehlt (Nr. 4725, 6780)
* Unterstützung für den gemeinsamen Image-Katalog über `az sig` hinzugefügt

## <a name="august-28-2018"></a>28. August 2018

Version 2.0.45

### <a name="core"></a>Core

* Das Problem, aufgrund dessen eine leere Konfigurationsdatei geladen wurde, wurde behoben.
* Unterstützung für Profil `2018-03-01-hybrid` für Azure Stack hinzugefügt

### <a name="acr"></a>ACR

* Problemumgehung für Laufzeitvorgänge ohne ARM-Anforderungen hinzugefügt
* Änderung vorgenommen, um im Befehl `build` Versionskontrolldateien (etwa „.git“ und „.gitignore“) standardmäßig aus der TAR-Datei auszuschließen

### <a name="acs"></a>ACS

* `aks create` geändert, dass standardmäßig virtuelle Computer vom Typ `Standard_DS2_v2` erstellt werden
* `aks get-credentials` geändert, um nun neue APIs zum Abrufen der Clusteranmeldeinformationen aufzurufen

### <a name="appservice"></a>AppService

* Unterstützung für CORS in „functionapp“ und „webapp“ hinzugefügt
* ARM-Tagunterstützung in Erstellungsbefehlen hinzugefügt
* `[webapp|functionapp] identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden

### <a name="backup"></a>Backup

* `backup vault backup-properties show` geändert, um bei fehlender Ressource mit Code 3 zu beenden

### <a name="bot-service"></a>Botdienst

* Anfängliches Release der Botdienst-CLI

### <a name="cognitive-services"></a>Cognitive Services

* Neuer Parameter `--api-properties,` hinzugefügt, der zum Erstellen einiger Dienste erforderlich ist

### <a name="iot"></a>IoT

* Problem mit dem Zuweisen verknüpfter Hubs behoben

### <a name="monitor"></a>Überwachen

* `monitor metrics alert`-Befehle für Metrikwarnungen nahezu in Echtzeit hinzugefügt
* `monitor alert`-Befehle als veraltet markiert

### <a name="network"></a>Netzwerk

* `network application-gateway ssl-policy predefined show` geändert, um bei fehlender Ressource mit Code 3 zu beenden

### <a name="resource"></a>Resource

* `provider operation show` geändert, um bei fehlender Ressource mit Code 3 zu beenden

### <a name="storage"></a>Storage

* `storage share policy show` geändert, um bei fehlender Ressource mit Code 3 zu beenden

### <a name="vm"></a>VM

* `vm/vmss identity show` geändert, um bei fehlender Ressource mit Code 3 zu beenden 
* `--storage-caching` für `vm create` eingestellt

## <a name="auguest-14-2018"></a>14. August 2018

Version 2.0.44

### <a name="core"></a>Core

* Numerische Anzeige in `table`-Ausgabe korrigiert
* YAML-Ausgabeformat hinzugefügt

### <a name="telemetry"></a>Telemetrie

* Verbesserte Berichterstellung für Telemetriedaten

### <a name="acr"></a>ACR

* Befehle vom Typ `content-trust policy` hinzugefügt
* Problem behoben, aufgrund dessen `.dockerignore` nicht richtig verarbeitet wurde

### <a name="acs"></a>ACS

* `az acs/aks install-cli` für die Installation in `%USERPROFILE%\.azure-kubectl` unter Windows geändert
* `az aks install-connector` geändert, um zu ermitteln, ob der Cluster über RBAC verfügt, und um den ACI-Connector entsprechend zu konfigurieren
* Geändert in Rollenzuweisung zum Subnetz bei entsprechender Angabe
* Neue Option zum Überspringen der Rollenzuweisung für Subnetz hinzugefügt, wenn dieses angegeben ist                                 
* Geändert, um Rollenzuweisung zum Subnetz zu überspringen, wenn bereits eine Zuweisung vorhanden ist                

### <a name="appservice"></a>AppService

* Fehler behoben, der das Erstellen einer Funktions-App mithilfe von Speicherkonten in externen Ressourcengruppen verhinderte
* Absturz bei ZIP-Bereitstellung behoben

### <a name="batchai"></a>Batch AI

* Protokollierungsausgabe für die automatische Speicherkontoerstellung geändert, sodass nun „Ressourcen*gruppe*“ angegeben wird        

### <a name="container"></a>Container

* `--secure-environment-variables` zum Übergeben sicherer Umgebungsvariablen an einen Container hinzugefügt      

### <a name="iot"></a>IoT

* [BREAKING CHANGE] Veraltete Befehle entfernt, die in die IoT-Erweiterung verschoben wurden
* Elemente aktualisiert, um nicht die Domäne `azure-devices.net` anzunehmen

### <a name="iot-central"></a>Iot Central

* Erstes Release des IoT Central-Moduls

### <a name="keyvault"></a>KeyVault


* Befehle zum Verwalten von Speicherkonten und SAS-Definitionen hinzugefügt
* Befehle für Netzwerkregeln hinzugefügt                                                           
* Parameter `--id` zu Geheimnis-, Schlüssel- und Zertifikatvorgängen hinzugefügt
* Unterstützung für Version mit mehreren APIs zur Schlüsseltresorverwaltung hinzugefügt
* Unterstützung für Version mit mehreren APIs zur Schlüsseltresordatenebene hinzugefügt

### <a name="relay"></a>Relay

* Erste Veröffentlichung

### <a name="sql"></a>Sql

* Befehle vom Typ `sql failover-group` hinzugefügt

### <a name="storage"></a>Storage

* [BREAKING CHANGE]`storage account show-usage` geändert, um Parameter `--location` erforderlich zu machen. Auflistung nach Region
* Parameter `--resource-group` geändert, sodass er für `storage account`-Befehle optional ist
* Warnungen vom Typ „Fehler bei Vorbedingung“ für einzelne Fehler in Batch-Befehlen für eine aggregiert Nachricht entfernt
* `[blob|file] delete-batch`-Befehle geändert, sodass kein Array mit Null-Werten mehr ausgegeben wird
* `blob [download|upload|delete-batch]`-Befehle geändert, um SAS-Token aus Container-URL zu lesen

### <a name="vm"></a>VM

* Allgemeine Filter zu `vm list-skus` für höhere Benutzerfreundlichkeit hinzugefügt

## <a name="july-31-2018"></a>31. Juli 2018

Version 2.0.43

### <a name="acr"></a>ACR

* Flag `--with-secure-properties` zum Befehl `acr build-task show` hinzugefügt
* Befehl `acr build-task update-build` hinzugefügt

### <a name="acs"></a>ACS

* Änderung, um 0 (Erfolg) zurückzugeben, wenn `az aks browse` durch Drücken von [STRG+C] beendet wird

### <a name="batch"></a>Batch

* Korrektur eines Fehlers bei der Anzeige des AAD-Tokens in Cloud Shell

### <a name="container"></a>Container

* Voraussetzung von `--log-analytics-workspace-key` für Name oder ID im festgelegten Abonnement entfernt

### <a name="network"></a>Netzwerk

* DNS-Unterstützung zu „2017-03-09-profile“ für Azure Stack hinzugefügt 

### <a name="resource"></a>Resource

* `--rollback-on-error` zu `group deployment create` hinzugefügt, um bei einem Fehler eine als funktionierend bekannte Bereitstellung auszuführen
* Problem behoben, aufgrund dessen `--parameters {}` mit `group deployment create` zu einem Fehler führte

### <a name="role"></a>Role

* Unterstützung für das Stack-Profil „2017-03-09-profile“ hinzugefügt
* Problem behoben, aufgrund dessen das generische Update von Parametern auf `app update` nicht funktionierte

### <a name="search"></a>Suchen,

* Befehle für Azure Search-Dienst hinzugefügt

### <a name="service-bus"></a>Service Bus

* Migrationsbefehlsgruppe hinzugefügt, um einen Namespace von Service Bus Standard zu Premium zu migrieren
* Neue optionale Eigenschaften zu Service Bus-Warteschlange und -Abonnement hinzugefügt
  *  `--enable-batched-operations` und `--enable-dead-lettering-on-message-expiration` in `queue`
  *  `--dead-letter-on-filter-exceptions` in `subscriptions`

### <a name="storage"></a>Storage

* Unterstützung für den Download großer Dateien über eine einzelne Verbindung hinzugefügt
* `show`-Befehle konvertiert, bei denen im Falle einer fehlenden Ressource kein Fehler mit dem Exitcode 3 ausgelöst wurde

### <a name="vm"></a>VM

* Unterstützung zum Auflisten von Verfügbarkeitsgruppen nach Abonnement hinzugefügt
* Unterstützung für `StandardSSD_LRS` wurde hinzugefügt.
* Unterstützung für Anwendungssicherheitsgruppe beim Erstellen einer VM-Skalierungsgruppe hinzugefügt
* [BREAKING CHANGE]`[vm|vmss] create`, `[vm|vmss] identity assign` und `[vm|vmss] identity remove` wurden geändert, um vom Benutzer zugewiesene Identitäten im Wörterbuchformat auszugeben.

## <a name="july-18-2018"></a>18. Juli 2018

Version 2.0.42

### <a name="core"></a>Core

* Unterstützung für browserbasierte Anmeldung WSL-Bash-Fenster hinzugefügt
* `--force-string`-Flag für alle generischen Updatebefehle hinzugefügt
* [BREAKING CHANGE] Befehle vom Typ „show“ so geändert, dass die Fehlermeldung protokolliert wird und der Vorgang bei einer fehlenden Ressource mit dem Exitcode 3 fehlschlägt

### <a name="acr"></a>ACR

* [BREAKING CHANGE] „--no-push“ in Befehl „acr build“ in reines Flag geändert
* Befehle `show` und `update` unter Gruppe `acr repository` hinzugefügt
* `--detail`-Flag für `show-manifests` und `show-tags` hinzugefügt, um ausführlichere Informationen anzuzeigen
* Parameter `--image` zur Unterstützung des Abrufs von Builddetails oder Protokollen anhand eines Images hinzugefügt

### <a name="acs"></a>ACS

* `az aks create` so geändert, dass mit Fehler beendet wird, wenn `--max-pods` kleiner als 5 ist

### <a name="appservice"></a>AppService

* Unterstützung für PremiumV2-SKUs hinzugefügt

### <a name="batch"></a>Batch

* Korrektur eines Fehlers bei der Verwendung von Anmeldeinformationen im Cloud Shell-Modus
* JSON-Eingabe so geändert, dass Groß-/Kleinschreibung nicht beachtet wird

### <a name="batch-ai"></a>Batch KI

* Befehl `az batchai job exec` korrigiert

### <a name="container"></a>Container

* Anforderung von Benutzername und Kennwort für Nicht-DockerHub-Registrierungen entfernt
* Fehler beim Erstellen von Containergruppen aus YAML-Datei behoben

### <a name="network"></a>Netzwerk

* Unterstützung für `--no-wait` zu `network nic [create|update|delete]` hinzugefügt 
* `network nic wait` hinzugefügt
* `--ids`-Argument für `network vnet [subnet|peering] list` als veraltet markiert
* `--include-default`-Flag hinzugefügt, um Standardsicherheitsregeln in die Ausgabe von `network nsg rule list` aufzunehmen  

### <a name="resource"></a>Resource

* Unterstützung für `--no-wait` zu `group deployment delete` hinzugefügt
* Unterstützung für `--no-wait` zu `deployment delete` hinzugefügt
* Befehl `deployment wait` hinzugefügt
* Problem behoben, aufgrund dessen die `az deployment`-Befehle auf Abonnementebene fälschlicherweise für Profil „2017-03-09-profile“ angezeigt wurden

### <a name="sql"></a>SQL

* Fehler „Der angegebene Ressourcengruppenname ... entsprach nicht dem Namen in der URL“ beim Angeben des Namens des Pools für elastische Datenbanken für `sql db copy`-und `sql db replica create`-Befehle behoben
* Konfigurieren des Standard-SQL Servers durch Ausführen von `az configure --defaults sql-server=<name>` zulässig
* Tabellenformatierer für Befehle `sql server`, `sql server firewall-rule`, `sql list-usages` und `sql show-usage` hinzugefügt

### <a name="storage"></a>Storage

* `pageRanges`-Eigenschaft zu `storage blob show`-Ausgabe hinzugefügt, die für Seitenblobs ausgefüllt wird

### <a name="vm"></a>VM

* [BREAKING CHANGE]`vmss create` so geändert, dass `Standard_DS1_v2` als standardmäßige Instanzgröße verwendet wird
* Unterstützung für `--no-wait` zu `vm extension [set|delete]` und `vmss extension [set|delete]` hinzugefügt
* `vm extension wait` hinzugefügt

## <a name="july-3-2018"></a>3\. Juli 2018

Version 2.0.41

### <a name="aks"></a>AKS

* Überwachung geändert, sodass Abonnement-ID verwendet wird

## <a name="july-3-2018"></a>3\. Juli 2018

Version 2.0.40

### <a name="core"></a>Core

* Neuer Autorisierungscode-Flow für interaktive Anmeldung hinzugefügt

### <a name="acr"></a>ACR

* Abruf-Buildstatus hinzugefügt
* Unterstützung für Enumerationswerte ohne Berücksichtigung von Groß-/Kleinschreibung hinzugefügt
* Parameter `--top` und `--orderby` für `show-manifests` hinzugefügt

### <a name="acs"></a>ACS

* [BREAKING CHANGE] Standardmäßiges Aktivieren der rollenbasierten Zugriffssteuerung für Kubernetes
* Argument `--disable-rbac` hinzugefügt und `--enable-rbac` als veraltet festgelegt, da es nun der Standard ist
* Optionen für Befehl `aks browse` wurden aktualisiert. Unterstützung für `--listen-port` hinzugefügt
* Standardmäßiges Helm-Diagrammpaket für Befehl `aks install-connector` wurde aktualisiert. Verwenden von „virtual-kubelet-for-aks-latest.tgz“
* Befehle `aks enable-addons` und `aks disable-addons` zum Aktualisieren eines vorhandenen Clusters hinzugefügt

### <a name="appservice"></a>AppService

* Unterstützung für das Deaktivieren der Identität über `webapp identity remove` hinzugefügt
* `preview`-Tag für Identitätsfunktion entfernt

### <a name="backup"></a>Backup

* Moduldefinition aktualisiert

### <a name="batchai"></a>Batch AI

* Tabellenausgabe für Befehle `batchai cluster node list` und `batchai job node list` korrigiert

### <a name="cloud"></a>Cloud

* Serversuffix `acr login` zu Cloudkonfiguration hinzugefügt

### <a name="container"></a>Container

* `container create` zu Standard für Vorgang mit langer Ausführungsdauer geändert
* Log Analytics-Parameter `--log-analytics-workspace` und `--log-analytics-workspace-key` hinzugefügt
* Parameter `--protocol` zum Festlegen des zu verwendenden Netzwerkprotokolls hinzugefügt

### <a name="extension"></a>Durchwahl

* `extension list-available` geändert, sodass nur mit der CLI-Version kompatible Erweiterungen angezeigt werden

### <a name="network"></a>Netzwerk

* Problem behoben, aufgrund dessen bei Datensatztypen die Groß-/Kleinschreibung beachtet werden musste ([#6602](https://github.com/Azure/azure-cli/issues/6602))

### <a name="rdbms"></a>Rdbms

* Befehle vom Typ `[postgres|myql] server vnet-rule` hinzugefügt

### <a name="resource"></a>Resource

* Neue Vorgangsgruppe `deployment` hinzugefügt

### <a name="vm"></a>VM

* Unterstützung für das Entfernen der vom System zugewiesenen Identität hinzugefügt

## <a name="june-25-2018"></a>25. Juni 2018

Version 2.0.39

### <a name="cli"></a>Befehlszeilenschnittstelle (CLI)

* Dateieinschränkung in MSI-Installer aktualisiert, um Problem mit der Erweiterungsinstallation zu beheben

## <a name="june-19-2018"></a>19. Juni 2018

Version 2.0.38

### <a name="core"></a>Core

* Globale Unterstützung für `--subscription` zu den meisten Befehlen hinzugefügt

### <a name="acr"></a>ACR

* `azure-storage-blob` als Abhängigkeit hinzugefügt
* CPU-Standardkonfiguration für `acr build-task create` geändert, sodass zwei Kerne verwendet werden

### <a name="acs"></a>ACS

* Optionen des Befehls `aks use-dev-spaces` wurden aktualisiert. Unterstützung für `--update` hinzugefügt
* `aks get-credentials --admin` geändert, sodass der Benutzerkontext in `$HOME/.kube/config` ersetzt wird
* Schreibgeschützte `nodeResourceGroup`-Eigenschaft in verwalteten Clustern verfügbar gemacht
* Befehlsfehler `acs browse` korrigiert
* `--connector-name` für `aks install-connector`, `aks upgrade-connector` und `aks remove-connector` als optional festgelegt
* Neue Azure Container Instances-Regionen für `aks install-connector` hinzugefügt
* Normalisierter Speicherort im Helm-Versionsnamen und Knotenname zu `aks install-connector` hinzugefügt

### <a name="appservice"></a>AppService

* Unterstützung für neuere Versionen von „urllib“ hinzugefügt
* Unterstützung der Verwendung eines App Service-Plans aus externen Ressourcengruppen zu `functionapp create` hinzugefügt

### <a name="batch"></a>Batch

* `azure-batch-extensions`-Abhängigkeit entfernt

### <a name="batch-ai"></a>Batch KI

* Unterstützung für Arbeitsbereiche wurde hinzugefügt. Arbeitsbereiche ermöglichen das Zusammenfassen von Clustern, Dateiservern und Experimenten in Gruppen ohne Beschränkung der Anzahl von Ressourcen, die erstellt werden können.
* Unterstützung für Experimente wurde hinzugefügt. Experimente ermöglichen das Zusammenfassen von Aufträgen in Sammlungen ohne Beschränkung der Anzahl von erstellten Aufträgen.
* Unterstützung für das Konfigurieren von `/dev/shm` für Aufträge hinzugefügt, die in einem Docker-Container ausgeführt werden
* Die Befehle `batchai cluster node exec` und `batchai job node exec` wurden hinzugefügt. Diese Befehle ermöglichen die Ausführung aller Befehle direkt auf Knoten und bieten Funktionen zur Portweiterleitung.
* Unterstützung für `--ids` zu `batchai`-Befehlen hinzugefügt
* [BREAKING CHANGE] Alle Cluster und Dateiserver müssen unter Arbeitsbereichen erstellt werden.
* [BREAKING CHANGE] Aufträge müssen unter Experimenten erstellt werden.
* [BREAKING CHANGE]`--nfs-resource-group` wurde aus den Befehlen `cluster create` und `job create` entfernt. Geben Sie zum Bereitstellen eines NFS, das einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Dateiservers über die Option `--nfs` an.
* [BREAKING CHANGE]`--cluster-resource-group` wurde aus dem Befehl `job create` entfernt. Geben Sie zum Übermitteln eines Auftrags, der einem anderen Arbeitsbereich/einer anderen Ressourcengruppe angehört, die ARM-ID des Clusters über die Option `--cluster` an.
* [BREAKING CHANGE] Attribut `location` wurde aus Aufträgen, Clustern und Dateiservern entfernt. „Location“ ist jetzt ein Attribut eines Arbeitsbereichs.
* [BREAKING CHANGE]`--location` wurde aus den Befehlen `job create`, `cluster create` und `file-server create` entfernt.
* [BREAKING CHANGE] Namen von Kurzoptionen wurden geändert, um die Schnittstelle konsistenter zu machen:
  - [`--config`, `-c`] in [`--config-file`, `-f`] umbenannt
  - [`--cluster`, `-r`] in [`--cluster`, `-c`] umbenannt
  - [`--cluster`, `-n`] in [`--cluster`, `-c`] umbenannt
  - [`--job`, `-n`] in [`--job`, `-j`] umbenannt

### <a name="maps"></a>Karten

* [BREAKING CHANGE]`maps account create` wurde so geändert, dass Nutzungsbedingungen entweder durch interaktive Eingabeaufforderung oder `--accept-tos`-Flag akzeptiert werden müssen.

### <a name="network"></a>Netzwerk

* Unterstützung für `https` zu `network lb probe create` hinzugefügt [Nr. 6571](https://github.com/Azure/azure-cli/issues/6571)
* Problem behoben, aufgrund dessen die Groß-/Kleinschreibung von `--endpoint-status` berücksichtigt wurde. [#6502](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a>Reservations

* [BREAKING CHANGE] Erforderlicher Parameter `ReservedResourceType` zu `reservations catalog show` hinzugefügt
* Parameter `Location` zu `reservations catalog show` hinzugefügt
* [BREAKING CHANGE]`kind` aus `ReservationProperties` entfernt
* [BREAKING CHANGE]`capabilities` wurde in `Catalog` in `sku_properties` umbenannt
* [BREAKING CHANGE] Eigenschaften `size` und `tier` aus `Catalog` entfernt
* Parameter `InstanceFlexibility` zu `reservations reservation update` hinzugefügt

### <a name="role"></a>Role

* Fehlerbehandlung verbessert

### <a name="sql"></a>SQL

* Verwirrender Fehler behoben, der beim Ausführen von `az sql db list-editions` für einen Ort auftrat, der für Ihr Abonnement nicht verfügbar ist

### <a name="storage"></a>Storage

* Lesbarkeit der Tabellenausgabe für `storage blob download` verbessert

### <a name="vm"></a>VM

* Verbesserte Einschränkung der VM-Größenüberprüfung für Unterstützung von beschleunigten Netzwerken in `vm create`
* Warnung für `vmss create` hinzugefügt, dass die VM-Standardgröße von `Standard_D1_v2` auf `Standard_DS1_v2` umgestellt wird
* `--force-update` zu `[vm|vmss] extension set` hinzugefügt, um die Erweiterung auch dann zu aktualisieren, wenn die Konfiguration nicht geändert wurde

## <a name="june-13-2018"></a>13. Juni 2018

Version 2.0.37

### <a name="core"></a>Core

* Verbesserte interaktive Telemetrie

## <a name="june-13-2018"></a>13. Juni 2018

Version 2.0.36

### <a name="aks"></a>AKS

* Zusätzliche erweiterte Netzwerkoptionen zu `aks create` hinzugefügt
* Argumente zu `aks create` zum Aktivieren der Überwachung und HTTP-Routing hinzugefügt
* Argument `--no-ssh-key` zu `aks create` hinzugefügt
* Argument `--enable-rbac` zu `aks create` hinzugefügt
* [VORSCHAUVERSION] Unterstützung für Azure Active Directory-Authentifizierung zu `aks create` hinzugefügt

### <a name="appservice"></a>AppService

* Problem mit inkompatiblen urllib-Versionen behoben

## <a name="june-5-2018"></a>5\. Juni 2018

Version 2.0.35

### <a name="interactive"></a>Interactive

* Grenzwerte für die Abhängigkeiten des interaktiven Modus hinzugefügt

## <a name="june-5-2018"></a>5\. Juni 2018

Version 2.0.34

### <a name="core"></a>Core

* Unterstützung für mandantenübergreifende Ressourcenverweise hinzugefügt
* Verbesserte Zuverlässigkeit bei Telemetrieuploads

### <a name="acr"></a>ACR

* Unterstützung für VSTS als Remotequellort hinzugefügt
* Befehl `acr import` hinzugefügt

### <a name="aks"></a>AKS

* `aks get-credentials` wurde geändert, um die Kube-Konfigurationsdatei mit sichereren Dateisystemberechtigungen zu erstellen.

### <a name="batch"></a>Batch

* Fehler bei der Formatierung der Poollistentabelle behoben [[Problem 4378](https://github.com/Azure/azure-cli/issues/4378)]

### <a name="iot"></a>IoT

* Unterstützung für das Erstellen von IoT Hub-Instanzen im Tarif „Basic“ hinzugefügt

### <a name="network"></a>Netzwerk

* `network vnet peering` wurde verbessert.

### <a name="policy-insights"></a>Policy Insights

* Erstrelease

### <a name="arm"></a>ARM

* Befehle vom Typ `account management-group` hinzugefügt

### <a name="sql"></a>SQL

* Neue Befehle für verwaltete Instanzen hinzugefügt:
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* Neue Befehle für verwaltete Datenbanken hinzugefügt:
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a>Storage

* Zusätzliche MimeTypes für JSON und JavaScript hinzugefügt (abzuleiten aus Dateierweiterungen)

### <a name="vm"></a>VM

* `vm list-skus` wurde geändert, um feste Spalten zu verwenden und eine Warnung hinzuzufügen, dass `Tier` und `Size` entfernt werden.
* Option `--accelerated-networking` zu `vm create` hinzugefügt
* `--tags` zu `identity create` hinzugefügt

## <a name="may-22-2018"></a>22. Mai 2018

Version 2.0.33

### <a name="core"></a>Core

* Unterstützung für das Erweitern von `@` in Dateinamen hinzugefügt

### <a name="acs"></a>ACS

* Neue Dev Spaces-Befehle `aks use-dev-spaces` und `aks remove-dev-spaces` hinzugefügt
* Tippfehler in Hilfemeldung korrigiert

### <a name="appservice"></a>AppService

* Verbesserte generische Aktualisierungsbefehle
* Asynchrone Unterstützung für `webapp deployment source config-zip` hinzugefügt

### <a name="container"></a>Container

* Unterstützung für das Exportieren einer Containergruppe im YAML-Format hinzugefügt
* Unterstützung für die Verwendung einer YAML-Datei zum Erstellen/Aktualisieren einer Containergruppe hinzugefügt

### <a name="extension"></a>Durchwahl

* Verbesserte Entfernung von Erweiterungen

### <a name="interactive"></a>Interactive

* Protokollierung geändert, um Parser für Abschlüsse zu deaktivieren
* Verbesserte Verarbeitung beschädigter Hilfscaches

### <a name="keyvault"></a>KeyVault

* keyvault-Befehle wurden korrigiert, damit sie in Cloud Shell oder auf virtuellen Computern mit Identität verwendet werden können.

### <a name="network"></a>Netzwerk

* Problem behoben, aufgrund dessen `network watcher show-topology` nicht mit einem VNET und/oder Subnetznamen verwendet werden konnte ([#6326](https://github.com/Azure/azure-cli/issues/6326))
* Problem behoben, aufgrund dessen einige `network watcher`-Befehle fälschlicherweise angaben, dass Network Watcher nicht für bestimmte Regionen aktiviert ist ([#6264](https://github.com/Azure/azure-cli/issues/6264))

### <a name="sql"></a>SQL

* [BREAKING CHANGE] Von den Befehlen `db` und `dw` zurückgegebene Antwortobjekte geändert:
    * Eigenschaft `serviceLevelObjective` in `currentServiceObjectiveName` umbenannt
    * Eigenschaften `currentServiceObjectiveId` und `requestedServiceObjectiveId` entfernt
    * Eigenschaft `maxSizeBytes` geändert (ist nun keine Zeichenfolge mehr, sondern ein Ganzzahlwert)
* [BREAKING CHANGE] Die folgenden `db`- und `dw`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:
    * `requestedServiceObjectiveName`.  Verwenden Sie zum Aktualisieren den Parameter `--service-objective`, oder legen Sie die Eigenschaft `sku.name` fest.
    * `edition`. Verwenden Sie zum Aktualisieren den Parameter `--edition`, oder legen Sie die Eigenschaft `sku.tier` fest.
    * `elasticPoolName`. Verwenden Sie zum Aktualisieren den Parameter `--elastic-pool`, oder legen Sie die Eigenschaft `elasticPoolId` fest.
* [BREAKING CHANGE] Die folgenden `elastic-pool`-Eigenschaften wurden geändert und sind jetzt schreibgeschützt:
    * `edition`. Verwenden Sie zum Aktualisieren den Parameter `--edition`.
    * `dtu`. Verwenden Sie zum Aktualisieren den Parameter `--capacity`.
    *  `databaseDtuMin`. Verwenden Sie zum Aktualisieren den Parameter `--db-min-capacity`.
    *  `databaseDtuMax`. Verwenden Sie zum Aktualisieren den Parameter `--db-max-capacity`.
* Die Parameter `--family` und `--capacity` wurden zu den `db`-, `dw`- und `elastic-pool`-Befehlen hinzugefügt.
* Den `db`-, `dw`- und `elastic-pool`-Befehlen wurden Tabellenformatierer hinzugefügt.

### <a name="storage"></a>Storage

* Vervollständigung für das Argument `--account-name` hinzugefügt
* Problem mit `storage entity query` behoben

### <a name="vm"></a>VM

* [BREAKING CHANGE]`--write-accelerator` aus `vm create` entfernt. Die gleiche Unterstützung kann über `vm update` oder `vm disk attach` erzielt werden.
* Erweiterungsimageabgleich in `[vm|vmss] extension` korrigiert
* `--boot-diagnostics-storage` zu `vm create` zur Erfassung des Startprotokolls hinzugefügt
* `--license-type` zu `[vm|vmss] update` hinzugefügt

## <a name="may-7-2018"></a>7\. Mai 2018

Version 2.0.32

### <a name="core"></a>Core

* Ein Ausnahmefehler wurde behoben, der beim Abrufen von Geheimnissen aus einem Dienstprinzipalkonto mit Zertifikat auftrat.
* Eingeschränkte Unterstützung für positionelle Argumente hinzugefügt
* Problem behoben, aufgrund dessen `--query` nicht mit `--ids` verwendet werden konnte [#5591](https://github.com/Azure/azure-cli/issues/5591)
* Pipingszenarien von Befehlen bei Verwendung von `--ids` verbessert Unterstützt `-o tsv` mit angegebener Abfrage bzw. `-o json` ohne angegeben Abfrage
* Befehlsvorschläge bei Fehler hinzugefügt, wenn Befehle Tippfehler enthielten
* Fehler bei der Eingabe von `az ''` behandelt
* Unterstützung für benutzerdefinierte Ressourcentypen für Befehlsmodule und -erweiterungen hinzugefügt

### <a name="acr"></a>ACR

* ACR Build-Befehle hinzugefügt
* Fehlermeldungen vom Typ „Ressource nicht gefunden.“ verbessert
* Höhere Leistung bei der Ressourcenerstellung und optimierte Fehlerbehandlung
* ACR-Anmeldung bei nicht standardmäßigen Konsolen und WSL optimiert
* Fehlermeldungen zu Repositorybefehlen optimiert
* Tabellenspalten und -reihenfolge aktualisiert

### <a name="acs"></a>ACS

* Warnung hinzugefügt, dass `az aks` eine Vorschauversion des Diensts ist
* Berechtigungsproblem in `aks install-connector` behoben, wenn `--aci-resource-group` nicht angegeben wird

### <a name="ams"></a>AMS

* Erste Version: Verwalten von Azure Media Services-Ressourcen

### <a name="appservice"></a>AppService

* Ein Problem in `webapp delete` wurde behoben, das bei Angabe von `--slot` auftrat.
* `--runtime-version` aus `webapp auth update` entfernt
* Unterstützung für „min\_tls\_version“ und „https2.0“ hinzugefügt
* Unterstützung für mehrere Container hinzugefügt

### <a name="batch-ai"></a>Batch KI

* `batchai create cluster` wurde geändert, um die in der Konfigurationsdatei des Clusters konfigurierte VM-Priorität zu berücksichtigen.

### <a name="cognitive-services"></a>Cognitive Services

* Tippfehler im Beispiel für `cognitiveservices account create` behoben [Nr. 5603](https://github.com/Azure/azure-cli/issues/5603)

### <a name="consumption"></a>Nutzung

* Neue Befehle für Budget-API hinzugefügt

### <a name="container"></a>Container

* `--registry-server` muss nicht mehr für `container create` angegeben werden, wenn ein Registrierungsserver im Imagenamen enthalten ist.

### <a name="cosmos-db"></a>Cosmos DB

* VNET-Unterstützung für Azure CLI eingeführt: Cosmos DB

### <a name="dms"></a>DMS

* Erste Version: Die Migration von SQL zu Azure SQL wird nun unterstützt.

### <a name="extension"></a>Durchwahl

* Fehler behoben, aufgrund dessen Erweiterungsmetadaten nicht mehr angezeigt wurden

### <a name="interactive"></a>Interactive

* Interaktive Vervollständigung funktioniert nun auch mit positionellen Argumenten.
* Benutzerfreundlichere Ausgabe bei der Eingabe von '\'
* Abschlüsse für Parameter ohne Hilfe korrigiert
* Beschreibungen für Befehlsgruppen korrigiert

### <a name="lab"></a>Labor

* Regressionen aus Knack-Umwandlung korrigiert

### <a name="network"></a>Netzwerk

* [BREAKING CHANGE] Parameter `--ids` entfernt für:
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a>Profil

* Quellerkennung für `disk create` korrigiert
* [BREAKING CHANGE]`--msi-port` und `--identity-port` entfernt, da sie nicht mehr verwendet werden
* Tippfehler in kurzer Zusammenfassung für `account get-access-token` korrigiert

### <a name="redis"></a>Redis

* `redis patch-schedule patch-schedule show` wurde durch `redis patch-schedule show` ersetzt.
* `redis list-all` als veraltet markiert Diese Funktion wurde in `redis list` integriert.
* `redis import-method` wurde durch `redis import` ersetzt.
* Unterstützung für `--ids` zu verschiedenen Befehlen hinzugefügt

### <a name="role"></a>Role

* [BREAKING CHANGE] Veralteter Befehl `ad sp reset-credentials` entfernt

### <a name="storage"></a>Storage

* Zulassen, dass das Ziel-SAS-Token für die Blobkopie auf die Quelle angewendet wird, wenn Quell-SAS und Kontoschlüssel nicht angegeben werden
* Verfügbar gemacht: Socket-Timeout für Blobuploads und -downloads
* Blobnamen, die mit Pfadtrennzeichen beginnen, als relative Pfade behandeln
* Zulassen, dass `storage blob copy --source-sas` mit dem Abfragezeichen „?“ beginnt
* `storage entity query --marker` korrigiert, um Liste von Schlüsselwerten zu akzeptieren

### <a name="vm"></a>VM

* Ungültige Erkennungslogik für nicht verwalteten Blob-URI korrigiert
* Unterstützung für Datenträgerverschlüsselung ohne vom Benutzer bereitgestellte Dienstprinzipale hinzugefügt
* [BREAKING CHANGE] Verwenden Sie nicht „ManagedIdentityExtension“ des virtuellen Computers für MSI-Unterstützung.
* Unterstützung für Entfernungsrichtlinie zu `vmss` hinzugefügt
* [BREAKING CHANGE]`--ids` entfernt aus:
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* Unterstützung für Schreibbeschleunigung hinzugefügt
* `vmss perform-maintenance` hinzugefügt
* `vm diagnostics set` korrigiert, um zuverlässig den Betriebssystemtyp des virtuellen Computers zu erkennen
* `vm resize` geändert, um zu überprüfen, ob die angeforderte Größe von der derzeit festgelegten Größe abweicht, und nur bei einer Änderung eine Aktualisierung auszuführen


## <a name="april-10-2018"></a>10. April 2018

Version 2.0.31

### <a name="acr"></a>ACR

* Verbesserte Fehlerbehandlung für wincred-Fallback

### <a name="acs"></a>ACS

* Gültigkeit von per AKS erstellten SPNs in fünf Jahre geändert

### <a name="appservice"></a>AppService

* [BREAKING CHANGE]: Removed `assign-identity`
* Nicht abgefangene Ausnahme für nicht vorhandene Web-App-Pläne behoben

### <a name="batchai"></a>Batch AI

* Unterstützung für API 2018-03-01 hinzugefügt

  - Bereitstellung auf Auftragsebene
  - Umgebungsvariablen mit Geheimniswerten
  - Einstellungen von Leistungsindikatoren
  - Berichtstellung für auftragsspezifisches Pfadsegment
  - Unterstützung für Unterordner in Listendateien-API
  - Berichterstellung zur Nutzung und zu Grenzwerten
  - Zulassen der Angabe des Cachetyps für NFS-Server
  - Unterstützung für benutzerdefinierte Images
  - Unterstützung für pyTorch-Toolkit hinzugefügt

* Befehl `job wait` hinzugefügt, der das Warten auf die Auftragsfertigstellung ermöglicht und den Code für die Auftragsbeendigung meldet
* Befehl `usage show` hinzugefügt, mit dem die aktuelle Nutzung von Batch KI-Ressourcen und die Grenzwerte für verschiedene Regionen aufgelistet werden
* Nationale Clouds werden unterstützt
* Befehlszeilenargumente für Aufträge hinzugefügt, um das Bereitstellen von Dateisystemen auf Auftragsebene zusätzlich zu Konfigurationsdateien zu ermöglichen
* Weitere Optionen zum Anpassen von Clustern hinzugefügt – VM-Priorität, Subnetz, anfängliche Knotenanzahl für Cluster mit automatischer Skalierung, Angeben eines benutzerdefinierten Images
* Befehlszeilenoption zum Angeben des Cachetyps für NFS mit Verwaltung per Batch KI hinzugefügt
* Angeben der Bereitstellung von Dateisystemen in Konfigurationsdateien vereinfacht. Weglassen von Anmeldeinformationen für Azure-Dateifreigaben und Azure-Blobcontainer ist jetzt möglich. Die CLI füllt fehlende Anmeldeinformationen auf, indem der Speicherkontoschlüssel verwendet wird, der über Befehlszeilenparameter oder per Umgebungsvariable angegeben wird, oder der Schlüssel wird über Azure Storage abgefragt (sofern das Speicherkonto zum aktuellen Abonnement gehört).
* Der Befehl zum Streamen von Auftragsdateien wird jetzt automatisch abgeschlossen, nachdem der Auftrag beendet ist (Erfolg, Fehler, Beendigung oder Löschung)
* Verbesserte `table`-Ausgabe für `show`-Vorgänge
* Option `--use-auto-storage` für die Clustererstellung hinzugefügt. Diese Option erleichtert die Verwaltung von Speicherkonten und die Bereitstellung von Azure-Dateifreigaben und Azure-Blobcontainern in Clustern.
* `--generate-ssh-keys` für `cluster create` und `file-server create` hinzugefügt
* Möglichkeit zum Angeben der Knotensetupaufgabe über die Befehlszeile
* [BREAKING CHANGE] Befehl `job stream-file` und `job list-files` in die Gruppe `job file` verschoben
* [BREAKING CHANGE]`--admin-user-name` im Befehl `file-server create` in `--user-name` umbenannt, um Einheitlichkeit mit dem Befehl `cluster create` zu erzielen

### <a name="billing"></a>Abrechnung

* Registrierungskontobefehle hinzugefügt

### <a name="consumption"></a>Nutzung

* Befehle vom Typ `marketplace` hinzugefügt
* [BREAKING CHANGE]`reservations summaries` in `reservation summary` umbenannt
* [BREAKING CHANGE]`reservations details` in `reservation detail` umbenannt
* [BREAKING CHANGE] Kurzoptionen `--reservation-order-id` und `--reservation-id` für `reservation`-Befehle entfernt
* [BREAKING CHANGE]`--grain`-Kurzoptionen für `reservation summary`-Befehle entfernt
* [BREAKING CHANGE]`--include-meter-details`-Kurzoptionen für `pricesheet`-Befehle entfernt

### <a name="container"></a>Container

* Parameter für die Volumebereitstellung für das Git-Repository hinzugefügt: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` und `--gitrepo-mount-path`
* [#5926](https://github.com/Azure/azure-cli/issues/5926) behoben: Fehler bei `az container exec`, wenn „--container-name“ angegeben wurde

### <a name="extension"></a>Durchwahl

* Meldung für Distributionsüberprüfung in Debugebene geändert

### <a name="interactive"></a>Interactive

* Geändert: Verhinderung des Abschlusses bei nicht erkannten Befehlen
* Ereignishooks vor und nach der Erstellung der Teilstruktur von Befehlen hinzugefügt
* Abschluss für `--ids`-Parameter hinzugefügt

### <a name="network"></a>Netzwerk

* [#5936](https://github.com/Azure/azure-cli/issues/5936) behoben: `application-gateway create`-Tags konnten nicht festgelegt werden
* Argument `--auth-certs` zum Anfügen von Authentifizierungszertifikaten für `application-gateway http-settings [create|update]` hinzugefügt. [#4910](https://github.com/Azure/azure-cli/issues/4910)
* `ddos-protection`-Befehle zum Erstellen von DDoS-Schutzplänen hinzugefügt
* Unterstützung von `--ddos-protection-plan` für `vnet [create|update]` hinzugefügt, um das Zuordnen eines VNET zu einem DDoS-Schutzplan zu ermöglichen
* Problem mit `--disable-bgp-route-propagation`-Flag in `network route-table [create|update]` behoben
* Dummy-Argumente `--public-ip-address-type` und `--subnet-type` für `network lb [create|update]` entfernt
* Unterstützung für TXT-Datensätze mit RFC 1035-Escapesequenzen für `network dns zone [import|export]` und `network dns record-set txt add-record` hinzugefügt

### <a name="profile"></a>Profil

* Unterstützung für klassische Azure-Konten in `account list` hinzugefügt
* [BREAKING CHANGE]`--msi` & `--msi-port`-Argumente entfernt

### <a name="rdbms"></a>RDBMS

* Befehl `georestore` hinzugefügt
* Speichergrößenbeschränkung aus Befehl `create` entfernt

### <a name="resource"></a>Resource

* Unterstützung für `--metadata` zu `policy definition create` hinzugefügt
* Unterstützung von `--metadata`, `--set`, `--add`, `--remove` für `policy definition update` hinzugefügt

### <a name="sql"></a>SQL

* `sql elastic-pool op list` und `sql elastic-pool op cancel` hinzugefügt

### <a name="storage"></a>Storage

* Fehlermeldungen für falsch formatierte Verbindungszeichenfolgen verbessert

### <a name="vm"></a>VM

* Unterstützung für die Konfiguration der Plattform-Fehlerdomänenanzahl für `vmss create` hinzugefügt
* `vmss create` geändert, damit standardmäßig „Standard LB“ für zonales, großes oder per einzelner Platzierungsgruppe deaktiviertes Scale Set festgelegt wird
* [BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* Unterstützung für SKU mit öffentlicher IP für `vm create` hinzugefügt
* Argumente `--keyvault` und `--resource-group` für `vm secret format` hinzugefügt, um Szenarien zu unterstützen, bei denen der Befehl die Tresor-ID nicht auflösen kann. [#5718](https://github.com/Azure/azure-cli/issues/5718)
* Bessere Fehler für `[vm|vmss create]`, wenn der Standort einer Ressourcengruppe keine Zonenunterstützung aufweist


## <a name="march-27-2018"></a>27. März 2018

Version 2.0.30

### <a name="core"></a>Core

* Anzeigen einer Meldung für Erweiterungen, die in der Hilfe als Vorschauversion gekennzeichnet sind

### <a name="acs"></a>ACS

* Behebung eines Fehlers bei der SSL-Zertifikatprüfung für `aks install-cli` in Cloud Shell

### <a name="appservice"></a>AppService

* Unterstützung nur von HTTPS zu `webapp update` hinzugefügt
* Unterstützung für Slots zu `az webapp identity [assign|show]` und `az functionapp identity [assign|show]` hinzugefügt

### <a name="backup"></a>Backup

* Neuer Befehl `az backup protection isenabled-for-vm` hinzugefügt. Mit diesem Befehl kann überprüft werden, ob ein virtueller Computer von einem beliebigen Tresor im Abonnement gesichert wird.
* Azure-Objekt-IDs für Parameter `--resource-group` und `--vault-name` für die folgenden Befehle aktiviert:
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
* `--name`-Parameter wurden geändert, um das Ausgabeformat von `backup ... show`-Befehlen zu akzeptieren.

### <a name="container"></a>Container

* Befehl `container exec` hinzugefügt. Ausführung von Befehlen in einem Container für eine ausgeführte Containergruppe
* Zulassen der Tabellenausgabe zum Erstellen und Aktualisieren einer Containergruppe

### <a name="extension"></a>Durchwahl

* Meldung für `extension add` hinzugefügt, wenn sich die Erweiterung in der Vorschauphase befindet
* `extension list-available` geändert, um vollständige Erweiterungsdaten mit `--show-details` anzuzeigen
* [BREAKING CHANGE]`extension list-available` geändert, um standardmäßig vereinfachte Erweiterungsdaten anzuzeigen

### <a name="interactive"></a>Interactive

* Vervollständigungen wurden geändert und werden jetzt aktiviert, sobald das Laden der Befehlstabelle abgeschlossen ist.
* Fehler bei der Verwendung des Parameters `--style` behoben
* Interaktiver Lexer nach Befehlstabellensicherung instanziiert (sofern nicht vorhanden)
* Verbesserte Unterstützung der Vervollständigung

### <a name="lab"></a>Labor

* Probleme mit Befehl `create environment` behoben

### <a name="monitor"></a>Überwachen

* Unterstützung für `--top`, `--orderby` und `--namespace` zu `metrics list` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)
* [#4529](https://github.com/Azure/azure-cli/issues/5785) behoben: `metrics list` akzeptiert eine durch Leerzeichen getrennte Liste von abzurufenden Metriken
* Unterstützung für `--namespace` zu `metrics list-definitions` hinzugefügt [Nr. 5785](https://github.com/Azure/azure-cli/issues/5785)

### <a name="network"></a>Netzwerk

* Unterstützung für private DNS-Zonen hinzugefügt

### <a name="profile"></a>Profil

* Warnung für `--identity-port` und `--msi-port` zu `login` hinzugefügt

### <a name="rdbms"></a>RDBMS

* GA-API-Version 2017-12-01 (Geschäftsmodell) hinzugefügt

### <a name="resource"></a>Resource

* [BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a>Role

* Unterstützung für erforderliche Zugriffskonfigurationen und native Clients zu `az ad app create` hinzugefügt
* `rbac`-Befehle geändert, um maximal 1.000 IDs für Objektauflösung zurückzugeben
* Befehle zur Verwaltung von Anmeldeinformationen (`ad sp credential [reset|list|delete]`) hinzugefügt
* [BREAKING CHANGE] „properties“ aus `az role assignment [list|show]`-Ausgabe entfernt
* Unterstützung für `dataActions`- und `notDataActions`-Berechtigungen zu `role definition` hinzugefügt

### <a name="storage"></a>Storage

* Problem beim Hochladen von Dateien mit einer Größe von 195 GB bis 200 GB behoben
* [#4049](https://github.com/Azure/azure-cli/issues/4049) behoben: Probleme bei Uploads von Anfügeblobs behoben, die ein Ignorieren der Bedingungsparameter verursacht haben

### <a name="vm"></a>VM

* Warnung für anstehende BREAKING CHANGEen für Sätze mit mehr als 100 Instanzen zu `vmss create` hinzugefügt
* Unterstützung der Zonenresilienz zu `vm [snapshot|image]` hinzugefügt
* Datenträgerinstanzansicht geändert, um besseren Verschlüsselungsstatus zu melden
* [BREAKING CHANGE]`vm extension delete` geändert, um keine Ausgabe mehr zurückzugeben

## <a name="march-13-2018"></a>13. März 2018

Version 2.0.29

### <a name="acr"></a>ACR

* Unterstützung für den Parameter `--image` zu `repository delete` hinzugefügt
* Parameter `--manifest` und `--tag` des Befehls `repository delete` als veraltet markiert
* Befehl `repository untag` zum Entfernen eines Tags ohne das Löschen von Daten hinzugefügt

### <a name="acs"></a>ACS

* Befehl `aks upgrade-connector` zum Aktualisieren eines vorhandenen Connectors hinzugefügt
* `kubectl`-Konfigurationsdateien zur Verwendung von besser lesbarem YAML im Blockstil geändert

### <a name="advisor"></a>Advisor

* [BREAKING CHANGE]`advisor configuration get` in `advisor configuration list` umbenannt
* [BREAKING CHANGE]`advisor configuration set` in `advisor configuration update` umbenannt
* [BREAKING CHANGE]`advisor recommendation generate` entfernt
* Parameter `--refresh` zu `advisor recommendation list` hinzugefügt
* Befehl `advisor recommendation show` hinzugefügt

### <a name="appservice"></a>AppService

* `[webapp|functionapp] assign-identity` als veraltet markiert
* Befehle `webapp identity [assign|show]` und `functionapp identity [assign|show]` für verwaltete Identität hinzugefügt

### <a name="eventhubs"></a>Event Hubs

* Erste Veröffentlichung

### <a name="extension"></a>Durchwahl

* Überprüfung zum Warnen von Benutzern hinzugefügt, wenn sich die verwendete Distribution von der in der Paketquelldatei gespeicherten Distribution unterscheidet, da dies Fehlern führen kann

### <a name="interactive"></a>Interactive

* [#5625](https://github.com/Azure/azure-cli/issues/5625) behoben: Verlauf über verschiedene Sitzungen hinweg beibehalten
* [#3016](https://github.com/Azure/azure-cli/issues/3016) behoben: Verlauf nicht aufgezeichnet, obwohl er innerhalb des Bereichs liegt
* [#5688](https://github.com/Azure/azure-cli/issues/5688) behoben: Abschlüsse wurden nicht angezeigt, wenn beim Laden der Befehlstabelle eine Ausnahme aufgetreten ist
* Statusanzeige für lang ausgeführte Vorgänge korrigiert

### <a name="monitor"></a>Überwachen

* `monitor autoscale-settings`-Befehle als veraltet markiert
* Befehle vom Typ `monitor autoscale` hinzugefügt
* Befehle vom Typ `monitor autoscale profile` hinzugefügt
* Befehle vom Typ `monitor autoscale rule` hinzugefügt

### <a name="network"></a>Netzwerk

* [BREAKING CHANGE] Parameter `--tags` aus `route-filter rule create` entfernt
* Einige fehlerhafte Standardwerte für die folgenden Befehle entfernt:
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* `network watcher connection-monitor`-Befehle hinzugefügt
* Parameter `--vnet` und `--subnet` zu `network watcher show-topology` hinzugefügt

### <a name="profile"></a>Profil

* Parameter `--msi` für `az login` als veraltet markiert
* Parameter `--identity` für `az login` als Ersatz vor `--msi` hinzugefügt

### <a name="rdbms"></a>RDBMS

* [VORSCHAU] Geändert, sodass die API „2017-12-01-preview“ verwendet wird

### <a name="service-bus"></a>Service Bus

* Erste Veröffentlichung

### <a name="storage"></a>Storage

* [#4971](https://github.com/Azure/azure-cli/issues/4971) behoben: `storage blob copy` unterstützt jetzt andere Azure-Clouds.
* [#5286](https://github.com/Azure/azure-cli/issues/5286) behoben: Batchbefehle `storage blob [delete-batch|download-batch|upload-batch]` lösen bei Vorbedingungsfehlern keinen Fehler mehr aus

### <a name="vm"></a>VM

* `[vm|vmss] create` unterstützt jetzt das Anfügen nicht verwalteter Datenträger und das Konfigurieren der Zwischenspeicherung.
* `[vm|vmss] assign-identity` und `[vm|vmss] remove-identity` als veraltet markiert
* Befehle `vm identity [assign|remove|show]` und `vmss identity [assign|remove|show]` als Ersatz für veraltete Befehle hinzugefügt
* Standardpriorität in `vmss create` auf „Keine“ geändert

## <a name="february-27-2018"></a>27. Februar 2018

Version 2.0.28

### <a name="core"></a>Core

* [#5184](https://github.com/Azure/azure-cli/issues/5184) behoben: Problem beim Installieren von Homebrew
* Unterstützung für Erweiterungstelemetrie mit benutzerdefinierten Schlüsseln hinzugefügt
* HTTP-Protokollierung zu `--debug` hinzugefügt

### <a name="acs"></a>ACS

* Geändert, sodass für `aks install-connector` standardmäßig das Helm-Diagramm `virtual-kubelet-for-aks` verwendet wird
* Problem behoben: Unzureichende Berechtigungen für Dienstprinzipale zum Erstellen einer ACI-Containergruppe
* Parameter `--aci-container-group`, `--location` und `--image-tag` zu `aks install-connector` hinzugefügt
* Veraltungshinweis aus `aks get-versions` entfernt

### <a name="appservice"></a>AppService

* Updates für die neue SDK-Version (azure-mgmt-web 0.35.0)
* [5538](https://github.com/Azure/azure-cli/issues/5538) behoben: `Free` wurde als ungültige SKU gemeldet.

### <a name="cognitive-services"></a>Cognitive Services

* Hinweis beim Erstellen eines neuen Cognitive Services-Kontos aktualisiert

### <a name="consumption"></a>Nutzung

* Neue Befehle für PriceSheet-API hinzugefügt
* Vorhandene Formate für Nutzungsdetails und Reservierungsdetails aktualisiert

### <a name="container"></a>Container

* Argumente `--secrets` und `--secrets-mount-path` zu `container create` hinzugefügt, um Geheimnisse in ACI verwenden zu können

### <a name="network"></a>Netzwerk

* [#5559](https://github.com/Azure/azure-cli/issues/5559) behoben: Fehlender Client in `network vnet-gateway vpn-client generate`

### <a name="resource"></a>Resource

* `group deployment export` geändert, um eine partielle Vorlage und ggf. Fehler anzuzeigen, wenn der Vorgang nicht erfolgreich war

### <a name="role"></a>Role

* `role assignment list-changelogs` hinzugefügt, um die Überprüfung von Dienstprinzipalrollen zu ermöglichen

### <a name="sql"></a>SQL

* Zonenredundanzunterstützung für Datenbanken und Pools für elastische Datenbanken hinzugefügt (bei Erstellung und Aktualisierung)

### <a name="storage"></a>Storage

* Angabe von Zielpfad/Präfix für `storage blob [upload-batch|download-batch]` ermöglicht

### <a name="vm"></a>VM

* Unterstützung für das Anfügen/Trennen von Datenträgern für eine einzelne VMSS-Instanz hinzugefügt


## <a name="february-13-2018"></a>13. Februar 2018

Version 2.0.27

### <a name="core"></a>Core

* Authentifizierung für Abonnement-ID und Namen bei der MSI-Anmeldung in Authentifizierung mit Schlüssel geändert

### <a name="acs"></a>ACS

* [BREAKING CHANGE]`aks get-versions` aus Gründen der Genauigkeit in `aks get-upgrades` umbenannt
* `aks get-versions` zur Anzeige der verfügbaren Kubernetes-Versionen für `aks create` geändert
* Standardwerte von `aks create` in Auswahl der Kubernetes-Version durch den Server geändert
* Hilfemeldungen zu dem von AKS generierten Dienstprinzipal aktualisiert
* Standardknotengrößen für `aks create` von „Standard\_D1\_v2“ in „Standard\_DS1\_v2“ geändert
* Zuverlässigkeit der Suche nach dem Dashboardpod für `az aks browse` verbessert
* `aks get-credentials` korrigiert, um Unicode-Fehler beim Laden von Kubernetes-Konfigurationsdateien zu behandeln
* Meldung zu `az aks install-cli` hinzugefügt, um das Abrufen von `kubectl` in `$PATH` zu erleichtern

### <a name="appservice"></a>AppService

* Problem behoben, das zu einem Fehler von `webapp [backup|restore]` aufgrund eines Nullverweises führte
* Unterstützung für Standard-App Service-Pläne durch `az configure --defaults appserviceplan=my-asp` hinzugefügt

### <a name="cdn"></a>CDN

* Befehle vom Typ `cdn custom-domain [enable-https|disable-https]` hinzugefügt

### <a name="container"></a>Container

* Option `--follow` zu `az container logs` für Streamingprotokolle hinzugefügt
* Befehl `container attach` hinzugefügt, der die lokale Standardausgabe und Fehlerdatenströme an einen Container in einer Containergruppe angefügt

### <a name="cosmosdb"></a>CosmosDB

* Unterstützung für Einstellungsfunktionen hinzugefügt

### <a name="extension"></a>Durchwahl

* Unterstützung für den Parameter `--pip-proxy` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt
* Unterstützung für das Argument `--pip-extra-index-urls` zu Befehlen vom Typ `az extension [add|update]` hinzugefügt

### <a name="feedback"></a>Feedback

* Erweiterungsinformationen zu Telemetriedaten hinzugefügt

### <a name="interactive"></a>Interactive

* Problem behoben, aufgrund dessen der Benutzer bei Verwendung des interaktiven Modus in Cloud Shell zur Anmeldung aufgefordert wird
* Regression mit fehlenden Parametervervollständigungen korrigiert

### <a name="iot"></a>IoT

* Problem behoben, aufgrund dessen `iot dps access policy [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt
* Problem behoben, aufgrund dessen `iot dps linked-hub [create|update]` bei erfolgreicher Ausführung einen Fehler „nicht gefunden“ zurückgibt
* Unterstützung für `--no-wait` zu `iot dps access policy [create|update]` und `iot dps linked-hub [create|update]` hinzugefügt
* `iot hub create` geändert, um die Angabe der Anzahl von Partitionen zu ermöglichen

### <a name="monitor"></a>Überwachen

* Befehl `az monitor log-profiles create` korrigiert

### <a name="network"></a>Netzwerk

* Option `--tags` für folgende Befehle korrigiert:
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a>Profil

* `az login` im interaktiven Modus aktiviert

### <a name="resource"></a>Resource

* `feature show` wieder hinzugefügt

### <a name="role"></a>Role

* Argument `--available-to-other-tenants` zu `ad app update` hinzugefügt

### <a name="sql"></a>SQL

* Befehle vom Typ `sql server dns-alias` hinzugefügt
* `sql db rename` hinzugefügt
* Unterstützung für das Argument `--ids` für alle SQL-Befehle hinzugefügt

### <a name="storage"></a>Storage

* Befehle `storage blob service-properties delete-policy` und `storage blob undelete` hinzugefügt, um vorläufiges Löschen zu ermöglichen

### <a name="vm"></a>VM

* Absturz bei unvollständiger Initialisierung der VM-Verschlüsselung behoben
* Prinzipal-ID-Ausgabe beim Aktivieren von MSI hinzugefügt
* `vm boot-diagnostics get-boot-log` (feststehend)


## <a name="january-31-2018"></a>31. Januar 2018

Version 2.0.26

### <a name="core"></a>Core

* Unterstützung für das Abrufen von unformatierten Token im MSI-Kontext hinzugefügt
* Abrufindikator-Zeichenfolge nach Fertigstellung von LRO für die Windows-Datei „cmd.exe“ entfernt
* Warnung hinzugefügt, die angezeigt wird, wenn ein konfigurierter Standardwert in einen Eintrag auf INFO-Ebene geändert wurde. `--verbose` zum Anzeigen verwenden.
* Statusanzeige für Wait-Befehle hinzugefügt

### <a name="acs"></a>ACS

* Argument `--disable-browser` erläutert
* Vervollständigung mit der TAB-TASTE für Argumente vom Typ `--vm-size` verbessert

### <a name="appservice"></a>AppService

* `webapp log [tail|download]` (feststehend)
* Überprüfung `kind` für Web-Apps und Funktionen entfernt

### <a name="cdn"></a>CDN

* Problem mit fehlendem Client für `cdn custom-domain create` behoben

### <a name="cosmosdb"></a>CosmosDB

* Parameterbeschreibung für Failoverrichtlinien korrigiert

### <a name="interactive"></a>Interactive

* Problem behoben, aufgrund dessen Vervollständigungen von Befehlsoptionen nicht mehr angezeigt wurden

### <a name="network"></a>Netzwerk

* Schutz für `--cert-password` zu `application-gateway create` hinzugefügt
* Problem mit `application-gateway update` behoben, aufgrund dessen `--sku` fälschlicherweise einen Standardwert anwendete
* Schutz für `--shared-key` und `--authorization-key` zu `vpn-connection create` hinzugefügt
* Problem mit fehlendem Client für `asg create` behoben
* Parameter `--file-name / -f` für exportierte Namen zu `dns zone export` hinzugefügt
* Folgende Probleme mit `dns zone export` behoben:
  * Problem behoben, aufgrund dessen lange TXT-Einträge nicht korrekt exportiert wurden
  * Problem behoben, aufgrund dessen TXT-Einträge in Anführungszeichen fälschlich ohne Anführungszeichen in Escapezeichen exportiert wurden
* Problem behoben, aufgrund dessen bestimmte Datensätze zweimal mit `dns zone import` importiert wurden
* Befehle `vnet-gateway root-cert` und `vnet-gateway revoked-cert` wiederhergestellt

### <a name="profile"></a>Profil

* `get-access-token` zur Verwendung auf einer VM mit Identität korrigiert

### <a name="resource"></a>Resource

* Fehler mit `deployment [create|validate]` korrigiert, aufgrund dessen fälschlich eine Warnung angezeigt wurde, wenn ein Vorlagenfeld „Typ“ Werte in Großbuchstaben enthielt

### <a name="storage"></a>Storage

* Problem mit der Migration von Storage V1-Konten zu Storage V2 behoben
* Statusberichterstellung für alle Upload-/Downloadbefehle hinzugefügt
* Fehler korrigiert, der die Verwendung der arg-Option „-n“ mit `storage account check-name` verhindert hat
* Spalte „Momentaufnahme“ zur Tabellenausgabe für `blob [list|show]` hinzugefügt
* Fehler mit verschiedenen Parametern korrigiert, die als Int-Typen analysiert werden mussten

### <a name="vm"></a>VM

* Befehl `vm image accept-terms` hinzugefügt, um die Erstellung von VMs aus Images mit zusätzlichen Gebühren zu ermöglichen
* `[vm|vmss create]` korrigiert, um sicherzustellen, dass Befehle unter einem Proxy mit nicht signierten Zertifikaten ausgeführt werden können
* [VORSCHAU] Unterstützung für „niedrige“ Priorität zu VMSS hinzugefügt
* Schutz für `--admin-password` zu `[vm|vmss] create` hinzugefügt


## <a name="january-17-2018"></a>17. Januar 2018

Version 2.0.25

### <a name="acr"></a>ACR

* Fallback auf ACR-Anmeldung bei Fehlern mit Windows-Anmeldeinformationen hinzugefügt
* Registrierungsprotokolle aktiviert

### <a name="acs"></a>ACS

* Befehl `get-credentials` korrigiert
* SPN-Rollenanforderung entfernt

### <a name="appservice"></a>AppService

* Fehler mit `config ssl upload` behoben, bei dem `hosting_environment_profile` NULL war
* Unterstützung benutzerdefinierter URLs zu `browse` hinzugefügt
* Slotunterstützung für `log tail` korrigiert

### <a name="backup"></a>Backup

* Option `--container-name` von `backup item list` geändert (ist jetzt optional)
* Speicherkontooptionen zu `backup restore restore-disks` hinzugefügt
* Standortüberprüfung in `backup protection enable-for-vm` korrigiert (Groß-/Kleinschreibung wird jetzt nicht mehr beachtet)
* Problem behoben, durch das bei Befehlen mit ungültigem Containernamen ein Fehler auftrat
* `backup item list` geändert (Integritätsstatus jetzt standardmäßig enthalten)

### <a name="batch"></a>Batch

* `batch login` geändert, um Authentifizierungsdetails zurückzugeben

### <a name="cloud"></a>Cloud

* Beim Festlegen von `--profile` für eine Cloud werden nun keine Endpunkte mehr benötigt.

### <a name="consumption"></a>Nutzung

* Neue Befehle für Reservierungen hinzugefügt: `consumption reservations summaries` und `consumption reservations details`

### <a name="event-grid"></a>Event Grid

* [BREAKING CHANGE] Die Befehle vom Typ `az eventgrid topic event-subscription` wurden in `eventgrid event-subscription` verschoben.
* [BREAKING CHANGE] Die Befehle vom Typ `az eventgrid resource event-subscription` wurden in `eventgrid event-subscription` verschoben.
* [BREAKING CHANGE] Der Befehl `eventgrid event-subscription show-endpoint-url` wurde entfernt. Verwenden Sie stattdessen `eventgrid event-subscription show --include-full-endpoint-url`.
* Befehl `eventgrid topic update` hinzugefügt
* Befehl `eventgrid event-subscription update` hinzugefügt
* Parameter `--ids` für Befehle vom Typ `eventgrid topic` hinzugefügt
* Unterstützung der Vervollständigung mit der TAB-TASTE für Themennamen hinzugefügt

### <a name="interactive"></a>Interactive

* Problem behoben, das dazu führte, dass der interaktive Modus nicht mit Python 2.x verwendet werden konnte
* Fehler beim Start behoben
* Problem behoben, das dazu führte, dass einige Befehle nicht im interaktiven Modus ausgeführt werden konnten

### <a name="iot"></a>IoT

* Unterstützung für Gerätebereitstellungsdienst hinzugefügt
* Benachrichtigungen zu veralteten Elementen in Befehlen und in der Befehlshilfe hinzugefügt
* IoT-Überprüfung hinzugefügt, um Benutzer über die IoT-Erweiterung zu informieren

### <a name="monitor"></a>Überwachen

* Unterstützung mehrerer Diagnoseeinstellung hinzugefügt. Der Parameter `--name` ist nun für `az monitor diagnostic-settings create` erforderlich.
* Befehl `monitor diagnostic-settings categories` zum Abrufen der Diagnoseeinstellungskategorie hinzugefügt

### <a name="network"></a>Netzwerk

* Problem behoben, das beim Ändern des aktiven Standbymodus mit `vnet-gateway update` auftrat
* Unterstützung für HTTP2 zu `application-gateway [create|update]` hinzugefügt

### <a name="profile"></a>Profil

* Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt

### <a name="role"></a>Role

* Argument `--assignee-object-id` zu `role assignment create` hinzugefügt, um Graph-Abfrage zu umgehen

### <a name="service-fabric"></a>Service Fabric

* Ausführliche Fehler zur Überprüfungsantwort bei der Clustererstellung hinzugefügt
* Problem mit fehlendem Client für verschiedene Befehle behoben

### <a name="vm"></a>VM

* [VORSCHAUVERSION] Zonenübergreifende Unterstützung für `vmss`
* [BREAKING CHANGE] Standard für Einzelzone (`vmss`) in Standardlastenausgleich geändert
* [BREAKING CHANGE]`externalIdentities` in `userAssignedIdentities` geändert für EMSI
* [VORSCHAUVERSION] Unterstützung für Austausch des Betriebssystemdatenträgers hinzugefügt
* Unterstützung der Verwendung von VM-Images aus anderen Abonnements hinzugefügt
* Argumente `--plan-name`, `--plan-product`, `--plan-promotion-code` und `--plan-publisher` zu `[vm|vmss] create` hinzugefügt
* Fehlerbedingte Probleme mit `[vm|vmss] create` behoben
* Übermäßige Ressourcenverwendung durch `vm image list --all` behoben

## <a name="december-19-2017"></a>19. Dezember 2017

Version 2.0.23

* Unterstützung für die Anmeldung mit durch Benutzer zugewiesenen Identitäten hinzugefügt

### <a name="container"></a>Container

* Falsche Reihenfolge der Parameter für Containerprotokolle behoben

### <a name="network"></a>Netzwerk

* Argument `--disable-bgp-route-propagation` zu `route-table [create|update]` hinzugefügt
* Argument `--ip-tags` zu `public-ip [create|update]` hinzugefügt

### <a name="storage"></a>Storage

* Unterstützung für Storage V2 hinzugefügt

### <a name="vm"></a>VM

* [VORSCHAUVERSION] Unterstützung für durch Benutzer zugewiesene Identitäten für virtuelle Computer und VMSSs hinzugefügt


## <a name="december-5-2017"></a>5\. Dezember 2017

Version 2.0.22

* `az component`-Befehle wurden entfernt. Verwenden Sie stattdessen `az extension`.

### <a name="core"></a>Core
* Der `AZURE_US_GOV_CLOUD`-Autoritätsendpunkt von AAD wurde von „login.microsoftonline.com“ in „login.microsoftonline.us“ geändert.
* Problem behoben, aufgrund dessen Telemetriedaten fortlaufend neu gesendet wurden

### <a name="acs"></a>ACS

* Die Befehle `aks install-connector` und `aks remove-connector` wurden hinzugefügt.
* Verbesserte Fehlerberichterstellung für `acs create`
* Feste Verwendung von `aks get-credentials -f` ohne vollqualifizierten Pfad

### <a name="advisor"></a>Advisor

* Erste Veröffentlichung

### <a name="appservice"></a>AppService

* Erstellung feststehender Zertifikatnamen mit `webapp config ssl upload`
* `webapp [list|show]` und `functionapp [list|show]` wurden verbessert, um die richtigen Apps anzuzeigen
* Standardwert für `WEBSITE_NODE_DEFAULT_VERSION` hinzugefügt

### <a name="consumption"></a>Nutzung

* Unterstützung für API-Version 2017-11-30 hinzugefügt

### <a name="container"></a>Container

* Feste Regression für Standardports

### <a name="monitor"></a>Überwachen

* Unterstützung mehrerer Dimensionen zu Metrikbefehl hinzugefügt

### <a name="resource"></a>Resource

* Argument `--include-response-body` zu `resource show` hinzugefügt

### <a name="role"></a>Role

* Anzeige von Standardzuweisungen für „klassische“ Administratoren zu `role assignment list` hinzugefügt
* Unterstützung für das Hinzufügen (anstelle der Überschreibung) von Anmeldeinformationen zu `ad sp reset-credentials` hinzugefügt
* Verbesserte Fehlerberichterstellung für `ad sp create-for-rbac`

### <a name="sql"></a>SQL

* Die Befehle `sql db list-usages` und `sql db show-usage` wurden hinzugefügt.
* Die Befehle `sql server conn-policy show` und `sql server conn-policy update` wurden hinzugefügt.

### <a name="vm"></a>VM

* Zoneninformationen zu `az vm list-skus` hinzugefügt


## <a name="november-14-2017"></a>14. November 2017

Version 2.0.21

### <a name="acr"></a>ACR

* Unterstützung für das Erstellen von Webhooks in Replikationsregionen hinzugefügt


### <a name="acs"></a>ACS

* Formulierung in AKS von „Agent“ in „Knoten“ geändert
* Option `--orchestrator-release` für `acs create` als veraltet gekennzeichnet
* VM-Standardgröße für AKS in `Standard_D1_v2` geändert
* `az aks browse` für Windows korrigiert
* `az aks get-credentials` für Windows korrigiert

### <a name="appservice"></a>AppService

* Bereitstellungsquelle `config-zip` für Web-Apps und Funktions-Apps hinzugefügt
* Option `--docker-container-logging` zu `az webapp log config` hinzugefügt
* Option `storage` aus dem Parameter `--web-server-logging` von `az webapp log config` entfernt
* Fehlermeldungen für `deployment user set` verbessert
* Unterstützung für das Erstellen von Linux-Funktions-Apps hinzugefügt
* `list-locations` (feststehend)

### <a name="batch"></a>Batch

* Fehler im Poolerstellungsbefehl korrigiert, der bei Verwendung einer Ressourcen-ID mit dem Flag `--image` aufgetreten ist

### <a name="batchai"></a>BatchAI

* Kurzoption (`-s`) für `--vm-size` zur Angabe der VM-Größe im Befehl `file-server create` hinzugefügt
* Argumente für Speicherkontoname und -schlüssel zum Parameter `cluster create` hinzugefügt
* Dokumentation für `job list-files` und `job stream-file` korrigiert
* Kurzoption (`-r`) für `--cluster-name` zur Angabe des Clusternamens im Befehl `job create` hinzugefügt

### <a name="cloud"></a>Cloud

* `cloud [register|update]` geändert, um die Registrierung von Clouds ohne erforderliche Endpunkte zu verhindern

### <a name="container"></a>Container

* Unterstützung für das Öffnen mehrerer Ports hinzugefügt
* Neustartrichtlinie für Containergruppen hinzugefügt
* Unterstützung zum Einbinden einer Azure-Dateifreigabe als Volume hinzugefügt
* Hilfedokumente aktualisiert

### <a name="data-lake-analytics"></a>Data Lake Analytics

* `[job|account] list` geändert, um präzisere Informationen zu erhalten

### <a name="data-lake-store"></a>Data Lake Store

* `account list` geändert, um präzisere Informationen zu erhalten

### <a name="extension"></a>Durchwahl

* `extension list-available` hinzugefügt, um das Auflisten offizieller Microsoft-Erweiterungen zu ermöglichen
* `--name` zu `extension [add|update]` hinzugefügt, um das Installieren von Erweiterungen nach Name zu ermöglichen

### <a name="iot"></a>IoT

* Unterstützung für Zertifizierungsstellen (CAs) und Zertifikatketten hinzugefügt

### <a name="monitor"></a>Überwachen

* Befehle vom Typ `activity-log alert` hinzugefügt

### <a name="network"></a>Netzwerk

* Unterstützung für CAA-DNS-Einträge hinzugefügt
* Problem behoben, durch das Endpunkte nicht mit `traffic-manager profile update` aktualisiert werden konnten
* Problem behoben, durch das `vnet update --dns-servers` je nach VNet-Erstellungsmethode nicht funktionierte
* Problem behoben, durch das relative DNS-Namen durch `dns zone import` nicht korrekt importiert wurden

### <a name="reservations"></a>Reservations

* Erste Vorschauversion

### <a name="resource"></a>Resource

* Unterstützung für Ressourcen-IDs zum Parameter `--resource` und Sperren auf Ressourcenebene hinzugefügt

### <a name="sql"></a>SQL

* Parameter `--ignore-missing-vnet-service-endpoint` zu `sql server vnet-rule [create|update]` hinzugefügt

### <a name="storage"></a>Storage

* `storage account create` geändert, sodass die SKU `Standard_RAGRS` als Standard verwendet wird
* Fehler im Zusammenhang mit Datei-/Blobnamen korrigiert, die ASCII-fremde Zeichen enthalten
* Fehler korrigiert, der die Verwendung von `--source-uri` mit `storage [blob|file] copy start-batch` verhindert hat
* Befehle zum Globalisieren und Löschen mehrerer Objekte mit `storage [blob|file] delete-batch` hinzugefügt
* Problem beim Aktivieren von Metriken mit `storage metrics update` behoben
* Problem mit Dateien über 200 GB bei Verwendung von `storage blob upload-batch` behoben
* Problem behoben, durch das `--bypass` und `--default-action` von `storage account [create|update]` ignoriert wurden

### <a name="vm"></a>VM

* Fehler mit `vmss create` korrigiert, der die Verwendung der Größenebene `Basic` verhindert hat
* `--plan`-Argumente zu `[vm|vmss] create` für benutzerdefinierte Images mit Abrechnungsinformationen hinzugefügt
* Befehle hinzugefügt: `vm secret `[add|remove|list]
* `vm format-secret` in `vm secret format` umbenannt
* Argument `--encrypt format` zu `vm encryption enable` hinzugefügt

## <a name="october-24-2017"></a>24. Oktober 2017

Version 2.0.20

### <a name="core"></a>Core

* Aktualisierung von `2017-03-09-profile` zur Verwendung von Version `2016-01-01` der `MGMT_STORAGE`-API

### <a name="acr"></a>ACR

* Die Ressourcenverwaltung wurde aktualisiert und verweist nun auf die API-Version `2017-10-01`.
* SKU „Bring Your Own Storage“ wurde in „Klassisch“ geändert.
* Die Registrierungs-SKUs wurden in „Basic“, „Standard“ und „Premium“ umbenannt.

### <a name="acs"></a>ACS

* [VORSCHAUVERSION] Befehle vom Typ `az aks` hinzugefügt
* Problem mit `get-credentials` in Kubernetes behoben

### <a name="appservice"></a>AppService

* Problem behoben, aufgrund dessen heruntergeladene `webapp`-Protokolle unter Umständen ungültig waren

### <a name="component"></a>Komponente

* Deutlichere Meldung zur Einstellung für alle Installer und für Bestätigungsaufforderung hinzugefügt

### <a name="monitor"></a>Überwachen

* Befehle vom Typ `action-group` hinzugefügt

### <a name="resource"></a>Resource

* Inkompatibilität mit der aktuellen Version der msrest-Abhängigkeit in `group export` behoben
* Problem mit `policy assignment create` behoben, sodass der Befehl mit integrierten Richtliniendefinitionen und Richtliniensatzdefinitionen verwendet werden kann

### <a name="vm"></a>VM

* Argument `--accelerated-networking` zu `vmss create` hinzugefügt


## <a name="october-9-2017"></a>9\. Oktober 2017

Version 2.0.19

### <a name="core"></a>Core

* Verarbeitung von ADFS-Autoritäts-URLs wurde mit einem nachgestellten Schrägstrich zu Azure Stack hinzugefügt.

### <a name="appservice"></a>AppService

* Mit dem neuen Befehl `webapp update` wurde ein allgemeines Update hinzugefügt.

### <a name="batch"></a>Batch

* Aktualisierung auf Batch SDK 4.0.0
* Die Option `--image` von „VirtualMachineConfiguration“ wurde aktualisiert, um zusätzlich zu „publish:offer:sku:version“ ARM-Imageverweise zu unterstützen.
* Unterstützung für das neue CLI-Erweiterungsmodell für Batch-Erweiterungsbefehle hinzugefügt
* Batch-Unterstützung aus dem Komponentenmodell entfernt

### <a name="batchai"></a>BatchAI

* Erste Version des Batch KI-Moduls

### <a name="keyvault"></a>KeyVault

* Key Vault-Authentifizierungsproblem behoben, das bei Verwendung von ADFS in Azure Stack auftrat. [(#4448)](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a>Netzwerk

* Das Argument `--server` von `application-gateway address-pool create` ist nun optional, sodass leere Adresspools zulässig sind.
* `traffic-manager` wurde aktualisiert, um aktuelle Features zu unterstützen.

### <a name="resource"></a>Resource

* Zusätzliche Unterstützung für `--resource-group/-g`-Optionen für Ressourcengruppennamen zu `group` hinzugefügt
* Befehle für `account lock` hinzugefügt, um die Verwendung mit Sperren auf Abonnementebene zu ermöglichen.
* Befehle für `group lock` hinzugefügt, um die Verwendung mit Sperren auf Gruppenebene zu ermöglichen.
* Befehle für `resource lock` hinzugefügt, um die Verwendung mit Sperren auf Ressourcenebene zu ermöglichen.

### <a name="sql"></a>Sql

* Unterstützung für SQL Transparent Data Encryption (TDE) und TDE für Bring Your Own Key-Szenarien hinzugefügt
* Der Befehl `db list-deleted` und der Parameter `db restore --deleted-time` wurden hinzugefügt, um die Ermittlung und Wiederherstellung gelöschter Datenbanken zu ermöglichen.
* `db op list` und `db op cancel` wurden hinzugefügt, um das Auflisten und Abbrechen ausgeführter Vorgänge für eine Datenbank zu ermöglichen.

### <a name="storage"></a>Storage

* Unterstützung für Momentaufnahme von Dateifreigaben hinzugefügt

### <a name="vm"></a>VM

* Korrektur eines Fehlers in `vm show`, bei dem die Verwendung von `-d` in Verbindung mit fehlenden privaten IP-Adressen einen Absturz verursachte
* [VORSCHAUVERSION] Unterstützung für paralleles Upgrade zu `vmss create` hinzugefügt
* Unterstützung für das Aktualisieren der Verschlüsselungseinstellungen mit `vm encryption enable` hinzugefügt
* Parameter `--os-disk-size-gb` zu `vm create` hinzugefügt
* Parameter `--license-type` für Windows zu `vmss create` hinzugefügt


## <a name="september-22-2017"></a>22. September 2017

Version 2.0.18

### <a name="resource"></a>Resource

* Unterstützung für das Anzeigen integrierter Richtliniendefinitionen hinzugefügt
* Unterstützungsmodusparameter zum Erstellen von Richtliniendefinitionen hinzugefügt
* Unterstützung für UI-Definitionen und -Vorlagen zu `managedapp definition create` hinzugefügt
* [BREAKING CHANGE] Der Ressourcentyp `managedapp` wurde von `appliances` in `applications` und von `applianceDefinitions` in `applicationDefinitions` geändert.

### <a name="network"></a>Netzwerk

* Unterstützung für Verfügbarkeitszone zu Unterbefehlen `network lb` und `network public-ip` hinzugefügt
* Unterstützung für IPv6-Microsoft-Peering zu `express-route` hinzugefügt
* Befehle für Anwendungssicherheitsgruppe `asg` hinzugefügt
* Argument `--application-security-groups` zu `nic [create|ip-config create|ip-config update]` hinzugefügt
* Argumente `--source-asgs` und `--destination-asgs` zu `nsg rule [create|update]` hinzugefügt
* Argumente `--ddos-protection` und `--vm-protection` zu `vnet [create|update]` hinzugefügt
* Befehle vom Typ `network [vnet-gateway|vpn-client|show-url]` hinzugefügt

### <a name="storage"></a>Storage

* Problem behoben, das nach der Aktualisierung des SDK unter Umständen einen Fehler der `storage account network-rule`-Befehle zur Folge hatte

### <a name="eventgrid"></a>Eventgrid

* Azure Event Grid Python SDK für die Verwendung der neueren API-Version „2017-09-15-preview“ aktualisiert

### <a name="sql"></a>SQL

* `sql server list`-Argument `--resource-group` geändert, sodass es nun optional ist. Wird es nicht angegeben, werden alle SQL Server-Instanzen im Abonnement zurückgegeben.
* Parameter `--no-wait` zu `db [create|copy|restore|update|replica create|create|update]` und `dw [create|update]` hinzugefügt

### <a name="keyvault"></a>KeyVault

* Unterstützung für die Keyvault-Befehlsausführung hinter einem Proxy hinzugefügt

### <a name="vm"></a>VM

* Unterstützung für Verfügbarkeitszone zu `[vm|vmss|disk] create` hinzugefügt
* Problem behoben, das bei Verwendung von `--app-gateway ID` mit `vmss create` einen Fehler zur Folge hatte
* Argument `--asgs` zu `vm create` hinzugefügt
* Unterstützung für die Ausführung von Befehlen auf virtuellen Computern mit `vm run-command` hinzugefügt
* [VORSCHAU] Unterstützung für VMSS-Datenträgerverschlüsselung mit `vmss encryption` hinzugefügt
* Unterstützung für die Durchführung der Wartung auf virtuellen Computern mit `vm perform-maintenance` hinzugefügt

### <a name="acs"></a>ACS

* [VORSCHAU] Argument `--orchestrator-release` zu `acs create` für ACS-Vorschauregionen hinzugefügt

### <a name="appservice"></a>AppService

* Neue Möglichkeit zum Aktualisieren und Anzeigen der Authentifizierungseinstellungen mit `webapp auth [update|show]`

### <a name="backup"></a>Backup

* Vorschauversion


## <a name="september-11-2017"></a>11. September 2017

Version 2.0.17

### <a name="core"></a>Core

* Festlegung einer eigenen Korrelations-ID in Telemetrie durch das Befehlsmodul aktiviert
* Ein Problem mit der JSON-Sicherungsdatei wurde behoben, das beim Festlegen des Diagnosemodus für Telemetrie auftrat

### <a name="acs"></a>ACS

* Befehl `acs list-locations` hinzugefügt
* `ssh-key-file` wird mit dem erwarteten Standardwert versehen.

### <a name="appservice"></a>AppService

* Neue Möglichkeit zum Erstellen einer Web-App in einer anderen Ressourcengruppe als der des aktiven Diensttarifs

### <a name="cdn"></a>CDN

* Der Fehler bei `cdn custom-domain create`, dass „CustomDomain“ nicht wiederholbar ist, wurde behoben.

### <a name="extension"></a>Durchwahl

* Erstrelease

### <a name="keyvault"></a>KeyVault

* Problem behoben, aufgrund dessen bei den Berechtigungen für `keyvault set-policy` die Groß-/Kleinschreibung beachtet werden musste

### <a name="network"></a>Netzwerk

* `vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt
* Das Argument `--private-access-services` wurde für `vnet subnet create/update` in `--service-endpoints` umbenannt.
* Unterstützung für mehrere IP- und Portbereiche zu `nsg rule create/update` hinzugefügt
* Unterstützung für SKU zu `lb create` hinzugefügt
* Unterstützung für SKU zu `public-ip create` hinzugefügt

### <a name="resource"></a>Resource

* Übergabe von Parameterdefinitionen für Ressourcenrichtlinien in `policy definition create` und `policy definition update` zulassen
* Übergabe von Parameterwerten für `policy assignment create` zulassen
* Übergabe von JSON-Code oder einer Datei für alle Parameter zulassen
* Inkrementierte API-Version

### <a name="sql"></a>SQL

* Befehle vom Typ `sql server vnet-rule` hinzugefügt

### <a name="vm"></a>VM

* Behoben: Zugriff nur zuweisen, wenn `--scope` angegeben wird
* Behoben: Gleiche Erweiterungsbenennung wie Portal verwenden
* `subscription` aus der Ausgabe von `[vm|vmss] create` entfernt
* Behoben: Speicher-SKU vom Typ `[vm|vmss] create` wird nicht auf Datenträger mit einem Image angewendet.
* Behoben: `vm format-secret --secrets` akzeptierte keine durch neue Zeilen getrennte IDs.

## <a name="august-31-2017"></a>31. August 2017

Version 2.0.16

### <a name="keyvault"></a>KeyVault

* Fehler behoben, der beim Versuch auftrat, die Geheimniscodierung mit `secret download` automatisch aufzulösen

### <a name="sf"></a>Sf

* Alle Befehle wurden durch die Service Fabric-Befehlszeilenschnittstelle (sfctl) ersetzt.

### <a name="storage"></a>Storage

* Problem behoben, aufgrund dessen Speicherkonten nicht in Regionen erstellt werden konnten, die die NetworkACLs-Funktion nicht unterstützen
* Festlegen des Inhaltstyps und der Inhaltscodierung während Blob- und Dateiuploads, wenn weder Inhaltstyp noch Inhaltscodierung angegeben sind

## <a name="august-28-2017"></a>28. August 2017

Version 2.0.15

### <a name="cli"></a>Befehlszeilenschnittstelle (CLI)

* Rechtlichen Hinweis zu `--version` hinzugefügt

### <a name="acs"></a>ACS

* Vorschauregionen korrigiert
* Standardmäßiges DNS-Namenspräfix (`dns_name_prefix`) ordnungsgemäß formatiert
* ACS-Befehlsausgabe optimiert

### <a name="appservice"></a>AppService

* [BREAKING CHANGE] Inkonsistenzen in der Ausgabe von `az webapp config appsettings [delete|set]` behoben
* Neuen Alias (`-i`) für `az webapp config container set --docker-custom-image-name` hinzugefügt
* `az webapp log show` verfügbar gemacht
* Neue Argumente aus `az webapp delete` verfügbar gemacht, um App Service-Plan, Metriken oder DNS-Registrierung beizubehalten
* Behoben: Korrekte Erkennung der Sloteinstellungen

### <a name="iot"></a>IoT

* #3934 behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien

### <a name="network"></a>Netzwerk

* [BREAKING CHANGE]`vnet list-private-access-services` in `vnet list-endpoint-services` umbenannt
* [BREAKING CHANGE] Option `--private-access-services` für `--service-endpoints` in `vnet subnet [create|update]` umbenannt
* Unterstützung für mehrere IP- und Portbereiche zu `nsg rule [create|update]` hinzugefügt
* Unterstützung für SKU zu `lb create` hinzugefügt
* Unterstützung für SKU zu `public-ip create` hinzugefügt

### <a name="profile"></a>Profil

* `--msi` und `--msi-port` für die Anmeldung mit der Identität eines virtuellen Computers verfügbar gemacht

### <a name="service-fabric"></a>Service Fabric

* Vorschauversion
* Registrierungsbenutzer-/-kennwortregeln für Befehl vereinfacht
* Kennwortanforderung für Benutzer trotz Parameterübergabe behoben
* Unterstützung für leere Registrierungsanmeldeinformationen (`registry_cred`) hinzugefügt

### <a name="storage"></a>Storage

* Festlegen des Blobtarifs ermöglicht
* Argumente `--bypass` und `--default-action` zur Unterstützung von Diensttunneling zu `storage account [create|update]` hinzugefügt
* Befehle zum Hinzufügen von VNet-Regeln und IP-basierten Regeln zu `storage account network-rule` hinzugefügt
* Dienstverschlüsselung durch vom Kunden verwalteten Schlüssel ermöglicht
* [BREAKING CHANGE] Option `--encryption` für Befehl `az storage account create and az storage account update` in `--encryption-services` umbenannt
* Behoben (4220): `az storage account update encryption` – Syntaxkonflikt

### <a name="vm"></a>VM

* Problem behoben, aufgrund dessen bei Verwendung von `--instance-id *` zusätzliche, fehlerhafte Informationen für `vmss get-instance-view` angezeigt wurden
* Unterstützung für `--lb-sku` zu `vmss create` hinzugefügt:
* Menschliche Namen aus der Administratornamen-Blacklist für `[vm|vmss] create` entfernt
* Problem behoben, aufgrund dessen `[vm|vmss] create` einen Fehler ausgelöst hat, wenn aus einem Image keine Tarifinformationen extrahiert werden konnten
* Absturzproblem beim Erstellen einer VMMS-Skalierungsgruppe mit einem internen Lastenausgleich behoben
* Problem behoben, aufgrund dessen das Argument `--no-wait` nicht mit `vm availability-set create` verwendet werden konnte


## <a name="august-15-2017"></a>15. August 2017

Version 2.0.14

### <a name="acs"></a>ACS

* sshMaster0-Portnummer für Kubernetes korrigiert

### <a name="appservice"></a>AppService

* Ausnahme beim Erstellen einer neuen Git-basierten Linux-Web-App behoben

### <a name="event-grid"></a>Event Grid

* SDK-Abhängigkeiten hinzugefügt

## <a name="august-11-2017"></a>11. August 2017

Version 2.0.13

### <a name="acs"></a>ACS

* Weitere Vorschauregionen hinzugefügt

### <a name="batch"></a>Batch

* Auf Batch SDK 3.1.0 und Batch Management SDK 4.1.0 aktualisiert
* Neuen Befehl zum Anzeigen der Aufgabenanzahl eines Auftrags hinzugefügt
* Fehler in der SAS-URL-Verarbeitung der Ressourcendatei behoben
* Batch-Kontoendpunkt unterstützt nun optionales Präfix „https://“
* Unterstützung für das Hinzufügen von Listen mit mehr als 100 Aufgaben zu einem Auftrag
* Debugprotokollierung für das Laden des Erweiterungsbefehlsmoduls hinzugefügt

### <a name="component"></a>Komponente

* Warnung für veraltete Befehle vom Typ „az component“ hinzugefügt

### <a name="container"></a>Container

* `create`: Problem behoben, aufgrund dessen das Gleichheitszeichen innerhalb einer Umgebungsvariablen nicht zulässig war


### <a name="data-lake-store"></a>Data Lake Store

* Fortschrittsüberwachung ermöglicht

### <a name="event-grid"></a>Event Grid

* Erste Veröffentlichung

### <a name="network"></a>Netzwerk

* `lb`: Problem behoben, aufgrund dessen bestimmte Namen untergeordneter Ressourcen bei Auslassung nicht richtig aufgelöst wurden
* `application-gateway {subresource} delete`: Problem behoben, aufgrund dessen `--no-wait` nicht berücksichtigt wurde
* `application-gateway http-settings update`: Problem behoben, aufgrund dessen `--connection-draining-timeout` nicht deaktiviert werden konnte
* Fehler behoben: Unerwartetes Schlüsselwortargument `sa_data_size_kilobyes` bei `az network vpn-connection ipsec-policy add`

### <a name="profile"></a>Profil

* `account list`: `--refresh` hinzugefügt, um die neuesten Abonnements vom Server zu synchronisieren

### <a name="storage"></a>Storage

* Aktualisieren des Speicherkontos mit vom System zugewiesener Identität ermöglicht

### <a name="vm"></a>VM

* `availability-set`: Fehlerdomänenanzahl bei Konvertierung verfügbar gemacht
* Befehl `list-skus` verfügbar gemacht
* Unterstützung der Identitätszuweisung ohne Erstellung von Rollenzuweisungen
* Anwenden von Speicher-SKU beim Anfügen von Datenträgern
* Standardmäßiger Betriebssystemdatenträger-Name und Speicher-SKU bei Verwendung verwalteter Datenträger entfernt


## <a name="july-28-2017"></a>28. Juli 2017

Version 2.0.12

* Containerbefehle hinzugefügt
* Abrechnungs- und Nutzungsmodule hinzugefügt

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

### <a name="core"></a>Core

* Ausgabe von SDK-Authentifizierungsinformationen für Dienstprinzipale mit Zertifikaten
* Ausnahmen beim Bereitstellungsfortschritt behoben
* Verwendung des ARM-Endpunkts aus der aktuellen Cloud für die Erstellung des Abonnementclients
* Gleichzeitige Verarbeitung der Datei „clouds.config“ verbessert (3636)
* Aktualisierung der Clientanforderungs-ID für jede Befehlsausführung
* Erstellung von Abonnementclients mit richtigem SDK-Profil (3635)
* Statusmeldung für Vorlagenbereitstellungen (3510)
* Unterstützung für Auswahl von Tabellenausgabefeldern über jmespath Abfrage hinzugefügt (3581)
* Stummschaltung von Analyseargumenten und Anfügeverlauf mit Gesten verbessert (3434)
* Erstellung von Abonnementclients mit richtigem SDK-Profil
* Verschiebung aller vorhandenen Erfassungsdateien in den neuesten Ordner
* Idempotenz für VM-/VMSS-Erstellung behoben (3586)
* Bei Befehlspfaden wird die Groß-/Kleinschreibung nicht mehr beachtet.
* Bei bestimmten booleschen Parametern wird die Groß-/Kleinschreibung nicht mehr beachtet.
* Unterstützung der Anmeldung bei lokalem AD FS-Server wie Azure Stack
* Gleichzeitige Schreibvorgänge in „clouds.config“ behoben (3255)

### <a name="acr"></a>ACR

* Befehl `show-usage` für verwaltete Registrierungen hinzugefügt
* Unterstützung der SKU-Aktualisierung für verwaltete Registrierungen
* Verwaltete Registrierungen mit verwalteter SKU hinzugefügt
* Webhooks für verwaltete Registrierungen mit ACR-Webhook-Befehlsmodul hinzugefügt
* AAD-Authentifizierung mit ACR-Anmeldebefehl hinzugefügt
* Löschbefehl für Docker-Repositorys, Manifeste und Tags hinzugefügt

### <a name="acs"></a>ACS

* Unterstützung der API-Version 2017-07-01

### <a name="appservice"></a>AppService

* Fehler behoben, aufgrund dessen die Auflistung der Linux-Web-App keine Werte zurückgegeben hat
* Unterstützung für das Abrufen von Anmeldeinformationen aus dem ACR
* Entfernung aller Befehle unter `appservice web`
* Maskierung von Docker-Registrierungskennwörtern aus der Befehlsausgabe (3656)
* Gewährleistung der fehlerfreien Verwendung des Standardbrowsers unter macOS (3623)
* Verbesserung des Nutzens von `webapp log tail` und `webapp log download` (3624)
* Befehl `traffic-routing` zum Konfigurieren des statischen Routings verfügbar gemacht (3566)
* Zuverlässigkeit beim Konfigurieren der Quellcodeverwaltung verbessert (3245)
* Nicht unterstütztes Argument `--node-version` aus `webapp config update` für Windows-Web-Apps entfernt. Verwenden Sie stattdessen `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.

### <a name="batch"></a>Batch

* Auf Batch SDK 3.0.0 mit Unterstützung virtueller Computer mit niedriger Priorität in Pools aktualisiert
* `pool create`-Option `--target-dedicated` in `--target-dedicated-nodes` umbenannt
* `pool create`-Optionen `--target-low-priority-nodes` und `--application-licenses` hinzugefügt

### <a name="cdn"></a>CDN

* Besser verständliche Fehlermeldung für `cdn endpoint list`, wenn das von `--profile-name` angegebene Profil nicht vorhanden ist

### <a name="cloud"></a>Cloud

* API-Version des Cloudmetadaten-Endpunkts in das Format JJJJ-MM-TT umgewandelt
* Katalogendpunkt nicht erforderlich
* Unterstützung für die Cloudregistrierung nur mit ARM-Endpunkt
* Option für `cloud set` bereitgestellt, um beim Auswählen der aktuellen Cloud das Profil auswählen zu können
* `endpoint_vm_image_alias_doc` verfügbar gemacht

### <a name="cosmosdb"></a>CosmosDB

* Möglichkeit zum Erstellen einer Auflistung mit benutzerdefiniertem Partitionsschlüssel behoben
* Unterstützung für Auflistungs-Standardgültigkeitsdauer hinzugefügt

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Zusätzliche Befehle für Compute-Richtlinienverwaltung unter der Überschrift `dla account compute-policy` hinzugefügt
* `dla job pipeline show` hinzugefügt
* `dla job recurrence list` hinzugefügt

### <a name="data-lake-store"></a>Data Lake Store

* Unterstützung für vom Benutzer verwaltete Schlüsseltresor-Schlüsselrotation in `dls account update` hinzugefügt
* Zugrunde liegende SDK-Version des Data Lake Store-Dateisystems aktualisiert, um ein Leistungsproblem zu behandeln
* Befehl `dls enable-key-vault` hinzugefügt. Dieser Befehl versucht, eine vom Benutzer angegebene Key Vault-Instanz zur Verschlüsselung der Daten in einem Data Lake Store-Konto zu aktivieren.

### <a name="interactive"></a>Interactive

* Startzeit durch Verwendung zwischengespeicherter Befehle verbessert
* Testabdeckung verbessert
* ?-Geste erweitert, sodass sie auch in den nächsten Befehl eingefügt wird
* Interaktive Fehler mit dem Profil „2017-03-09-profile-preview“ behoben (3587)
* `--version` als Parameter für den interaktiven Modus zugelassen (3645)
* Beseitigung von Fehlern im interaktiven Modus beim Abschluss von Überprüfungen (3570)
* Statusmeldung für Vorlagenbereitstellungen (3510)
* Flag `--progress` hinzugefügt
* `--debug` und `--verbose` aus Abschlüssen entfernt
* `interactive` aus Abschlüssen entfernt (3324)

### <a name="iot"></a>IoT

* Behoben: Richtlinienerstellung führt nicht mehr zur Löschung bereits vorhandener Richtlinien (3934)

### <a name="key-vault"></a>Schlüsseltresor

* Befehle für Schlüsseltresor-Wiederherstellungsfeatures hinzugefügt:
  * `keyvault`-Unterbefehle: `purge`, `recover`, `keyvault list-deleted`
  * `keyvault secret`-Unterbefehle: `backup`, `restore`, `purge`, `recover`, `list-deleted`
  * `keyvault certificate`-Unterbefehle: `purge`, `recover`, `list-deleted`
  * `keyvault key`-Unterbefehle: `purge`, `recover`, `list-deleted`
* Dienstprinzipal-Schlüsseltresorintegration hinzugefügt (3133)
* Schlüsseltresor-Datenebene auf 0.3.2. aktualisiert (3307)

### <a name="lab"></a>Labor

* Unterstützung für Übernahme eines beliebigen virtuellen Computers im Labor über `az lab vm claim` hinzugefügt
* Tabellenausgabeformatierer für `az lab vm list` und `az lab vm show` hinzugefügt

### <a name="monitor"></a>Überwachen

* Korrektur für Vorlagendatei mit Befehl `monitor autoscale-settings get-parameters-template` (3349)
* `monitor alert-rule-incidents list` in `monitor alert list-incidents` umbenannt
* `monitor alert-rule-incidents show` in `monitor alert show-incident` umbenannt
* `monitor metric-defintions list` in `monitor metrics list-definitions` umbenannt
* `monitor alert-rules` in `monitor alert` umbenannt
* `monitor alert create` geändert:
  * Unterbefehle vom Typ `condition` und `action` akzeptieren keinen JSON-Code mehr.
  * Hinzufügung zahlreicher Parameter zur Vereinfachung der Regelerstellung
  * `location` nicht mehr erforderlich
  * Hinzufügung von Namen- und ID-Unterstützung für Ziel
  * Entfernung von `--alert-rule-resource-name`
  * Umbenennung von `is-enabled` in `enabled` (nicht mehr erforderlich)
  * `description` wird nun abhängig von der angegebenen Bedingung auf einen Standardwert festgelegt.
  *  Hinzufügung von Beispielen zur Verdeutlichung des neuen Formats
* Unterstützung von Namen oder IDs für Befehle vom Typ `monitor metric`
* Komfortargumente und Beispiele zu `monitor alert rule update` hinzugefügt

### <a name="network"></a>Netzwerk

* Befehl `list-private-access-services` hinzugefügt
* Argument `--private-access-services` zu `vnet subnet create` und `vnet subnet update` hinzugefügt
* Problem behoben, das einen Fehler für `application-gateway redirect-config create` zur Folge hatte
* Problem behoben, aufgrund dessen `application-gateway redirect-config update` nicht mit `--no-wait` verwendet werden konnte
* Fehler behoben, der bei der Verwendung des Arguments `--servers` mit `application-gateway address-pool create` und `application-gateway address-pool update` aufgetreten ist
* Befehle vom Typ `application-gateway redirect-config` hinzugefügt
* Befehle zu `application-gateway ssl-policy` hinzugefügt: `list-options`, `predefined list`, `predefined show`
* Argumente zu `application-gateway ssl-policy set` hinzugefügt: `--name`, `--cipher-suites`, `--min-protocol-version`
* Argumente zu `application-gateway http-settings create` und `application-gateway http-settings update` hinzugefügt: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`
* Argumente zu `application-gateway url-path-map create` und `application-gateway url-path-map update` hinzugefügt: `--default-redirect-config`, `--redirect-config`
* Argument `--redirect-config` zu `application-gateway url-path-map rule create` hinzugefügt
* Unterstützung für `--no-wait` zu `application-gateway url-path-map rule delete` hinzugefügt
* Argumente zu `application-gateway probe create` und `application-gateway probe update` hinzugefügt: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`
* Argument `--redirect-config` zu `application-gateway rule create` und `application-gateway rule update` hinzugefügt
* Unterstützung für `--accelerated-networking` zu `nic create` und `nic update` hinzugefügt
* Argument `--internal-dns-name-suffix` von `nic create` entfernt
* Unterstützung für `--dns-servers` zu `nic update` und `nic create` hinzugefügt: Hinzufügung von Unterstützung für --dns-servers
* Fehler korrigiert, aufgrund dessen `--local-address-prefixes` von `local-gateway create` ignoriert wurde
* Unterstützung für `--dns-servers` zu `vnet update` hinzugefügt
* Fehler beim Erstellen eines Peerings ohne Routenfilterung mit `express-route peering create` korrigiert
* Fehler korrigiert, aufgrund dessen die Argumente `--provider` und `--bandwidth` nicht mit `express-route update` verwendet werden konnten
* Fehler mit Standardlogik von `network watcher show-topology` korrigiert
* Ausgabeformatierung für `network list-usages` verbessert
* Verwendung der standardmäßigen Front-End-IP-Adresse für `application-gateway http-listener create` (sofern vorhanden)
* Verwendung des Standardadresspools, der HTTP-Standardeinstellungen und des HTTP-Standardlisteners für `application-gateway rule create` (sofern vorhanden)
* Verwendung der standardmäßigen Front-End-IP-Adresse und des standardmäßigen Back-End-Pools für `lb rule create` (sofern vorhanden)
* Verwendung der standardmäßigen Front-End-IP-Adresse für `lb inbound-nat-rule create` (sofern vorhanden)

### <a name="profile"></a>Profil

* Unterstützung der Anmeldung innerhalb eines virtuellen Computers mit einer verwalteten Identität
* Unterstützung der Ausgabe für `account show` im SDK-Authentifizierungsdateiformat
* Anzeige von Warnungen für veraltete Befehle bei Verwendung von „--expanded-view“
* Befehl `get-access-token` für die Bereitstellung eines unformatierten AAD-Tokens hinzugefügt
* Unterstützung der Anmeldung mit einem Benutzerkonto ohne zugeordnete Abonnements

### <a name="rdbms"></a>RDBMS

* Unterstützung der abonnementübergreifenden Auflistung von Servern (3417)
* Behoben: `%s` wird aufgrund von fehlendem `% server_type` nicht verarbeitet (3393)
* Dokumentquellenzuordnung behoben und CI-Aufgabe zur Überprüfung hinzugefügt (3361)
* MySQL- und PostgreSQL-Hilfe korrigiert (3369)

### <a name="resource"></a>Resource

* Eingabeaufforderungen bei fehlenden Parametern für `group deployment create` verbessert
* Analyse der Syntax `--parameters KEY=VALUE` verbessert
* Probleme behoben, durch die Parameterdateien von `group deployment create` bei Verwendung der Syntax `@<file>` nicht mehr erkannt wurden
* Unterstützung des Arguments `--ids` für Befehle vom Typ `resource` und `managedapp`
* Einige Analyse- und Fehlermeldungen korrigiert (3584)
* Analyse vom Typ `--resource-type` für den Befehl `lock` korrigiert, sodass `<resource-namespace>` und `<resource-type>` akzeptiert werden
* Parameterüberprüfung für Vorlagenlinkvorlagen hinzugefügt (3629)
* Unterstützung für die Angabe von Bereitstellungsparametern mit der Syntax `KEY=VALUE` hinzugefügt

### <a name="role"></a>Role

* Unterstützung der Ausgabe im SDK-Authentifizierungsdateiformat für `create-for-rbac`
* Rollenzuweisungen und dazugehörige AAD-Anwendung beim Löschen eines Dienstprinzipals bereinigt (3610)
* Einbeziehung des Zeitformats in Beschreibungen vom Typ `--start-date` und `--end-date` für `app create`-Argumente
* Anzeige von Warnungen für veraltete Befehle bei Verwendung von `--expanded-view`
* Schlüsseltresorintegration zu den Befehlen `create-for-rbac` und `reset-credentials` hinzugefügt

### <a name="service-fabric"></a>Service Fabric
* Problem behoben, aufgrund dessen große Dateien in Anwendungen beim Hochladen gekürzt wurden (3666)
* Tests für Service Fabric-Befehle hinzugefügt (3424)
* Zahlreiche Service Fabric-Befehle korrigiert (3234)

### <a name="sql"></a>SQL

* Fehlerhafte1 Parameter `--identity` für `sql server create` entfernt
* Kennwortwerte aus der Befehlsausgabe von `sql server create` und `sql server update` entfernt
* Befehle `sql db list-editions` und `sql elastic-pool list-editions` hinzugefügt

### <a name="storage"></a>Storage

* Option `--marker` für die Befehle `storage blob list`, `storage container list` und `storage share list` entfernt (3745)
* Erstellung eines reinen HTTPS-Speicherkontos ermöglicht
* Speichermetriken, Protokollierung und CORS-Befehle aktualisiert (3495)
* Ausnahmemeldung von „cors add“ umformuliert (3638) (3362)
* Generator im Probelaufmodus des Downloadbatchbefehls in eine Liste konvertiert (3592)
* Problem bei Probelauf des Blobdownloadbatchs behoben (3640) (3592)

### <a name="vm"></a>VM

* Unterstützung der NSG-Konfiguration
* Fehler behoben, aufgrund dessen der DNS-Server nicht ordnungsgemäß konfiguriert wurde
* Unterstützung verwalteter Dienstidentitäten
* Problem behoben, aufgrund dessen `cmss create` mit einem vorhandenen Lastenausgleich `--backend-pool-name` benötigte
* Festlegung, dass die LUN von mit `vm image create` erstellten Datenträgern mit 0 beginnt


## <a name="may-10-2017"></a>10. Mai 2017

Version 2.0.6

* Umbenennen von „documentdb“ in „cosmosdb“
* Hinzufügen von rdbms (mysql, postgres)
* Einbeziehen der Data Lake Analytics- und Data Lake Store-Module
* Einbeziehen des Cognitive Services-Moduls
* Einbeziehen des Service Fabric-Moduls
* Einbeziehen des interaktiven Moduls (Umbenennen von „az-shell“)
* Hinzufügen von Unterstützung für CDN-Befehle
* Entfernen des Containermoduls
* Hinzufügen von „az -v“ als Verknüpfung für „az --version“ ([#2926](https://github.com/Azure/azure-cli/issues/2926))
* Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))

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

### <a name="core"></a>Core

* Core: Erfassen von Ausnahmen, die durch einen nicht registrierten Anbieter verursacht werden, und automatische Registrierung
* Leistung: Dauerhaftes Speichern des ADAL-Tokencaches im Arbeitsspeicher bis zum Prozessende ([#2603](https://github.com/Azure/azure-cli/issues/2603))
* Korrigieren der vom hexadezimalen Fingerabdruck -o tsv zurückgegebenen Bytes ([#3053](https://github.com/Azure/azure-cli/issues/3053))
* Verbessern des Downloads des Schlüsseltresorzertifikats und der AAD-SP-Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))
* Hinzufügen des Python-Speicherorts zu „az –version“ ([#2986](https://github.com/Azure/azure-cli/issues/2986))
* Anmeldung: Unterstützung der Anmeldung, wenn keine Abonnements vorhanden sind ([#2929](https://github.com/Azure/azure-cli/issues/2929))
* Core: Beheben eines Fehlers bei zweimaliger Verwendung eines Dienstprinzipals bei der Anmeldung ([#2800](https://github.com/Azure/azure-cli/issues/2800))
* Core: Ermöglichen der Konfiguration des Dateipfads von „accessTokens.json“ über eine Umgebungsvariable ([#2605](https://github.com/Azure/azure-cli/issues/2605))
* Core: Zulassen der Anwendung konfigurierter Standardwerte auf optionale Argumente ([#2703](https://github.com/Azure/azure-cli/issues/2703))
* Core: Verbesserte Leistung
* Core: Zertifikate von benutzerdefinierter Zertifizierungsstelle – Unterstützung für das Festlegen der REQUESTS_CA_BUNDLE-Umgebungsvariablen
* Core: Cloudkonfiguration – Verwenden des Endpunkts „resource manager“, wenn Endpunkt „management“ nicht festgelegt ist

### <a name="acs"></a>ACS

* Korrigieren der Master- und Agentanzahl als ganze Zahl statt Zeichenfolge
* Verfügbarmachen von „az acs create --no-wait“ und „az acs wait“ für die asynchrone Erstellung
* Verfügbarmachen von „az acs create --validate“ für Probelaufüberprüfungen
* Entfernen von Windows-Profil vor PUT-Aufruf für Skalierungsbefehl ([#2755](https://github.com/Azure/azure-cli/issues/2755))

### <a name="appservice"></a>AppService

* functionapp: Hinzufügen der vollständigen functionapp-Unterstützung, einschließlich Erstellen, Anzeigen, Auflisten, Löschen, Hostname, SSL usw.
* Hinzufügen von Team Services (vsts) als Continuous Delivery-Option zu „appservice web source-control config“
* Erstellen von „az webapp“ als Ersatz für „az appservice web“ (für Abwärtskompatibilität bleibt „az appservice web“ für 2 weitere Releases erhalten)
* Verfügbarmachen von Argumenten zum Konfigurieren von Bereitstellung und Laufzeitstapeln beim Erstellen von Web-Apps
* Verfügbarmachen von „webapp list-runtimes“
* Unterstützen der Konfiguration von Verbindungszeichenfolgen ([#2647](https://github.com/Azure/azure-cli/issues/2647))
* Unterstützen des Slottauschs mit Vorschau
* Beheben von Fehlern in appservice-Befehlen ([#2948](https://github.com/Azure/azure-cli/issues/2948))
* Verwenden der Ressourcengruppe des App Service-Plans für Zertifizierungsvorgänge ([#2750](https://github.com/Azure/azure-cli/issues/2750))

### <a name="cosmosdb"></a>CosmosDB

* Umbenennen des documentdb-Moduls in cosmosdb
* Zusätzliche Unterstützung für documentdb-APIs auf Datenebene: Datenbank- und Sammlungsverwaltung
* Zusätzliche Unterstützung für das Aktivieren des automatischen Failovers für Datenbankkonten
* Zusätzliche Unterstützung für die neue ConsistentPrefix-Konsistenzrichtlinie

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Beheben eines Fehlers, bei dem das Filtern von Auftragslisten nach Ergebnis und Status einen Fehler auslöst
* Hinzufügen von Unterstützung für den neuen Katalogelementtyp „Paket“ Zugriff über: `az dla catalog package`
* Ermöglichen der Auflistung folgender Katalogelemente innerhalb einer Datenbank (keine Schemaspezifikation erforderlich):

  * Tabelle
  * Tabellenwertfunktion
  * Sicht
  * Tabellenstatistiken. Können auch mit einem Schema, jedoch ohne Angabe eines Tabellennamens aufgelistet werden.

### <a name="data-lake-store"></a>Data Lake Store

* Aktualisieren der Version des zugrunde liegenden Dateisystem-SDK, wodurch eine bessere Unterstützung für die Verarbeitung von Drosselungsszenarien auf Serverseite gewährt wird
* Verbessern der Leistung des Paketladevorgangs und der Befehlsausführung ([#2819](https://github.com/Azure/azure-cli/issues/2819))
* Fehlende Hilfe für Zugriffsanzeige hinzugefügt ([#2743](https://github.com/Azure/azure-cli/issues/2743))

### <a name="find"></a>Suchen

* Verbessern von Suchergebnissen und Ermöglichen der Versionsverwaltung des Suchindex

### <a name="keyvault"></a>KeyVault

* BC:`az keyvault certificate download` Ändern von „-e“ von Zeichenfolge oder Binärdatentyp in PEM oder DER zur besseren Darstellung der Optionen
* BC: Entfernen von „--expires“ und „--not-before“ aus `keyvault certificate create`, da diese Parameter nicht vom Dienst unterstützt werden
* Hinzufügen des Parameters „--validity“ zu `keyvault certificate create`, um gezielt den Wert in „--policy“ zu überschreiben
* Beheben des Problems in `keyvault certificate get-default-policy`, bei dem „expires“ und „not_before“ verfügbar gemacht wurden, „validity_in_months“ hingegen nicht
* Keyvault-Korrektur für den Import von PEM und PFX ([#2754](https://github.com/Azure/azure-cli/issues/2754))

### <a name="lab"></a>Labor

* Hinzufügen der Befehle „create“, „show“, „delete“ und „list“ für die Laborumgebung
* Hinzufügen der Befehle „show“ und „list“ zur Anzeige von ARM-Vorlagen im Labor
* Hinzufügen des Kennzeichens „--environment“ in `az lab vm list`, um virtuelle Computer nach Umgebung im Labor zu filtern
* Hinzufügen des benutzerfreundlichen Befehls `az lab formula export-artifacts` zum Exportieren des Artefaktgerüsts innerhalb der Formel eines Labors
* Hinzufügen von Befehlen zum Verwalten von Geheimnissen in einem Labor

### <a name="monitor"></a>Überwachen

* Fehlerbehebung: Modellieren von `--actions` von `az alert-rules create` zum Verarbeiten von JSON-Zeichenfolgen ([#3009](https://github.com/Azure/azure-cli/issues/3009))
* Programmfehlerbehebung: Beim Erstellen von Diagnoseeinstellungen werden Protokolle/Metriken aus Anzeigebefehlen nicht akzeptiert ([#2913](https://github.com/Azure/azure-cli/issues/2913))

### <a name="network"></a>Netzwerk

* Hinzufügen des `network watcher test-connectivity`-Befehls
* Hinzufügen von Unterstützung für den `--filters`-Parameter für `network watcher packet-capture create`
* Hinzufügen von Unterstützung für den Application Gateway-Verbindungsausgleich
* Hinzufügen von Unterstützung für die Konfiguration von Application Gateway-WAF-Regelsätzen
* Hinzufügen von Unterstützung für ExpressRoute-Routenfilter und -Regeln
* Hinzufügen von Unterstützung für geografisches TrafficManager-Routing
* Hinzufügen von Unterstützung für richtlinienbasierte Datenverkehrsselektoren für VPN-Verbindungen
* Hinzufügen von Unterstützung für IPSec-Richtlinien für VPN-Verbindungen
* Korrektur eines Fehlers bei `vpn-connection create` bei Verwendung der Parameter `--no-wait` oder `--validate`
* Hinzufügen von Unterstützung für Aktiv/Aktiv-VNET-Gateways
* Entfernen von NULL-Werten aus der Ausgabe von `network vpn-connection list/show`-Befehlen
* BC: Korrektur eines Fehlers in der Ausgabe von `vpn-connection create`
* Korrektur eines Fehlers, bei dem das Argument „--key-length“ von „vpn-connection create“ nicht ordnungsgemäß analysiert wurde
* Korrektur eines Fehlers in `dns zone import`, bei dem Datensätze nicht ordnungsgemäß importiert wurden
* Korrektur eines Fehlers, bei dem `traffic-manager endpoint update` nicht funktionierte
* Hinzufügen von Network Watcher-Vorschaubefehlen

### <a name="profile"></a>Profil

* Unterstützung der Anmeldung, wenn keine Abonnements gefunden werden ([#2560](https://github.com/Azure/azure-cli/issues/2560))
* Unterstützung für kurze Parameternamen in „az account set --subscription“ ([#2980](https://github.com/Azure/azure-cli/issues/2980))

### <a name="redis"></a>Redis

* Hinzufügen des Updatebefehls, durch den auch die Möglichkeit zum Skalieren für Redis Cache hinzugefügt wird
* Verwerfen des Befehls „update-settings“

### <a name="resource"></a>Resource

* Hinzufügen der Befehle „managedapp“ und „managedapp definition“ ([#2985](https://github.com/Azure/azure-cli/issues/2985))
* Unterstützung für die „provider operation“-Befehle ([#2908](https://github.com/Azure/azure-cli/issues/2908))
* Unterstützung für die Erstellung generischer Ressourcen ([#2606](https://github.com/Azure/azure-cli/issues/2606))
* Korrigieren der Ressourcenanalyse und der API-Versionssuche ([#2781](https://github.com/Azure/azure-cli/issues/2781))
* Hinzufügen von Dokumenten für „az lock update“ ([#2702](https://github.com/Azure/azure-cli/issues/2702))
* Beenden mit Fehler bei dem Versuch, Ressourcen für eine nicht vorhandene Gruppe aufzulisten ([#2769](https://github.com/Azure/azure-cli/issues/2769))
* [Compute] Beheben von Problemen mit dem Update von VMSS- und VM-Verfügbarkeitsgruppen ([#2773](https://github.com/Azure/azure-cli/issues/2773))
* Korrigieren des Erstellungs- und Löschvorgangs für Sperren, wenn „parent-resource-path“ auf „None“ festgelegt ist ([#2742](https://github.com/Azure/azure-cli/issues/2742))

### <a name="role"></a>Role

* create-for-rbac: Sicherstellen, dass das SP-Enddatum nicht das Ablaufdatum des Zertifikats überschreitet ([#2989](https://github.com/Azure/azure-cli/issues/2989))
* RBAC: Hinzufügen vollständiger Unterstützung für „ad group“ ([#2016](https://github.com/Azure/azure-cli/issues/2016))
* Rolle: Beheben von Probleme beim Rollendefinitionsupdate ([#2745](https://github.com/Azure/azure-cli/issues/2745))
* create-for-rbac: Sicherstellen, dass das angegebene Benutzerkennwort übernommen wird

### <a name="sql"></a>SQL

* Hinzufügen der Befehle „az sql server list-usages“ und „az sql db list-usages“
* SQL: Möglichkeit zur direkten Verbindung mit Ressourcenanbieter ([#2832](https://github.com/Azure/azure-cli/issues/2832))

### <a name="storage"></a>Storage

* Festlegen des Ressourcengruppenstandorts als Standardstandort für `storage account create`
* Hinzufügen von Unterstützung für das inkrementelle Kopieren von Blobs
* Hinzufügen von Unterstützung für den Upload umfangreicher Blockblobs
* Ändern der Blockgröße auf 100 MB, wenn die hochzuladende Datei größer als 200 GB ist

### <a name="vm"></a>VM

* avail-set: Festlegen der UD- und FD-Domänenanzahl als optional

  Hinweis: VM-Befehle in unabhängigen Clouds: Vermeiden Sie Features im Zusammenhang mit verwalteten Datenträgern, einschließlich der folgenden:
  1. az disk/snapshot/image
  2. az vm/vmss disk
  3. Verwenden Sie in „az vm/vmss create“ den Befehl „—use-unmanaged-disk“, um verwaltete Datenträger zu vermeiden. Andere Befehle sollten funktionieren.
* vm/vmss: Verbessern des Warnungstexts beim Generieren von SSH-Schlüsselpaaren
* vm/vmss: Unterstützen der Erstellung über ein Marketplace-Image, für das Planinformationen erforderlich sind ([#1209](https://github.com/Azure/azure-cli/issues/1209))


## <a name="april-3-2017"></a>3\. April 2017

Version 2.0.2

In dieser Version wurden die Komponenten ACR, Batch, KeyVault und SQL eingeführt.

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

### <a name="core"></a>Core

* Hinzufügen der Module „acr“, „lab“, „monitor“ und „find“ zur Standardliste
* Anmeldung: Überspringen des fehlerhaften Mandanten ([#2634](https://github.com/Azure/azure-cli/pull/2634))
* Anmeldung: Festlegen des Standardabonnements auf ein Abonnement mit dem Status „Enabled“ ([#2575](https://github.com/Azure/azure-cli/pull/2575))
* Hinzufügen von wait-Befehlen und Unterstützung von „--no-wait“ für mehr Befehle ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* Core: Unterstützen der Anmeldung per Dienstprinzipal mit einem Zertifikat ([#2457](https://github.com/Azure/azure-cli/pull/2457))
* Hinzufügen der Meldung zu fehlenden Vorlagenparametern ([#2364](https://github.com/Azure/azure-cli/pull/2364))
* Unterstützen des Festlegens von Standardwerten für häufig verwendete Argumente, z.B. Standardressourcengruppe, Standardweb und Standard-VM
* Unterstützen der Anmeldung an einem bestimmten Mandanten

### <a name="acs"></a>ACS

* [ACS] Hinzufügen von Unterstützung für die Konfiguration eines ACS-Standardclusters ([#2554](https://github.com/Azure/azure-cli/pull/2554))
* Hinzufügen von Unterstützung der Aufforderung zur Kennworteingabe für SSH-Schlüssel ([#2044](https://github.com/Azure/azure-cli/pull/2044))
* Hinzufügen von Unterstützung für Windows-Cluster ([#2211](https://github.com/Azure/azure-cli/pull/2211))
* Wechseln von der Rolle „Besitzer“ zur Rolle „Mitwirkender“ ([#2321](https://github.com/Azure/azure-cli/pull/2321))

### <a name="appservice"></a>AppService

* appservice: Unterstützung für das Abrufen der externen IP-Adresse für DNS A-Einträge ([#2627](https://github.com/Azure/azure-cli/pull/2627))
* appservice: Unterstützung der Bindung von Platzhalterzertifikaten ([#2625](https://github.com/Azure/azure-cli/pull/2625))
* appservice: Unterstützung von Veröffentlichungsprofilen für Listen ([#2504](https://github.com/Azure/azure-cli/pull/2504))
* AppService: Auslösen der Synchronisierung der Quellcodeverwaltung nach der Konfiguration ([#2326](https://github.com/Azure/azure-cli/pull/2326))

### <a name="datalake"></a>DataLake

* Erste Version des Data Lake Analytics-Moduls
* Erste Version des Data Lake Store-Moduls

### <a name="docuemntdb"></a>DocumentDB

* DocumentDB: Hinzufügen von Unterstützung für das Auflisten von Verbindungszeichenfolgen ([#2580](https://github.com/Azure/azure-cli/pull/2580))

### <a name="vm"></a>VM

* [Compute] Hinzufügen von AppGateway-Unterstützung für Erstellung von VM-Skalierungsgruppen ([#2570](https://github.com/Azure/azure-cli/pull/2570))
* [VM/VMSS] Verbesserte Unterstützung für die Datenträgerzwischenspeicherung ([#2522](https://github.com/Azure/azure-cli/pull/2522))
* VM/VMSS: Einbinden der vom Portal verwendeten Logik zur Überprüfung von Anmeldeinformationen ([#2537](https://github.com/Azure/azure-cli/pull/2537))
* Hinzufügen von wait-Befehlen und Unterstützung für „--no-wait“ ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* VM-Skalierungsgruppe: Unterstützung von „*“ zum Auflisten der übergreifenden Instanzansicht für VMs ([#2467](https://github.com/Azure/azure-cli/pull/2467))
* Hinzufügen – Geheimnisse für virtuellen Computer und VM-Skalierungsgruppe ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))
* Zulassen der VM-Erstellung mit spezialisierter VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))

## <a name="february-27-2017"></a>27. Februar 2017

Version 2.0.0

Diese Version der Azure CLI 2.0 ist die erste „allgemein verfügbare“ Version. Die allgemeine Verfügbarkeit gilt für die folgenden Befehlsmodule:
- Container Service (acs)
- Compute (einschließlich Resource Manager, VM, VM-Skalierungsgruppen, Managed Disks)
- Netzwerk
- Storage

Diese Befehlsmodule können in der Produktion verwendet werden und verfügen über Unterstützung durch eine Standard-SLA von Microsoft. Sie können Anfragen zu Problemen direkt beim Microsoft-Support oder in der [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/) öffnen. Sie haben die Möglichkeit, Fragen in [StackOverflow mit dem Tag „azure-cli“](http://stackoverflow.com/questions/tagged/azure-cli) zu stellen oder sich unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) an das Produktteam zu wenden. Außerdem können Sie über die Befehlszeile mit dem Befehl `az feedback` Feedback senden.

Die Befehle in diesen Modulen sind stabil, und es ist nicht zu erwarten, dass sich die Syntax in den anstehenden Veröffentlichungen dieser Version der Azure CLI ändern.

Verwenden Sie zum Überprüfen der Version der CLI den Befehl `az --version`. In der Ausgabe werden die Version der CLI selbst (für diese Veröffentlichung 2.0.0), die einzelnen Befehlsmodule und die von Ihnen genutzten Versionen von Python und GCC aufgeführt.

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
> Einige Befehlsmodule verfügen über das Postfix „b*n*“ oder „rc*n*“. Diese Befehlsmodule befinden sich noch in der Vorschauphase und werden später die allgemeine Verfügbarkeit erlangen.

Außerdem werden jeden Abend Vorschaubuilds der CLI bereitgestellt. Informationen hierzu finden Sie in der [Anleitung zum Abrufen der abendlichen Builds](https://github.com/Azure/azure-cli#nightly-builds) und im Abschnitt zum [Setup für Entwickler und Beitragen von Code](https://github.com/Azure/azure-cli#developer-setup).

Sie können für die abendlichen Vorschaubuilds wie folgt Probleme melden:
- Über die [GitHub-Liste mit Problemen](https://github.com/azure/azure-cli/issues/)
- Per Kontaktaufnahme mit dem Produktteam unter [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)
- Senden von Feedback über die Befehlszeile mit dem Befehl `az feedback`

# <a name="beta-release-notes"></a>[Versionshinweise zur Betaversion](#tab/azure-cli-beta)

Die Azure CLI-Betaversion ist eine Migration der Authentifizierungsmethode der AAD-Plattform (v1.0) zu [Microsoft Identity Platform (v2.0)](/azure/active-directory/develop/v2-overview).

## <a name="june-23-2020"></a>23. Juni 2020

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a>Wissenswertes über die neue Azure CLI-Betaversion

-   Die Betaversion der Azure CLI unterstützt alle CLI-Befehle, die in der aktuellen veröffentlichten Version verfügbar sind.
-   Nach der Installation der Betaversion ist eine erneute Anmeldung erforderlich.
-   Die Betaversion unterstützt nur die Windows-Plattform.
-   Azure Stack wird nicht unterstützt.
-   Parameter `--use-cert-sn-issuer` wird nicht unterstützt, wenn für die Authentifizierung ein Dienstprinzipalschlüssel verwendet wird.
-   Das Überspringen der SSL-Überprüfung über die Umgebung `ADAL_PYTHON_SSL_NO_VERIFY` wird nicht unterstützt.

Sollten Probleme in der Betaversion auftreten, können Sie auf [GitHub](https://github.com/Azure/azure-cli/issues/new/choose) gerne Kommentare für das Azure CLI-Entwicklungsteam hinterlassen.

---

---
title: Dienstübergreifende Links für das Arbeiten mit der Azure CLI
description: Links zu beliebten Tutorials, Schnellstarts, Beispielen, Konzepten und Schrittanleitungen, Azure CLI, VMs, Azure Kubernetes Service (AKS), Batch, Azure CLI (Core), Azure Resource Manager, Key Vault, Azure Stack Hub, Functions, Datenbank, Event Hubs, App Configuration, App Config, Deutschland, Sicherheit, Governance, Insights, IoT, Internet der Dinge, DevOps, Virtual Network, Compute, Networking, Entwicklertools, Datenbanken, Analytics, Verwaltung und Governance, Hybrid, Storage, Sicherheit, KI, KI und Machine Learning, Linux, Windows, Ubuntu, Automatisierung, Anwendung, Web-App, Skript
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 03/01/2020
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 42e9de630530568a15bc6f9f05d2442d790d8b68
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/09/2020
ms.locfileid: "89563143"
---
# <a name="popular-articles-using-the-azure-cli"></a>Beliebte Artikel zur Azure CLI

Die Azure CLI wird in vielen Azure-Diensten verwendet, was dazu führt, dass Artikel in verschiedenen Dokumentrepositorys verteilt werden.  Diese Seite enthält Links zu ausgewählten beliebten Artikeln.  

## <a name="compute"></a>Compute

| | | | |
|-|-|-|-|
|Virtual Machines | Tutorial: Linux | [Erstellen einer Linux-VM mit der Azure CLI](azure-cli-vm-tutorial.yml) | Erstellen Sie eine VM.  Erfahren Sie mehr über Ausgabeabfragen und das Festlegen von Umgebungsvariablen.
|Virtual Machines | Schnellstart: Linux | [Erstellen eines virtuellen Linux-Computers mit der Azure CLI](/azure/virtual-machines/linux/quick-create-cli) | Erstellen Sie eine Linux-VM, und stellen Sie sie bereit.  Öffnen Sie einen Port für Webdatenverkehr, und installieren Sie einen Webserver.
|Virtual Machines | Schrittanleitung: Linux |[Erstellen eines Linus-Images einer VM oder einer VHD](/azure/virtual-machines/linux/capture-image) | Heben Sie die Bereitstellung einer vorhandenen VM auf, erstellen Sie ein Image, und erstellen Sie eine neue VM aus dem erfassten Image.
|Virtual Machines | Schrittanleitung: Linux | [Hochladen einer VHD in Azure mithilfe der Azure CLI](/azure/virtual-machines/linux/disks-upload-vhd-to-managed-disk-cli) | Erstellen Sie einen leeren verwalteten Datenträger, laden Sie Ihre lokale VHD-Datei hoch, und kopieren Sie einen verwalteten Datenträger.
|Virtual Machines | Schrittanleitung: Linux | [Erstellen eines Katalogs mit freigegebenen Images mit der Azure-Befehlszeilenschnittstelle](/azure/virtual-machines/linux/shared-images) | Erstellen Sie eine Shared Image Gallery-Instanz benutzerdefinierter VM-Images mit anderen Personen in Ihrer Organisation, innerhalb einer Region, regionsübergreifend oder innerhalb eines Azure Active Directory-Mandanten.
|Virtual Machines | Schrittanleitung: Linux | [Vorschau: Bereitstellen von Spot-VMs mithilfe der Azure-Befehlszeilenschnittstelle](/azure/virtual-machines/linux/spot-cli) | Stellen Sie eine Linux-Spot-VM bereit, die nicht basierend auf dem Preis entfernt wird.
|Virtual Machines | Schnellstart: Windows | [Schnellstart: Erstellen eines virtuellen Windows-Computers mit der Azure-Befehlszeilenschnittstelle](/azure/virtual-machines/windows/quick-create-cli) | Stellen Sie eine VM in Azure bereit, auf der Windows Server 2016 ausgeführt wird.
|Virtual Machines | Lernmodul | [Verwalten von virtuellen Computern mit der Azure CLI](https://docs.microsoft.com/learn/modules/manage-virtual-machines-with-azure-cli/) | Erstellen, starten und beenden Sie zusätzliche Verwaltungsaufgaben im Zusammenhang mit VMs, und führen Sie diese Aufgaben aus.
|Azure Kubernetes Service (AKS)| Schnellstart | [Schnellstart: Bereitstellen eines AKS-Clusters (Azure Kubernetes Service) über die Azure-Befehlszeilenschnittstelle](/azure/aks/kubernetes-walkthrough) | Stellen Sie AKS-Cluster bereit, und verwalten Sie diese.  Erfahren Sie, wie Sie den Zustand des Clusters und der Pods überwachen können, in denen Ihre Anwendung ausgeführt wird.
|Azure Batch|Beispiel | [CLI-Beispiel: Ausführen eines Auftrags und von Aufgaben mit Azure Batch](/azure/batch/scripts/batch-cli-sample-run-job) | Erstellen Sie einen Batch-Auftrag, und fügen Sie dem Auftrag eine Reihe von Aufgaben hinzu. Überwachen Sie einen Auftrag und die zugehörigen Aufgaben.
|Azure Batch|Beispiel | [CLI-Beispiel: Erstellen und Verwalten eines Windows-Pools in Azure Batch](/azure/batch/scripts/batch-cli-sample-manage-windows-pool) | Erstellen und verwalten Sie einen Pool von Windows-Computeknoten mit einer Cloud Services-Konfiguration.
|Azure Container Instances|Schnellstart | [Schnellstart: Bereitstellen einer Containerinstanz in Azure mithilfe der Azure-Befehlszeilenschnittstelle](/azure/container-instances/container-instances-quickstart) | Stellen Sie mithilfe der Azure CLI einen isolierten Docker-Container bereit, und machen Sie seine Anwendung über einen vollqualifizierten Domänennamen (Fully Qualified Domain Name, FQDN) verfügbar. Führen Sie einen einzigen Bereitstellungsbefehl aus, und navigieren Sie dann zur ausgeführten Anwendung im Container.
|Azure Function|Schnellstart |  [Schnellstart: Erstellen einer Funktion in Azure, die auf HTTP-Anforderungen antwortet](/azure/azure-functions/functions-create-first-azure-function-azure-cli) | Verwenden Sie Befehlszeilentools zum Erstellen einer Funktion, die auf HTTP-Anforderungen antwortet. Nachdem Sie den Code lokal getestet haben, stellen Sie die Funktion in der serverlosen Umgebung von Azure Functions bereit.

## <a name="networking"></a>Netzwerk

| | | | |
|-|-|-|-|
|Virtual Network|Schnellstart | [Erstellen eines virtuellen Netzwerks über die Azure-Befehlszeilenschnittstelle](/azure/virtual-network/quick-create-cli) | Erstellen Sie ein virtuelles Netzwerk, stellen Sie zwei VMs im virtuellen Netzwerk bereit, und stellen Sie über das Internet eine Verbindung mit den VMs her.
|Virtual Network|Schrittanleitung | [Erstellen eines virtuellen Linux-Computers mit beschleunigtem Netzwerkbetrieb mithilfe der Azure CLI](/azure/virtual-network/create-vm-accelerated-networking-cli) | Erstellen Sie eine Linux-VM, verwalten Sie die dynamische Bindung und die Sperrung der virtuellen Funktion, und aktivieren Sie den beschleunigten Netzwerkbetrieb.

## <a name="internet-of-things"></a>Internet der Dinge

| | | | |
|-|-|-|-|
|IoT Hub|Lernprogramm | [Tutorial: Verwenden der Azure CLI zum Konfigurieren des IoT Hub-Nachrichtenroutings](/azure/iot-hub/tutorial-routing) | Richten Sie benutzerdefinierte Routingabfragen mit IoT Hub ein, und verwenden Sie diese.

## <a name="developer-tools"></a>Entwicklertools

| | | | |
|-|-|-|-|
|Azure App Configuration|Beispiele |[Azure CLI-Beispiele für Azure App Configuration](/azure/azure-app-configuration/cli-samples) | Hier finden Sie Links zu Bash-Skripts, die die Azure CLI für Azure App Configuration verwenden.
|Azure DevOps| Erste Schritte: DevOps-Pipeline |[Erstellen Ihrer ersten Azure-Pipeline mit der Azure CLI](/azure/devops/pipelines/create-first-pipeline-cli) | Erstellen Sie eine neue Pipeline in einem geklonten GitHub-Verzeichnis, und verwalten und führen Sie Ihre Pipelines aus.
|Azure DevOps| Schrittanleitung: DevOps-Pipeline |[Bereitstellungsaufgaben der Azure-Pipeline unter Verwendung der Azure CLI](/azure/devops/pipelines/tasks/deploy/azure-cli?view=azure-devops) | Führen Sie in einer Build- oder Releasepipeline ein Shell- oder Batch-Skript aus, das die Azure CLI enthält.  Befehle werden auf plattformübergreifenden Agents ausgeführt, die wiederum unter Linux, macOS oder Windows ausgeführt werden.
|Azure DevOps| Tutorial: Jenkins-Pipeline |[Bereitstellen an Azure App Service mit Jenkins und der Azure CLI](/azure/jenkins/execute-cli-jenkins-pipeline) | Erstellen und konfigurieren Sie eine Jenkins-VM, erstellen Sie eine Web-App in Azure, und bereiten Sie ein GitHub-Repository vor.  Erstellen Sie die Jenkins-Pipeline, und führen Sie sie aus.

## <a name="databases"></a>Datenbanken

| | | | |
|-|-|-|-|
|SQL-Datenbank| Beispiel |[Azure CLI-Beispiele für Azure SQL-Datenbank](/azure/sql-database/sql-database-cli-samples?tabs=single-database) | Azure CLI-Beispiele für Azure SQL-Datenbank
|MySQL|Schnellstart |[Erstellen eines Azure Database for MySQL-Servers mithilfe der Azure CLI](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli) | Erstellen eines Azure-Datenbank für MySQL-Servers  Konfigurieren Sie eine Firewallregel und SSL-Einstellungen.  Rufen Sie Datenbankverbindungsinformationen ab, und verwenden Sie diese.
|Cosmos DB |Schrittanleitung |[Verwalten von Azure Cosmos-Ressourcen mit der Azure CLI](/azure/cosmos-db/manage-with-cli) | Verwenden Sie gängige Befehle zum Automatisieren der Verwaltung Ihrer Azure Cosmos DB-Konten und -Container.
|Cosmos DB |Beispiel |[Azure CLI-Beispiele für Azure Cosmos DB: SQL-API (Core-API)](/azure/cosmos-db/cli-samples) | Rufen Sie Links zu Azure CLI-Beispielskripts für die Azure Cosmos DB-SQL-API (Core) ab.

## <a name="analytics"></a>Analytics

| | | | |
|-|-|-|-|
Azure Event Hub |Schnellstart |[Schnellstart: Erstellen eines Event Hubs mithilfe der Azure CLI](/azure/event-hubs/event-hubs-quickstart-cli) | Erstellen Sie einen Event Hubs-Namespace und einen Event Hub.
HDInsight |Leitfaden |[Erstellen von HDInsight-Clustern mit der Azure-Befehlszeilenschnittstelle](/azure/hdinsight/hdinsight-hadoop-create-linux-clusters-azure-cli) | Erstellen Sie einen HDInsight 3.6-Cluster.
HDInsight |Lernprogramm |[Verwalten von Azure HDInsight-Clustern mit der Azure-Befehlszeilenschnittstelle](/azure/hdinsight/hdinsight-administer-use-command-line) | Listen Sie HDInsight-Cluster auf, zeigen Sie sie an, und löschen und skalieren Sie sie.

## <a name="management-and-governance"></a>Verwaltung und Governance

| | | | |
|-|-|-|-|
Resource Manager-Vorlagen |Schrittanleitung |[Bereitstellen von Ressourcen mit Azure Resource Manager-Vorlagen und Azure-CLI](/azure/azure-resource-manager/templates/deploy-cli) | Stellen Sie Ihre Ressourcen mithilfe von Vorlagen in Azure bereit.
Resource Manager-Gruppen |Schrittanleitung |[Verwalten von Azure Resource Manager-Gruppen mithilfe der Azure CLI](/azure/azure-resource-manager/management/manage-resource-groups-cli) | Verwenden Sie Azure Resource Manager, um Ihre Azure Resource Manager-Gruppen zu verwalten.
Resource Graph |Schnellstart |[Schnellstart: Ausführen Ihrer ersten Resource Graph-Abfrage mithilfe der Azure CLI](/azure/governance/resource-graph/first-query-azurecli) | Fügen Sie Ihrer installierten Azure CLI-Instanz Azure Resource Graph hinzu, und führen Sie Ihre erste Resource Graph-Abfrage aus.
Richtlinienzuweisung |Schnellstart |[Schnellstart: Erstellen einer Richtlinienzuweisung zum Identifizieren nicht konformer Ressourcen mit Azure CLI](/azure/governance/policy/assign-policy-azurecli) | Erstellen Sie eine Richtlinienzuweisung zur Identifizierung von VMs, die keine verwalteten Datenträger verwenden.

## <a name="hybrid"></a>Hybrid

| | | | |
|-|-|-|-|
Azure Stack Hub| Schnellstart: Linux-VM |[Schnellstart: Erstellen eines virtuellen Linux-Servers mithilfe der Azure CLI in Azure Stack Hub](/azure-stack/user/azure-stack-quick-create-vm-linux-cli) | Erstellen Sie eine Ubuntu Server 16.04 LTS-VM, stellen Sie über einen Remoteclient eine Verbindung mit der VM her, und installieren Sie einen NGINX-Webserver.
Azure Stack Hub| Schnellstart: Windows-VM |[Schnellstart: Erstellen eines virtuellen Windows Server-Computers mithilfe der Azure CLI in Azure Stack Hub](/azure-stack/user/azure-stack-quick-create-vm-windows-cli) |Erstellen Sie eine Windows Server 2016-VM, stellen Sie über einen Remoteclient eine Verbindung mit der VM her, und installieren Sie den IIS-Webserver.
Azure Stack Hub| Schrittanleitung: ASDK-Ressourcen |[Verwalten und Bereitstellen von Ressourcen in Azure Stack Hub mit der Azure CLI](/azure-stack/user/azure-stack-version-profiles-azurecli2) | Richten Sie die Azure CLI zum Verwalten von ASDK-Ressourcen (Azure Stack Development Kit) über Linux-, Mac- und Windows-Clientplattformen ein.

## <a name="storage"></a>Storage

| | | | |
|-|-|-|-|
Blob Storage |Schnellstart |  [Erstellen, Hochladen, Herunterladen und Auflisten von Blobs über die Azure CLI](/azure/storage/blobs/storage-quickstart-blobs-cli) | Laden Sie Dateien in Azure Blob Storage hoch und aus Azure Blob Storage herunter.
Blob Storage |Schrittanleitung |[Autorisieren des Zugriffs auf Blob- oder Warteschlangendaten mit der Azure CLI](/azure/storage/common/authorize-data-operations-cli) | Geben Sie an, wie Datenvorgänge autorisiert werden, und legen Sie Umgebungsvariablen für Parameter fest.
Blob Storage |Schrittanleitung |[Verwenden der Azure CLI zum Verwalten von Verzeichnissen, Dateien und Zugriffssteuerungslisten in Azure Data Lake Storage Gen2 (Vorschau)](/azure/storage/blobs/data-lake-storage-directory-file-acl-cli) | Erstellen und verwalten Sie Verzeichnisse, Dateien und Berechtigungen in Speicherkonten, die einen hierarchischen Namespace aufweisen.
File Storage |Schnellstart |[Schnellstart: Erstellen, Herunterladen und Auflisten von Blobs mit der Azure-Befehlszeilenschnittstelle](/azure/storage/files/storage-how-to-use-files-cli) | Erstellen und verwenden Sie Azure-Dateifreigaben.  Erstellen und verwalten Sie Freigabemomentaufnahmen.

## <a name="security"></a>Sicherheit

| | | | |
|-|-|-|-|
Dienstprinzipal |Schrittanleitung |[Erstellen eines Azure-Dienstprinzipals mit der Azure-Befehlszeilenschnittstelle](/cli/azure/create-an-azure-service-principal-azure-cli) | Mit der Azure CLI können Sie einen Dienstprinzipal erstellen, Informationen darüber abrufen und ihn zurücksetzen.
RBAC |Schrittanleitung |[Hinzufügen oder Entfernen von Rollenzuweisungen mithilfe von Azure RBAC und der Azure-Befehlszeilenschnittstelle](/azure/role-based-access-control/role-assignments-cli) | Weisen Sie der rollenbasierten Zugriffskontrolle von Azure Rollen zu.
Key Vault |Schrittanleitung |[Verwalten von Key Vault mit der Azure CLI](/azure/key-vault/key-vault-manage-with-cli2) | Erstellen und verwalten Sie eine Azure Key Vault-Instanz.  Registrieren und autorisieren Sie eine Anwendung, legen Sie erweiterte Zugriffsrichtlinien fest, und lernen Sie plattformübergreifende Befehle der Befehlszeilenschnittstelle kennen.
Key Vault |Lernprogramm |[Verwalten von Speicherkontoschlüsseln mit Key Vault und der Azure-Befehlszeilenschnittstelle](/azure/key-vault/key-vault-ovw-storage-keys) | Verwalten Sie Speicherkontoschlüssel, und generieren Sie Token für Shared Acces Signatures.

## <a name="ai--machine-learning"></a>KI und Machine Learning

| | | | |
|-|-|-|-|
Machine Learning |Reference |[Verwenden der Azure CLI-Erweiterung für Azure Machine Learning](/azure/machine-learning/reference-azure-machine-learning-cli) | Führen Sie Experimente durch, um Machine Learning-Modelle zu erstellen und Machine Learning-Modelle für die Nutzung durch Kunden zu registrieren.  Lesen Sie, wie Sie Machine Learning-Modelle packen und bereitstellen und ihren Lebenszyklus nachverfolgen.
Cognitive Services |Leitfaden |[Erstellen einer Cognitive Services-Ressource mithilfe der Azure-Befehlszeilenschnittstelle](/azure/cognitive-services/cognitive-services-apis-create-account-cli) | Registrieren Sie sich für Azure Cognitive Services, und erstellen Sie ein Konto mit einem Abonnement mit einem einzelnen Dienst oder mit mehreren Diensten.  Verwenden Sie die Schlüssel den generierten Endpunkt, die für Sie zum Authentifizieren Ihrer Anwendungen generiert wurden.
Azure Monitor |Schrittanleitung |[Erstellen eines Log Analytics-Arbeitsbereichs mit der Azure CLI](/azure/azure-monitor/learn/quick-create-workspace-cli) | Erstellen Sie einen Log Analytics-Arbeitsbereich, und stellen Sie ihn bereit.

## <a name="geographies"></a>Geografische Regionen

| | | | |
|-|-|-|-|
Azure Deutschland |Erste Schritte |[Herstellen einer Verbindung mit Azure Deutschland über die Azure CLI](/azure/germany/germany-get-started-connect-with-cli) | Verwalten Sie mit Azure Deutschland ein großes Abonnement über Skripts, und greifen Sie auf Funktionen zu, die derzeit nicht im globalen Azure-Portal verfügbar sind.
Azure Government|Erste Schritte |[Herstellen einer Verbindung mit Azure Government über die Azure-Befehlszeilenschnittstelle](/azure/azure-government/documentation-government-get-started-connect-with-cli)|Greifen Sie auf Verwaltungsressourcen in Azure Government zu, und starten Sie diese.

## <a name="see-also"></a>Weitere Informationen

* [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)
* [Vollständige Liste mit Befehlsreferenzen für die Azure CLI](/cli/azure/reference-index)
* [Dienste, die von der Azure CLI verwaltet werden können](azure-services-the-azure-cli-can-manage.md)

---
title: Effektive Verwendung der Azure CLI
description: Dieser Artikel enthält Tipps zur effektiven Verwendung der Azure CLI, und Sie erfahren u. a. mehr über Ausgabeformate, Übergeben von Parameterwerten und Regeln für Anführungszeichen für verschiedene Shells.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 03/19/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: fa0b53da592010211e8378ce7c4c00a3de2122c4
ms.sourcegitcommit: 612554c029ba1f28d3a43fd22e743104a1a30ea0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/07/2021
ms.locfileid: "106876356"
---
# <a name="use-azure-cli-effectively"></a>Effektive Verwendung der Azure CLI

Mit der Azure CLI können Sie Azure über Bash, PowerShell oder ein Eingabeaufforderungsfenster konfigurieren und verwalten. Die Azure CLI unterstützt die Wiederverwendung von Befehlen sowohl auf Ad-hoc-Basis als auch über Skripts. Sie müssen die Funktionen der von Ihnen ausgeführten Shell kennen.

In diesem Artikel werden nützliche Tipps für die Azure CLI sowie zur Vermeidung von Fehlern erläutert.

[!INCLUDE [azure-cli-prepare-your-environment.md](includes/azure-cli-prepare-your-environment.md)]

Wenn Sie Fragen zu einem Azure CLI-Befehl haben, durchsuchen Sie die [Referenz zur Azure CLI](/cli/azure/reference-index).

## <a name="output-formatting"></a>Ausgabeformatierung

Mit vielen Azure CLI-Befehlen werden Ihnen Daten in der Konsole angezeigt. Der Zweck eines Befehls können diese Informationen sein. Dies wird in diesem Beispiel veranschaulicht, in dem mit dem Befehl [az account show](/cli/azure/account#az_account_show) Ihr aktuelles Abonnement angezeigt wird:

```azurecli
az account show
```

Manchmal spiegeln die Informationen, die mit einem Befehl angezeigt werden, die von Ihnen vorgenommenen Änderungen wider. In diesem Beispiel wird mithilfe des Befehls [az group create](/cli/azure/group#az_group_create) eine Ressourcengruppe erstellt:

```azurecli
az group create --name MyResourceGroup --location eastus
```

Wenn Sie diesen Befehl ausführen, wird in der Azure CLI-Konsole die soeben von Ihnen erstellte Ressourcengruppe angezeigt.

Sie können durch Angabe des Parameters `--output` das Format für die Ausgabe auswählen. In diesem Beispiel listet der Befehl [az account list](/cli/azure/account#az_account_list) alle Abonnements, auf die Sie zugreifen können, in einer Tabelle auf:

```azurecli
az account list --output table
```

Hier sehen Sie drei gängige Formate:

* Das `json`-Format zeigt Informationen als JSON-Zeichenfolge an. Dieses Format liefert die umfassendsten Informationen. Dies ist das Standardformat. Sie können das Standardformat mithilfe des Befehls [az configure](/cli/azure/reference-index#az_configure) ändern.
* Das `table`-Format stellt die Ausgabe als für Menschen lesbare Tabelle dar. Sie können angeben, welche Werte in der Tabelle angezeigt werden, und Abfragen verwenden, um die Ausgabe anzupassen.
* Das `tsv`-Format gibt durch Tabstopp oder Zeilenumbruch getrennte Werte ohne zusätzliche Formatierung, Schlüssel oder andere Symbole zurück.

Weitere Informationen zu diesen und anderen Formaten finden Sie unter [Ausgabeformate für Azure CLI-Befehle](format-output-azure-cli.md).

## <a name="pass-values-to-another-command"></a>Übergeben von Werten an einen anderen Befehl

Azure CLI-Befehle werden in einer Shell ausgeführt. In diesem Artikel wird Bash verwendet, es gibt jedoch auch andere Optionen. Sie können die Standardshellsyntax verwenden, um die Nutzung der Azure CLI zu vereinfachen.

Ein Wert kann als Variable gespeichert werden. Variablen ermöglichen es Ihnen, Werte mehrmals zu verwenden oder allgemeinere Skripts zu erstellen. In diesem Beispiel wird einer Variablen eine ID zugewiesen, die mit dem Befehl [az vm list](/cli/azure/vm#az_vm_list) ermittelt wurde.

```azurecli
running_vm_ids=$(az vm list --resource-group MyResourceGroup --show-details \
   --query "[?powerState=='VM running'].id" --output tsv)
```

> [!TIP]
> Verwenden Sie unbedingt den Ausgabetyp `tsv`. Andere Ausgabetypen enthalten unter Umständen unerwünschte Symbole wie Anführungszeichen.

Verwenden Sie den Wert später in Befehlen. Sie können den Wert durch Wiedergeben der Variablen überprüfen.

```azurecli
echo $running_vm_ids
```

Sie können auch einen Wert von einem Befehl an einen anderen übergeben. In diesem Beispiel wird die Bash-Standardsyntax für die Suche nach einem Wert verwendet:

```azurecli
az vm list --query "[?powerState=='VM running'].name" --output tsv | grep my_vm
```

Beachten Sie bei der Verwendung von Azure CLI-Befehlen, wie Ihre Shell Anführungszeichen und Escapezeichen verwendet. Wenn Sie in verschiedenen Shells verwendete Skripts unterstützen, müssen Sie verstehen, wie sich die Shells unterscheiden.

* Bash. [Anführungszeichen](https://www.gnu.org/software/bash/manual/html_node/Quoting.html)
* PowerShell. [Informationen zu Regeln für Anführungszeichen](/powershell/module/microsoft.powershell.core/about/about_quoting_rules)
* Windows-Eingabeaufforderung: [Escapezeichen, Trennzeichen und Anführungszeichen in der Windows-Befehlszeile](https://ss64.com/nt/syntax-esc.html)

> [!NOTE]
> Aufgrund eines bekannten Problems in PowerShell gelten für Escapezeichen einige zusätzliche Regeln. Weitere Informationen finden Sie unter [Probleme mit Anführungszeichen bei PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md).

### <a name="using-hyphen-characters-in-values"></a>Verwenden von Bindestrichen in Werten

Beginnt ein Wert mit einem Bindestrich, versucht die Azure CLI, ihn als Parameternamen zu analysieren. Verwenden Sie Anführungszeichen, um ihn als Wert zu analysieren: `--password="-VerySecret"`.

### <a name="using-quotation-marks-in-values"></a>Verwenden von Anführungszeichen in Werten

Wenn Sie einen Parameter als Wert angeben, der Leerzeichen enthält, schließen Sie ihn in Anführungszeichen ein. Beachten Sie folgende Tipps:

* In Bash oder PowerShell werden sowohl einfache als auch doppelte Anführungszeichen interpretiert. In der Windows-Eingabeaufforderung werden nur doppelte Anführungszeichen interpretiert. Einfache Anführungszeichen werden als Teil des Werts interpretiert.

* Verwenden Sie für reine Bash-Befehle einfache Anführungszeichen, um JSON-Inline-Code zu vereinfachen. Dieser JSON-Code ist beispielsweise in Bash korrekt: `'{"key": "value"}'`. In der Windows-Eingabeaufforderung lautet die Entsprechung `"{\"key\": \"value\"}"`.

* Einige Azure CLI-Befehle verwenden eine Liste mit durch Leerzeichen getrennten Werten. Wenn der Schlüsselname oder -wert Leerzeichen enthält, umschließen Sie das gesamte Paar: `"my key=my value"`.

* Bash wertet doppelte Anführungszeichen in exportierten Variablen aus. Entspricht dieses Verhalten nicht Ihren Vorstellungen, versehen Sie die Variable mit Escapezeichen: `"\$variable"`.

* Es gibt Sonderzeichen in PowerShell, z. B. `@`. Fügen Sie zum Ausführen der Azure CLI in PowerShell `` ` `` als Escapezeichen vor dem Sonderzeichen ein. Stattdessen können Sie den Wert in einfache oder doppelte Anführungszeichen `"`/`"` setzen.

  ```azurecli
  `@parameters.json
  '@parameters.json'
  ```

* Bei Verwendung des Parameters `--query` mit einem Befehl müssen einige Zeichen von [JMESPath](https://jmespath.org/specification.html) in der Shell mit Escapezeichen versehen werden.

  Diese drei Befehle führen in Bash zum gleichen Ergebnis:

  ```azurecli
  az version --query '"azure-cli"'
  az version --query \"azure-cli\"
  az version --query "\"azure-cli\""
  ```

  Diese beiden Befehle führen in der Windows-Eingabeaufforderung zum gleichen Ergebnis:

  ```azurecli
  az version --query "\"azure-cli\""
  az version --query \"azure-cli\"
  ```

  Diese fünf Befehle führen in PowerShell zum gleichen Ergebnis:

  ```azurecli
  az version --query '\"azure-cli\"'
  az version --query "\`"azure-cli\`""
  az version --query "\""azure-cli\"""
  az --% version --query "\"azure-cli\""
  az --% version --query \"azure-cli\"
  ```

## <a name="asynchronous-operations"></a>Asynchrone Vorgänge

Vorgänge in Azure können beträchtliche Zeit in Anspruch nehmen. Die Konfiguration eines virtuellen Computers in einem Rechenzentrum irgendwo auf der Welt erfolgt beispielsweise nicht sofort. Die Azure CLI wartet, bis der Befehl abgeschlossen ist, bevor andere Befehle akzeptiert werden.

In vielen Befehlen kann der Parameter `--no-wait` verwendet werden, der die Ausführung weiterer Befehle ermöglicht. Im folgenden Beispiel wird eine Ressourcengruppe entfernt:

```azurecli
az group delete --name MyResourceGroup --no-wait
```

Beim Entfernen einer Ressourcengruppe werden auch alle dazugehörigen Ressourcen entfernt. Die Freigabe dieser Ressourcen kann sehr lange dauern. Mit dem Parameter `--no-wait` kann die Konsole bei Ausführung dieses Befehls sofort Befehle akzeptieren, auch wenn noch der erste Befehl verarbeitet wird.

Viele Befehle bieten eine Warteoption, mit der die Konsole angehalten wird, bis eine Bedingung erfüllt ist. Im folgenden Beispiel wird der Befehl [az vm wait](/cli/azure/vm#az_vm_wait) verwendet, um das parallele Erstellen unabhängiger Ressourcen zu unterstützen:

```azurecli
az vm create --resource-group VMResources --name virtual-machine-01 --image centos --no-wait
az vm create --resource-group VMResources --name virtual-machine-02 --image centos --no-wait

subscription=$(az account show --query "id" -o tsv)
vm1_id="/subscriptions/$subscription/resourceGroups/VMResources/providers/Microsoft.Compute/virtualMachines/virtual-machine-01"
vm2_id="/subscriptions/$subscription/resourceGroups/VMResources/providers/Microsoft.Compute/virtualMachines/virtual-machine-02"
az vm wait --created --ids $vm1_id $vm2_id
```

Nach der Erstellung der beiden IDs können Sie die Konsole wieder nutzen.

## <a name="work-behind-a-proxy"></a>Verwendung hinter einem Proxy

Wenn Sie die Azure CLI über einen Proxyserver verwenden, kann dies den folgenden Fehler verursachen: `SSLError("bad handshake: Error([('SSL routines', 'tls_process_server_certificate', 'certificate verify failed')],)",)`. Legen Sie zur Behebung dieses Fehlers die Umgebungsvariable `REQUESTS_CA_BUNDLE` auf den Pfad der Bundlezertifikatdatei der Zertifizierungsstelle im PEM-Format fest.

| Betriebssystem                     | Standardbundle der Zertifizierungsstelle                                                  |
|----------------------- |-------------------------------------------------------------------------------------- |
| Windows                | C:\Programme (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\certifi\cacert.pem |
| Ubuntu/Debian Linux    | /opt/az/lib/python3.6/site-packages/certifi/cacert.pem                                |
| CentOS/RHEL/SUSE Linux | /usr/lib64/az/lib/python3.6/site-packages/certifi/cacert.pem                          |

Fügen Sie das Zertifikat des Proxyservers an diese Datei an, oder kopieren Sie den Inhalt in eine andere Zertifikatdatei, und legen Sie anschließend `REQUESTS_CA_BUNDLE` dafür fest. Möglicherweise müssen Sie auch die Umgebungsvariable `HTTP_PROXY` oder `HTTPS_PROXY` festlegen.

Einige Proxys erfordern eine Authentifizierung. Das Format der Umgebungsvariablen `HTTP_PROXY` oder `HTTPS_PROXY` sollte die Authentifizierung beinhalten, etwa `HTTPS_PROXY="https://username:password@proxy-server:port"`. Ausführliche Informationen finden Sie unter [Konfigurieren von Proxys für die Azure-Bibliotheken](/azure/developer/python/azure-sdk-configure-proxy?tabs=bash).

## <a name="concurrent-builds"></a>Gleichzeitige Buildvorgänge

Wenn Sie die Azure CLI auf einem Buildcomputer ausführen, auf dem mehrere Aufträge parallel ausgeführt werden können, werden Zugriffstoken unter Umständen von zwei Buildaufträgen gemeinsam genutzt, die unter demselben Betriebssystembenutzer ausgeführt werden.  Legen Sie zur Vermeidung von Verwechslungen AZURE_CONFIG_DIR auf ein Verzeichnis fest, in dem die Zugriffstoken gespeichert werden.

## <a name="generic-update-arguments"></a>Generische Updateargumente

Azure CLI-Befehlsgruppen enthalten häufig einen update-Befehl. [Azure Virtual Machines](/cli/azure/vm) enthält beispielsweise den Befehl [az vm update](/cli/azure/vm#az_vm_update). Die meisten update-Befehle bieten diese drei generischen Parameter: `--add`, `--set` und `--remove`.

Die Parameter `--set` und `--add` verwenden eine Liste von durch Leerzeichen getrennten Schlüssel-Wert-Paaren: `key1=value1 key2=value2`. Verwenden Sie zum Anzeigen der Eigenschaften, die aktualisiert werden können, einen show-Befehl, etwa [az vm show](/cli/azure/vm#az_vm_show).

```azurecli
az vm show --resource-group VMResources --name virtual-machine-01
```

Sie können eine JSON-Zeichenfolge verwenden, um den Befehl zu vereinfachen. Verwenden Sie beispielsweise den folgenden Wert, um einen neuen Datenträger an einen virtuellen Computer anzufügen:

```azurecli
az vm update --resource-group VMResources --name virtual-machine-01 \
--add storageProfile.dataDisks "{\"createOption\": \"Attach\", \"managedDisk\": 
   {\"id\": 
   \"/subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/yg/providers/Microsoft.Compute/disks/yg-disk\"}, 
   \"lun\": 1}"
```

## <a name="generic-resource-commands"></a>Generische Ressourcenbefehle

Ein Dienst, den Sie verwenden möchten, wird möglicherweise noch nicht von der Azure CLI unterstützt. Sie können die Befehle vom Typ [az resource](/cli/azure/resource) verwenden, um mit diesen Ressourcen zu arbeiten.

Wenn Sie nur create- oder update-Befehle benötigen, verwenden Sie [az deployment group create](/cli/azure/deployment/group#az_deployment_group_create). Arbeitsbeispiele finden Sie unter [Azure-Schnellstartvorlagen](/resources/templates/).

## <a name="rest-api-commands"></a>REST-API-Befehle

Wenn generische update-Argumente und [az resource](/cli/azure/resource) Ihre Anforderungen nicht erfüllen, können Sie den Befehl [az rest](/cli/azure/reference-index#az_rest) verwenden, um die REST-API aufzurufen. Bei dem Befehl wird die Authentifizierung automatisch mit den bereits eingegebenen Anmeldeinformationen durchgeführt und der Header `Content-Type: application/json` festgelegt. Weitere Informationen finden Sie unter [Azure-REST-API-Referenz](/rest/api/azure/).

Dieses Beispiel funktioniert mit der [Microsoft Graph-API](/graph/api/overview?toc=./ref/toc.json). Rufen Sie zum Aktualisieren von Umleitungs-URIs für eine [Anwendung](/graph/api/resources/application) die REST-API zum [Aktualisieren der Anwendung](/graph/api/application-update?tabs=http) auf, wie in diesem Code gezeigt:

```azurecli
# Get the application
az rest --method GET \
    --uri 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001'

# Update `redirectUris` for `web` property
az rest --method PATCH \
    --uri 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001' \
    --body '{"web":{"redirectUris":["https://myapp.com"]}}'
```

## <a name="scripts"></a>Skripts

Verwenden Sie das folgende Windows-Batchskript zum Speichern von IDs in Variablen:

```console
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (
   `az vm list --resource-group VMResources --show-details --query "[?powerState=='VM running'].id" --output tsv`
) DO (
    SET "vm_ids=%%F %vm_ids%"  :: construct the id list
)
az vm stop --ids %vm_ids% :: CLI stops all VMs in parallel
```

Verwenden Sie das folgende Windows PowerShell-Skript zum Speichern von IDs in Variablen:

```powershell
$vm_ids=(az vm list --resource-group VMResources --show-details --query "[?powerState=='VM running'].id" --output tsv)
az vm stop --ids $vm_ids # CLI stops all VMs in parallel
```

Verwenden Sie das folgende Windows-Batchskript zum Durchlaufen einer Liste per Schleifenvorgang:

```console
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (
    `az vm list --resource-group VMResources --show-details --query "[?powerState=='VM running'].id" --output tsv`
) DO (
    ECHO Stopping %%F
    az vm stop --ids %%F
)
```

Verwenden Sie das folgende Windows PowerShell-Skript zum Durchlaufen einer Liste per Schleifenvorgang:

```powershell
$vm_ids=(az vm list --resource-group VMResources --show-details --query "[?powerState=='VM running'].id" --output tsv)
foreach ($vm_id in $vm_ids) {
    Write-Output "Stopping $vm_id"
    az vm stop --ids $vm_id
}
```

Nachfolgend sind Azure CLI-Umgebungsvariablen aufgeführt:

|  Umgebungsvariable          | BESCHREIBUNG            |
|--------------------------------|------------------------|
| **AZURE_CONFIG_DIR**           | Das globale Verzeichnis für Konfigurationsdateien, Protokolle und Telemetriedaten. Wenn keine Angabe erfolgt, wird dieser Wert standardmäßig auf `~/.azure.` festgelegt. |
| **AZURE_EXTENSION_DIR**        | Das Verzeichnis mit Erweiterungsinstallationen. Wenn keine Angabe erfolgt, wird für diesen Wert standardmäßig das Unterverzeichnis `cliextensions` innerhalb des globalen Konfigurationsverzeichnisses verwendet. |

## <a name="next-steps"></a>Nächste Schritte

* [Angeben von Werten in Azure CLI-Befehlen](azure-cli-variables.md)
* [Abfragen der Azure CLI-Befehlsausgabe](query-azure-cli.md)
* [Ausgabeformate für Azure CLI-Befehle](format-output-azure-cli.md)
* [Verwenden von Azure-Abonnements mit der Azure CLI](manage-azure-subscriptions-azure-cli.md)

---
title: Tipps für die effektive Verwendung der Azure CLI
description: Tipps für die effektive Verwendung der Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/07/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 720e0866b97db0d56417db95f2518d5567836571
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/09/2020
ms.locfileid: "89563058"
---
# <a name="tips-for-using-azure-cli-effectively"></a>Tipps für die effektive Verwendung der Azure CLI

Aus Gründen der Übersichtlichkeit werden Bash-Skripts inline verwendet. Windows-Batch- bzw. PowerShell-Beispiele, mit denen Sie ähnliche Beispiele erstellen können, sind im Anhang angegeben.

## <a name="output-formatting-json-table-or-tsv"></a>Ausgabeformatierung (JSON, TABLE oder TSV)

1. Das Format `json` ist die Standardeinstellung der CLI und dafür ausgelegt, Ihnen die umfassendsten Informationen zu liefern. Falls Sie ein anderes Format vorziehen, sollten Sie das Argument `--output` verwenden, um einen einzelnen Befehlsaufruf außer Kraft zu setzen. Sie können auch `az configure` verwenden, um Ihre globale Standardeinstellung zu aktualisieren. Beachten Sie hierbei, dass beim JSON-Format die doppelten Anführungszeichen beibehalten werden. Dies bedeutet im Allgemeinen, dass das Format für Skripterstellungszwecke nicht geeignet ist.

2. Das Format `table` ist nützlich, um eine Zusammenfassung der gewünschten Informationen zu erhalten. Dies gilt besonders für Auflistungsbefehle. Falls Ihnen die Felder im Standardtabellenformat nicht zusagen (oder kein Standardformat vorhanden ist), können Sie mit `--output json` alle Informationen anzeigen oder `--query` verwenden, um das gewünschte Format anzugeben.

    ```sh
    az vm show -g my_rg -n my_vm --query "{name: name, os:storageProfile.imageReference.offer}" -otable
    Name    Os
    ------  ------------
    my_vm   UbuntuServer
    ```

3. `tsv` ist gut für kompakte Ausgaben und Skripterstellungszwecke geeignet. Beim TSV-Format werden doppelte Anführungszeichen entfernt, die im JSON-Format beibehalten werden. Verwenden Sie das Argument `--query`, um das gewünschte Format für TSV anzugeben.

    ```sh
    export vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    az vm stop --ids $vm_ids
    ```

## <a name="pass-values-from-one-command-to-another"></a>Übergeben von Werten von einem Befehl an einen anderen

1. Wenn der Wert mehrmals verwendet wird, sollten Sie ihn einer Variablen zuweisen. Beachten Sie die Verwendung von `-o tsv` im folgenden Beispiel:

    ```sh
    running_vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    ```
2. Erwägen Sie den Einsatz von Piping, wenn der Wert nur einmal verwendet wird:
    ```sh
    az vm list --query "[?powerState=='VM running'].name" | grep my_vm
    ```
3. Berücksichtigen Sie für Listen die folgenden Vorschläge:

   Verwenden Sie eine „for“-Schleife, falls Sie weitere Kontrollen für das Ergebnis benötigen:
    ```sh
    #!/usr/bin/env bash
    for vm in $(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv); do
        echo stopping $vm
        az vm stop --ids $vm
        if [ $? -ne 0 ]; then
            echo "Failed to stop $vm"
            exit 1
        fi
        echo $vm stopped
    done
    ```

    Verwenden Sie alternativ `xargs` und ggf. das Flag `-P`, um die Vorgänge parallel auszuführen und so die Leistung zu verbessern:
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | xargs -I {} -P 10 az vm start --ids "{}"
    ```
    Darüber hinaus verfügt die Azure CLI noch über integrierte Unterstützung für die Verarbeitung von Befehlen mit mehreren parallelen `--ids`, um den gleichen Effekt wie mit „xargs“ zu erzielen. Beachten Sie, dass `@-` zum Abrufen von Werten aus der Pipe verwendet wird:
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | az vm start --ids @-
    ```

## <a name="async-operations"></a>Asynchrone Vorgänge

Bei vielen Befehlen und Gruppen werden `--no-wait`-Flags für die zeitintensiven Vorgänge sowie ein dedizierter `wait`-Befehl verfügbar gemacht. Dies ist für bestimmte Szenarien hilfreich:

1. Bereinigen von Ressourcen, wenn nicht die Bereinigung eines nachfolgenden Vorgangs genutzt wird, z. B. das Löschen einer Ressourcengruppe:
    ```sh
    az group delete -n my_rg --no-wait
    ```
2. Paralleles Erstellen mehrerer unabhängiger Ressourcen. Dies ähnelt dem Erstellen von Threads und dem Durchführen des Beitritts:

    ```sh
    az vm create -g my_rg -n vm1 --image centos --no-wait
    az vm create -g my_rg -n vm2 --image centos --no-wait

    subscription=$(az account show --query "id" -otsv)
    vm1_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm1"
    vm2_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm2"
    az vm wait --created --ids $vm1_id $vm2_id
    ```

## <a name="generic-update-arguments"></a>Generische Updateargumente

Die meisten Updatebefehle in der CLI verfügen über die drei folgenden generischen Argumente: `--add`, `--set` und `--remove`. Diese Argumente sind leistungsfähig, aber häufig nicht so komfortabel wie die stark typisierten Argumente, die in Updatebefehlen normalerweise verwendet werden. Die CLI verfügt zur Steigerung der Benutzerfreundlichkeit über stark typisierte Argumente für die meisten gängigen Szenarien. Falls die gewünschte Eigenschaft aber nicht aufgeführt ist, stellen die generischen Updateargumente häufig eine Lösung dar, ohne dass Sie auf ein neues Release warten müssen.

1. Da die Syntax für generische Updates nicht sehr benutzerfreundlich ist, ist etwas Geduld gefordert.
2. Überprüfen Sie, ob für den Updatebefehl die Gruppe `Generic Update Arguments` verfügbar gemacht wird. Wenn nicht, sollten Sie ein Problem melden. Falls die Gruppe verfügbar ist, können Sie versuchen, sie für das Szenario zu nutzen.
3. Verwenden Sie den Befehl `show` für die gewünschte Ressource, um zu ermitteln, welchen Pfad Sie in den generischen Argumenten angeben sollten. Führen Sie vor dem Ausprobieren von `az vm update` beispielsweise `az vm show` aus, um den richtigen Pfad zu ermitteln. Im Allgemeinen verwenden Sie die Punktsyntax, um auf die Wörterbucheigenschaften zuzugreifen, und Klammern für die Indizierung in Listen.
4. Sehen Sie sich die Arbeitsbeispiele an, um zu beginnen. Gute Beispiele finden Sie unter `az vm update -h`.
5. Für `--set` und `--add` wird eine Liste mit Schlüssel-Wert-Paaren im Format `<key1>=<value1> <key2>=<value2>` verwendet. Verwenden Sie diese zum Erstellen von nicht trivialen Nutzlasten. Falls die Syntax zu unübersichtlich wird, können Sie die Verwendung einer JSON-Zeichenfolge erwägen. Ein Beispiel hierfür ist das Anfügen eines neuen Datenträgers an eine VM:
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks "{\"createOption\": \"Attach\", \"managedDisk\": {\"id\": \"/subscriptions/0b1f6471-1bf0-4dda-aec3-cb9272f09590/resourceGroups/yg/providers/Microsoft.Compute/disks/yg-disk\"}, \"lun\": 1}"
    ```
6. Unter Umständen ist es für Sie auch besser, die `@{file}`-Konvention der CLI zu nutzen, bei der der JSON-Code in eine Datei eingefügt und dann geladen wird. Hierdurch wird der obige Befehl vereinfacht:
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks @~/my_disk.json
    ```

## <a name="generic-resource-commands---az-resource"></a>Generische Ressourcenbefehle: `az resource`

Es kann vorkommen, das für einen Dienst, an dem Sie interessiert sind, keine CLI-Befehlsabdeckung besteht. Sie können die Befehle `az resource create/show/list/delete/update/invoke-action` verwenden, um mit diesen Ressourcen zu arbeiten. Hier sind einige Vorschläge angegeben:
1. Wenn es nur um `create/update` geht, können Sie erwägen, `az group deployment create` zu verwenden. Nutzen Sie [Azure-Schnellstartvorlagen](https://github.com/Azure/azure-quickstart-templates) für Arbeitsbeispiele.
2. Sehen Sie sich die REST-API-Referenz zu den Bereichen Anforderungsnutzlast, URL und API-Version an. Lesen Sie beispielsweise in der Community die Kommentare zum [Erstellen von AppInsights](https://github.com/Azure/azure-cli/issues/5543).

## <a name="rest-api-command---az-rest"></a>REST-API-Befehl: `az rest`

Falls Ihre Anforderungen weder durch generische Updateargumente noch durch `az resource` erfüllt werden, können Sie die REST-API mit dem Befehl `az rest` aufrufen. Hierbei wird die Authentifizierung automatisch mit den bereits eingegebenen Anmeldeinformationen durchgeführt und der Header `Content-Type: application/json` festgelegt.

Dies ist äußerst hilfreich, um die [Microsoft Graph-API](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-1.0) aufzurufen, die von CLI-Befehlen derzeit nicht unterstützt wird ([#12946](https://github.com/Azure/azure-cli/issues/12946)).

Um beispielsweise `redirectUris` für eine [Anwendung](/graph/api/resources/application?view=graph-rest-1.0) aufzurufen, rufen wir die REST-API für die [Updateanwendung](/graph/api/application-update?view=graph-rest-1.0&tabs=http) wie folgt auf:

```sh
# Line breaks for legibility only

# Get the application
az rest --method GET
        --uri 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001'

# Update `redirectUris` for `web` property
az rest --method PATCH
        --uri 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001'
        --body '{"web":{"redirectUris":["https://myapp.com"]}}'
```

Bei Verwendung von `--uri-parameters` für Anforderungen in Form von OData sollten Sie darauf achten, `$` in unterschiedlichen Umgebungen mit Escapezeichen zu versehen: in `Bash` sollte `$` zu `\$` werden, und in `PowerShell` sollte `$` zu `` `$`` werden.

## <a name="quoting-issues"></a>Probleme mit Anführungszeichen

Ein Problem kann sich ergeben, weil die Anführungszeichen und Leerzeichen von der Befehlsshell (Bash, Zsh, Windows-Eingabeaufforderung, PowerShell usw.) interpretiert werden, wenn diese den CLI-Befehl analysiert. Sehen Sie immer in den Dokumenten nach, wenn Sie bei der Nutzung einer Shell unsicher sind:

- Bash: [Anführungszeichen](https://www.gnu.org/software/bash/manual/html_node/Quoting.html)
- PowerShell: [Informationen zu Regeln für Anführungszeichen](/powershell/module/microsoft.powershell.core/about/about_quoting_rules)
    - Aufgrund des bekannten Problems [#1995](https://github.com/PowerShell/PowerShell/issues/1995) von PowerShell gelten für Escapezeichen einige zusätzliche Regeln. Weitere Informationen finden Sie unter [Probleme mit Anführungszeichen bei PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md).
- Windows-Eingabeaufforderung: [Gewusst wie: Escapezeichen, Trennzeichen und Anführungszeichen in der Windows-Befehlszeile](https://ss64.com/nt/syntax-esc.html)

Hier sind einige Vorschläge angegeben, mit denen unerwartete Ergebnisse vermieden werden können:

1. Wenn der Wert Leerzeichen enthält, müssen Sie ihn in Anführungszeichen einschließen.
2. In Bash und Windows PowerShell werden sowohl einfache als auch doppelte Anführungszeichen interpretiert, während in der Windows-Eingabeaufforderung nur doppelte Anführungszeichen verarbeitet werden. Dies bedeutet, dass einzelne Anführungszeichen als Teil des Werts interpretiert werden.
3. Falls Ihr Befehl nur in Bash (oder Zsh) ausgeführt wird, haben einfache Anführungszeichen den Vorteil, dass der darin eingeschlossene Inhalt beibehalten wird. Dies kann sehr hilfreich sein, wenn Sie JSON-Code inline angeben. Beispielsweise funktioniert dies in Bash wie folgt: `'{"foo": "bar"}'`
4. Wenn Ihr Befehl über die Windows-Eingabeaufforderung ausgeführt wird, müssen Sie ausschließlich doppelte Anführungszeichen verwenden. Falls der Wert doppelte Anführungszeichen enthält, müssen Sie ihn mit Escapezeichen versehen: `"i like to use \" a lot"`. Die Entsprechung des obigen Codes für die Eingabeaufforderung lautet: `"{\"foo\": \"bar\"}"`
5. In Bash werden exportierte Variablen ausgewertet, die in doppelten Anführungszeichen stehen. Falls Sie dies nicht wünschen, sollten sie wiederum Escapezeichen der Form `\ ` verwenden, z. B. in `"\$var"`. Sie können auch einfache Anführungszeichen verwenden, z. B. `'$var'`.
6. Für einige CLI-Argumente, z. B. die generischen Updateargumente, wird eine Liste mit durch Leerzeichen getrennten Werten verwendet, z. B. `<key1>=<value1> <key2>=<value2>`. Da für den Schlüsselnamen und -wert eine beliebige Zeichenfolge verwendet werden kann, die unter Umständen Leerzeichen enthält, müssen Anführungszeichen genutzt werden. Umschließen Sie das Paar, und nicht nur den Schlüssel bzw. den Wert. `"my name"=john` ist also nicht richtig. Verwenden Sie stattdessen `"my name=john"`. Beispiel:
    ```sh
    az webapp config appsettings set -g my_rg -n my_web --settings "client id=id1" "my name=john"
    ```
7. Verwenden Sie die `@<file>`-Konvention der CLI für das Laden aus der Datei, um die Interpretationsmechanismen der Shell zu umgehen:
    ```sh
    az ad app create --display-name my-native --native-app --required-resource-accesses @manifest.json
    ```
8. Wenn für ein CLI-Argument angegeben ist, dass eine durch Leerzeichen getrennte Liste akzeptiert wird, sind die folgenden Formate zulässig:
    - `--arg foo bar`: OK. Ohne Anführungszeichen, durch Leerzeichen getrennte Liste
    - `--arg "foo" "bar"`: OK: Mit Anführungszeichen, durch Leerzeichen getrennte Liste
    - `--arg "foo bar"`: NICHT GUT. Dies ist eine Zeichenfolge, die ein Leerzeichen enthält, und keine durch Leerzeichen getrennte Liste.
9. Beim Ausführen von Azure CLI-Befehlen in PowerShell treten Analysefehler auf, wenn die Argumente Sonderzeichen aus PowerShell enthalten, z. B. `@`. Sie können dieses Problem beheben, indem Sie vor dem Sonderzeichen als Escapezeichen `` ` `` einfügen oder das Argument in einfache oder doppelte Anführungszeichen (`'`/`"`) setzen. `az group deployment create --parameters @parameters.json` funktioniert in PowerShell beispielsweise nicht, weil `@` als [Aufteilungssymbol](/powershell/module/microsoft.powershell.core/about/about_splatting) (Splatting) analysiert wird. Zur Behebung können Sie das Argument in `` `@parameters.json`` oder `'@parameters.json'` ändern.
10. Bei Verwendung von `--query` mit einem Befehl müssen einige Zeichen von [JMESPath](https://jmespath.org/specification.html) in der Shell mit Escapezeichen versehen werden. Beispiel in Bash:
    ```sh
    # Wrong, as the dash needs to be quoted in a JMESPath query
    $ az version --query azure-cli
    az version: error: argument --query: invalid jmespath_type value: 'azure-cli'

    # Wrong, as the dash needs to be quoted in a JMESPath query, but quotes are interpreted by Bash
    $ az version --query "azure-cli"
    az version: error: argument --query: invalid jmespath_type value: 'azure-cli'

    # Correct
    $ az version --query '"azure-cli"'
    "2.5.1"

    $ az version --query \"azure-cli\"
    "2.5.1"

    $ az version --query "\"azure-cli\""
    "2.5.1"
    ```

    In der Eingabeaufforderung:
    ```cmd
    > az version --query "\"azure-cli\""
    "2.5.1"

    > az version --query \"azure-cli\"
    "2.5.1"
    ```

    In PowerShell (zusätzliche Escapezeichen erforderlich):
    ```powershell
    > az version --query '\"azure-cli\"'
    "2.5.1"

    > az version --query "\`"azure-cli\`""
    "2.5.1"

    > az version --query "\""azure-cli\"""
    "2.5.1"

    > az --% version --query "\"azure-cli\""
    "2.5.1"

    > az --% version --query \"azure-cli\"
    "2.5.1"
    ```

11. Die beste Möglichkeit zur Behandlung eines Problems mit Anführungszeichen ist die Ausführung des Befehls mit dem Flag `--debug`. Hiermit werden die Argumente, die von der CLI tatsächlich empfangen werden, in [Python-Syntax](https://docs.python.org/3/tutorial/introduction.html#strings) angezeigt. Beispiel in Bash:

    ```sh
    # Wrong, as quotes and spaces are interpreted by Bash
    $ az {"key": "value"} --debug
    Command arguments: ['{key:', 'value}', '--debug']

    # Wrong, as quotes are interpreted by Bash
    $ az {"key":"value"} --debug
    Command arguments: ['{key:value}', '--debug']

    # Correct
    $ az '{"key":"value"}' --debug
    Command arguments: ['{"key":"value"}', '--debug']

    # Correct
    $ az "{\"key\":\"value\"}" --debug
    Command arguments: ['{"key":"value"}', '--debug']
    ```

## <a name="work-behind-a-proxy"></a>Verwendung hinter einem Proxy

Ein Proxy wird in Unternehmensnetzwerken häufig im Hintergrund genutzt oder ist aufgrund von Ablaufverfolgungstools wie Fiddler, mitmproxy usw. vorhanden. Wenn für den Proxy selbstsignierte Zertifikate verwendet werden, wird von der Python-Bibliothek mit den Anforderungen ([Requests](https://github.com/kennethreitz/requests)), die von der CLI genutzt wird, Folgendes ausgelöst: `SSLError("bad handshake: Error([('SSL routines', 'tls_process_server_certificate', 'certificate verify failed')],)",)`. Es gibt zwei Möglichkeiten, diesen Fehler zu behandeln:

1. Legen Sie die Umgebungsvariable `REQUESTS_CA_BUNDLE` auf den Pfad der Bundlezertifikatdatei der Zertifizierungsstelle im PEM-Format fest. Wir empfehlen Ihnen diese Vorgehensweise, wenn Sie die CLI häufig hinter einem Unternehmensproxy verwenden. Die Standardbundledatei der Zertifizierungsstelle, die von der CLI verwendet wird, befindet sich bei Windows unter `C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\certifi\cacert.pem` und bei Linux unter ` /opt/az/lib/python3.6/site-packages/certifi/cacert.pem`. Sie können das Zertifikat des Proxyservers an diese Datei anfügen oder den Inhalt in eine andere Zertifikatdatei kopieren und anschließend `REQUESTS_CA_BUNDLE` dafür festlegen. Beispiel:

    ```
    <Original cacert.pem>

    -----BEGIN CERTIFICATE-----
    <Your proxy's certificate here>
    -----END CERTIFICATE-----
    ```

   Es wird häufig gefragt, ob die Umgebungsvariablen `HTTP_PROXY` bzw. `HTTPS_PROXY` festgelegt werden sollten. Die Antwort ist, dass dies vom jeweiligen Fall abhängt. Bei Verwendung von Fiddler unter Windows fungiert die Anwendung beim Start standardmäßig als Systemproxy, sodass Sie nichts festlegen müssen. Wenn die Option deaktiviert ist oder wenn Sie andere Tools verwenden, die nicht als Systemproxy fungieren, sollten Sie die Variablen festlegen. Da fast der gesamte Datenverkehr von der CLI SSL-basiert ist, sollte nur `HTTPS_PROXY` festgelegt werden. Falls Sie unsicher sind, können Sie auch einfach beide Variablen festlegen. Denken Sie aber daran, dies rückgängig zu machen, nachdem der Proxy heruntergefahren wurde. Der Standardwert für Fiddler ist `http://localhost:8888`.

   Weitere Informationen finden Sie im [Blog von Stefan](https://blog.jhnr.ch/2018/05/16/working-with-azure-cli-behind-ssl-intercepting-proxy-server/).

2. Deaktivieren Sie die Zertifikatüberprüfung für die gesamte Azure CLI, indem Sie die Umgebungsvariable `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION=1` festlegen. Dies ist nicht sicher, aber für kurze Einsätze trotzdem gut geeignet, z. B. die Erfassung einer Netzwerkablaufverfolgung für einen bestimmten Befehl und die sofortige Deaktivierung nach Abschluss des Vorgangs. Aufgrund von zugrunde liegenden Einschränkungen des SDK funktioniert dies unter Umständen für einige Datenebenenbefehle nicht.

## <a name="concurrent-builds"></a>Gleichzeitige Buildvorgänge

Wenn Sie „az“ auf einem Buildcomputer verwenden und mehrere Aufträge parallel ausgeführt werden können, besteht das Risiko, dass die Anmeldetoken für zwei Buildaufträge gemeinsam verwendet werden, falls die Aufträge mit demselben Betriebssystembenutzer ausgeführt werden.  Legen Sie zur Vermeidung von Verwechslungen dieser Art AZURE_CONFIG_DIR auf ein Verzeichnis fest, in dem die Anmeldetoken gespeichert werden sollen.  Hierbei kann es sich um einen zufällig erstellten Ordner oder einfach um den Namen des Jenkins-Arbeitsbereichs handeln, z. B. ```AZURE_CONFIG_DIR=.```.

## <a name="appendix"></a>Anhang

### <a name="windows-batch-scripts-for-saving-to-variables-and-using-it-later"></a>Windows-Batchskripts für die Speicherung in Variablen und die spätere Verwendung

```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    SET "vm_ids=%%F %vm_ids%"  :: construct the id list
)
az vm stop --ids %vm_ids% :: CLI stops all VMs in parallel
```

### <a name="windows-powershell-scripts-for-saving-to-variables-and-using-it-later"></a>Windows PowerShell-Skripts für die Speicherung in Variablen und die spätere Verwendung

```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
az vm stop --ids $vm_ids # CLI stops all VMs in parallel
```

### <a name="windows-batch-scripts-to-loop-through-a-list"></a>Windows-Batchskripts zum Durchlaufen einer Liste per Schleifenvorgang
```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    ECHO Stopping %%F
    az vm stop --ids %%F
)
```

### <a name="windows-powershell-scripts-to-loop-through-a-list"></a>Windows PowerShell-Skripts zum Durchlaufen einer Liste per Schleifenvorgang
```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
foreach ($vm_id in $vm_ids) {
    Write-Output "Stopping $vm_id"
    az vm stop --ids $vm_id
}
```

### <a name="cli-environment-variables"></a>CLI-Umgebungsvariablen

|  Umgebungsvariable          | BESCHREIBUNG            |
|--------------------------------|------------------------|
| **AZURE_CONFIG_DIR**           | Globales Konfigurationsverzeichnis für Konfigurationsdateien, Protokolle und Telemetriedaten. Wenn nichts angegeben wird, wird standardmäßig `~/.azure` verwendet. |
| **AZURE_EXTENSION_DIR**        | Installationsverzeichnis für Erweiterungen. Wenn nichts angegeben wird, wird standardmäßig das Verzeichnis `cliextensions` im globalen Konfigurationsverzeichnis verwendet. |

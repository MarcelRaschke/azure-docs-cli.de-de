---
title: Ausgabeformate für die Azure CLI
description: Erfahren Sie, wie Sie die Ausgabe von Azure CLI-Befehlen in Tabellen, Listen oder JSON-Code formatieren.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/23/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 7bc31ba89234dbdb7b939f3a09886f31184ac65f
ms.sourcegitcommit: 18973ac471bbd12af2c8f8fa32a233b0abe5b020
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/13/2020
ms.locfileid: "75913551"
---
# <a name="output-formats-for-azure-cli-commands"></a>Ausgabeformate für Azure CLI-Befehle

Die Azure CLI verwendet JSON als Standardausgabeformat, aber es sind auch andere Formate möglich.  Verwenden Sie den Parameter `--output` (`--out` oder `-o`) zum Formatieren der CLI-Ausgabe. Die Argumentwerte und Typen der Ausgabe lauten wie folgt:

--output | BESCHREIBUNG
---------|-------------------------------
`json`   | JSON-Zeichenfolge. Dies ist die Standardeinstellung.
`jsonc`  | Farbiger JSON-Code.
`yaml`   | YAML, eine maschinenlesbare Alternative zu JSON.
`table`  | ASCII-Tabelle mit Schlüsseln als Spaltenüberschriften.
`tsv`    | Per Tabulator getrennte Werte ohne Schlüssel

## <a name="json-output-format"></a>JSON-Ausgabeformat

Im folgenden Beispiel wird die Liste mit den virtuellen Computern Ihrer Abonnements im JSON-Standardformat angezeigt.

```azurecli-interactive
az vm list --output json
```

In der folgenden Ausgabe wurden einige Felder aus Platzgründen weggelassen, und identifizierende Informationen wurden ersetzt.

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/.../resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "demorg1"
        }
      ]
    },
          ...
          ...
          ...
]
```

## <a name="yaml-output-format"></a>YAML-Ausgabeformat

Das Format `yaml` gibt die Ausgabe als [YAML](http://yaml.org/) (ein Nur-Text-Datenserialisierungsformat) aus. YAML ist in der Regel leichter lesbar als JSON und lässt sich problemlos diesem Format zuordnen. Einige Anwendungen und CLI-Befehle verwenden als Konfigurationseingabe YAML anstelle von JSON.

```azurecli-interactive
az vm list --out yaml
```

In der folgenden Ausgabe wurden einige Felder aus Platzgründen weggelassen, und identifizierende Informationen wurden ersetzt.

```yaml
- availabilitySet: null
  diagnosticsProfile: null
  hardwareProfile:
    vmSize: Standard_DS1_v2
  id: /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010
  identity: null
  instanceView: null
  licenseType: null
  location: westus
  name: ExampleVM1
  networkProfile:
    networkInterfaces:
    - id: /subscriptions/.../resourceGroups/DemoRG1/providers/Microsoft.Network/networkInterfaces/DemoVM010Nic
      primary: null
      resourceGroup: DemoRG1
  ...
...
```

## <a name="table-output-format"></a>Tabellenausgabeformat

Beim `table`-Format wird die Ausgabe als ASCII-Tabelle zurückgegeben, die einfach gelesen und überprüft werden kann. Geschachtelte Objekte sind in der Tabellenausgabe nicht enthalten, können jedoch im Rahmen einer Abfrage gefiltert werden. Einige Felder sind nicht in der Tabelle enthalten, daher ist dieses Format am besten geeignet, wenn Sie eine schnelle und von Menschen durchsuchbare Übersicht über Daten benötigen.

```azurecli-interactive
az vm list --out table
```

```output
Name         ResourceGroup    Location
-----------  ---------------  ----------
DemoVM010    DEMORG1          westus
demovm212    DEMORG1          westus
demovm213    DEMORG1          westus
KBDemo001VM  RGDEMO001        westus
KBDemo020    RGDEMO001        westus
```

Sie können den Parameter `--query` verwenden, um die Eigenschaften und Spalten anzupassen, die Sie in der Listenausgabe anzeigen möchten. Im folgenden Beispiel wird veranschaulicht, wie Sie im Befehl `list` nur den VM-Namen und den Ressourcengruppennamen auswählen.

```azurecli-interactive
az vm list --query "[].{resource:resourceGroup, name:name}" -o table
```

```output
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

> [!NOTE]
> Einige Schlüssel werden standardmäßig nicht in der Tabellenansicht ausgegeben. Hierbei handelt es sich um `id`, `type`, und `etag`. Wenn Sie diese in der Ausgabe benötigen, können Sie die JMESPath-Funktion zum Erstellen neuer Schlüssel verwenden, um den Namen des Schlüssels zu ändern und das Filtern zu vermeiden.
>
> ```azurecli-interactive
> az vm list --query "[].{objectID:id}" -o table
> ```

Weitere Informationen zum Verwenden von Abfragen für die Filterung von Daten finden Sie unter [Verwenden von JMESPath-Abfragen mit der Azure CLI](/cli/azure/query-azure-cli).

## <a name="tsv-output-format"></a>TSV-Ausgabeformat

Das `tsv`-Ausgabeformat gibt durch Tabstopp oder Zeilenumbruch getrennte Werte ohne zusätzliche Formatierung, Schlüssel oder andere Symbole zurück. Mit diesem Format ist es leicht, die Ausgabe in anderen Befehlen und Tools zu nutzen, in denen der Text verarbeitet werden muss. Wie beim `table`-Format gibt `tsv` keine geschachtelten Objekte aus.

Wenn das obige Beispiel mit der Option `tsv` verwendet wird, wird das Ergebnis mit Tabulatortrennung ausgegeben.

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020   None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

Eine Einschränkung des TSV-Ausgabeformats besteht darin, dass es keine Garantie in Bezug auf die Ausgabereihenfolge gibt. Die CLI behält nach Möglichkeit die Reihenfolge bei, indem sie Schlüssel in der JSON-Antwort alphabetisch sortiert und dann ihre sortierten Werte für die TSV-Ausgabe ausgibt. Damit wird jedoch nicht garantiert, dass die Reihenfolge stets identisch ist, da sich das Antwortformat des Azure-Diensts ändern kann.

Zum Erzwingen einer konsistenten Reihenfolge müssen Sie den Parameter `--query` und das Format für die [Mehrfachauswahl](query-azure-cli.md#get-multiple-values) verwenden. Gibt ein CLI-Befehl ein einzelnes JSON-Wörterbuch zurück, erzwingen Sie mit dem allgemeinen Format `[key1, key2, ..., keyN]` eine Schlüsselreihenfolge.  Verwenden Sie für CLI-Befehle, die ein Array zurückgeben, das allgemeine Format `[].[key1, key2, ..., keyN]`, um Spaltenwerte zu sortieren.

So sortieren Sie beispielsweise die oben angezeigten Informationen nach ID, Standort, Ressourcengruppe und VM-Name:

```azurecli-interactive
az vm list --out tsv --query '[].[id, location, resourceGroup, name]'
```

```output
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    westus    DEMORG1    DemoVM010
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    westus    DEMORG1    demovm212
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    westus    DEMORG1    demovm213
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM     westus  RGDEMO001       KBDemo001VM
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020       westus  RGDEMO001       KBDemo020
```

Das nächste Beispiel zeigt, wie die `tsv`-Ausgabe an andere Befehle in Bash übergeben werden können. Mit der Abfrage wird die Ausgabe gefiltert und die Sortierung erzwungen. `grep` wählt Elemente aus, die den Text „RGD“ enthalten, und anschließend wird mit dem Befehl `cut` das vierte Feld für die Anzeige des Namens des virtuellen Computers in der Ausgabe ausgewählt.

```bash
az vm list --out tsv --query '[].[id, location, resourceGroup, name]' | grep RGD | cut -f4
```

```output
KBDemo001VM
KBDemo020
```

## <a name="set-the-default-output-format"></a>Festlegen des Standardausgabeformats

Verwenden Sie den interaktiven Befehl `az configure`, um Ihre Umgebung einzurichten und Standardeinstellungen für Ausgabeformate festzulegen. Das Standardausgabeformat ist `json`.

```azurecli-interactive
az configure
```

```output
Welcome to the Azure CLI! This command will guide you through logging in and setting some default values.

Your settings can be found at /home/defaultuser/.azure/config
Your current configuration is as follows:

  ...

Do you wish to change your settings? (y/N): y

What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses.
 [2] jsonc - Colored JSON formatted output that most closely matches API responses.
 [3] table - Human-readable output format.
 [4] tsv - Tab- and Newline-delimited. Great for GREP, AWK, etc.
 [5] yaml - YAML formatted output. An alternative to JSON. Great for configuration files.
 [6] none - No output, except for errors and warnings.
Please enter a choice [1]:
```

Weitere Informationen zum Konfigurieren der Umgebung finden Sie unter [Azure CLI-Konfiguration](/cli/azure/azure-cli-configuration).

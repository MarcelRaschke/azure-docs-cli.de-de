---
title: Ausgabeformate für Azure CLI 2.0
description: Erfahren Sie, wie Sie die Ausgabe von Azure CLI 2.0-Befehlen in Tabellen, Listen oder JSON-Code formatieren.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 07a5e9d913257d6aeb20a68263a6256ffadbe627
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388506"
---
# <a name="output-formats-for-azure-cli-20-commands"></a>Ausgabeformate für Azure CLI 2.0-Befehle

Die Azure CLI 2.0 verwendet JSON als Standardausgabeformat, sie bietet jedoch auch andere Formate.  Verwenden Sie den Parameter `--output` (`--out` oder `-o`) zum Formatieren der CLI-Ausgabe. Die Argumentwerte und Typen der Ausgabe lauten wie folgt:

--output | BESCHREIBUNG
---------|-------------------------------
`json`   | JSON-Zeichenfolge. Dies ist die Standardeinstellung.
`jsonc`  | Farbiger JSON-Code.
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

```azurecli
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
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

Weitere Informationen zum Verwenden von Abfragen zum Filtern von Daten finden Sie unter [Verwenden von JMESPath-Abfragen mit der Azure CLI 2.0](/cli/azure/query-azure-cli).

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
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

Das nächste Beispiel zeigt, wie die `tsv`-Ausgabe an andere Befehle in Bash übergeben werden können. `grep` wählt Elemente aus, die den Text „RGD“ enthalten, und anschließend wird mit dem Befehl `cut` das achte Feld für die Anzeige des Namens des virtuellen Computers in der Ausgabe ausgewählt.

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

Für die Verarbeitung von durch Tabstopp getrennten Feldern weisen die Werte die gleiche Reihenfolge wie im gedruckten JSON-Objekt auf. Diese Reihenfolge ist zwischen den Ausführungen des Befehls garantiert konsistent.

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
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab- and Newline-delimited, great for GREP, AWK, etc.
Please enter a choice [1]:
```

Weitere Informationen zum Konfigurieren der Umgebung finden Sie unter [Konfiguration der Azure CLI 2.0](/cli/azure/azure-cli-configuration).
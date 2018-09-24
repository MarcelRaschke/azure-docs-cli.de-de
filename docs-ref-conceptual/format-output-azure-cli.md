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
ms.openlocfilehash: 1430d817a7e6c10a8f8021cf9d763f62d560ba71
ms.sourcegitcommit: 8318ce761c279afa4cd45a81a58d83fc38c616bc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/13/2018
ms.locfileid: "45561557"
---
# <a name="output-formats-for-azure-cli-20-commands"></a><span data-ttu-id="8cc87-103">Ausgabeformate für Azure CLI 2.0-Befehle</span><span class="sxs-lookup"><span data-stu-id="8cc87-103">Output formats for Azure CLI 2.0 commands</span></span>

<span data-ttu-id="8cc87-104">Die Azure CLI 2.0 verwendet JSON als Standardausgabeformat, sie bietet jedoch auch andere Formate.</span><span class="sxs-lookup"><span data-stu-id="8cc87-104">Azure CLI 2.0 uses JSON as its default output format, but offers other formats.</span></span>  <span data-ttu-id="8cc87-105">Verwenden Sie den Parameter `--output` (`--out` oder `-o`) zum Formatieren der CLI-Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="8cc87-105">Use the `--output` (`--out` or `-o`) parameter to format CLI output.</span></span> <span data-ttu-id="8cc87-106">Die Argumentwerte und Typen der Ausgabe lauten wie folgt:</span><span class="sxs-lookup"><span data-stu-id="8cc87-106">The argument values and types of output are:</span></span>

<span data-ttu-id="8cc87-107">--output</span><span class="sxs-lookup"><span data-stu-id="8cc87-107">--output</span></span> | <span data-ttu-id="8cc87-108">BESCHREIBUNG</span><span class="sxs-lookup"><span data-stu-id="8cc87-108">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="8cc87-109">JSON-Zeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="8cc87-109">JSON string.</span></span> <span data-ttu-id="8cc87-110">Dies ist die Standardeinstellung.</span><span class="sxs-lookup"><span data-stu-id="8cc87-110">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="8cc87-111">Farbiger JSON-Code.</span><span class="sxs-lookup"><span data-stu-id="8cc87-111">Colorized JSON.</span></span>
`yaml`   | <span data-ttu-id="8cc87-112">YAML, eine maschinenlesbare Alternative zu JSON.</span><span class="sxs-lookup"><span data-stu-id="8cc87-112">YAML, a machine-readable alternative to JSON.</span></span>
`table`  | <span data-ttu-id="8cc87-113">ASCII-Tabelle mit Schlüsseln als Spaltenüberschriften.</span><span class="sxs-lookup"><span data-stu-id="8cc87-113">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="8cc87-114">Per Tabulator getrennte Werte ohne Schlüssel</span><span class="sxs-lookup"><span data-stu-id="8cc87-114">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="8cc87-115">JSON-Ausgabeformat</span><span class="sxs-lookup"><span data-stu-id="8cc87-115">JSON output format</span></span>

<span data-ttu-id="8cc87-116">Im folgenden Beispiel wird die Liste mit den virtuellen Computern Ihrer Abonnements im JSON-Standardformat angezeigt.</span><span class="sxs-lookup"><span data-stu-id="8cc87-116">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="8cc87-117">In der folgenden Ausgabe wurden einige Felder aus Platzgründen weggelassen, und identifizierende Informationen wurden ersetzt.</span><span class="sxs-lookup"><span data-stu-id="8cc87-117">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="yaml-output-format"></a><span data-ttu-id="8cc87-118">YAML-Ausgabeformat</span><span class="sxs-lookup"><span data-stu-id="8cc87-118">YAML output format</span></span>

<span data-ttu-id="8cc87-119">Das Format `yaml` gibt die Ausgabe als [YAML](http://yaml.org/) (ein Nur-Text-Datenserialisierungsformat) aus.</span><span class="sxs-lookup"><span data-stu-id="8cc87-119">The `yaml` format prints output as [YAML](http://yaml.org/), a plain-text data serialization format.</span></span> <span data-ttu-id="8cc87-120">YAML ist in der Regel leichter lesbar als JSON und lässt sich problemlos diesem Format zuordnen.</span><span class="sxs-lookup"><span data-stu-id="8cc87-120">YAML tends to be easier to read than JSON, and easily maps to that format.</span></span> <span data-ttu-id="8cc87-121">Einige Anwendungen und CLI-Befehle verwenden als Konfigurationseingabe YAML anstelle von JSON.</span><span class="sxs-lookup"><span data-stu-id="8cc87-121">Some applications and CLI commands take YAML as configuration input, instead of JSON.</span></span>

```azurecli-interactive
az vm list --out yaml
```

<span data-ttu-id="8cc87-122">In der folgenden Ausgabe wurden einige Felder aus Platzgründen weggelassen, und identifizierende Informationen wurden ersetzt.</span><span class="sxs-lookup"><span data-stu-id="8cc87-122">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="table-output-format"></a><span data-ttu-id="8cc87-123">Tabellenausgabeformat</span><span class="sxs-lookup"><span data-stu-id="8cc87-123">Table output format</span></span>

<span data-ttu-id="8cc87-124">Beim `table`-Format wird die Ausgabe als ASCII-Tabelle zurückgegeben, die einfach gelesen und überprüft werden kann.</span><span class="sxs-lookup"><span data-stu-id="8cc87-124">The `table` format prints output as an ASCII table, making it easy to read and scan.</span></span> <span data-ttu-id="8cc87-125">Geschachtelte Objekte sind in der Tabellenausgabe nicht enthalten, können jedoch im Rahmen einer Abfrage gefiltert werden.</span><span class="sxs-lookup"><span data-stu-id="8cc87-125">Nested objects aren't included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="8cc87-126">Einige Felder sind nicht in der Tabelle enthalten, daher ist dieses Format am besten geeignet, wenn Sie eine schnelle und von Menschen durchsuchbare Übersicht über Daten benötigen.</span><span class="sxs-lookup"><span data-stu-id="8cc87-126">Some fields aren't included in the table, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="8cc87-127">Sie können den Parameter `--query` verwenden, um die Eigenschaften und Spalten anzupassen, die Sie in der Listenausgabe anzeigen möchten.</span><span class="sxs-lookup"><span data-stu-id="8cc87-127">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="8cc87-128">Im folgenden Beispiel wird veranschaulicht, wie Sie im Befehl `list` nur den VM-Namen und den Ressourcengruppennamen auswählen.</span><span class="sxs-lookup"><span data-stu-id="8cc87-128">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

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
> <span data-ttu-id="8cc87-129">Einige Schlüssel werden standardmäßig nicht in der Tabellenansicht ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="8cc87-129">Some keys are not printed in the table view by default.</span></span> <span data-ttu-id="8cc87-130">Hierbei handelt es sich um `id`, `type`, und `etag`.</span><span class="sxs-lookup"><span data-stu-id="8cc87-130">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="8cc87-131">Wenn Sie diese in der Ausgabe benötigen, können Sie die JMESPath-Funktion zum Erstellen neuer Schlüssel verwenden, um den Namen des Schlüssels zu ändern und das Filtern zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="8cc87-131">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="8cc87-132">Weitere Informationen zum Verwenden von Abfragen zum Filtern von Daten finden Sie unter [Verwenden von JMESPath-Abfragen mit der Azure CLI 2.0](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="8cc87-132">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI 2.0](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="8cc87-133">TSV-Ausgabeformat</span><span class="sxs-lookup"><span data-stu-id="8cc87-133">TSV output format</span></span>

<span data-ttu-id="8cc87-134">Das `tsv`-Ausgabeformat gibt durch Tabstopp oder Zeilenumbruch getrennte Werte ohne zusätzliche Formatierung, Schlüssel oder andere Symbole zurück.</span><span class="sxs-lookup"><span data-stu-id="8cc87-134">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="8cc87-135">Mit diesem Format ist es leicht, die Ausgabe in anderen Befehlen und Tools zu nutzen, in denen der Text verarbeitet werden muss.</span><span class="sxs-lookup"><span data-stu-id="8cc87-135">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="8cc87-136">Wie beim `table`-Format gibt `tsv` keine geschachtelten Objekte aus.</span><span class="sxs-lookup"><span data-stu-id="8cc87-136">Like the `table` format, `tsv` doesn't print nested objects.</span></span>

<span data-ttu-id="8cc87-137">Wenn das obige Beispiel mit der Option `tsv` verwendet wird, wird das Ergebnis mit Tabulatortrennung ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="8cc87-137">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

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

<span data-ttu-id="8cc87-138">Das nächste Beispiel zeigt, wie die `tsv`-Ausgabe an andere Befehle in Bash übergeben werden können.</span><span class="sxs-lookup"><span data-stu-id="8cc87-138">The next example shows how `tsv` output can be piped to other commands in bash.</span></span> <span data-ttu-id="8cc87-139">`grep` wählt Elemente aus, die den Text „RGD“ enthalten, und anschließend wird mit dem Befehl `cut` das achte Feld für die Anzeige des Namens des virtuellen Computers in der Ausgabe ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="8cc87-139">`grep` selects items that have text "RGD" in them, then the `cut` command selects the eighth field to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

<span data-ttu-id="8cc87-140">Für die Verarbeitung von durch Tabstopp getrennten Feldern weisen die Werte die gleiche Reihenfolge wie im gedruckten JSON-Objekt auf.</span><span class="sxs-lookup"><span data-stu-id="8cc87-140">For the purposes of processing tab-separated fields, the values are in the same order that they appear in the printed JSON object.</span></span> <span data-ttu-id="8cc87-141">Diese Reihenfolge ist zwischen den Ausführungen des Befehls garantiert konsistent.</span><span class="sxs-lookup"><span data-stu-id="8cc87-141">This order is guaranteed to be consistent between runs of the command.</span></span>

## <a name="set-the-default-output-format"></a><span data-ttu-id="8cc87-142">Festlegen des Standardausgabeformats</span><span class="sxs-lookup"><span data-stu-id="8cc87-142">Set the default output format</span></span>

<span data-ttu-id="8cc87-143">Verwenden Sie den interaktiven Befehl `az configure`, um Ihre Umgebung einzurichten und Standardeinstellungen für Ausgabeformate festzulegen.</span><span class="sxs-lookup"><span data-stu-id="8cc87-143">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="8cc87-144">Das Standardausgabeformat ist `json`.</span><span class="sxs-lookup"><span data-stu-id="8cc87-144">The default output format is `json`.</span></span>

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

<span data-ttu-id="8cc87-145">Weitere Informationen zum Konfigurieren der Umgebung finden Sie unter [Konfiguration der Azure CLI 2.0](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="8cc87-145">To learn more about configuring your environment, see [Azure CLI 2.0 configuration](/cli/azure/azure-cli-configuration).</span></span>
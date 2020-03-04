---
title: Ausgabeformate für die Azure CLI
description: Erfahren Sie, wie Sie die Ausgabe von Azure CLI-Befehlen in Tabellen, Listen oder JSON-Code formatieren.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/23/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 7f28a5cc7acd7e5d41e1ab91424a9f360a25b702
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/28/2020
ms.locfileid: "77779957"
---
# <a name="output-formats-for-azure-cli-commands"></a><span data-ttu-id="b8271-103">Ausgabeformate für Azure CLI-Befehle</span><span class="sxs-lookup"><span data-stu-id="b8271-103">Output formats for Azure CLI commands</span></span>

<span data-ttu-id="b8271-104">Die Azure CLI verwendet JSON als Standardausgabeformat, aber es sind auch andere Formate möglich.</span><span class="sxs-lookup"><span data-stu-id="b8271-104">The Azure CLI uses JSON as its default output format, but offers other formats.</span></span>  <span data-ttu-id="b8271-105">Verwenden Sie den Parameter `--output` (`--out` oder `-o`) zum Formatieren der CLI-Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="b8271-105">Use the `--output` (`--out` or `-o`) parameter to format CLI output.</span></span> <span data-ttu-id="b8271-106">Die Argumentwerte und Typen der Ausgabe lauten wie folgt:</span><span class="sxs-lookup"><span data-stu-id="b8271-106">The argument values and types of output are:</span></span>

<span data-ttu-id="b8271-107">--output</span><span class="sxs-lookup"><span data-stu-id="b8271-107">--output</span></span> | <span data-ttu-id="b8271-108">BESCHREIBUNG</span><span class="sxs-lookup"><span data-stu-id="b8271-108">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="b8271-109">JSON-Zeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="b8271-109">JSON string.</span></span> <span data-ttu-id="b8271-110">Dies ist die Standardeinstellung.</span><span class="sxs-lookup"><span data-stu-id="b8271-110">This setting is the default</span></span>
`jsonc`  | <span data-ttu-id="b8271-111">Farbiger JSON-Code</span><span class="sxs-lookup"><span data-stu-id="b8271-111">Colorized JSON</span></span>
`yaml`   | <span data-ttu-id="b8271-112">YAML, eine maschinenlesbare Alternative zu JSON</span><span class="sxs-lookup"><span data-stu-id="b8271-112">YAML, a machine-readable alternative to JSON</span></span>
`table`  | <span data-ttu-id="b8271-113">ASCII-Tabelle mit Schlüsseln als Spaltenüberschriften</span><span class="sxs-lookup"><span data-stu-id="b8271-113">ASCII table with keys as column headings</span></span>
`tsv`    | <span data-ttu-id="b8271-114">Per Tabulator getrennte Werte ohne Schlüssel</span><span class="sxs-lookup"><span data-stu-id="b8271-114">Tab-separated values, with no keys</span></span>
`none`   | <span data-ttu-id="b8271-115">Keine andere Ausgabe als Fehler und Warnungen</span><span class="sxs-lookup"><span data-stu-id="b8271-115">No output other than errors and warnings</span></span>

## <a name="json-output-format"></a><span data-ttu-id="b8271-116">JSON-Ausgabeformat</span><span class="sxs-lookup"><span data-stu-id="b8271-116">JSON output format</span></span>

<span data-ttu-id="b8271-117">Im folgenden Beispiel wird die Liste mit den virtuellen Computern Ihrer Abonnements im JSON-Standardformat angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b8271-117">The following example displays the list of virtual machines in your subscriptions in the default JSON format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="b8271-118">In der folgenden Ausgabe wurden einige Felder aus Platzgründen weggelassen, und identifizierende Informationen wurden ersetzt.</span><span class="sxs-lookup"><span data-stu-id="b8271-118">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="yaml-output-format"></a><span data-ttu-id="b8271-119">YAML-Ausgabeformat</span><span class="sxs-lookup"><span data-stu-id="b8271-119">YAML output format</span></span>

<span data-ttu-id="b8271-120">Das Format `yaml` gibt die Ausgabe als [YAML](http://yaml.org/) (ein Nur-Text-Datenserialisierungsformat) aus.</span><span class="sxs-lookup"><span data-stu-id="b8271-120">The `yaml` format prints output as [YAML](http://yaml.org/), a plain-text data serialization format.</span></span> <span data-ttu-id="b8271-121">YAML ist in der Regel leichter lesbar als JSON und lässt sich problemlos diesem Format zuordnen.</span><span class="sxs-lookup"><span data-stu-id="b8271-121">YAML tends to be easier to read than JSON, and easily maps to that format.</span></span> <span data-ttu-id="b8271-122">Einige Anwendungen und CLI-Befehle verwenden als Konfigurationseingabe YAML anstelle von JSON.</span><span class="sxs-lookup"><span data-stu-id="b8271-122">Some applications and CLI commands take YAML as configuration input, instead of JSON.</span></span>

```azurecli-interactive
az vm list --out yaml
```

<span data-ttu-id="b8271-123">In der folgenden Ausgabe wurden einige Felder aus Platzgründen weggelassen, und identifizierende Informationen wurden ersetzt.</span><span class="sxs-lookup"><span data-stu-id="b8271-123">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="table-output-format"></a><span data-ttu-id="b8271-124">Tabellenausgabeformat</span><span class="sxs-lookup"><span data-stu-id="b8271-124">Table output format</span></span>

<span data-ttu-id="b8271-125">Beim `table`-Format wird die Ausgabe als ASCII-Tabelle zurückgegeben, die einfach gelesen und überprüft werden kann.</span><span class="sxs-lookup"><span data-stu-id="b8271-125">The `table` format prints output as an ASCII table, making it easy to read and scan.</span></span> <span data-ttu-id="b8271-126">Geschachtelte Objekte sind in der Tabellenausgabe nicht enthalten, können jedoch im Rahmen einer Abfrage gefiltert werden.</span><span class="sxs-lookup"><span data-stu-id="b8271-126">Nested objects aren't included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="b8271-127">Einige Felder sind nicht in der Tabelle enthalten, daher ist dieses Format am besten geeignet, wenn Sie eine schnelle und von Menschen durchsuchbare Übersicht über Daten benötigen.</span><span class="sxs-lookup"><span data-stu-id="b8271-127">Some fields aren't included in the table, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="b8271-128">Sie können den Parameter `--query` verwenden, um die Eigenschaften und Spalten anzupassen, die Sie in der Listenausgabe anzeigen möchten.</span><span class="sxs-lookup"><span data-stu-id="b8271-128">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="b8271-129">Im folgenden Beispiel wird veranschaulicht, wie Sie im Befehl `list` nur den VM-Namen und den Ressourcengruppennamen auswählen.</span><span class="sxs-lookup"><span data-stu-id="b8271-129">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

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
> <span data-ttu-id="b8271-130">Einige Schlüssel werden standardmäßig nicht in der Tabellenansicht ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8271-130">Some keys are not printed in the table view by default.</span></span> <span data-ttu-id="b8271-131">Hierbei handelt es sich um `id`, `type`, und `etag`.</span><span class="sxs-lookup"><span data-stu-id="b8271-131">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="b8271-132">Wenn Sie diese in der Ausgabe benötigen, können Sie die JMESPath-Funktion zum Erstellen neuer Schlüssel verwenden, um den Namen des Schlüssels zu ändern und das Filtern zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="b8271-132">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli-interactive
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="b8271-133">Weitere Informationen zum Verwenden von Abfragen für die Filterung von Daten finden Sie unter [Verwenden von JMESPath-Abfragen mit der Azure CLI](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="b8271-133">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="b8271-134">TSV-Ausgabeformat</span><span class="sxs-lookup"><span data-stu-id="b8271-134">TSV output format</span></span>

<span data-ttu-id="b8271-135">Das `tsv`-Ausgabeformat gibt durch Tabstopp oder Zeilenumbruch getrennte Werte ohne zusätzliche Formatierung, Schlüssel oder andere Symbole zurück.</span><span class="sxs-lookup"><span data-stu-id="b8271-135">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="b8271-136">Mit diesem Format ist es leicht, die Ausgabe in anderen Befehlen und Tools zu nutzen, in denen der Text verarbeitet werden muss.</span><span class="sxs-lookup"><span data-stu-id="b8271-136">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="b8271-137">Wie beim `table`-Format gibt `tsv` keine geschachtelten Objekte aus.</span><span class="sxs-lookup"><span data-stu-id="b8271-137">Like the `table` format, `tsv` doesn't print nested objects.</span></span>

<span data-ttu-id="b8271-138">Wenn das obige Beispiel mit der Option `tsv` verwendet wird, wird das Ergebnis mit Tabulatortrennung ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8271-138">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

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

<span data-ttu-id="b8271-139">Eine Einschränkung des TSV-Ausgabeformats besteht darin, dass es keine Garantie in Bezug auf die Ausgabereihenfolge gibt.</span><span class="sxs-lookup"><span data-stu-id="b8271-139">One restriction of the TSV output format is that there isn't a guarantee on output ordering.</span></span> <span data-ttu-id="b8271-140">Die CLI behält nach Möglichkeit die Reihenfolge bei, indem sie Schlüssel in der JSON-Antwort alphabetisch sortiert und dann ihre sortierten Werte für die TSV-Ausgabe ausgibt.</span><span class="sxs-lookup"><span data-stu-id="b8271-140">The CLI makes a best effort to preserve ordering by sorting keys in the response JSON alphebetically, and then printing their values in order for TSV output.</span></span> <span data-ttu-id="b8271-141">Damit wird jedoch nicht garantiert, dass die Reihenfolge stets identisch ist, da sich das Antwortformat des Azure-Diensts ändern kann.</span><span class="sxs-lookup"><span data-stu-id="b8271-141">This isn't a guarantee that the order is always identical though, since the Azure service response format may change.</span></span>

<span data-ttu-id="b8271-142">Zum Erzwingen einer konsistenten Reihenfolge müssen Sie den Parameter `--query` und das Format für die [Mehrfachauswahl](query-azure-cli.md#get-multiple-values) verwenden.</span><span class="sxs-lookup"><span data-stu-id="b8271-142">In order to enforce consistent ordering, you'll need to use the `--query` parameter and the [multiselect list](query-azure-cli.md#get-multiple-values) format.</span></span> <span data-ttu-id="b8271-143">Gibt ein CLI-Befehl ein einzelnes JSON-Wörterbuch zurück, erzwingen Sie mit dem allgemeinen Format `[key1, key2, ..., keyN]` eine Schlüsselreihenfolge.</span><span class="sxs-lookup"><span data-stu-id="b8271-143">When a CLI command returns a single JSON dictionary, use the general format `[key1, key2, ..., keyN]` to force a key order.</span></span>  <span data-ttu-id="b8271-144">Verwenden Sie für CLI-Befehle, die ein Array zurückgeben, das allgemeine Format `[].[key1, key2, ..., keyN]`, um Spaltenwerte zu sortieren.</span><span class="sxs-lookup"><span data-stu-id="b8271-144">For CLI commands which return an array, use the general format `[].[key1, key2, ..., keyN]` to order column values.</span></span>

<span data-ttu-id="b8271-145">So sortieren Sie beispielsweise die oben angezeigten Informationen nach ID, Standort, Ressourcengruppe und VM-Name:</span><span class="sxs-lookup"><span data-stu-id="b8271-145">For example, to order the information displayed above by ID, location, resource group, and VM name:</span></span>

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

<span data-ttu-id="b8271-146">Das nächste Beispiel zeigt, wie die `tsv`-Ausgabe an andere Befehle in Bash übergeben werden können.</span><span class="sxs-lookup"><span data-stu-id="b8271-146">The next example shows how `tsv` output can be piped to other commands in bash.</span></span> <span data-ttu-id="b8271-147">Mit der Abfrage wird die Ausgabe gefiltert und die Sortierung erzwungen. `grep` wählt Elemente aus, die den Text „RGD“ enthalten, und anschließend wird mit dem Befehl `cut` das vierte Feld für die Anzeige des Namens des virtuellen Computers in der Ausgabe ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="b8271-147">The query is used to filter output and force ordering, `grep` selects items that have text "RGD" in them, then the `cut` command selects the fourth field to show the name of the VM in output.</span></span>

```azurecli-interactive
az vm list --out tsv --query '[].[id, location, resourceGroup, name]' | grep RGD | cut -f4
```

```output
KBDemo001VM
KBDemo020
```

## <a name="set-the-default-output-format"></a><span data-ttu-id="b8271-148">Festlegen des Standardausgabeformats</span><span class="sxs-lookup"><span data-stu-id="b8271-148">Set the default output format</span></span>

<span data-ttu-id="b8271-149">Verwenden Sie den interaktiven Befehl `az configure`, um Ihre Umgebung einzurichten und Standardeinstellungen für Ausgabeformate festzulegen.</span><span class="sxs-lookup"><span data-stu-id="b8271-149">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="b8271-150">Das Standardausgabeformat ist `json`.</span><span class="sxs-lookup"><span data-stu-id="b8271-150">The default output format is `json`.</span></span>

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

<span data-ttu-id="b8271-151">Weitere Informationen zum Konfigurieren der Umgebung finden Sie unter [Azure CLI-Konfiguration](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="b8271-151">To learn more about configuring your environment, see [Azure CLI configuration](/cli/azure/azure-cli-configuration).</span></span>

---
title: Ausgabeformate für Azure CLI 2.0
description: Erfahren Sie, wie Sie die Ausgabe von Azure CLI 2.0-Befehlen in Tabellen, Listen oder JSON-Code formatieren.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: b402ce89cbf51adb3d521a604e992dd1fb5a42fa
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967604"
---
# <a name="output-formats-for-azure-cli-20-commands"></a><span data-ttu-id="752ab-103">Ausgabeformate für Azure CLI 2.0-Befehle</span><span class="sxs-lookup"><span data-stu-id="752ab-103">Output formats for Azure CLI 2.0 commands</span></span>

<span data-ttu-id="752ab-104">Für Azure CLI 2.0 wird JSON als Standardoption für die Ausgabe verwendet, aber Sie haben verschiedene Möglichkeiten, die Ausgabe von Befehlen zu formatieren.</span><span class="sxs-lookup"><span data-stu-id="752ab-104">Azure CLI 2.0 uses json as its default output option, but offers various ways for you to format the output of any command.</span></span>  <span data-ttu-id="752ab-105">Verwenden Sie den Parameter `--output` (oder `--out` oder `-o`), um die Ausgabe des Befehls basierend auf einem der Ausgabetypen zu formatieren, die in der folgenden Tabelle angegeben sind:</span><span class="sxs-lookup"><span data-stu-id="752ab-105">Use the `--output` (or `--out` or `-o`) parameter to format the output of the command into one of the output types noted in the following table:</span></span>

<span data-ttu-id="752ab-106">--output</span><span class="sxs-lookup"><span data-stu-id="752ab-106">--output</span></span> | <span data-ttu-id="752ab-107">BESCHREIBUNG</span><span class="sxs-lookup"><span data-stu-id="752ab-107">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="752ab-108">JSON-Zeichenfolge.</span><span class="sxs-lookup"><span data-stu-id="752ab-108">JSON string.</span></span> <span data-ttu-id="752ab-109">Dies ist die Standardeinstellung.</span><span class="sxs-lookup"><span data-stu-id="752ab-109">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="752ab-110">Farbiger JSON-Code.</span><span class="sxs-lookup"><span data-stu-id="752ab-110">Colorized JSON.</span></span>
`table`  | <span data-ttu-id="752ab-111">ASCII-Tabelle mit Schlüsseln als Spaltenüberschriften.</span><span class="sxs-lookup"><span data-stu-id="752ab-111">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="752ab-112">Per Tabulator getrennte Werte ohne Schlüssel</span><span class="sxs-lookup"><span data-stu-id="752ab-112">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="752ab-113">JSON-Ausgabeformat</span><span class="sxs-lookup"><span data-stu-id="752ab-113">JSON output format</span></span>

<span data-ttu-id="752ab-114">Im folgenden Beispiel wird die Liste mit den virtuellen Computern Ihrer Abonnements im JSON-Standardformat angezeigt.</span><span class="sxs-lookup"><span data-stu-id="752ab-114">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="752ab-115">In der folgenden Ausgabe wurden einige Felder aus Platzgründen weggelassen, und identifizierende Informationen wurden ersetzt.</span><span class="sxs-lookup"><span data-stu-id="752ab-115">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="table-output-format"></a><span data-ttu-id="752ab-116">Tabellenausgabeformat</span><span class="sxs-lookup"><span data-stu-id="752ab-116">Table output format</span></span>

<span data-ttu-id="752ab-117">Das Ausgabeformat `table` bietet die einfache Ausgabe formatiert als Zeilen und Spalten von sortierten Daten, die einfach zu lesen und überprüfen sind.</span><span class="sxs-lookup"><span data-stu-id="752ab-117">The `table` output format provides plain output formatted as rows and columns of collated data, making it easy to read and scan.</span></span> <span data-ttu-id="752ab-118">Geschachtelte Objekte sind in der Tabellenausgabe nicht enthalten, können jedoch im Rahmen einer Abfrage gefiltert werden.</span><span class="sxs-lookup"><span data-stu-id="752ab-118">Nested objects are not included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="752ab-119">Auch bei den Tabellendaten werden einige Felder weggelassen, d.h. dieses Format ist am besten geeignet, wenn Sie eine schnelle und von Menschen durchsuchbare Übersicht über Daten möchten.</span><span class="sxs-lookup"><span data-stu-id="752ab-119">Some fields are also omitted from the table data, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="752ab-120">Sie können den Parameter `--query` verwenden, um die Eigenschaften und Spalten anzupassen, die Sie in der Listenausgabe anzeigen möchten.</span><span class="sxs-lookup"><span data-stu-id="752ab-120">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="752ab-121">Im folgenden Beispiel wird veranschaulicht, wie Sie im Befehl `list` nur den VM-Namen und den Ressourcengruppennamen auswählen.</span><span class="sxs-lookup"><span data-stu-id="752ab-121">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

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
> <span data-ttu-id="752ab-122">Bestimmte Schlüssel werden herausgefiltert und nicht in der Tabellenansicht gedruckt.</span><span class="sxs-lookup"><span data-stu-id="752ab-122">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="752ab-123">Hierbei handelt es sich um `id`, `type`, und `etag`.</span><span class="sxs-lookup"><span data-stu-id="752ab-123">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="752ab-124">Wenn Sie diese in der Ausgabe benötigen, können Sie die JMESPath-Funktion zum Erstellen neuer Schlüssel verwenden, um den Namen des Schlüssels zu ändern und das Filtern zu vermeiden.</span><span class="sxs-lookup"><span data-stu-id="752ab-124">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="752ab-125">Weitere Informationen zum Verwenden von Abfragen zum Filtern von Daten finden Sie unter [Verwenden von JMESPath-Abfragen mit der Azure CLI 2.0](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="752ab-125">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI 2.0](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="752ab-126">TSV-Ausgabeformat</span><span class="sxs-lookup"><span data-stu-id="752ab-126">TSV output format</span></span>

<span data-ttu-id="752ab-127">Das `tsv`-Ausgabeformat gibt durch Tabstopp oder Zeilenumbruch getrennte Werte ohne zusätzliche Formatierung, Schlüssel oder andere Symbole zurück.</span><span class="sxs-lookup"><span data-stu-id="752ab-127">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="752ab-128">Mit diesem Format ist es leicht, die Ausgabe in anderen Befehlen und Tools zu nutzen, in denen der Text verarbeitet werden muss.</span><span class="sxs-lookup"><span data-stu-id="752ab-128">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="752ab-129">Genau wie das `table`-Format druckt die `tsv`-Ausgabeoption keine geschachtelten Objekte.</span><span class="sxs-lookup"><span data-stu-id="752ab-129">Like the `table` format, the `tsv` output option does not print nested objects.</span></span>

<span data-ttu-id="752ab-130">Wenn das obige Beispiel mit der Option `tsv` verwendet wird, wird das Ergebnis mit Tabulatortrennung ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="752ab-130">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

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

<span data-ttu-id="752ab-131">Das folgende Beispiel zeigt, wie die `tsv`-Ausgabe an andere Befehle in UNIX-Systemen zum Extrahieren spezifischerer Daten weitergeleitet werden kann.</span><span class="sxs-lookup"><span data-stu-id="752ab-131">The next example shows how the `tsv` output can be piped to other commands on UNIX systems to extract more specific data.</span></span> <span data-ttu-id="752ab-132">Mit dem Befehl `grep` werden Elemente ausgewählt, die den Text „RGD“ enthalten, und anschließend wird mit dem Befehl `cut` das achte Feld (durch Tabstopp getrennt) für die Anzeige des Namens des virtuellen Computers in der Ausgabe ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="752ab-132">The `grep` command selects items that have text "RGD" in them, and then the `cut` command selects the eighth field (separated by tabs) to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

<span data-ttu-id="752ab-133">Für die Verarbeitung von durch Tabstopp getrennten Feldern weisen die Werte die gleiche Reihenfolge wie im gedruckten JSON-Objekt auf.</span><span class="sxs-lookup"><span data-stu-id="752ab-133">For the purposes of processing tab-separated fields, the values are in the same order that they appear in the printed JSON object.</span></span> <span data-ttu-id="752ab-134">Diese Reihenfolge ist zwischen den Ausführungen des Befehls garantiert konsistent.</span><span class="sxs-lookup"><span data-stu-id="752ab-134">This order is guaranteed to be consistent between runs of the command.</span></span>

## <a name="set-the-default-output-format"></a><span data-ttu-id="752ab-135">Festlegen des Standardausgabeformats</span><span class="sxs-lookup"><span data-stu-id="752ab-135">Set the default output format</span></span>

<span data-ttu-id="752ab-136">Verwenden Sie den interaktiven Befehl `az configure`, um Ihre Umgebung einzurichten und Standardeinstellungen für Ausgabeformate festzulegen.</span><span class="sxs-lookup"><span data-stu-id="752ab-136">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="752ab-137">Das Standardausgabeformat ist `json`.</span><span class="sxs-lookup"><span data-stu-id="752ab-137">The default output format is `json`.</span></span>

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

<span data-ttu-id="752ab-138">Weitere Informationen zum Konfigurieren der Umgebung finden Sie unter [Konfiguration der Azure CLI 2.0](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="752ab-138">To learn more about configuring your environment, see [Azure CLI 2.0 configuration](/cli/azure/azure-cli-configuration).</span></span>
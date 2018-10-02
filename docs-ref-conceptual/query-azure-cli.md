---
title: Abfragen von Befehlsergebnissen mit der Azure CLI
description: Es wird beschrieben, wie Sie JMESPath-Abfragen für die Ausgabe von Azure CLI-Befehlen ausführen.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 4522242952e5d257449c9c593885c62de2f56d0f
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2018
ms.locfileid: "47178030"
---
# <a name="use-jmespath-queries-with-azure-cli"></a><span data-ttu-id="75895-103">Verwenden von JMESPath-Abfragen mit der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="75895-103">Use JMESPath queries with Azure CLI</span></span> 

<span data-ttu-id="75895-104">Die Azure CLI verwendet das Argument `--query`, um eine [JMESPath-Abfrage](http://jmespath.org) für die Ergebnisse von Befehlen auszuführen.</span><span class="sxs-lookup"><span data-stu-id="75895-104">The Azure CLI uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="75895-105">JMESPath ist eine Abfragesprache für JSON, die es ermöglicht, Daten aus der CLI-Ausgabe auszuwählen und zu präsentieren.</span><span class="sxs-lookup"><span data-stu-id="75895-105">JMESPath is a query language for JSON, giving you the ability to select and present data from CLI output.</span></span> <span data-ttu-id="75895-106">Diese Abfragen werden für die JSON-Ausgabe ausgeführt, bevor irgendeine Anzeigeformatierung stattfindet.</span><span class="sxs-lookup"><span data-stu-id="75895-106">These queries are executed on the JSON output before any display formatting.</span></span>

<span data-ttu-id="75895-107">Das Argument `--query` wird von allen Befehlen der Azure-Befehlszeilenschnittstelle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="75895-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="75895-108">Die Beispiele in diesem Artikel decken allgemeine Anwendungsfälle ab und veranschaulichen die Verwendung der Features von JMESPath.</span><span class="sxs-lookup"><span data-stu-id="75895-108">This article's examples cover common use cases and demonstrate how to use the features of JMESPath.</span></span>

## <a name="work-with-dictionary-output"></a><span data-ttu-id="75895-109">Verwenden einer Wörterbuchausgabe</span><span class="sxs-lookup"><span data-stu-id="75895-109">Work with dictionary output</span></span>

<span data-ttu-id="75895-110">Befehle, die ein JSON-Wörterbuch zurückgeben, können allein anhand ihrer Schlüsselnamen durchsucht werden.</span><span class="sxs-lookup"><span data-stu-id="75895-110">Commands that return a JSON dictionary can be explored by their key names alone.</span></span> <span data-ttu-id="75895-111">Bei Schlüsselpfaden wird als Trennzeichen das `.`-Zeichen verwendet.</span><span class="sxs-lookup"><span data-stu-id="75895-111">Key paths use the `.` character as a separator.</span></span> <span data-ttu-id="75895-112">Im folgenden Beispiel wird mithilfe von Pull eine Liste mit den öffentlichen SSH-Schlüsseln abgerufen, die beim Herstellen einer Verbindung mit einem virtuellen Linux-Computer zulässig sind:</span><span class="sxs-lookup"><span data-stu-id="75895-112">The following example pulls a list of the public SSH keys allowed to connect to a Linux VM:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

<span data-ttu-id="75895-113">Mehrere Werte können in einem sortierten Array platziert werden.</span><span class="sxs-lookup"><span data-stu-id="75895-113">Multiple values can be put into an ordered array.</span></span> <span data-ttu-id="75895-114">Das folgende Beispiel zeigt das Abrufen des Azure-Imageangebotsnamens und der Größe des Betriebssystemdatenträgers:</span><span class="sxs-lookup"><span data-stu-id="75895-114">The following example shows how to retrieve the Azure image offering name and the size of the OS disk:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

<span data-ttu-id="75895-115">Wenn die Ausgabe Schlüssel enthalten soll, können Sie eine alternative Wörterbuchsyntax verwenden.</span><span class="sxs-lookup"><span data-stu-id="75895-115">If you want keys in your output, you can use an alternate dictionary syntax.</span></span>  <span data-ttu-id="75895-116">Bei der Auswahl von Elementen in einem Wörterbuch wird das Format `{displayKey:keyPath, ...}` verwendet, um nach dem `keyPath`-JMESPath-Ausdruck zu filtern.</span><span class="sxs-lookup"><span data-stu-id="75895-116">Element selection into a dictionary uses the format `{displayKey:keyPath, ...}` to filter on the `keyPath` JMESPath expression.</span></span> <span data-ttu-id="75895-117">In den Ausgabewerten werden die Schlüssel-Wert-Paare in `{displayKey: value}` geändert.</span><span class="sxs-lookup"><span data-stu-id="75895-117">In the output values, the key/value pairs are changed to `{displayKey: value}`.</span></span> <span data-ttu-id="75895-118">Das nächste Beispiel baut auf der Abfrage des letzten Beispiels auf und weist der Ausgabe Schlüssel zu, um sie deutlicher zu machen:</span><span class="sxs-lookup"><span data-stu-id="75895-118">The next example takes the last example's query, and makes it clearer by assigning keys to the output:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

<span data-ttu-id="75895-119">Beim Anzeigen von Informationen im Ausgabeformat `table` ermöglicht die Wörterbuchanzeige das Festlegen eigener Spaltenüberschriften.</span><span class="sxs-lookup"><span data-stu-id="75895-119">When displaying information in the `table` output format, dictionary display allows setting your own column headers.</span></span> <span data-ttu-id="75895-120">Weitere Informationen zu Ausgabeformaten finden Sie unter [Ausgabeformate für Azure CLI-Befehle](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="75895-120">For more information on output formats, see [Output formats for Azure CLI commands](/cli/azure/format-output-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="75895-121">Bestimmte Schlüssel werden herausgefiltert und nicht in der Tabellenansicht gedruckt.</span><span class="sxs-lookup"><span data-stu-id="75895-121">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="75895-122">Diese Schlüssel sind `id`, `type` und `etag`.</span><span class="sxs-lookup"><span data-stu-id="75895-122">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="75895-123">Wenn Sie diese Informationen benötigen, können Sie den Schlüsselnamen ändern und so die Filterung umgehen.</span><span class="sxs-lookup"><span data-stu-id="75895-123">If you need to see this information, you can change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a><span data-ttu-id="75895-124">Verwenden von Listenausgaben</span><span class="sxs-lookup"><span data-stu-id="75895-124">Work with list output</span></span>

<span data-ttu-id="75895-125">CLI-Befehle, die mehrere Werte zurückgeben können, geben ein Array zurück.</span><span class="sxs-lookup"><span data-stu-id="75895-125">CLI commands that may return  more than one value return an array.</span></span> <span data-ttu-id="75895-126">Auf Arrayelemente wird über einen Index zugegriffen, und sie werden unter Umständen nicht jedes Mal in der gleichen Reihenfolge zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="75895-126">Array elements are accessed by index and may not be returned in the same order every time.</span></span> <span data-ttu-id="75895-127">Sie können alle Arrayelemente gleichzeitig abfragen, indem Sie sie mit dem Operator `[]` vereinfachen.</span><span class="sxs-lookup"><span data-stu-id="75895-127">You can query all array elements at once by flattening them with the `[]` operator.</span></span> <span data-ttu-id="75895-128">Der Operator wird nach dem Array oder als erstes Element in einen Ausdruck eingefügt.</span><span class="sxs-lookup"><span data-stu-id="75895-128">The operator is put after the array or as the first element in an expression.</span></span> <span data-ttu-id="75895-129">Bei einem vereinfachten Array wird die darauffolgende Abfrage für jedes Arrayelement ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="75895-129">Flattening an array runs the query after it against each element of the array.</span></span>

<span data-ttu-id="75895-130">Im folgenden Beispiel werden jeweils der Name und das Betriebssystem der virtuellen Computer in einer Ressourcengruppe ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="75895-130">The following example prints out the name and OS running on each VM in a resource group.</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{name:name, image:storageProfile.imageReference.offer}'
```

```json
[
  {
    "image": "CentOS",
    "name": "CentBox"
  },
  {
    "image": "openSUSE-Leap",
    "name": "SUSEBox"
  },
  {
    "image": "UbuntuServer",
    "name": "TestVM"
  },
  {
    "image": "UbuntuServer",
    "name": "Test2"
  },
  {
    "image": "WindowsServer",
    "name": "WinServ"
  }
]
```

<span data-ttu-id="75895-131">Auch Arrays, die einem Schlüsselpfad angehören, können vereinfacht werden.</span><span class="sxs-lookup"><span data-stu-id="75895-131">Arrays that are part of a key path can be flattened as well.</span></span> <span data-ttu-id="75895-132">Die folgende Abfrage ruft die Azure-Objekt-IDs für die NICs ab, mit denen ein virtueller Computer verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="75895-132">The following query gets the Azure object IDs for the NICs a VM is connected to.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a><span data-ttu-id="75895-133">Filtern der Arrayausgabe mit Prädikaten</span><span class="sxs-lookup"><span data-stu-id="75895-133">Filter array output with predicates</span></span>

<span data-ttu-id="75895-134">JMESPath bietet [Filterausdrücke](http://jmespath.org/specification.html#filterexpressions) zum Herausfiltern der angezeigten Daten.</span><span class="sxs-lookup"><span data-stu-id="75895-134">JMESPath offers [filtering expressions](http://jmespath.org/specification.html#filterexpressions) to filter out the data displayed.</span></span> <span data-ttu-id="75895-135">Diese Ausdrücke sind besonders hilfreich, wenn sie mit [integrierten JMESPath-Funktionen](http://jmespath.org/specification.html#built-in-functions) kombiniert werden, um teilweise Übereinstimmungen zu ermitteln oder Daten in ein Standardformat zu konvertieren.</span><span class="sxs-lookup"><span data-stu-id="75895-135">These expressions are powerful, especially when combined with [JMESPath built-in functions](http://jmespath.org/specification.html#built-in-functions) to do partial matches or manipulate data into a standard format.</span></span> <span data-ttu-id="75895-136">Filterausdrücke können nur für Arraydaten verwendet werden. In allen anderen Fällen geben Sie den Wert `null` zurück.</span><span class="sxs-lookup"><span data-stu-id="75895-136">Filtering expressions only work on array data, and when used in any other situation, return the `null` value.</span></span> <span data-ttu-id="75895-137">Sie können beispielsweise die Ausgabe von Befehlen wie `vm list` filtern, um nach bestimmten Arten von virtuellen Computern zu suchen.</span><span class="sxs-lookup"><span data-stu-id="75895-137">For example, you can take the output of commands like `vm list` and filter on it to look for specific types of VMs.</span></span> <span data-ttu-id="75895-138">Das folgende Beispiel baut auf dem vorherigen Beispiel auf und filtert den VM-Typ heraus, um nur virtuelle Windows-Computer zu erfassen und deren Namen auszugeben.</span><span class="sxs-lookup"><span data-stu-id="75895-138">The following example expands on the previous by filtering out the VM type to capture only Windows VMs and print their name.</span></span>

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="75895-139">Interaktives Experimentieren mit Abfragen</span><span class="sxs-lookup"><span data-stu-id="75895-139">Experiment with queries interactively</span></span>

<span data-ttu-id="75895-140">Wenn Sie sich mit JMESPath vertraut machen möchten, können Sie in der interaktiven Umgebung des Python-Pakets [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) mit Abfragen experimentieren.</span><span class="sxs-lookup"><span data-stu-id="75895-140">To start learning JMESPath, the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package offers an interactive environment to experiment with queries.</span></span> <span data-ttu-id="75895-141">Daten werden als Eingabe übergeben. Anschließend werden programminterne Abfragen geschrieben und bearbeitet, um die Daten zu extrahieren.</span><span class="sxs-lookup"><span data-stu-id="75895-141">Data is piped as input, and then in-program queries are written and edited to extract the data.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```

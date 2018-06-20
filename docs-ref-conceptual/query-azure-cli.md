---
title: Abfragen von Befehlsergebnissen mit Azure CLI 2.0
description: Erfahren Sie, wie Sie JMESPath-Abfragen für die Ausgabe von Azure CLI 2.0-Befehlen ausführen.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: ed8f8ac160dd8225170ffcfff9619d94b92e456a
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/18/2018
ms.locfileid: "34306164"
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="e6834-103">Verwenden von JMESPath-Abfragen mit der Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="e6834-103">Use JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="e6834-104">Die Azure CLI 2.0 verwendet das Argument `--query`, um eine [JMESPath-Abfrage](http://jmespath.org) für die Ergebnisse von Befehlen auszuführen.</span><span class="sxs-lookup"><span data-stu-id="e6834-104">The Azure CLI 2.0 uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="e6834-105">JMESPath ist eine Abfragesprache für JSON, die es ermöglicht, Daten aus der CLI-Ausgabe auszuwählen und zu präsentieren.</span><span class="sxs-lookup"><span data-stu-id="e6834-105">JMESPath is a query language for JSON, giving you the ability to select and present data from CLI output.</span></span> <span data-ttu-id="e6834-106">Diese Abfragen werden für die JSON-Ausgabe ausgeführt, bevor irgendeine andere Anzeigeformatierung stattfindet.</span><span class="sxs-lookup"><span data-stu-id="e6834-106">These queries are executed on the JSON output, before performing any other display formatting.</span></span>

<span data-ttu-id="e6834-107">Das Argument `--query` wird von allen Befehlen der Azure-Befehlszeilenschnittstelle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e6834-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="e6834-108">Die Beispiele in diesem Artikel decken allgemeine Anwendungsfälle ab und veranschaulichen die Verwendung der Features von JMESPath.</span><span class="sxs-lookup"><span data-stu-id="e6834-108">This article's examples cover common use cases and demonstrate how to use the features of JMESPath.</span></span>

## <a name="work-with-dictionary-output"></a><span data-ttu-id="e6834-109">Verwenden einer Wörterbuchausgabe</span><span class="sxs-lookup"><span data-stu-id="e6834-109">Work with dictionary output</span></span>

<span data-ttu-id="e6834-110">Befehle, die ein JSON-Wörterbuch zurückgeben, können allein anhand ihrer Schlüsselnamen durchsucht werden.</span><span class="sxs-lookup"><span data-stu-id="e6834-110">Commands that return a JSON dictionary can be explored by their key names alone.</span></span> <span data-ttu-id="e6834-111">Bei Schlüsselpfaden wird als Trennzeichen das `.`-Zeichen verwendet.</span><span class="sxs-lookup"><span data-stu-id="e6834-111">Key paths use the `.` character as a separator.</span></span> <span data-ttu-id="e6834-112">Im folgenden Beispiel wird mithilfe von Pull eine Liste mit den öffentlichen SSH-Schlüsseln abgerufen, die beim Herstellen einer Verbindung mit einem virtuellen Linux-Computer zulässig sind:</span><span class="sxs-lookup"><span data-stu-id="e6834-112">The following example pulls a list of the public SSH keys allowed to connect to a Linux VM:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

<span data-ttu-id="e6834-113">Sie können auch mehrere Werte abrufen und in einem sortierten Array platzieren.</span><span class="sxs-lookup"><span data-stu-id="e6834-113">You can also get multiple values, putting them in an ordered array.</span></span> <span data-ttu-id="e6834-114">Das Array verfügt zwar über keinerlei Schlüsselinformationen, die Reihenfolge der Arrayelemente entspricht jedoch der Reihenfolge der abgefragten Schlüssel.</span><span class="sxs-lookup"><span data-stu-id="e6834-114">The array doesn't have any key information, but the order of the array's elements matches the order of the queried keys.</span></span> <span data-ttu-id="e6834-115">Das folgende Beispiel zeigt das Abrufen des Azure-Imageangebotsnamens und der Größe des Betriebssystemdatenträgers:</span><span class="sxs-lookup"><span data-stu-id="e6834-115">The following example shows how to retrieve the Azure image offering name and the size of the OS disk:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

<span data-ttu-id="e6834-116">Wenn die Ausgabe Schlüssel enthalten soll, können Sie eine alternative Wörterbuchsyntax verwenden.</span><span class="sxs-lookup"><span data-stu-id="e6834-116">If you want keys in your output, you can use an alternate dictionary syntax.</span></span> <span data-ttu-id="e6834-117">Bei der Auswahl mehrerer Elemente in einem Wörterbuch wird das Format `{displayKey:keyPath, ...}` verwendet, um nach dem `keyPath`-JMESPath-Ausdruck zu filtern.</span><span class="sxs-lookup"><span data-stu-id="e6834-117">Multiple element selection into a dictionary uses the format `{displayKey:keyPath, ...}` to filter on the `keyPath` JMESPath expression.</span></span> <span data-ttu-id="e6834-118">Dies wird in der Ausgabe als `{displayKey: value}` angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e6834-118">This displays in the output as `{displayKey: value}`.</span></span> <span data-ttu-id="e6834-119">Das nächste Beispiel baut auf der Abfrage des letzten Beispiels auf und weist der Ausgabe Schlüssel zu, um sie deutlicher zu machen:</span><span class="sxs-lookup"><span data-stu-id="e6834-119">The next example takes the last example's query, and makes it clearer by assigning keys to the output:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

<span data-ttu-id="e6834-120">Beim Anzeigen von Informationen im Ausgabeformat `table` ist die Wörterbuchanzeige besonders hilfreich.</span><span class="sxs-lookup"><span data-stu-id="e6834-120">When displaying information in the `table` output format, dictionary display is especially useful.</span></span> <span data-ttu-id="e6834-121">Hierbei können eigene Spaltenüberschriften festgelegt werden, um die Lesbarkeit der Ausgabe weiter zu verbessern.</span><span class="sxs-lookup"><span data-stu-id="e6834-121">This allows for setting your own column headers, making output even easier to read.</span></span> <span data-ttu-id="e6834-122">Weitere Informationen zu Ausgabeformaten finden Sie unter [Ausgabeformate für Azure CLI 2.0-Befehle](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="e6834-122">For more information on output formats, see [Output formats for Azure CLI 2.0 commands](/cli/azure/format-output-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="e6834-123">Bestimmte Schlüssel werden herausgefiltert und nicht in der Tabellenansicht gedruckt.</span><span class="sxs-lookup"><span data-stu-id="e6834-123">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="e6834-124">Diese Schlüssel sind `id`, `type` und `etag`.</span><span class="sxs-lookup"><span data-stu-id="e6834-124">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="e6834-125">Wenn Sie diese Informationen benötigen, können Sie den Schlüsselnamen ändern und so die Filterung umgehen.</span><span class="sxs-lookup"><span data-stu-id="e6834-125">If you need to see this information, you can change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a><span data-ttu-id="e6834-126">Verwenden von Listenausgaben</span><span class="sxs-lookup"><span data-stu-id="e6834-126">Work with list output</span></span>

<span data-ttu-id="e6834-127">CLI-Befehle, die mehrere Werte zurückgeben können, geben immer ein Array zurück.</span><span class="sxs-lookup"><span data-stu-id="e6834-127">CLI commands that may return more than one value always return an array.</span></span> <span data-ttu-id="e6834-128">Auf die Elemente eines Arrays kann über einen Index zugegriffen werden, es gibt jedoch niemals eine Reihenfolgengarantie von der Befehlszeilenschnittstelle.</span><span class="sxs-lookup"><span data-stu-id="e6834-128">Arrays can have their elements accessed by index, but there's never an order guarantee from the CLI.</span></span> <span data-ttu-id="e6834-129">Beim Abfragen eines Arrays von Werten empfiehlt es sich, die Werte mit dem Operator `[]` zu vereinfachen.</span><span class="sxs-lookup"><span data-stu-id="e6834-129">The best way to query an array of values is to flatten them with the `[]` operator.</span></span> <span data-ttu-id="e6834-130">Der Operator wird nach dem Schlüssel für das Array oder als erstes Element im Ausdruck geschrieben.</span><span class="sxs-lookup"><span data-stu-id="e6834-130">The operator is written after the key for the array, or as the first element in the expression.</span></span> <span data-ttu-id="e6834-131">Durch die Vereinfachung wird die darauf folgende Abfrage für jedes einzelne Element im Array ausgeführt, und die resultierenden Werte werden in einem neuen Array platziert.</span><span class="sxs-lookup"><span data-stu-id="e6834-131">Flattening runs the query following it against each individual element in the array, and places the resulting values into a new array.</span></span> <span data-ttu-id="e6834-132">Im folgenden Beispiel werden jeweils der Name und das Betriebssystem der virtuellen Computer in einer Ressourcengruppe ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="e6834-132">The following example prints out the name and OS running on each VM in a resource group.</span></span> 

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

<span data-ttu-id="e6834-133">Auch Arrays, die einem Schlüsselpfad angehören, können vereinfacht werden.</span><span class="sxs-lookup"><span data-stu-id="e6834-133">Arrays that are part of a key path can be flattened as well.</span></span> <span data-ttu-id="e6834-134">Dieses Beispiel zeigt eine Abfrage, die die Azure-Objekt-IDs für die NICs abruft, mit denen ein virtueller Computer verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="e6834-134">This example demonstrates a query that gets the Azure object IDs for the NICs a VM is connected to.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a><span data-ttu-id="e6834-135">Filtern der Arrayausgabe mit Prädikaten</span><span class="sxs-lookup"><span data-stu-id="e6834-135">Filter array output with predicates</span></span>

<span data-ttu-id="e6834-136">JMESPath bietet [Filterausdrücke](http://jmespath.org/specification.html#filterexpressions) zum Herausfiltern der angezeigten Daten.</span><span class="sxs-lookup"><span data-stu-id="e6834-136">JMESPath offers [filtering expressions](http://jmespath.org/specification.html#filterexpressions) to filter out the data displayed.</span></span> <span data-ttu-id="e6834-137">Diese Ausdrücke sind besonders hilfreich, wenn sie mit [integrierten JMESPath-Funktionen](http://jmespath.org/specification.html#built-in-functions) kombiniert werden, um teilweise Übereinstimmungen zu ermitteln oder Daten in ein Standardformat zu konvertieren.</span><span class="sxs-lookup"><span data-stu-id="e6834-137">These expressions are powerful, especially when combined with [JMESPath built-in functions](http://jmespath.org/specification.html#built-in-functions) to perform partial matches or manipulate data into a standard format.</span></span> <span data-ttu-id="e6834-138">Filterausdrücke können nur für Arraydaten verwendet werden. In allen anderen Fällen geben Sie den Wert `null` zurück.</span><span class="sxs-lookup"><span data-stu-id="e6834-138">Filtering expressions only work on array data, and when used in any other situation, return the `null` value.</span></span> <span data-ttu-id="e6834-139">Sie können beispielsweise die Ausgabe von Befehlen wie `vm list` filtern, um nach bestimmten Arten von virtuellen Computern zu suchen.</span><span class="sxs-lookup"><span data-stu-id="e6834-139">For example, you can take the output of commands like `vm list` and filter on it to look for specific types of VMs.</span></span> <span data-ttu-id="e6834-140">Das folgende Beispiel baut auf dem vorherigen Beispiel auf und filtert den VM-Typ heraus, um nur virtuelle Windows-Computer zu erfassen und deren Namen auszugeben.</span><span class="sxs-lookup"><span data-stu-id="e6834-140">The following example expands on the previous by filtering out the VM type to capture only Windows VMs and print their name.</span></span>

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="e6834-141">Interaktives Experimentieren mit Abfragen</span><span class="sxs-lookup"><span data-stu-id="e6834-141">Experiment with queries interactively</span></span>

<span data-ttu-id="e6834-142">Beim Experimentieren mit JMESPath-Ausdrücken empfiehlt sich eine Arbeitsweise, bei der Sie Abfragen schnell bearbeiten und die Ausgabe untersuchen können.</span><span class="sxs-lookup"><span data-stu-id="e6834-142">To experiment with JMESPath expressions, you might want to work in a way where you can quickly edit queries and inspect the output.</span></span> <span data-ttu-id="e6834-143">Das Python-Paket [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) bietet eine interaktive Umgebung, in der Sie Daten mittels Piping als Eingabe verwenden und programminterne Abfragen schreiben können, um die Daten zu extrahieren.</span><span class="sxs-lookup"><span data-stu-id="e6834-143">An interactive environment is offered by the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package, which allows for piping data as input and then writing in-program queries to extract the data.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```

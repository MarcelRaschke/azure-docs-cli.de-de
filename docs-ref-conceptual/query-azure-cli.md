---
title: Abfragen von Befehlsergebnissen mit der Azure CLI
description: Es wird beschrieben, wie Sie JMESPath-Abfragen für die Ausgabe von Azure CLI-Befehlen ausführen.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/12/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: e878c467f71423cc8c9caa1f8cfe270d0019c48b
ms.sourcegitcommit: 399f0a2997675fbb280243e4234cf63c3bbca819
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/18/2019
ms.locfileid: "67194852"
---
# <a name="query-azure-cli-command-output"></a><span data-ttu-id="d6958-103">Abfragen der Azure CLI-Befehlsausgabe</span><span class="sxs-lookup"><span data-stu-id="d6958-103">Query Azure CLI command output</span></span>

<span data-ttu-id="d6958-104">Die Azure CLI verwendet das Argument `--query`, um eine [JMESPath-Abfrage](http://jmespath.org) für die Ergebnisse von Befehlen auszuführen.</span><span class="sxs-lookup"><span data-stu-id="d6958-104">The Azure CLI uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="d6958-105">JMESPath ist eine Abfragesprache für JSON, die es ermöglicht, Daten aus der CLI-Ausgabe auszuwählen und zu ändern.</span><span class="sxs-lookup"><span data-stu-id="d6958-105">JMESPath is a query language for JSON, giving you the ability to select and modify data from CLI output.</span></span> <span data-ttu-id="d6958-106">Abfragen werden für die JSON-Ausgabe ausgeführt, bevor irgendeine Anzeigeformatierung stattfindet.</span><span class="sxs-lookup"><span data-stu-id="d6958-106">Queries are executed on the JSON output before any display formatting.</span></span>

<span data-ttu-id="d6958-107">Das Argument `--query` wird von allen Befehlen der Azure-Befehlszeilenschnittstelle unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d6958-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="d6958-108">In diesem Artikel wird anhand einer Reihe von kleinen, einfachen Beispielen beschrieben, wie die Features von JMESPath verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="d6958-108">This article covers how to use the features of JMESPath with a series of small, simple examples.</span></span>

## <a name="dictionary-and-list-cli-results"></a><span data-ttu-id="d6958-109">CLI-Ergebnisse im Wörterbuch- und Listenformat</span><span class="sxs-lookup"><span data-stu-id="d6958-109">Dictionary and list CLI results</span></span>

<span data-ttu-id="d6958-110">Selbst wenn Sie ein anderes Ausgabeformat als JSON verwenden, werden die Ergebnisse von CLI-Befehlen für Abfragen zunächst als JSON-Ausgabe behandelt.</span><span class="sxs-lookup"><span data-stu-id="d6958-110">Even when using an output format other than JSON, CLI command results are first treated as JSON for queries.</span></span> <span data-ttu-id="d6958-111">CLI-Ergebnisse werden in Form eines JSON-Arrays oder -Wörterbuchs zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d6958-111">CLI results are either a JSON array or dictionary.</span></span> <span data-ttu-id="d6958-112">Arrays sind Sequenzen von Objekten, die indiziert werden können, und Wörterbücher sind unsortierte Objekte, auf die mit Schlüsseln zugegriffen wird.</span><span class="sxs-lookup"><span data-stu-id="d6958-112">Arrays are sequences of objects that can be indexed, and dictionaries are unordered objects accessed with keys.</span></span> <span data-ttu-id="d6958-113">Befehle, die mehr als ein Objekt zurückgeben _können_, geben ein Array zurück, und Befehle, die _immer_ _nur_ ein einzelnes Objekt zurückgeben, geben ein Wörterbuch zurück.</span><span class="sxs-lookup"><span data-stu-id="d6958-113">Commands that _could_ return more than one object return an array, and commands that _always_ return _only_ a single object return a dictionary.</span></span>

## <a name="get-properties-in-a-dictionary"></a><span data-ttu-id="d6958-114">Abrufen von Eigenschaften in einem Wörterbuch</span><span class="sxs-lookup"><span data-stu-id="d6958-114">Get properties in a dictionary</span></span>

<span data-ttu-id="d6958-115">Bei der Arbeit mit Ergebnissen im Wörterbuchformat können Sie auf Eigenschaften der obersten Ebene nur mit dem Schlüssel zugreifen.</span><span class="sxs-lookup"><span data-stu-id="d6958-115">Working with dictionary results, you can access properties from the top level with just the key.</span></span> <span data-ttu-id="d6958-116">Das Zeichen `.` (__Teilausdruck__) wird verwendet, um auf Eigenschaften von geschachtelten Wörterbüchern zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="d6958-116">The `.` (__subexpression__) character is used to access properties of nested dictionaries.</span></span> <span data-ttu-id="d6958-117">Bevor wir uns mit Abfragen befassen, werfen wir einen Blick auf die unveränderte Ausgabe des Befehls `az vm show`:</span><span class="sxs-lookup"><span data-stu-id="d6958-117">Before introducing queries, take a look at the unmodified output of the `az vm show` command:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM -o json
```

<span data-ttu-id="d6958-118">Der Befehl gibt ein Wörterbuch aus.</span><span class="sxs-lookup"><span data-stu-id="d6958-118">The command will output a dictionary.</span></span> <span data-ttu-id="d6958-119">Teile des Inhalts wurden hier weggelassen.</span><span class="sxs-lookup"><span data-stu-id="d6958-119">Some content has been omitted.</span></span>

```json
{
  "additionalCapabilities": null,
  "availabilitySet": null,
  "diagnosticsProfile": {
    "bootDiagnostics": {
      "enabled": true,
      "storageUri": "https://xxxxxx.blob.core.windows.net/"
    }
  },
  ...
  "osProfile": {
    "adminPassword": null,
    "adminUsername": "azureuser",
    "allowExtensionOperations": true,
    "computerName": "TestVM",
    "customData": null,
    "linuxConfiguration": {
      "disablePasswordAuthentication": true,
      "provisionVmAgent": true,
      "ssh": {
        "publicKeys": [
          {
            "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
            "path": "/home/azureuser/.ssh/authorized_keys"
          }
        ]
      }
    },
    "secrets": [],
    "windowsConfiguration": null
  },
  ....
}
```

<span data-ttu-id="d6958-120">Der folgende Befehl ruft durch Hinzufügen einer Abfrage die öffentlichen SSH-Schlüssel ab, die zum Herstellen einer Verbindung mit der VM autorisiert sind:</span><span class="sxs-lookup"><span data-stu-id="d6958-120">The following command gets the SSH public keys authorized to connect to the VM by adding a query:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys -o json
```

```json
[
  {
    "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
    "path": "/home/azureuser/.ssh/authorized_keys"
  }
]
```

<span data-ttu-id="d6958-121">Um mehrere Eigenschaften abzurufen, schließen Sie Ausdrücke als durch Trennzeichen getrennte Liste in eckige Klammern `[ ]` (eine __Mehrfachauswahlliste__) ein.</span><span class="sxs-lookup"><span data-stu-id="d6958-121">To get more than one property, put expressions in square brackets  `[ ]` (a __multiselect list__) as a comma-separated list.</span></span> <span data-ttu-id="d6958-122">Mit dem folgenden Befehl können Sie den Namen der VM, den Administrator und den SSH-Schlüssel gleichzeitig abrufen:</span><span class="sxs-lookup"><span data-stu-id="d6958-122">To get the VM name, admin user, and SSH key all at once use the command:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '[name, osProfile.adminUsername, osProfile.linuxConfiguration.ssh.publicKeys[0].keyData]' -o json
```

```json
[
  "TestVM",
  "azureuser",
  "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
]
```

<span data-ttu-id="d6958-123">Diese Werte werden im Ergebnisarray in der Reihenfolge aufgeführt, in der sie in der Abfrage übergeben wurden.</span><span class="sxs-lookup"><span data-stu-id="d6958-123">These values are listed in the result array in the order they were given in the query.</span></span> <span data-ttu-id="d6958-124">Da das Ergebnis ein Array ist, sind keine Schlüssel mit den Ergebnissen verknüpft.</span><span class="sxs-lookup"><span data-stu-id="d6958-124">Since the result is an array, there are no keys associated with the results.</span></span>

## <a name="get-a-single-value"></a><span data-ttu-id="d6958-125">Abrufen eines einzelnen Werts</span><span class="sxs-lookup"><span data-stu-id="d6958-125">Get a single value</span></span>

<span data-ttu-id="d6958-126">Es kommt recht häufig vor, dass Sie nur _einen_ Wert aus einem CLI-Befehl abrufen müssen, wie etwa eine Azure-Ressourcen-ID, einen Ressourcennamen, einen Benutzernamen oder ein Kennwort.</span><span class="sxs-lookup"><span data-stu-id="d6958-126">A common case is that you need to only get _one_ value out of a CLI command, such as an Azure resource ID, a resource name, a username, or a password.</span></span> <span data-ttu-id="d6958-127">In dem Fall soll der Wert oft auch in einer lokalen Umgebungsvariablen gespeichert werden.</span><span class="sxs-lookup"><span data-stu-id="d6958-127">In that case, you also often want to store the value in a local environment variable.</span></span> <span data-ttu-id="d6958-128">Zum Abrufen einer einzelnen Eigenschaft stellen Sie zunächst sicher, dass Sie nur eine Eigenschaft aus der Abfrage abrufen.</span><span class="sxs-lookup"><span data-stu-id="d6958-128">To get a single property, first make sure that you're only getting one property out of the query.</span></span> <span data-ttu-id="d6958-129">Ändern des letzten Beispiels, um nur den Administratorbenutzernamen abzurufen:</span><span class="sxs-lookup"><span data-stu-id="d6958-129">Modifying the last example to get only the admin username:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json
```

```JSON
"azureuser"
```

<span data-ttu-id="d6958-130">Dies sieht wie ein gültiger einzelner Wert aus, beachten Sie jedoch, dass die Zeichen `"` als Teil der Ausgabe zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="d6958-130">This looks like a valid single value, but note that the `"` characters are returned as part of the output.</span></span> <span data-ttu-id="d6958-131">Dies weist darauf hin, dass das Objekt eine JSON-Zeichenfolge ist.</span><span class="sxs-lookup"><span data-stu-id="d6958-131">This indicates that the object is a JSON string.</span></span> <span data-ttu-id="d6958-132">Beachten Sie dabei, dass die Anführungszeichen von der Shell unter Umständen __nicht__ interpretiert werden, wenn Sie diesen Wert einer Umgebungsvariablen direkt als Ausgabe vom Befehl zuweisen:</span><span class="sxs-lookup"><span data-stu-id="d6958-132">It's important to note that when you assign this value directly as output from the command to an environment variable, the quotes may __not__ be interpreted by the shell:</span></span>

```bash
USER=$(az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json)
echo $USER
```

```output
"azureuser"
```

<span data-ttu-id="d6958-133">Dies ist sicherlich nicht erwünscht.</span><span class="sxs-lookup"><span data-stu-id="d6958-133">This is almost certainly not what you want.</span></span> <span data-ttu-id="d6958-134">Verwenden Sie in dem Fall besser ein Ausgabeformat, das die zurückgegebenen Werte nicht in die Typinformationen einschließt.</span><span class="sxs-lookup"><span data-stu-id="d6958-134">In this case, you want to use an output format which doesn't enclose returned values with type information.</span></span> <span data-ttu-id="d6958-135">`tsv`, per Tabulator getrennte Werte, stellen die beste Ausgabeoption dar, die die CLI für diesen Zweck bietet.</span><span class="sxs-lookup"><span data-stu-id="d6958-135">The best output option that the CLI offers for this purpose is `tsv`, tab-separated values.</span></span> <span data-ttu-id="d6958-136">Insbesondere beim Abrufen eines Werts, der nur ein einzelner Wert ist (keine Wörterbücher oder Listen), enthält die Ausgabe `tsv` definitiv keine Anführungszeichen.</span><span class="sxs-lookup"><span data-stu-id="d6958-136">In particular, when retrieving a value that's only a single value (not a dictionary or list), `tsv` output is guaranteed to be unquoted.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o tsv
```

```output
azureuser
```

<span data-ttu-id="d6958-137">Weitere Informationen zum `tsv`-Ausgabeformat finden Sie unter [Ausgabeformate – TSV-Ausgabeformat](format-output-azure-cli.md#tsv-output-format).</span><span class="sxs-lookup"><span data-stu-id="d6958-137">For more information about the `tsv` output format, see [Output formats - TSV output format](format-output-azure-cli.md#tsv-output-format)</span></span>

## <a name="rename-properties-in-a-query"></a><span data-ttu-id="d6958-138">Umbenennen von Eigenschaften in einer Abfrage</span><span class="sxs-lookup"><span data-stu-id="d6958-138">Rename properties in a query</span></span>

<span data-ttu-id="d6958-139">Um beim Abfragen mehrerer Werte ein Wörterbuch anstelle eines Arrays abzurufen, verwenden Sie den Operator `{ }` (__Mehrfachauswahl-Hash__).</span><span class="sxs-lookup"><span data-stu-id="d6958-139">To get a dictionary instead of an array when querying for multiple values, use the `{ }` (__multiselect hash__) operator.</span></span>
<span data-ttu-id="d6958-140">Das Format für einen Mehrfachauswahl-Hash ist `{displayName:JMESPathExpression, ...}`.</span><span class="sxs-lookup"><span data-stu-id="d6958-140">The format for a multiselect hash is `{displayName:JMESPathExpression, ...}`.</span></span>
<span data-ttu-id="d6958-141">`displayName` ist die in der Ausgabe angezeigte Zeichenfolge, und `JMESPathExpression` ist der JMESPath-Ausdruck, der ausgewertet werden soll.</span><span class="sxs-lookup"><span data-stu-id="d6958-141">`displayName` will be the string shown in output, and `JMESPathExpression` is the JMESPath expression to evaluate.</span></span> <span data-ttu-id="d6958-142">Im Folgenden wird wieder das Beispiel aus dem letzten Abschnitt verwendet, aber die Mehrfachauswahlliste in einen Hash geändert:</span><span class="sxs-lookup"><span data-stu-id="d6958-142">Modifying the example from the last section by changing the multiselect list to a hash:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKey:osProfile.linuxConfiguration.ssh.publicKeys[0].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "ssh-key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
}
```

## <a name="get-properties-in-an-array"></a><span data-ttu-id="d6958-143">Abrufen von Eigenschaften in einem Array</span><span class="sxs-lookup"><span data-stu-id="d6958-143">Get properties in an array</span></span>

<span data-ttu-id="d6958-144">Ein Array verfügt nicht über eigene Eigenschaften, kann aber indiziert werden.</span><span class="sxs-lookup"><span data-stu-id="d6958-144">An array has no properties of its own, but it can be indexed.</span></span> <span data-ttu-id="d6958-145">Dieses Feature wird im letzten Beispiel mit dem Ausdruck `publicKeys[0]` veranschaulicht, der das erste Element des `publicKeys`-Arrays abruft.</span><span class="sxs-lookup"><span data-stu-id="d6958-145">This feature is shown in the last example with the expression `publicKeys[0]`, which gets the first element of the `publicKeys` array.</span></span> <span data-ttu-id="d6958-146">Es gibt keine Garantie, dass die CLI-Ausgabe sortiert ist. Sie sollten daher die Indizierung nur dann verwenden, wenn Sie die Reihenfolge kennen oder das zurückgegebene Element für Sie nicht von Bedeutung ist.</span><span class="sxs-lookup"><span data-stu-id="d6958-146">There's no guarantee CLI output is ordered, so avoid using indexing unless you're sure of the order or don't care what element you get.</span></span> <span data-ttu-id="d6958-147">Um auf die Eigenschaften von Elementen in einem Array zuzugreifen, führen Sie einen von zwei Vorgängen aus: _Vereinfachen_ und _Filtern_.</span><span class="sxs-lookup"><span data-stu-id="d6958-147">To access the properties of elements in an array, you do one of two operations: _flattening_ and _filtering_.</span></span> <span data-ttu-id="d6958-148">In diesem Abschnitt wird beschrieben, wie ein Array vereinfacht wird.</span><span class="sxs-lookup"><span data-stu-id="d6958-148">This section covers how to flatten an array.</span></span>

<span data-ttu-id="d6958-149">Zum Vereinfachen eines Arrays wird der JMESPath-Operator `[]` verwendet.</span><span class="sxs-lookup"><span data-stu-id="d6958-149">Flattening an array is done with the `[]` JMESPath operator.</span></span> <span data-ttu-id="d6958-150">Alle Ausdrücke nach dem `[]`-Operator werden auf jedes Element im aktuellen Array angewendet.</span><span class="sxs-lookup"><span data-stu-id="d6958-150">All expressions after the `[]` operator are applied to each element in the current array.</span></span>
<span data-ttu-id="d6958-151">Wenn `[]` am Anfang der Abfrage steht, wird das Ergebnis des CLI-Befehls vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="d6958-151">If `[]` appears at the start of the query, it flattens the CLI command result.</span></span> <span data-ttu-id="d6958-152">Die Ergebnisse von `az vm list` können mit diesem Feature überprüft werden.</span><span class="sxs-lookup"><span data-stu-id="d6958-152">The results of `az vm list` can be inspected with this feature.</span></span>
<span data-ttu-id="d6958-153">Mit der folgenden Abfrage werden der Name, das Betriebssystem und der Administratorname für jede VM in einer Ressourcengruppe abgerufen:</span><span class="sxs-lookup"><span data-stu-id="d6958-153">To get the name, OS, and administrator name for each VM in a resource group:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, admin:osProfile.adminUsername}' -o json
```

```json
[
  {
    "Name": "Test-2",
    "OS": "Linux",
    "admin": "sttramer"
  },
  {
    "Name": "TestVM",
    "OS": "Linux",
    "admin": "azureuser"
  },
  {
    "Name": "WinTest",
    "OS": "Windows",
    "admin": "winadmin"
  }
]
```

<span data-ttu-id="d6958-154">Wird diese Abfrage mit dem Ausgabeformat `--output table` kombiniert, entsprechen die Spaltennamen dem `displayKey`-Wert des Mehrfachauswahl-Hashes:</span><span class="sxs-lookup"><span data-stu-id="d6958-154">When combined with the `--output table` output format, the column names match up with the `displayKey` value of the multiselect hash:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, Admin:osProfile.adminUsername}' --output table
```

```output
Name     OS       Admin
-------  -------  ---------
Test-2   Linux    sttramer
TestVM   Linux    azureuser
WinTest  Windows  winadmin
```

> [!NOTE]
>
> <span data-ttu-id="d6958-155">Bestimmte Schlüssel werden herausgefiltert und nicht in der Tabellenansicht gedruckt.</span><span class="sxs-lookup"><span data-stu-id="d6958-155">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="d6958-156">Diese Schlüssel sind `id`, `type` und `etag`.</span><span class="sxs-lookup"><span data-stu-id="d6958-156">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="d6958-157">Um diese Werte anzuzeigen, können Sie den Schlüsselnamen in einem Mehrfachauswahl-Hash ändern.</span><span class="sxs-lookup"><span data-stu-id="d6958-157">To see these values, you can change the key name in a multiselect hash.</span></span>
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

<span data-ttu-id="d6958-158">Jedes Array kann vereinfacht werden, nicht nur das vom Befehl zurückgegebene Ergebnis der obersten Ebene.</span><span class="sxs-lookup"><span data-stu-id="d6958-158">Any array can be flattened, not just the top-level result returned by the command.</span></span> <span data-ttu-id="d6958-159">Im letzten Abschnitt wurde der Ausdruck `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` verwendet, um den öffentlichen SSH-Schlüssel für die Anmeldung abzurufen.</span><span class="sxs-lookup"><span data-stu-id="d6958-159">In the last section, the expression `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` was used to get the SSH public key for sign-in.</span></span> <span data-ttu-id="d6958-160">Zum Abrufen _aller_ öffentlichen SSH-Schlüssel könnte der Ausdruck stattdessen als `osProfile.linuxConfiguration.ssh.publicKeys[].keyData` geschrieben werden.</span><span class="sxs-lookup"><span data-stu-id="d6958-160">To get _every_ SSH public key, the expression could instead be written as `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.</span></span>
<span data-ttu-id="d6958-161">Dieser Abfrageausdruck vereinfacht das Array `osProfile.linuxConfiguration.ssh.publicKeys` und führt dann den Ausdruck `keyData` für jedes Element aus:</span><span class="sxs-lookup"><span data-stu-id="d6958-161">This query expression flattens the `osProfile.linuxConfiguration.ssh.publicKeys` array, and then runs the `keyData` expression on each element:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKeys:osProfile.linuxConfiguration.ssh.publicKeys[].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "sshKeys": [
    "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso\n"
  ]
}
```

## <a name="filter-arrays"></a><span data-ttu-id="d6958-162">Filtern von Arrays</span><span class="sxs-lookup"><span data-stu-id="d6958-162">Filter arrays</span></span>

<span data-ttu-id="d6958-163">Der zweite Vorgang zum Abrufen von Daten aus einem Array ist das _Filtern_.</span><span class="sxs-lookup"><span data-stu-id="d6958-163">The other operation used to get data from an array is _filtering_.</span></span> <span data-ttu-id="d6958-164">Zum Filtern wird der JMESPath-Operator `[?...]` verwendet.</span><span class="sxs-lookup"><span data-stu-id="d6958-164">Filtering is done with the `[?...]` JMESPath operator.</span></span>
<span data-ttu-id="d6958-165">Dieser Operator akzeptiert ein Prädikat als Inhalt.</span><span class="sxs-lookup"><span data-stu-id="d6958-165">This operator takes a predicate as its contents.</span></span> <span data-ttu-id="d6958-166">Ein Prädikat ist eine beliebige Anweisung, die zu `true` oder `false` ausgewertet werden kann.</span><span class="sxs-lookup"><span data-stu-id="d6958-166">A predicate is any statement that can be evaluated to either `true` or `false`.</span></span> <span data-ttu-id="d6958-167">Ausdrücke, bei denen das Prädikat zu `true` ausgewertet wird, sind in der Ausgabe enthalten.</span><span class="sxs-lookup"><span data-stu-id="d6958-167">Expressions where the predicate evaluates to `true` are included in the output.</span></span>

<span data-ttu-id="d6958-168">JMESPath bietet die standardmäßigen Vergleichsoperatoren und logischen Operatoren.</span><span class="sxs-lookup"><span data-stu-id="d6958-168">JMESPath offers the standard comparison and logical operators.</span></span> <span data-ttu-id="d6958-169">Dazu zählen `<`, `<=`, `>`, `>=`, `==` und `!=`.</span><span class="sxs-lookup"><span data-stu-id="d6958-169">These include `<`, `<=`, `>`, `>=`, `==`, and `!=`.</span></span>
<span data-ttu-id="d6958-170">JMESPath unterstützt auch logisches AND (`&&`), OR (`||`) und NOT (`!`).</span><span class="sxs-lookup"><span data-stu-id="d6958-170">JMESPath also supports logical and (`&&`), or (`||`), and not (`!`).</span></span> <span data-ttu-id="d6958-171">Ausdrücke können zum Erstellen komplexerer Prädikatausdrücke in Klammern gruppiert werden.</span><span class="sxs-lookup"><span data-stu-id="d6958-171">Expressions can be grouped within parenthesis, allowing for more complex predicate expressions.</span></span> <span data-ttu-id="d6958-172">Ausführliche Informationen zu Prädikaten und logischen Vorgängen finden Sie in der [JMESPath-Spezifikation](http://jmespath.org/specification.html).</span><span class="sxs-lookup"><span data-stu-id="d6958-172">For the full details on predicates and logical operations, see the [JMESPath specification](http://jmespath.org/specification.html).</span></span>

<span data-ttu-id="d6958-173">Im letzten Abschnitt haben wir ein Array vereinfacht, um die vollständige Liste aller VMs in einer Ressourcengruppe abzurufen.</span><span class="sxs-lookup"><span data-stu-id="d6958-173">In the last section, we flattened an array to get the complete list of all VMs in a resource group.</span></span> <span data-ttu-id="d6958-174">Mithilfe von Filtern kann diese Ausgabe auf Linux-VMs beschränkt werden:</span><span class="sxs-lookup"><span data-stu-id="d6958-174">Using filters, this output can be restricted to only Linux VMs:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[?storageProfile.osDisk.osType=='Linux'].{Name:name,  admin:osProfile.adminUsername}" --output table
```

```output
Name    Admin
------  ---------
Test-2  sttramer
TestVM  azureuser
```

> [!IMPORTANT]
>
> <span data-ttu-id="d6958-175">In JMESPath werden Zeichenfolgen immer in einfache Anführungszeichen (`'`) gesetzt.</span><span class="sxs-lookup"><span data-stu-id="d6958-175">In JMESPath, strings are always surrounded by single quotes (`'`).</span></span> <span data-ttu-id="d6958-176">Wenn Sie in einem Filterprädikat doppelte Anführungszeichen innerhalb einer Zeichenfolge verwenden, ist die Ausgabe leer.</span><span class="sxs-lookup"><span data-stu-id="d6958-176">If you use double quotes as part of a string in a filter predicate, you'll get empty output.</span></span>

<span data-ttu-id="d6958-177">JMESPath verfügt auch über integrierte Funktionen, die das Filtern erleichtern.</span><span class="sxs-lookup"><span data-stu-id="d6958-177">JMESPath also has built-in functions that can help with filtering.</span></span> <span data-ttu-id="d6958-178">Eine dieser Funktionen ist `contains(string, substring)`. Diese Funktion überprüft, ob eine Zeichenfolge eine Teilzeichenfolge enthält.</span><span class="sxs-lookup"><span data-stu-id="d6958-178">One such function is `contains(string, substring)`, which checks to see if a string contains a substring.</span></span> <span data-ttu-id="d6958-179">Ausdrücke werden vor dem Aufrufen der Funktion ausgewertet. Das erste Argument kann daher ein vollständiger JMESPath-Ausdruck sein.</span><span class="sxs-lookup"><span data-stu-id="d6958-179">Expressions are evaluated before calling the function, so the first argument can be a full JMESPath expression.</span></span> <span data-ttu-id="d6958-180">Im nächsten Beispiel werden alle VMs mit SSD-Speicher für den Betriebssystemdatenträger abgerufen:</span><span class="sxs-lookup"><span data-stu-id="d6958-180">The next example finds all VMs using SSD storage for their OS disk:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[?contains(storageProfile.osDisk.managedDisk.storageAccountType,'SSD')].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

<span data-ttu-id="d6958-181">Diese Abfrage ist relativ lang.</span><span class="sxs-lookup"><span data-stu-id="d6958-181">This query is a little long.</span></span> <span data-ttu-id="d6958-182">Der Schlüssel `storageProfile.osDisk.managedDisk.storageAccountType` wird zweimal erwähnt und in der Ausgabe neu erstellt.</span><span class="sxs-lookup"><span data-stu-id="d6958-182">The `storageProfile.osDisk.managedDisk.storageAccountType` key is mentioned twice, and rekeyed in the output.</span></span> <span data-ttu-id="d6958-183">Eine Möglichkeit zum Kürzen der Abfrage besteht darin, den Filter nach dem Vereinfachen und Auswählen von Daten anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="d6958-183">One way to shorten it is to apply the filter after flattening and selecting data.</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}[?contains(Storage,'SSD')]" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

<span data-ttu-id="d6958-184">Bei großen Arrays lässt sich der Vorgang möglicherweise beschleunigen, indem der Filter vor der Auswahl von Daten angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="d6958-184">For large arrays, it may be faster to apply the filter before selecting data.</span></span>

<span data-ttu-id="d6958-185">Die vollständige Liste der Funktionen finden Sie in der JMESPath-Spezifikation unter [Built-in Functions](http://jmespath.org/specification.html#built-in-functions) (Integrierte Funktionen).</span><span class="sxs-lookup"><span data-stu-id="d6958-185">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="change-output"></a><span data-ttu-id="d6958-186">Änder der Ausgabe</span><span class="sxs-lookup"><span data-stu-id="d6958-186">Change output</span></span>

<span data-ttu-id="d6958-187">JMESPath-Funktionen haben zudem einen weiteren Zweck: das Bearbeiten bzw. Ändern der Ergebnisse einer Abfrage.</span><span class="sxs-lookup"><span data-stu-id="d6958-187">JMESPath functions also have another purpose, which is to operate on the results of a query.</span></span> <span data-ttu-id="d6958-188">Jede Funktion, die einen nicht booleschen Wert zurückgibt, ändert das Ergebnis eines Ausdrucks.</span><span class="sxs-lookup"><span data-stu-id="d6958-188">Any function that returns a non-boolean value changes the result of an expression.</span></span>
<span data-ttu-id="d6958-189">Mit `sort_by(array, &sort_expression)` können Sie Daten beispielsweise nach einem Eigenschaftswert sortieren.</span><span class="sxs-lookup"><span data-stu-id="d6958-189">For example, you can sort data by a property value with `sort_by(array, &sort_expression)`.</span></span> <span data-ttu-id="d6958-190">JMESPath verwendet einen speziellen Operator (`&`) für Ausdrücke, die später im Rahmen einer Funktion ausgewertet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="d6958-190">JMESPath uses a special operator, `&`, for expressions that should be evaluated later as part of a function.</span></span> <span data-ttu-id="d6958-191">Das nächste Beispiel zeigt, wie Sie eine VM-Liste nach der Größe des Betriebssystemdatenträgers sortieren:</span><span class="sxs-lookup"><span data-stu-id="d6958-191">The next example shows how to sort a VM list by OS disk size:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "sort_by([].{Name:name, Size:storageProfile.osDisk.diskSizeGb}, &Size)" --output table
```

```output
Name     Size
-------  ------
TestVM   30
Test-2   32
WinTest  127
```

<span data-ttu-id="d6958-192">Die vollständige Liste der Funktionen finden Sie in der JMESPath-Spezifikation unter [Built-in Functions](http://jmespath.org/specification.html#built-in-functions) (Integrierte Funktionen).</span><span class="sxs-lookup"><span data-stu-id="d6958-192">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="d6958-193">Interaktives Experimentieren mit Abfragen</span><span class="sxs-lookup"><span data-stu-id="d6958-193">Experiment with queries interactively</span></span>

<span data-ttu-id="d6958-194">Für Ihre ersten Experimente mit JMESPath bietet das Python-Paket [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) eine interaktive Umgebung zur Verwendung von Abfragen.</span><span class="sxs-lookup"><span data-stu-id="d6958-194">To start experimenting with JMESPath, the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package offers an interactive environment to work with queries.</span></span> <span data-ttu-id="d6958-195">Daten werden als Eingabe übergeben, und anschließend werden Abfragen geschrieben und im Editor ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="d6958-195">Data is piped as input, and then queries are written and run in the editor.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```

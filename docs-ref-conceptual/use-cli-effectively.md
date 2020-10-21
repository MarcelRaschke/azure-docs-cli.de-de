---
title: Effektive Verwendung der Azure CLI
description: Tipps für die effektive Verwendung der Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/07/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 4ffd47b7d88dafc717f496fe40d9db68c7af28a3
ms.sourcegitcommit: ce10a134cb3c73aec32bb4f5887b09d08f9bde53
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/21/2020
ms.locfileid: "92308062"
---
# <a name="use-azure-cli-effectively"></a><span data-ttu-id="e80fa-103">Effektive Verwendung der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e80fa-103">Use Azure CLI effectively</span></span>

<span data-ttu-id="e80fa-104">Aus Gründen der Übersichtlichkeit werden Bash-Skripts inline verwendet.</span><span class="sxs-lookup"><span data-stu-id="e80fa-104">For clarity, Bash scripts are used inline.</span></span> <span data-ttu-id="e80fa-105">Windows-Batch- bzw. PowerShell-Beispiele, mit denen Sie ähnliche Beispiele erstellen können, sind im Anhang angegeben.</span><span class="sxs-lookup"><span data-stu-id="e80fa-105">Windows batch or PowerShell examples are listed in the appendix, which you can use to build similar examples.</span></span>

## <a name="output-formatting-json-table-or-tsv"></a><span data-ttu-id="e80fa-106">Ausgabeformatierung (JSON, TABLE oder TSV)</span><span class="sxs-lookup"><span data-stu-id="e80fa-106">Output formatting (json, table, or tsv)</span></span>

1. <span data-ttu-id="e80fa-107">Das Format `json` ist die Standardeinstellung der CLI und dafür ausgelegt, Ihnen die umfassendsten Informationen zu liefern.</span><span class="sxs-lookup"><span data-stu-id="e80fa-107">`json` format is the CLI's default, and is intended to give you the most comprehensive information.</span></span> <span data-ttu-id="e80fa-108">Falls Sie ein anderes Format vorziehen, sollten Sie das Argument `--output` verwenden, um einen einzelnen Befehlsaufruf außer Kraft zu setzen. Sie können auch `az configure` verwenden, um Ihre globale Standardeinstellung zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="e80fa-108">If you prefer a different format, use the `--output` argument to override for an individual command invocation, or use `az configure` to update your global default.</span></span> <span data-ttu-id="e80fa-109">Beachten Sie hierbei, dass beim JSON-Format die doppelten Anführungszeichen beibehalten werden. Dies bedeutet im Allgemeinen, dass das Format für Skripterstellungszwecke nicht geeignet ist.</span><span class="sxs-lookup"><span data-stu-id="e80fa-109">Note that JSON format preserves the double quotes, generally making in unsuitable for scripting purposes.</span></span>

2. <span data-ttu-id="e80fa-110">Das Format `table` ist nützlich, um eine Zusammenfassung der gewünschten Informationen zu erhalten. Dies gilt besonders für Auflistungsbefehle.</span><span class="sxs-lookup"><span data-stu-id="e80fa-110">`table` is useful for getting a summary of focused information, particularly for list commands.</span></span> <span data-ttu-id="e80fa-111">Falls Ihnen die Felder im Standardtabellenformat nicht zusagen (oder kein Standardformat vorhanden ist), können Sie mit `--output json` alle Informationen anzeigen oder `--query` verwenden, um das gewünschte Format anzugeben.</span><span class="sxs-lookup"><span data-stu-id="e80fa-111">If you do not like the fields in the default table format (or there isn't a default format), you can use `--output json` to see all information, or leverage `--query` to specify a format you like.</span></span>

    ```sh
    az vm show -g my_rg -n my_vm --query "{name: name, os:storageProfile.imageReference.offer}" -otable
    Name    Os
    ------  ------------
    my_vm   UbuntuServer
    ```

3. <span data-ttu-id="e80fa-112">`tsv` ist gut für kompakte Ausgaben und Skripterstellungszwecke geeignet.</span><span class="sxs-lookup"><span data-stu-id="e80fa-112">`tsv` is useful for concise output and scripting purposes.</span></span> <span data-ttu-id="e80fa-113">Beim TSV-Format werden doppelte Anführungszeichen entfernt, die im JSON-Format beibehalten werden.</span><span class="sxs-lookup"><span data-stu-id="e80fa-113">The tsv will strip double quotes that the JSON format preserves.</span></span> <span data-ttu-id="e80fa-114">Verwenden Sie das Argument `--query`, um das gewünschte Format für TSV anzugeben.</span><span class="sxs-lookup"><span data-stu-id="e80fa-114">To specify the format you want for TSV, use the `--query` argument.</span></span>

    ```sh
    export vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    az vm stop --ids $vm_ids
    ```

## <a name="pass-values-from-one-command-to-another"></a><span data-ttu-id="e80fa-115">Übergeben von Werten von einem Befehl an einen anderen</span><span class="sxs-lookup"><span data-stu-id="e80fa-115">Pass values from one command to another</span></span>

1. <span data-ttu-id="e80fa-116">Wenn der Wert mehrmals verwendet wird, sollten Sie ihn einer Variablen zuweisen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-116">If the value will be used more than once, assign it to a variable.</span></span> <span data-ttu-id="e80fa-117">Beachten Sie die Verwendung von `-o tsv` im folgenden Beispiel:</span><span class="sxs-lookup"><span data-stu-id="e80fa-117">Note the use of `-o tsv` in the following example:</span></span>

    ```sh
    running_vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    ```
2. <span data-ttu-id="e80fa-118">Erwägen Sie den Einsatz von Piping, wenn der Wert nur einmal verwendet wird:</span><span class="sxs-lookup"><span data-stu-id="e80fa-118">If the value is used only once, consider piping:</span></span>
    ```sh
    az vm list --query "[?powerState=='VM running'].name" | grep my_vm
    ```
3. <span data-ttu-id="e80fa-119">Berücksichtigen Sie für Listen die folgenden Vorschläge:</span><span class="sxs-lookup"><span data-stu-id="e80fa-119">For lists consider the following suggestions:</span></span>

   <span data-ttu-id="e80fa-120">Verwenden Sie eine „for“-Schleife, falls Sie weitere Kontrollen für das Ergebnis benötigen:</span><span class="sxs-lookup"><span data-stu-id="e80fa-120">If you need more controls on the result, use "for" loop:</span></span>
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

    <span data-ttu-id="e80fa-121">Verwenden Sie alternativ `xargs` und ggf. das Flag `-P`, um die Vorgänge parallel auszuführen und so die Leistung zu verbessern:</span><span class="sxs-lookup"><span data-stu-id="e80fa-121">Alternatively, use `xargs` and consider using the `-P` flag to run the operations in parallel for improved performance:</span></span>
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | xargs -I {} -P 10 az vm start --ids "{}"
    ```
    <span data-ttu-id="e80fa-122">Darüber hinaus verfügt die Azure CLI noch über integrierte Unterstützung für die Verarbeitung von Befehlen mit mehreren parallelen `--ids`, um den gleichen Effekt wie mit „xargs“ zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-122">Finally, Azure CLI has built-in support to process commands with multiple `--ids` in parallel to achieve the same effect of xargs.</span></span> <span data-ttu-id="e80fa-123">Beachten Sie, dass `@-` zum Abrufen von Werten aus der Pipe verwendet wird:</span><span class="sxs-lookup"><span data-stu-id="e80fa-123">Note that `@-` is used to get values from the pipe:</span></span>
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | az vm start --ids @-
    ```

## <a name="async-operations"></a><span data-ttu-id="e80fa-124">Asynchrone Vorgänge</span><span class="sxs-lookup"><span data-stu-id="e80fa-124">Async operations</span></span>

<span data-ttu-id="e80fa-125">Bei vielen Befehlen und Gruppen werden `--no-wait`-Flags für die zeitintensiven Vorgänge sowie ein dedizierter `wait`-Befehl verfügbar gemacht.</span><span class="sxs-lookup"><span data-stu-id="e80fa-125">Many commands and group expose `--no-wait` flags on their long-running operations as well as a dedicated `wait` command.</span></span> <span data-ttu-id="e80fa-126">Dies ist für bestimmte Szenarien hilfreich:</span><span class="sxs-lookup"><span data-stu-id="e80fa-126">These become handy for certain scenarios:</span></span>

1. <span data-ttu-id="e80fa-127">Bereinigen von Ressourcen, wenn nicht die Bereinigung eines nachfolgenden Vorgangs genutzt wird, z. B. das Löschen einer Ressourcengruppe:</span><span class="sxs-lookup"><span data-stu-id="e80fa-127">Cleaning up resources when you aren't relying on the clean up for some subsequent operation, such as deleting a resource group:</span></span>
    ```sh
    az group delete -n my_rg --no-wait
    ```
2. <span data-ttu-id="e80fa-128">Paralleles Erstellen mehrerer unabhängiger Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-128">When you want to create multiple independent resources in parallel.</span></span> <span data-ttu-id="e80fa-129">Dies ähnelt dem Erstellen von Threads und dem Durchführen des Beitritts:</span><span class="sxs-lookup"><span data-stu-id="e80fa-129">This is similar to creating and joining threads:</span></span>

    ```sh
    az vm create -g my_rg -n vm1 --image centos --no-wait
    az vm create -g my_rg -n vm2 --image centos --no-wait

    subscription=$(az account show --query "id" -otsv)
    vm1_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm1"
    vm2_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm2"
    az vm wait --created --ids $vm1_id $vm2_id
    ```

## <a name="generic-update-arguments"></a><span data-ttu-id="e80fa-130">Generische Updateargumente</span><span class="sxs-lookup"><span data-stu-id="e80fa-130">Generic update arguments</span></span>

<span data-ttu-id="e80fa-131">Die meisten Updatebefehle in der CLI verfügen über die drei folgenden generischen Argumente: `--add`, `--set` und `--remove`.</span><span class="sxs-lookup"><span data-stu-id="e80fa-131">Most update commands in the CLI feature the three generic arguments: `--add`, `--set` and `--remove`.</span></span> <span data-ttu-id="e80fa-132">Diese Argumente sind leistungsfähig, aber häufig nicht so komfortabel wie die stark typisierten Argumente, die in Updatebefehlen normalerweise verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="e80fa-132">These arguments are powerful but often less convenient than the strongly-typed arguments typically featured in update commands.</span></span> <span data-ttu-id="e80fa-133">Die CLI verfügt zur Steigerung der Benutzerfreundlichkeit über stark typisierte Argumente für die meisten gängigen Szenarien. Falls die gewünschte Eigenschaft aber nicht aufgeführt ist, stellen die generischen Updateargumente häufig eine Lösung dar, ohne dass Sie auf ein neues Release warten müssen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-133">The CLI provides strongly-typed arguments for most common scenarios for ease-of-use, but if the property you want to set isn't listed, the generic update arguments will often present a path forward to unblock you without having to wait for a new release.</span></span>

1. <span data-ttu-id="e80fa-134">Da die Syntax für generische Updates nicht sehr benutzerfreundlich ist, ist etwas Geduld gefordert.</span><span class="sxs-lookup"><span data-stu-id="e80fa-134">The generic update syntax isn't the most user friendly, so it will require some patience.</span></span>
2. <span data-ttu-id="e80fa-135">Überprüfen Sie, ob für den Updatebefehl die Gruppe `Generic Update Arguments` verfügbar gemacht wird.</span><span class="sxs-lookup"><span data-stu-id="e80fa-135">Verify whether the update command has the `Generic Update Arguments` group exposed.</span></span> <span data-ttu-id="e80fa-136">Wenn nicht, sollten Sie ein Problem melden. Falls die Gruppe verfügbar ist, können Sie versuchen, sie für das Szenario zu nutzen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-136">If not, you'll need to file an issue, but if they are you can attempt you scenario using them.</span></span>
3. <span data-ttu-id="e80fa-137">Verwenden Sie den Befehl `show` für die gewünschte Ressource, um zu ermitteln, welchen Pfad Sie in den generischen Argumenten angeben sollten.</span><span class="sxs-lookup"><span data-stu-id="e80fa-137">Use the `show` command on the resource you are interested in to figure out what path you should supply in the generic arguments.</span></span> <span data-ttu-id="e80fa-138">Führen Sie vor dem Ausprobieren von `az vm update` beispielsweise `az vm show` aus, um den richtigen Pfad zu ermitteln.</span><span class="sxs-lookup"><span data-stu-id="e80fa-138">For example, before you try out `az vm update`, run `az vm show` to determine the right path.</span></span> <span data-ttu-id="e80fa-139">Im Allgemeinen verwenden Sie die Punktsyntax, um auf die Wörterbucheigenschaften zuzugreifen, und Klammern für die Indizierung in Listen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-139">Generally, you will use dot syntax to access dictionary properties and brackets to index into lists.</span></span>
4. <span data-ttu-id="e80fa-140">Sehen Sie sich die Arbeitsbeispiele an, um zu beginnen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-140">Check out working examples to get started.</span></span> <span data-ttu-id="e80fa-141">Gute Beispiele finden Sie unter `az vm update -h`.</span><span class="sxs-lookup"><span data-stu-id="e80fa-141">`az vm update -h` has good ones.</span></span>
5. <span data-ttu-id="e80fa-142">Für `--set` und `--add` wird eine Liste mit Schlüssel-Wert-Paaren im Format `<key1>=<value1> <key2>=<value2>` verwendet.</span><span class="sxs-lookup"><span data-stu-id="e80fa-142">`--set` and `--add` take a list of key value pairs in the format of `<key1>=<value1> <key2>=<value2>`.</span></span> <span data-ttu-id="e80fa-143">Verwenden Sie diese zum Erstellen von nicht trivialen Nutzlasten.</span><span class="sxs-lookup"><span data-stu-id="e80fa-143">Use them to construct non- trivial payloads.</span></span> <span data-ttu-id="e80fa-144">Falls die Syntax zu unübersichtlich wird, können Sie die Verwendung einer JSON-Zeichenfolge erwägen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-144">If the syntax gets too message, consider using a JSON string.</span></span> <span data-ttu-id="e80fa-145">Ein Beispiel hierfür ist das Anfügen eines neuen Datenträgers an eine VM:</span><span class="sxs-lookup"><span data-stu-id="e80fa-145">For example, to attach a new data disk to a VM:</span></span>
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks "{\"createOption\": \"Attach\", \"managedDisk\": {\"id\": \"/subscriptions/0b1f6471-1bf0-4dda-aec3-cb9272f09590/resourceGroups/yg/providers/Microsoft.Compute/disks/yg-disk\"}, \"lun\": 1}"
    ```
6. <span data-ttu-id="e80fa-146">Unter Umständen ist es für Sie auch besser, die `@{file}`-Konvention der CLI zu nutzen, bei der der JSON-Code in eine Datei eingefügt und dann geladen wird.</span><span class="sxs-lookup"><span data-stu-id="e80fa-146">You may find it more useful to leverage the CLI's `@{file}` convention, putting the JSON into a file and loading it.</span></span> <span data-ttu-id="e80fa-147">Hierdurch wird der obige Befehl vereinfacht:</span><span class="sxs-lookup"><span data-stu-id="e80fa-147">This simplifies the above command to:</span></span>
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks @~/my_disk.json
    ```

## <a name="generic-resource-commands---az-resource"></a><span data-ttu-id="e80fa-148">Generische Ressourcenbefehle: `az resource`</span><span class="sxs-lookup"><span data-stu-id="e80fa-148">Generic resource commands - `az resource`</span></span>

<span data-ttu-id="e80fa-149">Es kann vorkommen, das für einen Dienst, an dem Sie interessiert sind, keine CLI-Befehlsabdeckung besteht.</span><span class="sxs-lookup"><span data-stu-id="e80fa-149">There may be cases where a service you are interested in does not have CLI command coverage.</span></span> <span data-ttu-id="e80fa-150">Sie können die Befehle `az resource create/show/list/delete/update/invoke-action` verwenden, um mit diesen Ressourcen zu arbeiten.</span><span class="sxs-lookup"><span data-stu-id="e80fa-150">You can use the `az resource create/show/list/delete/update/invoke-action` commands to work with these resources.</span></span> <span data-ttu-id="e80fa-151">Hier sind einige Vorschläge angegeben:</span><span class="sxs-lookup"><span data-stu-id="e80fa-151">Here are a few suggestions:</span></span>
1. <span data-ttu-id="e80fa-152">Wenn es nur um `create/update` geht, können Sie erwägen, `az group deployment create` zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="e80fa-152">If only `create/update` are involved, consider using `az group deployment create`.</span></span> <span data-ttu-id="e80fa-153">Nutzen Sie [Azure-Schnellstartvorlagen](https://github.com/Azure/azure-quickstart-templates) für Arbeitsbeispiele.</span><span class="sxs-lookup"><span data-stu-id="e80fa-153">Leverage [Azure Quickstart Templates](https://github.com/Azure/azure-quickstart-templates) for working examples.</span></span>
2. <span data-ttu-id="e80fa-154">Sehen Sie sich die REST-API-Referenz zu den Bereichen Anforderungsnutzlast, URL und API-Version an.</span><span class="sxs-lookup"><span data-stu-id="e80fa-154">Check out the Rest API reference for the request payload, URL and API version.</span></span> <span data-ttu-id="e80fa-155">Lesen Sie beispielsweise in der Community die Kommentare zum [Erstellen von AppInsights](https://github.com/Azure/azure-cli/issues/5543).</span><span class="sxs-lookup"><span data-stu-id="e80fa-155">As an example, check out the community's comments on [how to create AppInsights](https://github.com/Azure/azure-cli/issues/5543).</span></span>

## <a name="rest-api-command---az-rest"></a><span data-ttu-id="e80fa-156">REST-API-Befehl: `az rest`</span><span class="sxs-lookup"><span data-stu-id="e80fa-156">REST API command - `az rest`</span></span>

<span data-ttu-id="e80fa-157">Falls Ihre Anforderungen weder durch generische Updateargumente noch durch `az resource` erfüllt werden, können Sie die REST-API mit dem Befehl `az rest` aufrufen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-157">If neither generic update arguments nor `az resource` meets your needs, you can use `az rest` command to call the REST API.</span></span> <span data-ttu-id="e80fa-158">Hierbei wird die Authentifizierung automatisch mit den bereits eingegebenen Anmeldeinformationen durchgeführt und der Header `Content-Type: application/json` festgelegt.</span><span class="sxs-lookup"><span data-stu-id="e80fa-158">It automatically authenticates using the logged-in credential and sets header `Content-Type: application/json`.</span></span>

<span data-ttu-id="e80fa-159">Dies ist äußerst hilfreich, um die [Microsoft Graph-API](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-1.0) aufzurufen, die von CLI-Befehlen derzeit nicht unterstützt wird ([#12946](https://github.com/Azure/azure-cli/issues/12946)).</span><span class="sxs-lookup"><span data-stu-id="e80fa-159">This is extremely useful for calling [Microsoft Graph API](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-1.0) which is not currently supported by CLI commands ([#12946](https://github.com/Azure/azure-cli/issues/12946)).</span></span>

<span data-ttu-id="e80fa-160">Um beispielsweise `redirectUris` für eine [Anwendung](/graph/api/resources/application?view=graph-rest-1.0) aufzurufen, rufen wir die REST-API für die [Updateanwendung](/graph/api/application-update?view=graph-rest-1.0&tabs=http) wie folgt auf:</span><span class="sxs-lookup"><span data-stu-id="e80fa-160">For example, to update `redirectUris` for an [Application](/graph/api/resources/application?view=graph-rest-1.0), we call the [Update application](/graph/api/application-update?view=graph-rest-1.0&tabs=http) REST API with:</span></span>

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

<span data-ttu-id="e80fa-161">Bei Verwendung von `--uri-parameters` für Anforderungen in Form von OData sollten Sie darauf achten, `$` in unterschiedlichen Umgebungen mit Escapezeichen zu versehen: in `Bash` sollte `$` zu `\$` werden, und in `PowerShell` sollte `$` zu `` `$`` werden.</span><span class="sxs-lookup"><span data-stu-id="e80fa-161">When using `--uri-parameters` for requests in the form of OData, please make sure to escape `$` in different environments: in `Bash`, escape `$` as `\$` and in `PowerShell`, escape `$` as `` `$``</span></span>

## <a name="quoting-issues"></a><span data-ttu-id="e80fa-162">Probleme mit Anführungszeichen</span><span class="sxs-lookup"><span data-stu-id="e80fa-162">Quoting issues</span></span>

<span data-ttu-id="e80fa-163">Ein Problem kann sich ergeben, weil die Anführungszeichen und Leerzeichen von der Befehlsshell (Bash, Zsh, Windows-Eingabeaufforderung, PowerShell usw.) interpretiert werden, wenn diese den CLI-Befehl analysiert.</span><span class="sxs-lookup"><span data-stu-id="e80fa-163">This becomes an issue because when the command shell (Bash, Zsh, Windows Command Prompt, PowerShell, etc) parses the CLI command, it will interpret the quotes and spaces.</span></span> <span data-ttu-id="e80fa-164">Sehen Sie immer in den Dokumenten nach, wenn Sie bei der Nutzung einer Shell unsicher sind:</span><span class="sxs-lookup"><span data-stu-id="e80fa-164">Always refer to the documents when you are uncertain about the usage of a shell:</span></span>

- <span data-ttu-id="e80fa-165">Bash: [Anführungszeichen](https://www.gnu.org/software/bash/manual/html_node/Quoting.html)</span><span class="sxs-lookup"><span data-stu-id="e80fa-165">Bash: [Quoting](https://www.gnu.org/software/bash/manual/html_node/Quoting.html)</span></span>
- <span data-ttu-id="e80fa-166">PowerShell: [Informationen zu Regeln für Anführungszeichen](/powershell/module/microsoft.powershell.core/about/about_quoting_rules)</span><span class="sxs-lookup"><span data-stu-id="e80fa-166">PowerShell: [About Quoting Rules](/powershell/module/microsoft.powershell.core/about/about_quoting_rules)</span></span>
    - <span data-ttu-id="e80fa-167">Aufgrund des bekannten Problems [#1995](https://github.com/PowerShell/PowerShell/issues/1995) von PowerShell gelten für Escapezeichen einige zusätzliche Regeln.</span><span class="sxs-lookup"><span data-stu-id="e80fa-167">Due to a known issue [#1995](https://github.com/PowerShell/PowerShell/issues/1995) of PowerShell, some extra escaping rules apply.</span></span> <span data-ttu-id="e80fa-168">Weitere Informationen finden Sie unter [Probleme mit Anführungszeichen bei PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md).</span><span class="sxs-lookup"><span data-stu-id="e80fa-168">See [Quoting issues with PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md) for more information.</span></span>
- <span data-ttu-id="e80fa-169">Windows-Eingabeaufforderung: [Gewusst wie: Escapezeichen, Trennzeichen und Anführungszeichen in der Windows-Befehlszeile](https://ss64.com/nt/syntax-esc.html)</span><span class="sxs-lookup"><span data-stu-id="e80fa-169">Windows Command Prompt: [How-to: Escape Characters, Delimiters and Quotes at the Windows command line](https://ss64.com/nt/syntax-esc.html)</span></span>

<span data-ttu-id="e80fa-170">Hier sind einige Vorschläge angegeben, mit denen unerwartete Ergebnisse vermieden werden können:</span><span class="sxs-lookup"><span data-stu-id="e80fa-170">To avoid unanticipated results, here are a few suggestions:</span></span>

1. <span data-ttu-id="e80fa-171">Wenn der Wert Leerzeichen enthält, müssen Sie ihn in Anführungszeichen einschließen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-171">If the value contains whitespace, you must wrap it in quotes.</span></span>
2. <span data-ttu-id="e80fa-172">In Bash und Windows PowerShell werden sowohl einfache als auch doppelte Anführungszeichen interpretiert, während in der Windows-Eingabeaufforderung nur doppelte Anführungszeichen verarbeitet werden. Dies bedeutet, dass einzelne Anführungszeichen als Teil des Werts interpretiert werden.</span><span class="sxs-lookup"><span data-stu-id="e80fa-172">In bash or Windows PowerShell, both single and double quotes will be interpreted, while in Windows Command Prompt, only double quotes are handled which means single quotes will be interpreted as a part of the value.</span></span>
3. <span data-ttu-id="e80fa-173">Falls Ihr Befehl nur in Bash (oder Zsh) ausgeführt wird, haben einfache Anführungszeichen den Vorteil, dass der darin eingeschlossene Inhalt beibehalten wird.</span><span class="sxs-lookup"><span data-stu-id="e80fa-173">If your command only runs on Bash (or Zsh), using single quotes has the benefit of preserving the content inside.</span></span> <span data-ttu-id="e80fa-174">Dies kann sehr hilfreich sein, wenn Sie JSON-Code inline angeben.</span><span class="sxs-lookup"><span data-stu-id="e80fa-174">This can be very helpful when supplying inline JSON.</span></span> <span data-ttu-id="e80fa-175">Beispielsweise funktioniert dies in Bash wie folgt: `'{"foo": "bar"}'`</span><span class="sxs-lookup"><span data-stu-id="e80fa-175">For example this works in bash: `'{"foo": "bar"}'`</span></span>
4. <span data-ttu-id="e80fa-176">Wenn Ihr Befehl über die Windows-Eingabeaufforderung ausgeführt wird, müssen Sie ausschließlich doppelte Anführungszeichen verwenden.</span><span class="sxs-lookup"><span data-stu-id="e80fa-176">If your command will run on Windows Command Prompt, you must use double quotes exclusively.</span></span> <span data-ttu-id="e80fa-177">Falls der Wert doppelte Anführungszeichen enthält, müssen Sie ihn mit Escapezeichen versehen: `"i like to use \" a lot"`.</span><span class="sxs-lookup"><span data-stu-id="e80fa-177">If the value contains double quotes, you must escape it: `"i like to use \" a lot"`.</span></span> <span data-ttu-id="e80fa-178">Die Entsprechung des obigen Codes für die Eingabeaufforderung lautet: `"{\"foo\": \"bar\"}"`</span><span class="sxs-lookup"><span data-stu-id="e80fa-178">The Command Prompt equivalent of the above would be: `"{\"foo\": \"bar\"}"`</span></span>
5. <span data-ttu-id="e80fa-179">In Bash werden exportierte Variablen ausgewertet, die in doppelten Anführungszeichen stehen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-179">Exported variables in bash inside double quotes will be evaluated.</span></span> <span data-ttu-id="e80fa-180">Falls Sie dies nicht wünschen, sollten sie wiederum Escapezeichen der Form `\ ` verwenden, z. B. in `"\$var"`. Sie können auch einfache Anführungszeichen verwenden, z. B. `'$var'`.</span><span class="sxs-lookup"><span data-stu-id="e80fa-180">If this is not what you want, again use `\ ` to escape it like `"\$var"` or use single quotes `'$var'`.</span></span>
6. <span data-ttu-id="e80fa-181">Für einige CLI-Argumente, z. B. die generischen Updateargumente, wird eine Liste mit durch Leerzeichen getrennten Werten verwendet, z. B. `<key1>=<value1> <key2>=<value2>`.</span><span class="sxs-lookup"><span data-stu-id="e80fa-181">A few CLI arguments, including the generic update arguments, take a list of space-separated values, like `<key1>=<value1> <key2>=<value2>`.</span></span> <span data-ttu-id="e80fa-182">Da für den Schlüsselnamen und -wert eine beliebige Zeichenfolge verwendet werden kann, die unter Umständen Leerzeichen enthält, müssen Anführungszeichen genutzt werden.</span><span class="sxs-lookup"><span data-stu-id="e80fa-182">Since the key name and value can take arbitrary string which might contain whitespace, using quotes will be necessary.</span></span> <span data-ttu-id="e80fa-183">Umschließen Sie das Paar, und nicht nur den Schlüssel bzw. den Wert.</span><span class="sxs-lookup"><span data-stu-id="e80fa-183">Wrap the pair, not individual key or value.</span></span> <span data-ttu-id="e80fa-184">`"my name"=john` ist also nicht richtig.</span><span class="sxs-lookup"><span data-stu-id="e80fa-184">So `"my name"=john` is wrong.</span></span> <span data-ttu-id="e80fa-185">Verwenden Sie stattdessen `"my name=john"`.</span><span class="sxs-lookup"><span data-stu-id="e80fa-185">Instead, use `"my name=john"`.</span></span> <span data-ttu-id="e80fa-186">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="e80fa-186">For example:</span></span>
    ```sh
    az webapp config appsettings set -g my_rg -n my_web --settings "client id=id1" "my name=john"
    ```
7. <span data-ttu-id="e80fa-187">Verwenden Sie die `@<file>`-Konvention der CLI für das Laden aus der Datei, um die Interpretationsmechanismen der Shell zu umgehen:</span><span class="sxs-lookup"><span data-stu-id="e80fa-187">Use CLI's `@<file>` convention to load from a file so to bypass the shell's interpretation mechanisms:</span></span>
    ```sh
    az ad app create --display-name my-native --native-app --required-resource-accesses @manifest.json
    ```
8. <span data-ttu-id="e80fa-188">Wenn für ein CLI-Argument angegeben ist, dass eine durch Leerzeichen getrennte Liste akzeptiert wird, sind die folgenden Formate zulässig:</span><span class="sxs-lookup"><span data-stu-id="e80fa-188">When a CLI argument says it accepts a space-separated list, these are the formats accepted:</span></span>
    - <span data-ttu-id="e80fa-189">`--arg foo bar`: OK.</span><span class="sxs-lookup"><span data-stu-id="e80fa-189">`--arg foo bar`: OK.</span></span> <span data-ttu-id="e80fa-190">Ohne Anführungszeichen, durch Leerzeichen getrennte Liste</span><span class="sxs-lookup"><span data-stu-id="e80fa-190">Unquoted, space-separated list</span></span>
    - <span data-ttu-id="e80fa-191">`--arg "foo" "bar"`: OK: Mit Anführungszeichen, durch Leerzeichen getrennte Liste</span><span class="sxs-lookup"><span data-stu-id="e80fa-191">`--arg "foo" "bar"`: OK: Quoted, space-separated list</span></span>
    - <span data-ttu-id="e80fa-192">`--arg "foo bar"`: NICHT GUT.</span><span class="sxs-lookup"><span data-stu-id="e80fa-192">`--arg "foo bar"`: BAD.</span></span> <span data-ttu-id="e80fa-193">Dies ist eine Zeichenfolge, die ein Leerzeichen enthält, und keine durch Leerzeichen getrennte Liste.</span><span class="sxs-lookup"><span data-stu-id="e80fa-193">This is a string with a space in it, not a space-separated list.</span></span>
9. <span data-ttu-id="e80fa-194">Beim Ausführen von Azure CLI-Befehlen in PowerShell treten Analysefehler auf, wenn die Argumente Sonderzeichen aus PowerShell enthalten, z. B. `@`.</span><span class="sxs-lookup"><span data-stu-id="e80fa-194">When running Azure CLI commands in PowerShell, parsing errors will occur when the arguments contain special characters of PowerShell, such as at `@`.</span></span> <span data-ttu-id="e80fa-195">Sie können dieses Problem beheben, indem Sie vor dem Sonderzeichen als Escapezeichen `` ` `` einfügen oder das Argument in einfache oder doppelte Anführungszeichen (`'`/`"`) setzen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-195">You can solve this problem by adding `` ` `` before the special character to escape it, or by enclosing the argument with single or double quotes `'`/`"`.</span></span> <span data-ttu-id="e80fa-196">`az group deployment create --parameters @parameters.json` funktioniert in PowerShell beispielsweise nicht, weil `@` als [Aufteilungssymbol](/powershell/module/microsoft.powershell.core/about/about_splatting) (Splatting) analysiert wird.</span><span class="sxs-lookup"><span data-stu-id="e80fa-196">For example, `az group deployment create --parameters @parameters.json` doesn't work in PowerShell because `@` is parsed as a [splatting symbol](/powershell/module/microsoft.powershell.core/about/about_splatting).</span></span> <span data-ttu-id="e80fa-197">Zur Behebung können Sie das Argument in `` `@parameters.json`` oder `'@parameters.json'` ändern.</span><span class="sxs-lookup"><span data-stu-id="e80fa-197">To fix this, you may change the argument to `` `@parameters.json`` or `'@parameters.json'`.</span></span>
10. <span data-ttu-id="e80fa-198">Bei Verwendung von `--query` mit einem Befehl müssen einige Zeichen von [JMESPath](https://jmespath.org/specification.html) in der Shell mit Escapezeichen versehen werden.</span><span class="sxs-lookup"><span data-stu-id="e80fa-198">When using `--query` with a command, some characters of [JMESPath](https://jmespath.org/specification.html) need to be escaped in the shell.</span></span> <span data-ttu-id="e80fa-199">Beispiel in Bash:</span><span class="sxs-lookup"><span data-stu-id="e80fa-199">For example, in Bash:</span></span>
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

    <span data-ttu-id="e80fa-200">In der Eingabeaufforderung:</span><span class="sxs-lookup"><span data-stu-id="e80fa-200">In Command Prompt:</span></span>
    ```cmd
    > az version --query "\"azure-cli\""
    "2.5.1"

    > az version --query \"azure-cli\"
    "2.5.1"
    ```

    <span data-ttu-id="e80fa-201">In PowerShell (zusätzliche Escapezeichen erforderlich):</span><span class="sxs-lookup"><span data-stu-id="e80fa-201">In PowerShell (extra escaping is needed):</span></span>
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

11. <span data-ttu-id="e80fa-202">Die beste Möglichkeit zur Behandlung eines Problems mit Anführungszeichen ist die Ausführung des Befehls mit dem Flag `--debug`.</span><span class="sxs-lookup"><span data-stu-id="e80fa-202">The best way to troubleshoot a quoting issue is to run the command with `--debug` flag.</span></span> <span data-ttu-id="e80fa-203">Hiermit werden die Argumente, die von der CLI tatsächlich empfangen werden, in [Python-Syntax](https://docs.python.org/3/tutorial/introduction.html#strings) angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e80fa-203">It reveals the actual arguments received by CLI in [Python's syntax](https://docs.python.org/3/tutorial/introduction.html#strings).</span></span> <span data-ttu-id="e80fa-204">Beispiel in Bash:</span><span class="sxs-lookup"><span data-stu-id="e80fa-204">For example, in Bash:</span></span>

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

## <a name="work-behind-a-proxy"></a><span data-ttu-id="e80fa-205">Verwendung hinter einem Proxy</span><span class="sxs-lookup"><span data-stu-id="e80fa-205">Work behind a proxy</span></span>

<span data-ttu-id="e80fa-206">Ein Proxy wird in Unternehmensnetzwerken häufig im Hintergrund genutzt oder ist aufgrund von Ablaufverfolgungstools wie Fiddler, mitmproxy usw. vorhanden. Wenn für den Proxy selbstsignierte Zertifikate verwendet werden, wird von der Python-Bibliothek mit den Anforderungen ([Requests](https://github.com/kennethreitz/requests)), die von der CLI genutzt wird, Folgendes ausgelöst: `SSLError("bad handshake: Error([('SSL routines', 'tls_process_server_certificate', 'certificate verify failed')],)",)`.</span><span class="sxs-lookup"><span data-stu-id="e80fa-206">Proxy is common behind corporate network or introduced by tracing tools like Fiddler, mitmproxy, etc. If the proxy uses self-signed certificates, the Python [Requests](https://github.com/kennethreitz/requests) library which CLI uses will throw `SSLError("bad handshake: Error([('SSL routines', 'tls_process_server_certificate', 'certificate verify failed')],)",)`.</span></span> <span data-ttu-id="e80fa-207">Es gibt zwei Möglichkeiten, diesen Fehler zu behandeln:</span><span class="sxs-lookup"><span data-stu-id="e80fa-207">There are 2 ways to handle this error:</span></span>

1. <span data-ttu-id="e80fa-208">Legen Sie die Umgebungsvariable `REQUESTS_CA_BUNDLE` auf den Pfad der Bundlezertifikatdatei der Zertifizierungsstelle im PEM-Format fest.</span><span class="sxs-lookup"><span data-stu-id="e80fa-208">Set environment variable `REQUESTS_CA_BUNDLE` to the path of CA bundle certificate file in PEM format.</span></span> <span data-ttu-id="e80fa-209">Wir empfehlen Ihnen diese Vorgehensweise, wenn Sie die CLI häufig hinter einem Unternehmensproxy verwenden.</span><span class="sxs-lookup"><span data-stu-id="e80fa-209">This is recommended if you use CLI frequently behind a corporate proxy.</span></span> <span data-ttu-id="e80fa-210">Die Standardbundledatei der Zertifizierungsstelle, die von der CLI verwendet wird, befindet sich bei Windows unter `C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\certifi\cacert.pem` und bei Linux unter ` /opt/az/lib/python3.6/site-packages/certifi/cacert.pem`.</span><span class="sxs-lookup"><span data-stu-id="e80fa-210">The default CA bundle which CLI uses is located at `C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\certifi\cacert.pem` on Windows and ` /opt/az/lib/python3.6/site-packages/certifi/cacert.pem` on Linux.</span></span> <span data-ttu-id="e80fa-211">Sie können das Zertifikat des Proxyservers an diese Datei anfügen oder den Inhalt in eine andere Zertifikatdatei kopieren und anschließend `REQUESTS_CA_BUNDLE` dafür festlegen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-211">You may append the proxy server's certificate to this file or copy the contents to another certificate file, then set `REQUESTS_CA_BUNDLE` to it.</span></span> <span data-ttu-id="e80fa-212">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="e80fa-212">For example:</span></span>

    ```
    <Original cacert.pem>

    -----BEGIN CERTIFICATE-----
    <Your proxy's certificate here>
    -----END CERTIFICATE-----
    ```

   <span data-ttu-id="e80fa-213">Es wird häufig gefragt, ob die Umgebungsvariablen `HTTP_PROXY` bzw. `HTTPS_PROXY` festgelegt werden sollten. Die Antwort ist, dass dies vom jeweiligen Fall abhängt.</span><span class="sxs-lookup"><span data-stu-id="e80fa-213">A frequent ask is whether or not `HTTP_PROXY` or `HTTPS_PROXY` environment variables should be set, the answer is it depends.</span></span> <span data-ttu-id="e80fa-214">Bei Verwendung von Fiddler unter Windows fungiert die Anwendung beim Start standardmäßig als Systemproxy, sodass Sie nichts festlegen müssen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-214">For Fiddler on Windows, by default it acts as system proxy on start, you don't need to set anything.</span></span> <span data-ttu-id="e80fa-215">Wenn die Option deaktiviert ist oder wenn Sie andere Tools verwenden, die nicht als Systemproxy fungieren, sollten Sie die Variablen festlegen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-215">If the option is off or using other tools which don't work as system proxy, you should set them.</span></span> <span data-ttu-id="e80fa-216">Da fast der gesamte Datenverkehr von der CLI SSL-basiert ist, sollte nur `HTTPS_PROXY` festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="e80fa-216">Since almost all traffic from CLI is SSL-based, only `HTTPS_PROXY` should be set.</span></span> <span data-ttu-id="e80fa-217">Falls Sie unsicher sind, können Sie auch einfach beide Variablen festlegen. Denken Sie aber daran, dies rückgängig zu machen, nachdem der Proxy heruntergefahren wurde.</span><span class="sxs-lookup"><span data-stu-id="e80fa-217">If you are not sure, just set them, but do remember to unset it after the proxy is shut down.</span></span> <span data-ttu-id="e80fa-218">Der Standardwert für Fiddler ist `http://localhost:8888`.</span><span class="sxs-lookup"><span data-stu-id="e80fa-218">For fiddler, the default value is `http://localhost:8888`.</span></span>

   <span data-ttu-id="e80fa-219">Für einige Proxys ist Authentifizierung erforderlich. Daher muss das Format der Umgebungsvariablen `HTTP_PROXY` oder `HTTPS_PROXY` die Authentifizierung beinhalten, z. B. `HTTPS_PROXY="https://username:password@proxy-server:port"`.</span><span class="sxs-lookup"><span data-stu-id="e80fa-219">Some proxies require authentication and therefore the format of the `HTTP_PROXY` or `HTTPS_PROXY` environment variables should include the authentication, e.g., `HTTPS_PROXY="https://username:password@proxy-server:port"`.</span></span> <span data-ttu-id="e80fa-220">Es wird von den zugrunde liegenden Python-Bibliotheken benötigt.</span><span class="sxs-lookup"><span data-stu-id="e80fa-220">This is needed by the underlying python libraries.</span></span> <span data-ttu-id="e80fa-221">Ausführliche Informationen finden Sie unter [Konfigurieren von Proxys für die Azure-Bibliotheken](https://docs.microsoft.com/azure/developer/python/azure-sdk-configure-proxy?tabs=bash).</span><span class="sxs-lookup"><span data-stu-id="e80fa-221">For details, see [How to configure proxies for the Azure libraries](https://docs.microsoft.com/azure/developer/python/azure-sdk-configure-proxy?tabs=bash)</span></span> 

   <span data-ttu-id="e80fa-222">Weitere Informationen finden Sie im [Blog von Stefan](https://blog.jhnr.ch/2018/05/16/working-with-azure-cli-behind-ssl-intercepting-proxy-server/).</span><span class="sxs-lookup"><span data-stu-id="e80fa-222">For other details, check out [Stefan's blog](https://blog.jhnr.ch/2018/05/16/working-with-azure-cli-behind-ssl-intercepting-proxy-server/).</span></span>

2. <span data-ttu-id="e80fa-223">Deaktivieren Sie die Zertifikatüberprüfung für die gesamte Azure CLI, indem Sie die Umgebungsvariable `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION=1` festlegen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-223">Disable the certificate check across Azure CLI by setting environment variable `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION=1`.</span></span> <span data-ttu-id="e80fa-224">Dies ist nicht sicher, aber für kurze Einsätze trotzdem gut geeignet, z. B. die Erfassung einer Netzwerkablaufverfolgung für einen bestimmten Befehl und die sofortige Deaktivierung nach Abschluss des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="e80fa-224">This is not safe, but good for a short period like capturing a network trace for a specific command and promptly turning it off when finished.</span></span> <span data-ttu-id="e80fa-225">Aufgrund von zugrunde liegenden Einschränkungen des SDK funktioniert dies unter Umständen für einige Datenebenenbefehle nicht.</span><span class="sxs-lookup"><span data-stu-id="e80fa-225">This may not work for some data-plane commands due to underlying SDK limitations.</span></span>

## <a name="concurrent-builds"></a><span data-ttu-id="e80fa-226">Gleichzeitige Buildvorgänge</span><span class="sxs-lookup"><span data-stu-id="e80fa-226">Concurrent builds</span></span>

<span data-ttu-id="e80fa-227">Wenn Sie „az“ auf einem Buildcomputer verwenden und mehrere Aufträge parallel ausgeführt werden können, besteht das Risiko, dass die Anmeldetoken für zwei Buildaufträge gemeinsam verwendet werden, falls die Aufträge mit demselben Betriebssystembenutzer ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="e80fa-227">If you are using az on a build machine, and multiple jobs can be run in parallel, then there is a risk that the login tokens are shared between two build jobs is the jobs run as the same OS user.</span></span>  <span data-ttu-id="e80fa-228">Legen Sie zur Vermeidung von Verwechslungen dieser Art AZURE_CONFIG_DIR auf ein Verzeichnis fest, in dem die Anmeldetoken gespeichert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-228">To avoid mix ups like this, set AZURE_CONFIG_DIR to a directory where the login tokens should be stored.</span></span>  <span data-ttu-id="e80fa-229">Hierbei kann es sich um einen zufällig erstellten Ordner oder einfach um den Namen des Jenkins-Arbeitsbereichs handeln, z. B. ```AZURE_CONFIG_DIR=.```.</span><span class="sxs-lookup"><span data-stu-id="e80fa-229">It could be a randomly created folder, or just the name of the jenkins workspace, like this ```AZURE_CONFIG_DIR=.```</span></span>

## <a name="appendix"></a><span data-ttu-id="e80fa-230">Anhang</span><span class="sxs-lookup"><span data-stu-id="e80fa-230">Appendix</span></span>

### <a name="windows-batch-scripts-for-saving-to-variables-and-using-it-later"></a><span data-ttu-id="e80fa-231">Windows-Batchskripts für die Speicherung in Variablen und die spätere Verwendung</span><span class="sxs-lookup"><span data-stu-id="e80fa-231">Windows batch scripts for saving to variables and using it later</span></span>

```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    SET "vm_ids=%%F %vm_ids%"  :: construct the id list
)
az vm stop --ids %vm_ids% :: CLI stops all VMs in parallel
```

### <a name="windows-powershell-scripts-for-saving-to-variables-and-using-it-later"></a><span data-ttu-id="e80fa-232">Windows PowerShell-Skripts für die Speicherung in Variablen und die spätere Verwendung</span><span class="sxs-lookup"><span data-stu-id="e80fa-232">Windows PowerShell scripts for saving to variables and using it later</span></span>

```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
az vm stop --ids $vm_ids # CLI stops all VMs in parallel
```

### <a name="windows-batch-scripts-to-loop-through-a-list"></a><span data-ttu-id="e80fa-233">Windows-Batchskripts zum Durchlaufen einer Liste per Schleifenvorgang</span><span class="sxs-lookup"><span data-stu-id="e80fa-233">Windows batch scripts to loop through a list</span></span>
```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    ECHO Stopping %%F
    az vm stop --ids %%F
)
```

### <a name="windows-powershell-scripts-to-loop-through-a-list"></a><span data-ttu-id="e80fa-234">Windows PowerShell-Skripts zum Durchlaufen einer Liste per Schleifenvorgang</span><span class="sxs-lookup"><span data-stu-id="e80fa-234">Windows PowerShell scripts to loop through a list</span></span>
```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
foreach ($vm_id in $vm_ids) {
    Write-Output "Stopping $vm_id"
    az vm stop --ids $vm_id
}
```

### <a name="cli-environment-variables"></a><span data-ttu-id="e80fa-235">CLI-Umgebungsvariablen</span><span class="sxs-lookup"><span data-stu-id="e80fa-235">CLI Environment Variables</span></span>

|  <span data-ttu-id="e80fa-236">Umgebungsvariable</span><span class="sxs-lookup"><span data-stu-id="e80fa-236">Environment Variable</span></span>          | <span data-ttu-id="e80fa-237">BESCHREIBUNG</span><span class="sxs-lookup"><span data-stu-id="e80fa-237">Description</span></span>            |
|--------------------------------|------------------------|
| <span data-ttu-id="e80fa-238">**AZURE_CONFIG_DIR**</span><span class="sxs-lookup"><span data-stu-id="e80fa-238">**AZURE_CONFIG_DIR**</span></span>           | <span data-ttu-id="e80fa-239">Globales Konfigurationsverzeichnis für Konfigurationsdateien, Protokolle und Telemetriedaten.</span><span class="sxs-lookup"><span data-stu-id="e80fa-239">Global config directory for config files, logs and telemetry.</span></span> <span data-ttu-id="e80fa-240">Wenn nichts angegeben wird, wird standardmäßig `~/.azure` verwendet.</span><span class="sxs-lookup"><span data-stu-id="e80fa-240">If unspecified, defaults to `~/.azure`.</span></span> |
| <span data-ttu-id="e80fa-241">**AZURE_EXTENSION_DIR**</span><span class="sxs-lookup"><span data-stu-id="e80fa-241">**AZURE_EXTENSION_DIR**</span></span>        | <span data-ttu-id="e80fa-242">Installationsverzeichnis für Erweiterungen.</span><span class="sxs-lookup"><span data-stu-id="e80fa-242">Extensions' installation directory.</span></span> <span data-ttu-id="e80fa-243">Wenn nichts angegeben wird, wird standardmäßig das Verzeichnis `cliextensions` im globalen Konfigurationsverzeichnis verwendet.</span><span class="sxs-lookup"><span data-stu-id="e80fa-243">If unspecified, defaults to `cliextensions` directory within the global config directory.</span></span> |

---
title: Aliaserweiterung der Azure CLI 2.0
description: Verwenden der Aliaserweiterung der Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 39996693d6b796c2d9a45cd909121829f00291a8
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/18/2018
ms.locfileid: "34306266"
---
# <a name="the-azure-cli-20-alias-extension"></a><span data-ttu-id="9212d-103">Aliaserweiterung der Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="9212d-103">The Azure CLI 2.0 alias extension</span></span>

<span data-ttu-id="9212d-104">Dank der Aliaserweiterung können Benutzer mithilfe von vorhandenen Befehlen benutzerdefinierte Befehle für die Azure CLI definieren.</span><span class="sxs-lookup"><span data-stu-id="9212d-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="9212d-105">Mit Aliasen können Sie durch die Bereitstellung von Verknüpfungen und die Verwendung von positionellen Argumenten prägnante, einfache Workflows erstellen.</span><span class="sxs-lookup"><span data-stu-id="9212d-105">Aliases help keep your workflow concise and simple by allowing shortcuts and giving you the ability to use positional arguments.</span></span> <span data-ttu-id="9212d-106">Aliase werden von der Jinja2-Vorlagenengine unterstützt und bieten daher sogar erweiterte Argumentverarbeitung.</span><span class="sxs-lookup"><span data-stu-id="9212d-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="9212d-107">Die Aliaserweiterung ist als öffentliche Vorschauversion verfügbar.</span><span class="sxs-lookup"><span data-stu-id="9212d-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="9212d-108">Die Funktionen und das Konfigurationsdateiformat können sich ändern.</span><span class="sxs-lookup"><span data-stu-id="9212d-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="9212d-109">Installieren der Aliaserweiterung</span><span class="sxs-lookup"><span data-stu-id="9212d-109">Install the alias extension</span></span>

<span data-ttu-id="9212d-110">Damit Sie die Aliaserweiterung verwenden können, ist mindestens Version **2.0.28** der Azure CLI erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9212d-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="9212d-111">Führen Sie zum Überprüfen der CLI-Version `az --version` aus.</span><span class="sxs-lookup"><span data-stu-id="9212d-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="9212d-112">Falls Sie die Installation aktualisieren müssen, befolgen Sie die Anweisungen unter [Installieren von Azure CLI 2.0](./install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="9212d-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI 2.0](./install-azure-cli.md).</span></span>

<span data-ttu-id="9212d-113">Installieren Sie die Erweiterung mit dem Befehl [az extension add](/cli/azure/extension#az-extension-add).</span><span class="sxs-lookup"><span data-stu-id="9212d-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli-interactive
az extension add --name alias
```

<span data-ttu-id="9212d-114">Überprüfen Sie die Installation der Erweiterung mithilfe von [az extension list](/cli/azure/extension#az-extension-list).</span><span class="sxs-lookup"><span data-stu-id="9212d-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="9212d-115">Wenn die Aliaserweiterung ordnungsgemäß installiert wurde, ist sie in der Befehlsausgabe aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="9212d-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli-interactive
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```

## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="9212d-116">Sicherstellen, dass die Erweiterung immer auf dem neuesten Stand ist</span><span class="sxs-lookup"><span data-stu-id="9212d-116">Keep the extension up to date</span></span>

<span data-ttu-id="9212d-117">Die Aliaserweiterung befindet sich in der aktiven Entwicklung, und es werden regelmäßig neue Versionen veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="9212d-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="9212d-118">Beim Aktualisieren der CLI werden neue Versionen nicht automatisch installiert.</span><span class="sxs-lookup"><span data-stu-id="9212d-118">New versions are not automatically installed whenever you update the CLI.</span></span> <span data-ttu-id="9212d-119">Installieren Sie die Updates für die Erweiterung mithilfe von [az extension update](/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="9212d-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name alias
```

## <a name="manage-aliases-for-the-azure-cli"></a><span data-ttu-id="9212d-120">Verwalten von Aliasen für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="9212d-120">Manage aliases for the Azure CLI</span></span>

<span data-ttu-id="9212d-121">Mit der Aliaserweiterung werden komfortable und vertraute Befehle für die Verwaltung von Aliasen bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="9212d-121">The alias extension provides convenient and familiar commands to manage aliases.</span></span> <span data-ttu-id="9212d-122">Rufen Sie den Aliasbefehl mit `--help` auf, um alle verfügbaren Befehle und Parameterdetails anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="9212d-122">To view all the available commands and parameter details, invoke the alias command with `--help`.</span></span>

```azurecli-interactive
az alias --help
```

## <a name="create-simple-alias-commands"></a><span data-ttu-id="9212d-123">Erstellen einfacher Aliasbefehle</span><span class="sxs-lookup"><span data-stu-id="9212d-123">Create simple alias commands</span></span>

<span data-ttu-id="9212d-124">Zum einen werden Aliase zum Kürzen vorhandener Befehlsgruppen oder Befehlsnamen verwendet.</span><span class="sxs-lookup"><span data-stu-id="9212d-124">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="9212d-125">Beispielsweise können Sie die Befehlsgruppe `group` auf `rg` und den Befehl `list` auf `ls` verkürzen.</span><span class="sxs-lookup"><span data-stu-id="9212d-125">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```azurecli-interactive
az alias create --name rg --command group
az alias create --name ls --command list
```

<span data-ttu-id="9212d-126">Diese neu definierten Aliase können nun anstelle ihrer Definition verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="9212d-126">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli-interactive
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="9212d-127">Nehmen Sie `az` nicht in den Befehl auf.</span><span class="sxs-lookup"><span data-stu-id="9212d-127">Do not include `az` as part of the command.</span></span>

<span data-ttu-id="9212d-128">Aliase können auch als Verknüpfungen für vollständige Befehle fungieren.</span><span class="sxs-lookup"><span data-stu-id="9212d-128">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="9212d-129">Im nächsten Beispiel werden verfügbare Ressourcengruppen und ihre Speicherorte in der Tabellenausgabe aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="9212d-129">The next example lists available resource groups and their locations in table output:</span></span>

```azurecli-interactive
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

<span data-ttu-id="9212d-130">`ls-groups` kann nun wie jeder andere CLI-Befehl ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="9212d-130">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli-interactive
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="9212d-131">Erstellen eines Aliasbefehls mit Argumenten</span><span class="sxs-lookup"><span data-stu-id="9212d-131">Create an alias command with arguments</span></span>

<span data-ttu-id="9212d-132">Sie können positionelle Argumente auch zu einem Aliasbefehl hinzufügen, indem Sie sie als `{{ arg_name }}` in den Aliasnamen aufnehmen.</span><span class="sxs-lookup"><span data-stu-id="9212d-132">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="9212d-133">Das Leerzeichen in den Klammern ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9212d-133">The whitespace inside the braces is required.</span></span>

```azurecli-interactive
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

<span data-ttu-id="9212d-134">Das nächste Beispiel zeigt, wie Sie mithilfe von positionellen Argumenten die öffentliche IP-Adresse für einen virtuellen Computer abrufen.</span><span class="sxs-lookup"><span data-stu-id="9212d-134">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```azurecli-interactive
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

<span data-ttu-id="9212d-135">Beim Ausführen dieses Befehls übergeben Sie Werte an die positionellen Argumente.</span><span class="sxs-lookup"><span data-stu-id="9212d-135">When running this command, you give values to the positional arguments.</span></span>

```azurecli-interactive
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="9212d-136">Sie können in von Aliasen aufgerufenen Befehlen auch Umgebungsvariablen verwenden, die zur Laufzeit ausgewertet werden.</span><span class="sxs-lookup"><span data-stu-id="9212d-136">You can also use environment variables in commands invoked by aliases, which are evaluated at runtime.</span></span> <span data-ttu-id="9212d-137">Im nächsten Beispiel wird der Alias `create-rg` hinzugefügt, der eine Ressourcengruppe in `eastus` erstellt und ein `owner`-Tag hinzufügt.</span><span class="sxs-lookup"><span data-stu-id="9212d-137">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="9212d-138">Diesem Tag wird der Wert der lokalen Umgebungsvariablen `USER` zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="9212d-138">This tag is assigned the value of the local environment variable `USER`.</span></span>

```azurecli-interactive
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

<span data-ttu-id="9212d-139">Zum Registrieren der Umgebungsvariablen im Befehl des Alias muss das Dollarzeichen (`$`) mit Escapezeichen versehen werden.</span><span class="sxs-lookup"><span data-stu-id="9212d-139">To register the environment variables inside the command of the alias, the dollar sign `$` must be escaped.</span></span>

## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="9212d-140">Verarbeiten von Argumenten mithilfe von Jinja2-Vorlagen</span><span class="sxs-lookup"><span data-stu-id="9212d-140">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="9212d-141">Die Argumentersetzung in der Aliaserweiterung wird von [Jinja2](http://jinja.pocoo.org/docs/2.10/) durchgeführt. Somit haben Sie Vollzugriff auf die Funktionen der Jinja2-Vorlagenengine.</span><span class="sxs-lookup"><span data-stu-id="9212d-141">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/), giving you full access to the capabilities of the Jinja2 template engine.</span></span> <span data-ttu-id="9212d-142">Vorlagen ermöglichen die Ausführung von Aktionen wie Datenextraktion und -ersetzung für Zeichenfolgen.</span><span class="sxs-lookup"><span data-stu-id="9212d-142">Templates allow you to perform actions like data extraction and substitution on strings.</span></span>

<span data-ttu-id="9212d-143">Mit Jinja2-Vorlagen können Sie Aliase schreiben, die andere Argumenttypen akzeptieren als der zugrunde liegende Befehl.</span><span class="sxs-lookup"><span data-stu-id="9212d-143">With Jinja2 templates, you can write aliases which take different types of arguments than the underlying command.</span></span> <span data-ttu-id="9212d-144">Beispielsweise können Sie einen Alias erstellen, der eine Speicher-URL übernimmt.</span><span class="sxs-lookup"><span data-stu-id="9212d-144">For example, you can make an alias which takes a storage URL.</span></span> <span data-ttu-id="9212d-145">Anschließend wird diese URL analysiert, um den Konto- und Containernamen an den Speicherbefehl zu übergeben.</span><span class="sxs-lookup"><span data-stu-id="9212d-145">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```azurecli-interactive
az alias create \
    --name 'storage-ls {{ url }}' \
    --command "storage blob list
        --account-name {{ url.replace('https://', '').split('.')[0] }}
        --container-name {{ url.replace('https://', '').split('/')[1] }}"
```

<span data-ttu-id="9212d-146">Informationen zur Jinja2-Vorlagenengine finden Sie in der [Jinja2-Dokumentation](http://jinja.pocoo.org/docs/2.10/templates/).</span><span class="sxs-lookup"><span data-stu-id="9212d-146">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>

## <a name="alias-configuration-file"></a><span data-ttu-id="9212d-147">Aliaskonfigurationsdatei</span><span class="sxs-lookup"><span data-stu-id="9212d-147">Alias configuration file</span></span>

<span data-ttu-id="9212d-148">Eine weitere Möglichkeit zum Erstellen und Ändern von Aliasen ist das Ändern der Aliaskonfigurationsdatei.</span><span class="sxs-lookup"><span data-stu-id="9212d-148">Another way to create and modify aliases is to alter the alias configuration file.</span></span> <span data-ttu-id="9212d-149">Aliasbefehlsdefinitionen werden in eine Konfigurationsdatei unter `$AZURE_USER_CONFIG/alias` geschrieben.</span><span class="sxs-lookup"><span data-stu-id="9212d-149">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="9212d-150">`AZURE_USER_CONFIG` hat standardmäßig den Wert `$HOME/.azure` (macOS und Linux) bzw. `%USERPROFILE%\.azure` (Windows).</span><span class="sxs-lookup"><span data-stu-id="9212d-150">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="9212d-151">Die Aliaskonfigurationsdatei wird im INI-Konfigurationsdateiformat geschrieben.</span><span class="sxs-lookup"><span data-stu-id="9212d-151">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="9212d-152">Das Format für Aliasbefehle lautet wie folgt:</span><span class="sxs-lookup"><span data-stu-id="9212d-152">The format for alias commands is:</span></span>

```ini
[alias_name]
command = invoked_commands
```

<span data-ttu-id="9212d-153">Für Aliase, die positionelle Argumente enthalten, haben die Aliasbefehle das folgende Format:</span><span class="sxs-lookup"><span data-stu-id="9212d-153">For aliases that contain positional arguments, the format for alias commands is:</span></span>

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```

## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a><span data-ttu-id="9212d-154">Erstellen eines Aliasbefehls mit Argumenten über die Aliaskonfigurationsdatei</span><span class="sxs-lookup"><span data-stu-id="9212d-154">Create an alias command with arguments via the alias configuration file</span></span>

<span data-ttu-id="9212d-155">Unten ist eine Aliaskonfigurationsdatei angegeben, die ein Beispiel für einen Aliasbefehl mit Argumenten enthält, mit dem die öffentliche IP-Adresse für eine VM abgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9212d-155">Below is an alias configuration file that contains an example alias command with arguments, which gets the public IP address for a VM.</span></span> <span data-ttu-id="9212d-156">Stellen Sie sicher, dass sich der aufgerufene Befehl in einer einzelnen Zeile befindet und die gleichen Argumente enthält, die im Alias definiert sind.</span><span class="sxs-lookup"><span data-stu-id="9212d-156">Ensure that the invoked command is in a single line, and contains the same arguments defined in the alias.</span></span>

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="9212d-157">Deinstallieren der Aliaserweiterung</span><span class="sxs-lookup"><span data-stu-id="9212d-157">Uninstall the alias extension</span></span>

<span data-ttu-id="9212d-158">Verwenden Sie zum Deinstallieren der Erweiterung den Befehl [az extension remove](/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="9212d-158">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```azurecli-interactive
az extension remove --name alias
```

<span data-ttu-id="9212d-159">Falls Sie die Erweiterung aufgrund eines Fehlers oder eines anderen Problems deinstalliert haben, melden Sie das Problem über [GitHub](https://github.com/Azure/azure-cli-extensions/issues), damit wir eine Lösung bereitstellen können.</span><span class="sxs-lookup"><span data-stu-id="9212d-159">If you uninstalled due to a bug or other problem with the extension, please [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>

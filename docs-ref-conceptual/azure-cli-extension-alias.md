---
title: Azure CLI-Aliaserweiterung
description: Verwenden der Azure CLI-Aliaserweiterung
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: cc6192c3e78f7bc895ed8f4c2f640aa1bf0e883c
ms.sourcegitcommit: 18973ac471bbd12af2c8f8fa32a233b0abe5b020
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/13/2020
ms.locfileid: "75913664"
---
# <a name="the-azure-cli-alias-extension"></a><span data-ttu-id="f2ee2-103">Azure CLI-Aliaserweiterung</span><span class="sxs-lookup"><span data-stu-id="f2ee2-103">The Azure CLI alias extension</span></span>

<span data-ttu-id="f2ee2-104">Dank der Aliaserweiterung können Benutzer mithilfe von vorhandenen Befehlen benutzerdefinierte Befehle für die Azure CLI definieren.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-104">The alias extension allows users to define custom commands for the Azure CLI by using existing commands.</span></span> <span data-ttu-id="f2ee2-105">Aliase ermöglichen die Verwendung von Verknüpfungen und vereinfachen dadurch Ihren Workflow.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-105">Aliases help keep your workflow simple by allowing shortcuts.</span></span> <span data-ttu-id="f2ee2-106">Aliase werden von der Jinja2-Vorlagenengine unterstützt und bieten daher sogar erweiterte Argumentverarbeitung.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-106">Since aliases are powered by the Jinja2 template engine, they even offer advanced argument processing.</span></span>

> [!NOTE]
> <span data-ttu-id="f2ee2-107">Die Aliaserweiterung ist als öffentliche Vorschauversion verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-107">The Alias Extension is in public preview.</span></span> <span data-ttu-id="f2ee2-108">Die Funktionen und das Konfigurationsdateiformat können sich ändern.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-108">The features and configuration file format may change.</span></span>

## <a name="install-the-alias-extension"></a><span data-ttu-id="f2ee2-109">Installieren der Aliaserweiterung</span><span class="sxs-lookup"><span data-stu-id="f2ee2-109">Install the alias extension</span></span>

<span data-ttu-id="f2ee2-110">Damit Sie die Aliaserweiterung verwenden können, ist mindestens Version **2.0.28** der Azure CLI erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-110">The minimum required Azure CLI version to use the alias extension is **2.0.28**.</span></span> <span data-ttu-id="f2ee2-111">Führen Sie zum Überprüfen der CLI-Version `az --version` aus.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-111">To check your CLI version, run `az --version`.</span></span> <span data-ttu-id="f2ee2-112">Falls Sie die Installation aktualisieren müssen, hilft Ihnen die Anleitung unter [Installieren der Azure CLI](./install-azure-cli.md) weiter.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-112">If you need to update your installation,  follow the instructions in [Install the Azure CLI](./install-azure-cli.md).</span></span>

<span data-ttu-id="f2ee2-113">Installieren Sie die Erweiterung mit dem Befehl [az extension add](/cli/azure/extension#az-extension-add).</span><span class="sxs-lookup"><span data-stu-id="f2ee2-113">Install the extension with the [az extension add](/cli/azure/extension#az-extension-add) command.</span></span>

```azurecli-interactive
az extension add --name alias
```

<span data-ttu-id="f2ee2-114">Überprüfen Sie die Installation der Erweiterung mithilfe von [az extension list](/cli/azure/extension#az-extension-list).</span><span class="sxs-lookup"><span data-stu-id="f2ee2-114">Verify the installation of the extension with [az extension list](/cli/azure/extension#az-extension-list).</span></span> <span data-ttu-id="f2ee2-115">Wenn die Aliaserweiterung ordnungsgemäß installiert wurde, ist sie in der Befehlsausgabe aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-115">If the alias extension was installed properly, it's listed in the command output.</span></span>

```azurecli-interactive
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```

## <a name="keep-the-extension-up-to-date"></a><span data-ttu-id="f2ee2-116">Sicherstellen, dass die Erweiterung immer auf dem neuesten Stand ist</span><span class="sxs-lookup"><span data-stu-id="f2ee2-116">Keep the extension up-to-date</span></span>

<span data-ttu-id="f2ee2-117">Die Aliaserweiterung befindet sich in der aktiven Entwicklung, und es werden regelmäßig neue Versionen veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-117">The alias extension is under active development and new versions are released regularly.</span></span> <span data-ttu-id="f2ee2-118">Beim Aktualisieren der CLI werden keine neuen Versionen installiert.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-118">New versions aren't installed when you update the CLI.</span></span> <span data-ttu-id="f2ee2-119">Installieren Sie die Updates für die Erweiterung mithilfe von [az extension update](/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="f2ee2-119">Install the updates for the extension with [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name alias
```

## <a name="manage-aliases-for-the-azure-cli"></a><span data-ttu-id="f2ee2-120">Verwalten von Aliasen für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="f2ee2-120">Manage aliases for the Azure CLI</span></span>

<span data-ttu-id="f2ee2-121">Die Aliaserweiterung ermöglicht das Erstellen und Verwalten von Aliasen für andere CLI-Befehle.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-121">The alias extension lets you create and manage aliases for other CLI commands.</span></span> <span data-ttu-id="f2ee2-122">Führen Sie den Aliasbefehl mit `--help` aus, um alle verfügbaren Befehle und Parameterdetails anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-122">To view all the available commands and parameter details, run the alias command with `--help`.</span></span>

```azurecli-interactive
az alias --help
```

## <a name="create-simple-alias-commands"></a><span data-ttu-id="f2ee2-123">Erstellen einfacher Aliasbefehle</span><span class="sxs-lookup"><span data-stu-id="f2ee2-123">Create simple alias commands</span></span>

<span data-ttu-id="f2ee2-124">Zum einen werden Aliase zum Kürzen vorhandener Befehlsgruppen oder Befehlsnamen verwendet.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-124">One use of aliases is for shortening existing command groups or command names.</span></span> <span data-ttu-id="f2ee2-125">Beispielsweise können Sie die Befehlsgruppe `group` auf `rg` und den Befehl `list` auf `ls` verkürzen.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-125">For example, you can shorten the `group` command group to `rg` and the `list` command to `ls`.</span></span>

```azurecli-interactive
az alias create --name rg --command group
az alias create --name ls --command list
```

<span data-ttu-id="f2ee2-126">Diese neu definierten Aliase können nun anstelle ihrer Definition verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-126">These newly defined aliases can now be used anywhere that their definition would be.</span></span>

```azurecli-interactive
az rg list
az rg ls
az vm ls
```

<span data-ttu-id="f2ee2-127">Nehmen Sie `az` nicht in den Befehl auf.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-127">Do not include `az` as part of the command.</span></span>

<span data-ttu-id="f2ee2-128">Aliase können auch als Verknüpfungen für vollständige Befehle fungieren.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-128">Aliases can also be shortcuts for complete commands.</span></span> <span data-ttu-id="f2ee2-129">Im nächsten Beispiel werden verfügbare Ressourcengruppen und ihre Speicherorte in der Tabellenausgabe aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="f2ee2-129">The next example lists available resource groups and their locations in table output:</span></span>

```azurecli-interactive
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

<span data-ttu-id="f2ee2-130">`ls-groups` kann nun wie jeder andere CLI-Befehl ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-130">Now `ls-groups` can be run like any other CLI command.</span></span>

```azurecli-interactive
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a><span data-ttu-id="f2ee2-131">Erstellen eines Aliasbefehls mit Argumenten</span><span class="sxs-lookup"><span data-stu-id="f2ee2-131">Create an alias command with arguments</span></span>

<span data-ttu-id="f2ee2-132">Sie können positionelle Argumente auch zu einem Aliasbefehl hinzufügen, indem Sie sie als `{{ arg_name }}` in den Aliasnamen aufnehmen.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-132">You can also add positional arguments to an alias command by including them as `{{ arg_name }}` in the alias name.</span></span> <span data-ttu-id="f2ee2-133">Das Leerzeichen in den Klammern ist erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-133">The whitespace inside the braces is required.</span></span>

```azurecli-interactive
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

<span data-ttu-id="f2ee2-134">Das nächste Beispiel zeigt, wie Sie mithilfe von positionellen Argumenten die öffentliche IP-Adresse für einen virtuellen Computer abrufen.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-134">The next example alias shows how to use positional arguments to get the public IP address for a VM.</span></span>

```azurecli-interactive
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

<span data-ttu-id="f2ee2-135">Beim Ausführen dieses Befehls übergeben Sie Werte an die positionellen Argumente.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-135">When running this command, you give values to the positional arguments.</span></span>

```azurecli-interactive
az get-vm-ip MyResourceGroup MyVM
```

<span data-ttu-id="f2ee2-136">Sie können in Aliasbefehlen auch Umgebungsvariablen verwenden, die zur Laufzeit ausgewertet werden.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-136">You can also use environment variables in aliased commands, which are evaluated at runtime.</span></span> <span data-ttu-id="f2ee2-137">Im nächsten Beispiel wird der Alias `create-rg` hinzugefügt, der eine Ressourcengruppe in `eastus` erstellt und ein `owner`-Tag hinzufügt.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-137">The next example adds the `create-rg` alias, which creates a resource group in `eastus` and adds an `owner` tag.</span></span> <span data-ttu-id="f2ee2-138">Diesem Tag wird der Wert der lokalen Umgebungsvariablen `USER` zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-138">This tag is assigned the value of the local environment variable `USER`.</span></span>

```azurecli-interactive
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

<span data-ttu-id="f2ee2-139">Zum Registrieren der Umgebungsvariablen im Befehl des Alias muss das Dollarzeichen (`$`) mit Escapezeichen versehen werden.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-139">To register the environment variables inside the command of the alias, the dollar sign `$` must be escaped.</span></span>

## <a name="process-arguments-using-jinja2-templates"></a><span data-ttu-id="f2ee2-140">Verarbeiten von Argumenten mithilfe von Jinja2-Vorlagen</span><span class="sxs-lookup"><span data-stu-id="f2ee2-140">Process arguments using Jinja2 templates</span></span>

<span data-ttu-id="f2ee2-141">Die Argumentersetzung in der Aliaserweiterung wird von [Jinja2](http://jinja.pocoo.org/docs/2.10/) durchgeführt.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-141">Argument substitution in the alias extension is performed by [Jinja2](http://jinja.pocoo.org/docs/2.10/).</span></span> <span data-ttu-id="f2ee2-142">Jinja2-Vorlagen ermöglichen die Bearbeitung der Argumente.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-142">Jinja2 templates allow for manipulating the arguments.</span></span>

<span data-ttu-id="f2ee2-143">Mit Jinja2-Vorlagen können Sie Aliase schreiben, die andere Argumenttypen akzeptieren als der zugrunde liegende Befehl.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-143">With Jinja2 templates, you can write aliases that take different types of arguments than the underlying command.</span></span> <span data-ttu-id="f2ee2-144">Beispielsweise können Sie einen Alias erstellen, der eine Speicher-URL übernimmt.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-144">For example, you can make an alias that takes a storage URL.</span></span> <span data-ttu-id="f2ee2-145">Anschließend wird diese URL analysiert, um den Konto- und Containernamen an den Speicherbefehl zu übergeben.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-145">Then this URL is parsed to pass the account and container names to the storage command.</span></span>

```azurecli-interactive
az alias create \
    --name 'storage-ls {{ url }}' \
    --command "storage blob list
        --account-name {{ url.replace('https://', '').split('.')[0] }}
        --container-name {{ url.replace('https://', '').split('/')[1] }}"
```

<span data-ttu-id="f2ee2-146">Informationen zur Jinja2-Vorlagenengine finden Sie in der [Jinja2-Dokumentation](http://jinja.pocoo.org/docs/2.10/templates/).</span><span class="sxs-lookup"><span data-stu-id="f2ee2-146">To learn about the Jinja2 template engine, see [the Jinja2 documentation](http://jinja.pocoo.org/docs/2.10/templates/).</span></span>

## <a name="alias-configuration-file"></a><span data-ttu-id="f2ee2-147">Aliaskonfigurationsdatei</span><span class="sxs-lookup"><span data-stu-id="f2ee2-147">Alias configuration file</span></span>

<span data-ttu-id="f2ee2-148">Eine weitere Möglichkeit zum Erstellen und Ändern von Aliasen ist das Ändern der Aliaskonfigurationsdatei.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-148">Another way to create and modify aliases is to alter the alias configuration file.</span></span> <span data-ttu-id="f2ee2-149">Aliasbefehlsdefinitionen werden in eine Konfigurationsdatei unter `$AZURE_USER_CONFIG/alias` geschrieben.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-149">Alias command definitions are written into a configuration file, located at `$AZURE_USER_CONFIG/alias`.</span></span> <span data-ttu-id="f2ee2-150">`AZURE_USER_CONFIG` hat standardmäßig den Wert `$HOME/.azure` (macOS und Linux) bzw. `%USERPROFILE%\.azure` (Windows).</span><span class="sxs-lookup"><span data-stu-id="f2ee2-150">The default value of `AZURE_USER_CONFIG` is `$HOME/.azure` on macOS and Linux, and `%USERPROFILE%\.azure` on Windows.</span></span> <span data-ttu-id="f2ee2-151">Die Aliaskonfigurationsdatei wird im INI-Konfigurationsdateiformat geschrieben.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-151">The alias configuration file is written in the INI configuration file format.</span></span> <span data-ttu-id="f2ee2-152">Das Format für Aliasbefehle lautet wie folgt:</span><span class="sxs-lookup"><span data-stu-id="f2ee2-152">The format for alias commands is:</span></span>

```ini
[alias_name]
command = invoked_commands
```

<span data-ttu-id="f2ee2-153">Für Aliase, die positionelle Argumente enthalten, haben die Aliasbefehle das folgende Format:</span><span class="sxs-lookup"><span data-stu-id="f2ee2-153">For aliases that have positional arguments, the format for alias commands is:</span></span>

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```

## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a><span data-ttu-id="f2ee2-154">Erstellen eines Aliasbefehls mit Argumenten über die Aliaskonfigurationsdatei</span><span class="sxs-lookup"><span data-stu-id="f2ee2-154">Create an alias command with arguments via the alias configuration file</span></span>

<span data-ttu-id="f2ee2-155">Das nächste Beispiel zeigt einen Alias für einen Befehl mit Argumenten.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-155">The next example shows an alias for a command with arguments.</span></span> <span data-ttu-id="f2ee2-156">Dieser Befehl ruft die öffentliche IP-Adresse für einen virtuellen Computer ab.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-156">This command gets the public IP address for a VM.</span></span> <span data-ttu-id="f2ee2-157">Aliasbefehle müssen sich in einer Zeile befinden und alle Argumente im Aliasnamen verwenden.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-157">Aliased commands must all be on a single line, and use all of the arguments in the alias name.</span></span>

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

## <a name="uninstall-the-alias-extension"></a><span data-ttu-id="f2ee2-158">Deinstallieren der Aliaserweiterung</span><span class="sxs-lookup"><span data-stu-id="f2ee2-158">Uninstall the alias extension</span></span>

<span data-ttu-id="f2ee2-159">Verwenden Sie zum Deinstallieren der Erweiterung den Befehl [az extension remove](/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="f2ee2-159">To uninstall the extension, use the [az extension remove](/cli/azure/extension#az-extension-remove) command.</span></span>

```azurecli-interactive
az extension remove --name alias
```

<span data-ttu-id="f2ee2-160">Falls Sie die Erweiterung aufgrund eines Fehlers oder eines anderen Problems deinstalliert haben, melden Sie das Problem über [GitHub](https://github.com/Azure/azure-cli-extensions/issues), damit wir eine Lösung bereitstellen können.</span><span class="sxs-lookup"><span data-stu-id="f2ee2-160">If you uninstalled because a bug or other problem with the extension, [file a GitHub issue](https://github.com/Azure/azure-cli-extensions/issues) so that we can provide a fix.</span></span>

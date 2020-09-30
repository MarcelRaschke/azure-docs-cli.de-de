---
title: Azure CLI-Erweiterungen
description: Verwenden von Erweiterungen mit der Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 08/06/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: a399fde57b85b7e0b46e426d35cb67fd10efed1a
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225744"
---
# <a name="use-extensions-with-azure-cli"></a><span data-ttu-id="3e555-103">Verwenden von Erweiterungen mit der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="3e555-103">Use extensions with Azure CLI</span></span> 

<span data-ttu-id="3e555-104">Die Azure CLI umfasst eine Funktion zum Laden von Erweiterungen.</span><span class="sxs-lookup"><span data-stu-id="3e555-104">The Azure CLI offers the capability to load extensions.</span></span> <span data-ttu-id="3e555-105">Erweiterungen sind Python-Wheels, die zusammen mit der CLI bereitgestellt, aber als CLI-Befehle ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="3e555-105">Extensions are Python wheels that aren't shipped as part of the CLI but run as CLI commands.</span></span>
<span data-ttu-id="3e555-106">Mit Erweiterungen erhalten Sie Zugriff auf experimentelle Befehle und Vorabversionen von Befehlen und können eigene CLIs schreiben.</span><span class="sxs-lookup"><span data-stu-id="3e555-106">With extensions, you gain access to experimental and pre-release commands along with the ability to write your own CLI interfaces.</span></span> <span data-ttu-id="3e555-107">Dieser Artikel behandelt die Verwaltung von Erweiterungen und enthält Antworten auf allgemeine Fragen zu ihrer Verwendung.</span><span class="sxs-lookup"><span data-stu-id="3e555-107">This article covers how to manage extensions and answers common questions about their use.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="3e555-108">Suchen von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="3e555-108">Find extensions</span></span>

<span data-ttu-id="3e555-109">Verwenden Sie den Befehl [az extension list-available](/cli/azure/extension#az-extension-list-available), um die von Microsoft bereitgestellten und verwalteten Erweiterungen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="3e555-109">To see the extensions provided and maintained by Microsoft, use the [az extension list-available](/cli/azure/extension#az-extension-list-available) command.</span></span>

```azurecli-interactive
az extension list-available --output table
```

<span data-ttu-id="3e555-110">Auf der Dokumentationswebsite wird darüber hinaus eine [Liste der Erweiterungen](azure-cli-extensions-list.md) bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="3e555-110">We also host a [list of extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="3e555-111">Installieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="3e555-111">Install extensions</span></span>

### <a name="install-extensions-manually"></a><span data-ttu-id="3e555-112">Manuelles Installieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="3e555-112">Install extensions manually</span></span>

<span data-ttu-id="3e555-113">Nachdem Sie eine zu installierende Erweiterung gefunden haben, können Sie [az extension add](/cli/azure/extension#az-extension-add) verwenden, um sie abzurufen.</span><span class="sxs-lookup"><span data-stu-id="3e555-113">Once you have found an extension to install, use [az extension add](/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="3e555-114">Wenn die Erweiterung in `az extension list-available` aufgeführt wird, können Sie die Erweiterung anhand des Namens installieren.</span><span class="sxs-lookup"><span data-stu-id="3e555-114">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli-interactive
az extension add --name <extension-name>
```

<span data-ttu-id="3e555-115">Wenn die Erweiterung von einer externen Ressource stammt oder Sie über einen direkten Link dafür verfügen, geben Sie die Quell-URL oder den lokalen Pfad an.</span><span class="sxs-lookup"><span data-stu-id="3e555-115">If the extension is from an external resource or you have a direct link to it, provide the source URL or local path.</span></span> <span data-ttu-id="3e555-116">Die Erweiterung _muss_ eine kompilierte Python-Wheeldatei sein.</span><span class="sxs-lookup"><span data-stu-id="3e555-116">The extension _must_ be a compiled Python wheel file.</span></span>

```azurecli-interactive
az extension add --source <URL-or-path>
```

<span data-ttu-id="3e555-117">Nach der Installation einer Erweiterung befindet sich diese unter dem Wert der Shellvariablen `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="3e555-117">Once an extension is installed, it's found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="3e555-118">Wenn diese Variable nicht festgelegt ist, befindet sich der Wert standardmäßig unter `$HOME/.azure/cliextensions` (Linux und macOS) bzw. `%USERPROFILE%\.azure\cliextensions` (Windows).</span><span class="sxs-lookup"><span data-stu-id="3e555-118">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

### <a name="install-extensions-automatically"></a><span data-ttu-id="3e555-119">Automatisches Installieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="3e555-119">Install extensions automatically</span></span>

<span data-ttu-id="3e555-120">Wenn Sie einen nicht installierten Erweiterungsbefehl ausführen, kann die Azure CLI ab der Version `2.10.0` den auszuführenden Befehl erkennen und die Erweiterung automatisch für Sie installieren.</span><span class="sxs-lookup"><span data-stu-id="3e555-120">When you run an extension command that is not installed, the Azure CLI can recognize the command you run, and automatically install the extension for you starting from version `2.10.0`.</span></span> <span data-ttu-id="3e555-121">Diese Funktion wird als **dynamische Installation** bezeichnet und kann in der Konfiguration aktiviert werden.</span><span class="sxs-lookup"><span data-stu-id="3e555-121">This feature, referred to as **dynamic install**, is enabled through configuration.</span></span>
```azurecli-interactive
az config set extension.use_dynamic_install=yes_prompt
```

<span data-ttu-id="3e555-122">Verwenden Sie den folgenden Konfigurationsbefehl, um die dynamische Installation ohne Aufforderung zu aktivieren:</span><span class="sxs-lookup"><span data-stu-id="3e555-122">Use the following configuration command to enable dynamic install without a prompt.</span></span>
```azurecli-interactive
az config set extension.use_dynamic_install=yes_without_prompt
```

<span data-ttu-id="3e555-123">Verwenden Sie den folgenden Konfigurationsbefehl, um die dynamische Installation zu deaktivieren und zum Standardverhalten zurückzukehren:</span><span class="sxs-lookup"><span data-stu-id="3e555-123">Use the following configuration command to turn off the dynamic install feature to revert to the default behavior.</span></span> <span data-ttu-id="3e555-124">Ist die Erweiterung nicht installiert, wird vom Erweiterungsbefehl ein Fehler aufgrund eines nicht gefundenen Befehls zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e555-124">The extension command will return a command-not-found error if the extension is not installed.</span></span>
```azurecli-interactive
az config set extension.use_dynamic_install=no
```

<span data-ttu-id="3e555-125">Erweiterungsbefehle, die eine dynamische Installation initiieren, werden standardmäßig nicht fortgesetzt.</span><span class="sxs-lookup"><span data-stu-id="3e555-125">By default, an extension command that prompts dynamic install will not continue to run.</span></span> <span data-ttu-id="3e555-126">Dieses Standardverhalten kann geändert werden, sodass der jeweilige Befehl weiter ausgeführt wird. Legen Sie hierzu die Eigenschaft `run_after_dynamic_install` auf `yes` fest:</span><span class="sxs-lookup"><span data-stu-id="3e555-126">You can change the default behavior and make the command continue by setting the `run_after_dynamic_install` property to `yes`.</span></span>
```azurecli-interactive
az config set extension.run_after_dynamic_install=yes
```

## <a name="update-extensions"></a><span data-ttu-id="3e555-127">Aktualisieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="3e555-127">Update extensions</span></span>

<span data-ttu-id="3e555-128">Wenn eine Erweiterung anhand des Namens installiert wurde, aktualisieren Sie sie mithilfe von [az extension update](/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="3e555-128">If an extension was installed by name, update it using [az extension update](/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name <extension-name>
```

<span data-ttu-id="3e555-129">Andernfalls kann eine Erweiterung anhand der Quelle gemäß den Anweisungen unter [Installieren von Erweiterungen](#install-extensions) aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="3e555-129">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="3e555-130">Falls der Name einer Erweiterung von der CLI nicht aufgelöst werden kann, deinstallieren Sie die Erweiterung, und installieren Sie sie anschließend erneut.</span><span class="sxs-lookup"><span data-stu-id="3e555-130">If an extension name can't be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="3e555-131">Die Erweiterung kann auch Teil der Basis-CLI geworden sein.</span><span class="sxs-lookup"><span data-stu-id="3e555-131">The extension could also have become part of the base CLI.</span></span>
<span data-ttu-id="3e555-132">Versuchen Sie, die CLI wie unter [Installieren der Azure CLI](install-azure-cli.md) beschrieben zu installieren, und überprüfen Sie, ob die Befehle der Erweiterung hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="3e555-132">Try updating the CLI as described in [Install the Azure CLI](install-azure-cli.md) and see if the extension's commands were added.</span></span>

## <a name="uninstall-extensions"></a><span data-ttu-id="3e555-133">Deinstallieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="3e555-133">Uninstall extensions</span></span>

<span data-ttu-id="3e555-134">Wenn Sie eine Erweiterung nicht mehr benötigen, entfernen Sie sie mit [az extension remove](/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="3e555-134">If you no longer need an extension, remove it with [az extension remove](/cli/azure/extension#az-extension-remove).</span></span>

```azurecli-interactive
az extension remove --name <extension-name>
```

<span data-ttu-id="3e555-135">Sie können eine Erweiterung auch manuell entfernen, indem Sie sie am Installationsspeicherort löschen.</span><span class="sxs-lookup"><span data-stu-id="3e555-135">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="3e555-136">Die Shellvariable `$AZURE_EXTENSION_DIR` legt fest, welche Module installiert werden.</span><span class="sxs-lookup"><span data-stu-id="3e555-136">The `$AZURE_EXTENSION_DIR` shell variable defines where modules are installed.</span></span>
<span data-ttu-id="3e555-137">Wenn diese Variable nicht festgelegt ist, befindet sich der Wert standardmäßig unter `$HOME/.azure/cliextensions` (Linux und macOS) bzw. `%USERPROFILE%\.azure\cliextensions` (Windows).</span><span class="sxs-lookup"><span data-stu-id="3e555-137">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

## <a name="faq"></a><span data-ttu-id="3e555-138">Häufig gestellte Fragen</span><span class="sxs-lookup"><span data-stu-id="3e555-138">FAQ</span></span>

<span data-ttu-id="3e555-139">Hier sind einige Antworten auf andere häufig gestellte Fragen zu CLI-Erweiterungen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="3e555-139">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="3e555-140">Welche Dateiformate sind für die Installation zulässig?</span><span class="sxs-lookup"><span data-stu-id="3e555-140">What file formats are allowed for installation?</span></span>

<span data-ttu-id="3e555-141">Derzeit können nur kompilierte Python-Wheels als Erweiterungen installiert werden.</span><span class="sxs-lookup"><span data-stu-id="3e555-141">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="3e555-142">Können Erweiterungen vorhandene Befehle ersetzen?</span><span class="sxs-lookup"><span data-stu-id="3e555-142">Can extensions replace existing commands?</span></span>

<span data-ttu-id="3e555-143">Ja.</span><span class="sxs-lookup"><span data-stu-id="3e555-143">Yes.</span></span> <span data-ttu-id="3e555-144">Erweiterungen können vorhandene Befehle ersetzen, aber vor dem Ausführen eines ersetzten Befehls wird von der CLI eine Warnung ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="3e555-144">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="3e555-145">Woran erkenne ich, dass es sich bei einer Erweiterung um eine Vorabversion handelt?</span><span class="sxs-lookup"><span data-stu-id="3e555-145">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="3e555-146">Anhand der Dokumentation und der Versionsverwaltung können Sie erkennen, ob es sich bei einer Erweiterung um eine Vorabversion handelt.</span><span class="sxs-lookup"><span data-stu-id="3e555-146">An extension's documentation and versioning will show if it's in pre-release.</span></span> <span data-ttu-id="3e555-147">Microsoft veröffentlicht häufig Vorschaubefehle als CLI-Erweiterungen, damit sie später ggf. in das CLI-Hauptprodukt aufgenommen werden können.</span><span class="sxs-lookup"><span data-stu-id="3e555-147">Microsoft often releases preview commands as CLI extensions, with the option of moving them into the main CLI product later.</span></span> <span data-ttu-id="3e555-148">Wenn Befehle aus Erweiterungen verschoben werden, muss die alte Erweiterung deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="3e555-148">When commands are moved out of extensions, the old extension should be uninstalled.</span></span> 

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="3e555-149">Können Erweiterungen voneinander abhängig sein?</span><span class="sxs-lookup"><span data-stu-id="3e555-149">Can extensions depend upon each other?</span></span>

<span data-ttu-id="3e555-150">Nein.</span><span class="sxs-lookup"><span data-stu-id="3e555-150">No.</span></span> <span data-ttu-id="3e555-151">Da die CLI keine Ladereihenfolge garantiert, werden Abhängigkeiten unter Umständen nicht ordnungsgemäß berücksichtigt.</span><span class="sxs-lookup"><span data-stu-id="3e555-151">Since the CLI doesn't guarantee a load order, dependencies might not be satisfied.</span></span> <span data-ttu-id="3e555-152">Das Entfernen einer Erweiterung wirkt sich nicht auf andere Erweiterungen aus.</span><span class="sxs-lookup"><span data-stu-id="3e555-152">Removing an extension won't affect any others.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="3e555-153">Werden Erweiterungen zusammen mit der CLI aktualisiert?</span><span class="sxs-lookup"><span data-stu-id="3e555-153">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="3e555-154">Nein.</span><span class="sxs-lookup"><span data-stu-id="3e555-154">No.</span></span> <span data-ttu-id="3e555-155">Erweiterungen müssen separat aktualisiert werden, wie unter [Aktualisieren von Erweiterungen](#update-extensions) beschrieben.</span><span class="sxs-lookup"><span data-stu-id="3e555-155">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>

### <a name="how-to-develop-our-own-extension"></a><span data-ttu-id="3e555-156">Wie entwickeln Sie Ihre eigene Erweiterung?</span><span class="sxs-lookup"><span data-stu-id="3e555-156">How to develop our own extension?</span></span>
<span data-ttu-id="3e555-157">Sehen Sie sich das offizielle Repository an, wenn Sie weitere Unterstützung benötigen.</span><span class="sxs-lookup"><span data-stu-id="3e555-157">Please refer to the official repository for more help.</span></span> [<span data-ttu-id="3e555-158">Azure/azure-cli-extensions</span><span class="sxs-lookup"><span data-stu-id="3e555-158">Azure/azure-cli-extensions</span></span>](https://github.com/Azure/azure-cli/tree/master/doc/extensions)
---
title: Azure CLI-Erweiterungen
description: Verwenden von Erweiterungen mit der Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/07/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 73488fc464ed052f22f071f6373fb6b8f682b778
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2020
ms.locfileid: "77779991"
---
# <a name="use-extensions-with-azure-cli"></a><span data-ttu-id="5c738-103">Verwenden von Erweiterungen mit der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="5c738-103">Use extensions with Azure CLI</span></span> 

<span data-ttu-id="5c738-104">Die Azure CLI umfasst eine Funktion zum Laden von Erweiterungen.</span><span class="sxs-lookup"><span data-stu-id="5c738-104">The Azure CLI offers the capability to load extensions.</span></span> <span data-ttu-id="5c738-105">Erweiterungen sind Python-Wheels, die zusammen mit der CLI bereitgestellt, aber als CLI-Befehle ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="5c738-105">Extensions are Python wheels that aren't shipped as part of the CLI but run as CLI commands.</span></span>
<span data-ttu-id="5c738-106">Mit Erweiterungen erhalten Sie Zugriff auf experimentelle Befehle und Vorabversionen von Befehlen und können eigene CLIs schreiben.</span><span class="sxs-lookup"><span data-stu-id="5c738-106">With extensions, you gain access to experimental and pre-release commands along with the ability to write your own CLI interfaces.</span></span> <span data-ttu-id="5c738-107">Dieser Artikel behandelt die Verwaltung von Erweiterungen und enthält Antworten auf allgemeine Fragen zu ihrer Verwendung.</span><span class="sxs-lookup"><span data-stu-id="5c738-107">This article covers how to manage extensions and answers common questions about their use.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="5c738-108">Suchen von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="5c738-108">Find extensions</span></span>

<span data-ttu-id="5c738-109">Verwenden Sie den Befehl [az extension list-available](/cli/azure/extension#az-extension-list-available), um die von Microsoft bereitgestellten und verwalteten Erweiterungen anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="5c738-109">To see the extensions provided and maintained by Microsoft, use the [az extension list-available](/cli/azure/extension#az-extension-list-available) command.</span></span>

```azurecli-interactive
az extension list-available --output table
```

<span data-ttu-id="5c738-110">Auf der Dokumentationswebsite wird darüber hinaus eine [Liste der Erweiterungen](azure-cli-extensions-list.md) bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="5c738-110">We also host a [list of extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="5c738-111">Installieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="5c738-111">Install extensions</span></span>

<span data-ttu-id="5c738-112">Nachdem Sie eine zu installierende Erweiterung gefunden haben, können Sie [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) verwenden, um sie abzurufen.</span><span class="sxs-lookup"><span data-stu-id="5c738-112">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="5c738-113">Wenn die Erweiterung in `az extension list-available` aufgeführt wird, können Sie die Erweiterung anhand des Namens installieren.</span><span class="sxs-lookup"><span data-stu-id="5c738-113">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli-interactive
az extension add --name <extension-name>
```

<span data-ttu-id="5c738-114">Wenn die Erweiterung von einer externen Ressource stammt oder Sie über einen direkten Link dafür verfügen, geben Sie die Quell-URL oder den lokalen Pfad an.</span><span class="sxs-lookup"><span data-stu-id="5c738-114">If the extension is from an external resource or you have a direct link to it, provide the source URL or local path.</span></span> <span data-ttu-id="5c738-115">Die Erweiterung _muss_ eine kompilierte Python-Wheeldatei sein.</span><span class="sxs-lookup"><span data-stu-id="5c738-115">The extension _must_ be a compiled Python wheel file.</span></span>

```azurecli-interactive
az extension add --source <URL-or-path>
```

<span data-ttu-id="5c738-116">Nach der Installation einer Erweiterung befindet sich diese unter dem Wert der Shellvariablen `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="5c738-116">Once an extension is installed, it's found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="5c738-117">Wenn diese Variable nicht festgelegt ist, befindet sich der Wert standardmäßig unter `$HOME/.azure/cliextensions` (Linux und macOS) bzw. `%USERPROFILE%\.azure\cliextensions` (Windows).</span><span class="sxs-lookup"><span data-stu-id="5c738-117">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="update-extensions"></a><span data-ttu-id="5c738-118">Aktualisieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="5c738-118">Update extensions</span></span>

<span data-ttu-id="5c738-119">Wenn eine Erweiterung anhand des Namens installiert wurde, aktualisieren Sie sie mithilfe von [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span><span class="sxs-lookup"><span data-stu-id="5c738-119">If an extension was installed by name, update it using [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name <extension-name>
```

<span data-ttu-id="5c738-120">Andernfalls kann eine Erweiterung anhand der Quelle gemäß den Anweisungen unter [Installieren von Erweiterungen](#install-extensions) aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="5c738-120">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="5c738-121">Falls der Name einer Erweiterung von der CLI nicht aufgelöst werden kann, deinstallieren Sie die Erweiterung, und installieren Sie sie anschließend erneut.</span><span class="sxs-lookup"><span data-stu-id="5c738-121">If an extension name can't be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="5c738-122">Die Erweiterung kann auch Teil der Basis-CLI geworden sein.</span><span class="sxs-lookup"><span data-stu-id="5c738-122">The extension could also have become part of the base CLI.</span></span>
<span data-ttu-id="5c738-123">Versuchen Sie, die CLI wie unter [Installieren der Azure CLI](install-azure-cli.md) beschrieben zu installieren, und überprüfen Sie, ob die Befehle der Erweiterung hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="5c738-123">Try updating the CLI as described in [Install the Azure CLI](install-azure-cli.md) and see if the extension's commands were added.</span></span>

## <a name="uninstall-extensions"></a><span data-ttu-id="5c738-124">Deinstallieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="5c738-124">Uninstall extensions</span></span>

<span data-ttu-id="5c738-125">Wenn Sie eine Erweiterung nicht mehr benötigen, entfernen Sie sie mit [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span><span class="sxs-lookup"><span data-stu-id="5c738-125">If you no longer need an extension, remove it with [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span></span>

```azurecli-interactive
az extension remove --name <extension-name>
```

<span data-ttu-id="5c738-126">Sie können eine Erweiterung auch manuell entfernen, indem Sie sie am Installationsspeicherort löschen.</span><span class="sxs-lookup"><span data-stu-id="5c738-126">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="5c738-127">Die Shellvariable `$AZURE_EXTENSION_DIR` legt fest, welche Module installiert werden.</span><span class="sxs-lookup"><span data-stu-id="5c738-127">The `$AZURE_EXTENSION_DIR` shell variable defines where modules are installed.</span></span>
<span data-ttu-id="5c738-128">Wenn diese Variable nicht festgelegt ist, befindet sich der Wert standardmäßig unter `$HOME/.azure/cliextensions` (Linux und macOS) bzw. `%USERPROFILE%\.azure\cliextensions` (Windows).</span><span class="sxs-lookup"><span data-stu-id="5c738-128">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

## <a name="faq"></a><span data-ttu-id="5c738-129">Häufig gestellte Fragen</span><span class="sxs-lookup"><span data-stu-id="5c738-129">FAQ</span></span>

<span data-ttu-id="5c738-130">Hier sind einige Antworten auf andere häufig gestellte Fragen zu CLI-Erweiterungen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="5c738-130">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="5c738-131">Welche Dateiformate sind für die Installation zulässig?</span><span class="sxs-lookup"><span data-stu-id="5c738-131">What file formats are allowed for installation?</span></span>

<span data-ttu-id="5c738-132">Derzeit können nur kompilierte Python-Wheels als Erweiterungen installiert werden.</span><span class="sxs-lookup"><span data-stu-id="5c738-132">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="5c738-133">Können Erweiterungen vorhandene Befehle ersetzen?</span><span class="sxs-lookup"><span data-stu-id="5c738-133">Can extensions replace existing commands?</span></span>

<span data-ttu-id="5c738-134">Ja.</span><span class="sxs-lookup"><span data-stu-id="5c738-134">Yes.</span></span> <span data-ttu-id="5c738-135">Erweiterungen können vorhandene Befehle ersetzen, aber vor dem Ausführen eines ersetzten Befehls wird von der CLI eine Warnung ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="5c738-135">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="5c738-136">Woran erkenne ich, dass es sich bei einer Erweiterung um eine Vorabversion handelt?</span><span class="sxs-lookup"><span data-stu-id="5c738-136">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="5c738-137">Anhand der Dokumentation und der Versionsverwaltung können Sie erkennen, ob es sich bei einer Erweiterung um eine Vorabversion handelt.</span><span class="sxs-lookup"><span data-stu-id="5c738-137">An extension's documentation and versioning will show if it's in pre-release.</span></span> <span data-ttu-id="5c738-138">Microsoft veröffentlicht häufig Vorschaubefehle als CLI-Erweiterungen, damit sie später ggf. in das CLI-Hauptprodukt aufgenommen werden können.</span><span class="sxs-lookup"><span data-stu-id="5c738-138">Microsoft often releases preview commands as CLI extensions, with the option of moving them into the main CLI product later.</span></span> <span data-ttu-id="5c738-139">Wenn Befehle aus Erweiterungen verschoben werden, muss die alte Erweiterung deinstalliert werden.</span><span class="sxs-lookup"><span data-stu-id="5c738-139">When commands are moved out of extensions, the old extension should be uninstalled.</span></span> 

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="5c738-140">Können Erweiterungen voneinander abhängig sein?</span><span class="sxs-lookup"><span data-stu-id="5c738-140">Can extensions depend upon each other?</span></span>

<span data-ttu-id="5c738-141">Nein.</span><span class="sxs-lookup"><span data-stu-id="5c738-141">No.</span></span> <span data-ttu-id="5c738-142">Da die CLI keine Ladereihenfolge garantiert, werden Abhängigkeiten unter Umständen nicht ordnungsgemäß berücksichtigt.</span><span class="sxs-lookup"><span data-stu-id="5c738-142">Since the CLI doesn't guarantee a load order, dependencies might not be satisfied.</span></span> <span data-ttu-id="5c738-143">Das Entfernen einer Erweiterung wirkt sich nicht auf andere Erweiterungen aus.</span><span class="sxs-lookup"><span data-stu-id="5c738-143">Removing an extension won't affect any others.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="5c738-144">Werden Erweiterungen zusammen mit der CLI aktualisiert?</span><span class="sxs-lookup"><span data-stu-id="5c738-144">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="5c738-145">Nein.</span><span class="sxs-lookup"><span data-stu-id="5c738-145">No.</span></span> <span data-ttu-id="5c738-146">Erweiterungen müssen separat aktualisiert werden, wie unter [Aktualisieren von Erweiterungen](#update-extensions) beschrieben.</span><span class="sxs-lookup"><span data-stu-id="5c738-146">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>

### <a name="how-to-develop-our-own-extension"></a><span data-ttu-id="5c738-147">Wie entwickeln Sie Ihre eigene Erweiterung?</span><span class="sxs-lookup"><span data-stu-id="5c738-147">How to develop our own extension?</span></span>
<span data-ttu-id="5c738-148">Sehen Sie sich das offizielle Repository an, wenn Sie weitere Unterstützung benötigen.</span><span class="sxs-lookup"><span data-stu-id="5c738-148">Please refer to the official repository for more help.</span></span> [<span data-ttu-id="5c738-149">Azure/azure-cli-extensions</span><span class="sxs-lookup"><span data-stu-id="5c738-149">Azure/azure-cli-extensions</span></span>](https://github.com/Azure/azure-cli/tree/master/doc/extensions)

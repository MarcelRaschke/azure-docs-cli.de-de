---
title: Azure CLI 2.0-Erweiterungen
description: Verwenden von Erweiterungen mit Azure CLI 2.0
keywords: Azure CLI, Erweiterungen
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 1b983faef4c1678763b3483192e94a6c96e24f32
ms.sourcegitcommit: 80189ff103c91f8c47ab8ebf586df815fff5dd5d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2018
ms.locfileid: "34479473"
---
# <a name="using-extensions-with-the-azure-cli-20"></a><span data-ttu-id="1db43-104">Verwenden von Erweiterungen mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="1db43-104">Using extensions with the Azure CLI 2.0</span></span>

<span data-ttu-id="1db43-105">Erweiterungen sind einzelne Module, die nicht mit der Azure CLI bereitgestellt werden und Funktionen über neue Befehle hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="1db43-105">Extensions are individual modules not shipped with the Azure CLI itself that add functionality through new commands.</span></span> <span data-ttu-id="1db43-106">Dies können experimentelle Angebote oder Vorabangebote, spezielle Tools von Microsoft oder von Ihnen selbst geschriebene benutzerdefinierte Features sein.</span><span class="sxs-lookup"><span data-stu-id="1db43-106">These might be experimental or pre-release offerings, specialized tools from Microsoft, or custom features you write yourself.</span></span> <span data-ttu-id="1db43-107">Erweiterungen ermöglichen das flexible Anpassen der CLI an Ihre eigenen Anforderungen, ohne dass Sie viele zusätzliche Pakete mitliefern müssen, die nicht als Teil des Kernfeaturesatzes angesehen werden.</span><span class="sxs-lookup"><span data-stu-id="1db43-107">Extensions allow for a degree of flexibility with the CLI that let you modify it to your own needs, without having to ship a lot of additional packages that aren't considered part of the core feature set.</span></span>

<span data-ttu-id="1db43-108">In diesem Artikel wird beschrieben, wie Sie Erweiterungen für die CLI installieren, aktualisieren und entfernen.</span><span class="sxs-lookup"><span data-stu-id="1db43-108">This article helps you understand how to install, update, and remove extensions for the CLI.</span></span> <span data-ttu-id="1db43-109">Außerdem werden häufige Fragen zum Verhalten von Erweiterungen beantwortet.</span><span class="sxs-lookup"><span data-stu-id="1db43-109">It also answers common questions about extension behavior.</span></span>

## <a name="find-extensions"></a><span data-ttu-id="1db43-110">Suchen von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="1db43-110">Find extensions</span></span>

<span data-ttu-id="1db43-111">Um zu ermitteln, welche Erweiterungen verfügbar sind, können Sie [az extension list-available](/cli/azure/extension#az-extension-list-available) verwenden.</span><span class="sxs-lookup"><span data-stu-id="1db43-111">In order to know what extensions are available, you can use [az extension list-available](/cli/azure/extension#az-extension-list-available).</span></span> <span data-ttu-id="1db43-112">Mit diesem Befehl werden die offiziellen Erweiterungen aufgeführt, die von Microsoft bereitgestellt und verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="1db43-112">This command lists the official extensions provided and maintained by Microsoft.</span></span>

```azurecli-interactive
az extension list-available --output table
```

<span data-ttu-id="1db43-113">Auf der Dokumentationswebsite wird darüber hinaus eine [Liste der Microsoft-Erweiterungen](azure-cli-extensions-list.md) bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="1db43-113">We also host a [list of Microsoft extensions](azure-cli-extensions-list.md) on the documentation site.</span></span>

## <a name="install-extensions"></a><span data-ttu-id="1db43-114">Installieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="1db43-114">Install extensions</span></span>

<span data-ttu-id="1db43-115">Nachdem Sie eine zu installierende Erweiterung gefunden haben, können Sie [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) verwenden, um sie abzurufen.</span><span class="sxs-lookup"><span data-stu-id="1db43-115">Once you have found an extension to install, use [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) to get it.</span></span> <span data-ttu-id="1db43-116">Wenn die Erweiterung in `az extension list-available` aufgeführt wird, können Sie die Erweiterung anhand des Namens installieren.</span><span class="sxs-lookup"><span data-stu-id="1db43-116">If the extension is listed in `az extension list-available`, you can install the extension by name.</span></span>

```azurecli-interactive
az extension add --name <extension-name>
```

<span data-ttu-id="1db43-117">Wenn die Erweiterung von einer externen Ressource stammt oder Sie über einen direkten Link dafür verfügen, können Sie die Quell-URL oder den lokalen Pfad angeben.</span><span class="sxs-lookup"><span data-stu-id="1db43-117">If the extension is from an external resource or you have a direct link to it, you can provide the source URL or local path.</span></span> <span data-ttu-id="1db43-118">Dies _muss_ eine kompilierte Python-Wheeldatei sein.</span><span class="sxs-lookup"><span data-stu-id="1db43-118">This _must_ be a compiled Python wheel file.</span></span>

```azurecli-interactive
az extension add --source <URL-or-path>
```

<span data-ttu-id="1db43-119">Nach der Installation einer Erweiterung befindet sich diese unter dem Wert der Shellvariablen `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="1db43-119">Once an extension is installed, it can be found under the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="1db43-120">Wenn diese Variable nicht festgelegt ist, befindet sich der Wert standardmäßig unter `$HOME/.azure/cliextensions` (Linux und macOS) bzw. `%USERPROFILE%\.azure\cliextensions` (Windows).</span><span class="sxs-lookup"><span data-stu-id="1db43-120">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

## <a name="update-extensions"></a><span data-ttu-id="1db43-121">Aktualisieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="1db43-121">Update extensions</span></span>

<span data-ttu-id="1db43-122">Wenn eine Erweiterung anhand des Namens installiert wurde, kann sie mithilfe von [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update) aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="1db43-122">If an extension was installed by name, it can be updated using [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update).</span></span>

```azurecli-interactive
az extension update --name <extension-name>
```

<span data-ttu-id="1db43-123">Andernfalls kann eine Erweiterung anhand der Quelle gemäß den Anweisungen unter [Installieren von Erweiterungen](#install-extensions) aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="1db43-123">Otherwise, an extension can be updated from source by following the [Install extensions](#install-extensions) instructions.</span></span>

<span data-ttu-id="1db43-124">Falls der Name einer Erweiterung von der CLI nicht aufgelöst werden kann, deinstallieren Sie die Erweiterung, und installieren Sie sie anschließend erneut.</span><span class="sxs-lookup"><span data-stu-id="1db43-124">If an extension name cannot be resolved by the CLI, uninstall it and attempt to reinstall.</span></span> <span data-ttu-id="1db43-125">Außerdem ist es möglich, dass die Erweiterung nicht mehr als Vorschauversion verfügbar und zu einem integrierten Befehl für die CLI geworden ist.</span><span class="sxs-lookup"><span data-stu-id="1db43-125">There's also the possibility that the extension was moved out of preview and became a built-in command for the CLI.</span></span> <span data-ttu-id="1db43-126">Versuchen Sie, die CLI wie unter [Installieren von Azure CLI 2.0](install-azure-cli.md) beschrieben zu installieren, und überprüfen Sie, ob die Befehle der Erweiterung hinzugefügt wurden.</span><span class="sxs-lookup"><span data-stu-id="1db43-126">Try updating the CLI as described in [Install the Azure CLI 2.0](install-azure-cli.md) and see if the extension's commands were added.</span></span> 

## <a name="uninstall-extensions"></a><span data-ttu-id="1db43-127">Deinstallieren von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="1db43-127">Uninstall extensions</span></span>

<span data-ttu-id="1db43-128">Wenn Sie eine Erweiterung nicht mehr benötigen, können Sie sie mit [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove) entfernen.</span><span class="sxs-lookup"><span data-stu-id="1db43-128">If you no longer need an extension, it can be removed with [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove).</span></span>

```azurecli-interactive
az extension remove --name <extension-name>
```

<span data-ttu-id="1db43-129">Sie können eine Erweiterung auch manuell entfernen, indem Sie sie am Installationsspeicherort löschen.</span><span class="sxs-lookup"><span data-stu-id="1db43-129">You can also remove an extension manually by deleting it from the location where it was installed.</span></span> <span data-ttu-id="1db43-130">Dies ist der Wert der Shellvariablen `$AZURE_EXTENSION_DIR`.</span><span class="sxs-lookup"><span data-stu-id="1db43-130">This will be the value of the `$AZURE_EXTENSION_DIR` shell variable.</span></span> <span data-ttu-id="1db43-131">Wenn diese Variable nicht festgelegt ist, befindet sich der Wert standardmäßig unter `$HOME/.azure/cliextensions` (Linux und macOS) bzw. `%USERPROFILE%\.azure\cliextensions` (Windows).</span><span class="sxs-lookup"><span data-stu-id="1db43-131">If this variable is unset, by default the value is `$HOME/.azure/cliextensions` on Linux and macOS, and `%USERPROFILE%\.azure\cliextensions` on Windows.</span></span>

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

<span data-ttu-id="1db43-132">Es wird empfohlen, die Deinstallation mit `az extension remove` durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="1db43-132">It is recommended that you uninstall using `az extension remove`.</span></span>

## <a name="faq"></a><span data-ttu-id="1db43-133">Häufig gestellte Fragen</span><span class="sxs-lookup"><span data-stu-id="1db43-133">FAQ</span></span>

<span data-ttu-id="1db43-134">Hier sind einige Antworten auf andere häufig gestellte Fragen zu CLI-Erweiterungen aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="1db43-134">Here are some answers to other common questions about CLI extensions.</span></span>

### <a name="what-file-formats-are-allowed-for-installation"></a><span data-ttu-id="1db43-135">Welche Dateiformate sind für die Installation zulässig?</span><span class="sxs-lookup"><span data-stu-id="1db43-135">What file formats are allowed for installation?</span></span>

<span data-ttu-id="1db43-136">Derzeit können nur kompilierte Python-Wheels als Erweiterungen installiert werden.</span><span class="sxs-lookup"><span data-stu-id="1db43-136">Currently, only compiled Python wheels can be installed as extensions.</span></span>

### <a name="can-extensions-replace-existing-commands"></a><span data-ttu-id="1db43-137">Können Erweiterungen vorhandene Befehle ersetzen?</span><span class="sxs-lookup"><span data-stu-id="1db43-137">Can extensions replace existing commands?</span></span>

<span data-ttu-id="1db43-138">Ja.</span><span class="sxs-lookup"><span data-stu-id="1db43-138">Yes.</span></span> <span data-ttu-id="1db43-139">Erweiterungen können vorhandene Befehle ersetzen, aber vor dem Ausführen eines ersetzten Befehls wird von der CLI eine Warnung ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="1db43-139">Extensions may replace existing commands, but before running a command that has been replaced the CLI will issue a warning.</span></span>

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a><span data-ttu-id="1db43-140">Woran erkenne ich, dass es sich bei einer Erweiterung um eine Vorabversion handelt?</span><span class="sxs-lookup"><span data-stu-id="1db43-140">How can I tell if an extension is in pre-release?</span></span>

<span data-ttu-id="1db43-141">Für eine Erweiterung sollte in der dazugehörigen Dokumentation und in den Versionsinformationen angegeben sein, wenn es sich um eine Vorabversion handelt.</span><span class="sxs-lookup"><span data-stu-id="1db43-141">An extension should indicate through its own documentation and versioning if it is in pre-release.</span></span> <span data-ttu-id="1db43-142">Es kommt auch häufiger vor, dass Microsoft Vorschauversionen von Befehlen für die CLI als Erweiterungen veröffentlicht, die nach der Vorschauphase des Produkts in die Hauptoberfläche der CLI integriert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="1db43-142">It is also common for Microsoft to release preview commands for the CLI as extensions, with plans to move them into the main CLI interface once the product is out of preview.</span></span>

### <a name="can-extensions-depend-upon-each-other"></a><span data-ttu-id="1db43-143">Können Erweiterungen voneinander abhängig sein?</span><span class="sxs-lookup"><span data-stu-id="1db43-143">Can extensions depend upon each other?</span></span>

<span data-ttu-id="1db43-144">Nein.</span><span class="sxs-lookup"><span data-stu-id="1db43-144">No.</span></span> <span data-ttu-id="1db43-145">Erweiterungen müssen einzelne Pakete sein, die nicht voneinander abhängig sind.</span><span class="sxs-lookup"><span data-stu-id="1db43-145">Extensions must be individual packages which do not rely on one another.</span></span> <span data-ttu-id="1db43-146">Dies liegt daran, dass für die CLI nicht garantiert ist, wann Erweiterungen geladen werden. Es kann also nicht sichergestellt werden, dass die Anforderungen von Abhängigkeiten erfüllt werden.</span><span class="sxs-lookup"><span data-stu-id="1db43-146">This is because the CLI gives no guarantee about when extensions are loaded, so dependencies could not be guaranteed to be satisfied.</span></span> <span data-ttu-id="1db43-147">Bei der Installation einer Erweiterung wird nur die jeweilige Erweiterung installiert, und sie sollte auch dann funktionieren, wenn Sie andere Erweiterungen entfernen.</span><span class="sxs-lookup"><span data-stu-id="1db43-147">Installing an extension installs that extension only, and it should continue to work even if you remove other extensions.</span></span>

### <a name="are-extensions-updated-along-with-the-cli"></a><span data-ttu-id="1db43-148">Werden Erweiterungen zusammen mit der CLI aktualisiert?</span><span class="sxs-lookup"><span data-stu-id="1db43-148">Are extensions updated along with the CLI?</span></span>

<span data-ttu-id="1db43-149">Nein.</span><span class="sxs-lookup"><span data-stu-id="1db43-149">No.</span></span> <span data-ttu-id="1db43-150">Erweiterungen müssen separat aktualisiert werden, wie unter [Aktualisieren von Erweiterungen](#update-extensions) beschrieben.</span><span class="sxs-lookup"><span data-stu-id="1db43-150">Extensions must be updated separately, as described in [Update extensions](#update-extensions).</span></span>

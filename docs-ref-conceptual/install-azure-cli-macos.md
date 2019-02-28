---
title: Installieren der Azure-Befehlszeilenschnittstelle für macOS
description: Installieren der Azure CLI unter macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/05/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 61be6c31e7251c8b374bf09072a9ecba9b914342
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/19/2019
ms.locfileid: "56422050"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="0d09c-103">Installieren der Azure CLI unter macOS</span><span class="sxs-lookup"><span data-stu-id="0d09c-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="0d09c-104">Bei Verwendung der macOS-Plattform können Sie die Azure CLI mit dem [Homebrew-Paket-Manager](https://brew.sh) installieren.</span><span class="sxs-lookup"><span data-stu-id="0d09c-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="0d09c-105">Mit Homebrew können Sie Ihre CLI-Installation ganz einfach auf dem neuesten Stand halten.</span><span class="sxs-lookup"><span data-stu-id="0d09c-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="0d09c-106">Das CLI-Paket wurde ab der macOS-Version 10.9 getestet.</span><span class="sxs-lookup"><span data-stu-id="0d09c-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install"></a><span data-ttu-id="0d09c-107">Installieren</span><span class="sxs-lookup"><span data-stu-id="0d09c-107">Install</span></span>

<span data-ttu-id="0d09c-108">Homebrew ist die einfachste Möglichkeit zum Verwalten der CLI-Installation.</span><span class="sxs-lookup"><span data-stu-id="0d09c-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="0d09c-109">Homebrew bietet praktische Optionen zum Installieren, Aktualisieren und Deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="0d09c-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="0d09c-110">Falls Homebrew auf Ihrem System nicht verfügbar ist, [installieren Sie Homebrew](https://docs.brew.sh/Installation.html), bevor Sie fortfahren.</span><span class="sxs-lookup"><span data-stu-id="0d09c-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="0d09c-111">Sie können die CLI installieren, indem Sie die Homebrew-Repositoryinformationen aktualisieren und dann den Befehl `install` ausführen:</span><span class="sxs-lookup"><span data-stu-id="0d09c-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

> [!IMPORTANT]
>
> <span data-ttu-id="0d09c-112">Die Azure CLI ist vom `python3`-Paket in Homebrew abhängig und installiert dieses Paket auch dann in Ihrem System, wenn Python 2 verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="0d09c-112">The Azure CLI has a dependency on the `python3` package in Homebrew, and will install it on your system, even if Python 2 is available.</span></span> <span data-ttu-id="0d09c-113">Die Azure CLI ist garantiert kompatibel mit der aktuellen Version von `python3`, die auf Homebrew veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="0d09c-113">The Azure CLI is guaranteed to be compatible with the latest version of `python3` published on Homebrew.</span></span>

<span data-ttu-id="0d09c-114">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="0d09c-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="0d09c-115">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="0d09c-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="0d09c-116">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0d09c-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="0d09c-117">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="0d09c-117">Troubleshooting</span></span>

<span data-ttu-id="0d09c-118">In diesem Abschnitt finden Sie einige allgemeine Fehler, die zu Problemen bei der Homebrew-basierten CLI-Installation führen können.</span><span class="sxs-lookup"><span data-stu-id="0d09c-118">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="0d09c-119">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="0d09c-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="0d09c-120">Python und installierte Pakete können nicht gefunden werden.</span><span class="sxs-lookup"><span data-stu-id="0d09c-120">Unable to find Python or installed packages</span></span>

<span data-ttu-id="0d09c-121">Bei der Installation von Homebrew weichen die Versionen unter Umständen geringfügig voneinander ab, oder es liegt ein anderes Problem vor.</span><span class="sxs-lookup"><span data-stu-id="0d09c-121">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="0d09c-122">Die CLI verwendet keine virtuelle Python-Umgebung und ist daher von der Ermittlung der installierten Python-Version abhängig.</span><span class="sxs-lookup"><span data-stu-id="0d09c-122">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="0d09c-123">Sie können das Problem möglicherweise beheben, indem Sie die `python3`-Abhängigkeit installieren und über Homebrew neu verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="0d09c-123">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="0d09c-124">CLI-Version 1.x wird installiert.</span><span class="sxs-lookup"><span data-stu-id="0d09c-124">CLI version 1.x is installed</span></span>

<span data-ttu-id="0d09c-125">Die Installation einer veralteten Version kann auf einen veralteten Homebrew-Cache zurückzuführen sein.</span><span class="sxs-lookup"><span data-stu-id="0d09c-125">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="0d09c-126">Gehen Sie gemäß der [Aktualisierungsanleitung](#Update) vor.</span><span class="sxs-lookup"><span data-stu-id="0d09c-126">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="0d09c-127">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0d09c-127">Update</span></span>

<span data-ttu-id="0d09c-128">Die CLI wird regelmäßig mit Fehlerbehebungen, Verbesserungen, neuen Features und Vorschaufunktionen aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="0d09c-128">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="0d09c-129">Ein neues Release ist ungefähr alle zwei Wochen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="0d09c-129">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="0d09c-130">Aktualisieren Sie Ihre lokalen Repositoryinformationen, und upgraden Sie anschließend das Paket `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="0d09c-130">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="0d09c-131">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="0d09c-131">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="0d09c-132">Verwenden Sie Homebrew, um das Paket `azure-cli` zu deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="0d09c-132">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="0d09c-133">Andere Installationsmethoden</span><span class="sxs-lookup"><span data-stu-id="0d09c-133">Other installation methods</span></span>

<span data-ttu-id="0d09c-134">Falls Sie die Azure-Befehlszeilenschnittstelle in Ihrer Umgebung nicht mithilfe von Homebrew installieren können, können Sie die manuelle Anleitung für Linux verwenden.</span><span class="sxs-lookup"><span data-stu-id="0d09c-134">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="0d09c-135">Beachten Sie, dass dieser Prozess nicht offiziell mit macOS kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="0d09c-135">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="0d09c-136">Es empfiehlt sich immer, einen Paket-Manager wie Homebrew zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="0d09c-136">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="0d09c-137">Verwenden Sie die manuelle Installationsmethode nur, wenn keine andere Option zur Verfügung steht.</span><span class="sxs-lookup"><span data-stu-id="0d09c-137">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="0d09c-138">Die Anleitung für die manuelle Installation finden Sie unter [Manuelles Installieren der Azure CLI unter Linux](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="0d09c-138">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="0d09c-139">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="0d09c-139">Next Steps</span></span>

<span data-ttu-id="0d09c-140">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="0d09c-140">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="0d09c-141">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="0d09c-141">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

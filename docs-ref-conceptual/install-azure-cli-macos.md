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
ms.openlocfilehash: 40415bc7bec056dc1564c58c8df3f7263bee348c
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593165"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="f86cf-103">Installieren der Azure CLI unter macOS</span><span class="sxs-lookup"><span data-stu-id="f86cf-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="f86cf-104">Bei Verwendung der macOS-Plattform können Sie die Azure CLI mit dem [Homebrew-Paket-Manager](https://brew.sh) installieren.</span><span class="sxs-lookup"><span data-stu-id="f86cf-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="f86cf-105">Mit Homebrew können Sie Ihre CLI-Installation ganz einfach auf dem neuesten Stand halten.</span><span class="sxs-lookup"><span data-stu-id="f86cf-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="f86cf-106">Das CLI-Paket wurde ab der macOS-Version 10.9 getestet.</span><span class="sxs-lookup"><span data-stu-id="f86cf-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

## <a name="install"></a><span data-ttu-id="f86cf-107">Installieren</span><span class="sxs-lookup"><span data-stu-id="f86cf-107">Install</span></span>

<span data-ttu-id="f86cf-108">Homebrew ist die einfachste Möglichkeit zum Verwalten der CLI-Installation.</span><span class="sxs-lookup"><span data-stu-id="f86cf-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="f86cf-109">Homebrew bietet praktische Optionen zum Installieren, Aktualisieren und Deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="f86cf-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="f86cf-110">Falls Homebrew auf Ihrem System nicht verfügbar ist, [installieren Sie Homebrew](https://docs.brew.sh/Installation.html), bevor Sie fortfahren.</span><span class="sxs-lookup"><span data-stu-id="f86cf-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="f86cf-111">Sie können die CLI installieren, indem Sie die Homebrew-Repositoryinformationen aktualisieren und dann den Befehl `install` ausführen:</span><span class="sxs-lookup"><span data-stu-id="f86cf-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

<span data-ttu-id="f86cf-112">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="f86cf-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="f86cf-113">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="f86cf-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="f86cf-114">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f86cf-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="f86cf-115">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="f86cf-115">Troubleshooting</span></span>

<span data-ttu-id="f86cf-116">In diesem Abschnitt finden Sie einige allgemeine Fehler, die zu Problemen bei der Homebrew-basierten CLI-Installation führen können.</span><span class="sxs-lookup"><span data-stu-id="f86cf-116">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="f86cf-117">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="f86cf-117">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="f86cf-118">Python und installierte Pakete können nicht gefunden werden.</span><span class="sxs-lookup"><span data-stu-id="f86cf-118">Unable to find Python or installed packages</span></span>

<span data-ttu-id="f86cf-119">Bei der Installation von Homebrew weichen die Versionen unter Umständen geringfügig voneinander ab, oder es liegt ein anderes Problem vor.</span><span class="sxs-lookup"><span data-stu-id="f86cf-119">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="f86cf-120">Die CLI verwendet keine virtuelle Python-Umgebung und ist daher von der Ermittlung der installierten Python-Version abhängig.</span><span class="sxs-lookup"><span data-stu-id="f86cf-120">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="f86cf-121">Sie können das Problem möglicherweise beheben, indem Sie die `python3`-Abhängigkeit installieren und über Homebrew neu verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="f86cf-121">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="f86cf-122">CLI-Version 1.x wird installiert.</span><span class="sxs-lookup"><span data-stu-id="f86cf-122">CLI version 1.x is installed</span></span>

<span data-ttu-id="f86cf-123">Die Installation einer veralteten Version kann auf einen veralteten Homebrew-Cache zurückzuführen sein.</span><span class="sxs-lookup"><span data-stu-id="f86cf-123">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="f86cf-124">Gehen Sie gemäß der [Aktualisierungsanleitung](#Update) vor.</span><span class="sxs-lookup"><span data-stu-id="f86cf-124">Follow the [update](#Update) instructions.</span></span>

## <a name="update"></a><span data-ttu-id="f86cf-125">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f86cf-125">Update</span></span>

<span data-ttu-id="f86cf-126">Die CLI wird regelmäßig mit Fehlerbehebungen, Verbesserungen, neuen Features und Vorschaufunktionen aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="f86cf-126">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="f86cf-127">Ein neues Release ist ungefähr alle zwei Wochen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f86cf-127">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="f86cf-128">Aktualisieren Sie Ihre lokalen Repositoryinformationen, und upgraden Sie anschließend das Paket `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="f86cf-128">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="f86cf-129">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="f86cf-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="f86cf-130">Verwenden Sie Homebrew, um das Paket `azure-cli` zu deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="f86cf-130">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="f86cf-131">Andere Installationsmethoden</span><span class="sxs-lookup"><span data-stu-id="f86cf-131">Other installation methods</span></span>

<span data-ttu-id="f86cf-132">Falls Sie die Azure-Befehlszeilenschnittstelle in Ihrer Umgebung nicht mithilfe von Homebrew installieren können, können Sie die manuelle Anleitung für Linux verwenden.</span><span class="sxs-lookup"><span data-stu-id="f86cf-132">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="f86cf-133">Beachten Sie, dass dieser Prozess nicht offiziell mit macOS kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="f86cf-133">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="f86cf-134">Es empfiehlt sich immer, einen Paket-Manager wie Homebrew zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="f86cf-134">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="f86cf-135">Verwenden Sie die manuelle Installationsmethode nur, wenn keine andere Option zur Verfügung steht.</span><span class="sxs-lookup"><span data-stu-id="f86cf-135">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="f86cf-136">Die Anleitung für die manuelle Installation finden Sie unter [Manuelles Installieren der Azure CLI unter Linux](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="f86cf-136">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="f86cf-137">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f86cf-137">Next Steps</span></span>

<span data-ttu-id="f86cf-138">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="f86cf-138">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f86cf-139">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="f86cf-139">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

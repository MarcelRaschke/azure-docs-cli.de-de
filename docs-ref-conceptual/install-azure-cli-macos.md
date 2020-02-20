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
ms.openlocfilehash: 9a5026634691f49d960f383c90e139754c862cb4
ms.sourcegitcommit: 91c1e5423bd054a948620999b559bc3a9828a688
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/19/2020
ms.locfileid: "77453751"
---
# <a name="install-azure-cli-on-macos"></a><span data-ttu-id="6d572-103">Installieren der Azure CLI unter macOS</span><span class="sxs-lookup"><span data-stu-id="6d572-103">Install Azure CLI on macOS</span></span>

<span data-ttu-id="6d572-104">Bei Verwendung der macOS-Plattform können Sie die Azure CLI mit dem [Homebrew-Paket-Manager](https://brew.sh) installieren.</span><span class="sxs-lookup"><span data-stu-id="6d572-104">For the macOS platform, you can install the Azure CLI with [homebrew package manager](https://brew.sh).</span></span> <span data-ttu-id="6d572-105">Mit Homebrew können Sie Ihre CLI-Installation ganz einfach auf dem neuesten Stand halten.</span><span class="sxs-lookup"><span data-stu-id="6d572-105">Homebrew makes it easy to keep your installation of the CLI update to date.</span></span> <span data-ttu-id="6d572-106">Das CLI-Paket wurde ab der macOS-Version 10.9 getestet.</span><span class="sxs-lookup"><span data-stu-id="6d572-106">The CLI package has been tested on macOS versions 10.9 and later.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-with-homebrew"></a><span data-ttu-id="6d572-107">Installieren mit Homebrew</span><span class="sxs-lookup"><span data-stu-id="6d572-107">Install with Homebrew</span></span>

<span data-ttu-id="6d572-108">Homebrew ist die einfachste Möglichkeit zum Verwalten der CLI-Installation.</span><span class="sxs-lookup"><span data-stu-id="6d572-108">Homebrew is the easiest way to manage your CLI install.</span></span> <span data-ttu-id="6d572-109">Homebrew bietet praktische Optionen zum Installieren, Aktualisieren und Deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="6d572-109">It provides convenient ways to install, update, and uninstall.</span></span>
<span data-ttu-id="6d572-110">Falls Homebrew auf Ihrem System nicht verfügbar ist, [installieren Sie Homebrew](https://docs.brew.sh/Installation.html), bevor Sie fortfahren.</span><span class="sxs-lookup"><span data-stu-id="6d572-110">If you don't have homebrew available on your system, [install homebrew](https://docs.brew.sh/Installation.html) before continuing.</span></span>

<span data-ttu-id="6d572-111">Sie können die CLI installieren, indem Sie die Homebrew-Repositoryinformationen aktualisieren und dann den Befehl `install` ausführen:</span><span class="sxs-lookup"><span data-stu-id="6d572-111">You can install the CLI by updating your brew repository information, and then running the `install` command:</span></span>

```bash
brew update && brew install azure-cli
```

> [!IMPORTANT]
>
> <span data-ttu-id="6d572-112">Die Azure CLI weist eine Abhängigkeit vom Homebrew-Paket `python3` auf und installiert es.</span><span class="sxs-lookup"><span data-stu-id="6d572-112">The Azure CLI has a dependency on the Homebrew `python3` package, and will install it.</span></span>
> <span data-ttu-id="6d572-113">Die Azure CLI ist garantiert kompatibel mit der aktuellen Version von `python3`, die auf Homebrew veröffentlicht wurde.</span><span class="sxs-lookup"><span data-stu-id="6d572-113">The Azure CLI is guaranteed to be compatible with the latest version of `python3` published on Homebrew.</span></span>

<span data-ttu-id="6d572-114">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="6d572-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="6d572-115">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="6d572-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="6d572-116">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="6d572-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="6d572-117">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="6d572-117">Troubleshooting</span></span>

<span data-ttu-id="6d572-118">In diesem Abschnitt finden Sie einige allgemeine Fehler, die zu Problemen bei der Homebrew-basierten CLI-Installation führen können.</span><span class="sxs-lookup"><span data-stu-id="6d572-118">If you encounter a problem when installing the CLI through Homebrew, here are some common errors.</span></span> <span data-ttu-id="6d572-119">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="6d572-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="completion-is-not-working"></a><span data-ttu-id="6d572-120">Die Vervollständigung funktioniert nicht.</span><span class="sxs-lookup"><span data-stu-id="6d572-120">Completion is not working</span></span>

<span data-ttu-id="6d572-121">Die Homebrew-Formel der Azure CLI installiert eine Vervollständigungsdatei namens `az` im Verzeichnis für von Homebrew verwaltete Vervollständigungen (Standardspeicherort: `/usr/local/etc/bash_completion.d/`).</span><span class="sxs-lookup"><span data-stu-id="6d572-121">The Homebrew formula of Azure CLI installs a completion file named `az` in the Homebrew-managed completions directory (default location is `/usr/local/etc/bash_completion.d/`).</span></span> <span data-ttu-id="6d572-122">Befolgen Sie zum Aktivieren der Vervollständigung [diese Anweisungen](https://docs.brew.sh/Shell-Completion) von Homebrew.</span><span class="sxs-lookup"><span data-stu-id="6d572-122">To enable completion, please follow Homebrew's instructions [here](https://docs.brew.sh/Shell-Completion).</span></span>

### <a name="unable-to-find-python-or-installed-packages"></a><span data-ttu-id="6d572-123">Python und installierte Pakete können nicht gefunden werden.</span><span class="sxs-lookup"><span data-stu-id="6d572-123">Unable to find Python or installed packages</span></span>

<span data-ttu-id="6d572-124">Bei der Installation von Homebrew weichen die Versionen unter Umständen geringfügig voneinander ab, oder es liegt ein anderes Problem vor.</span><span class="sxs-lookup"><span data-stu-id="6d572-124">There may be a minor version mismatch or other issue during homebrew installation.</span></span> <span data-ttu-id="6d572-125">Die CLI verwendet keine virtuelle Python-Umgebung und ist daher von der Ermittlung der installierten Python-Version abhängig.</span><span class="sxs-lookup"><span data-stu-id="6d572-125">The CLI doesn't use a Python virtual environment, so it relies on finding the installed Python version.</span></span> <span data-ttu-id="6d572-126">Sie können das Problem möglicherweise beheben, indem Sie die `python3`-Abhängigkeit installieren und über Homebrew neu verknüpfen.</span><span class="sxs-lookup"><span data-stu-id="6d572-126">A possible fix is to install and relink the `python3` dependency from Homebrew.</span></span>

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a><span data-ttu-id="6d572-127">CLI-Version 1.x wird installiert.</span><span class="sxs-lookup"><span data-stu-id="6d572-127">CLI version 1.x is installed</span></span>

<span data-ttu-id="6d572-128">Die Installation einer veralteten Version kann auf einen veralteten Homebrew-Cache zurückzuführen sein.</span><span class="sxs-lookup"><span data-stu-id="6d572-128">If an out-of-date version was installed, it could be because of a stale homebrew cache.</span></span> <span data-ttu-id="6d572-129">Gehen Sie gemäß der [Aktualisierungsanleitung](#update) vor.</span><span class="sxs-lookup"><span data-stu-id="6d572-129">Follow the [update](#update) instructions.</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="6d572-130">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="6d572-130">Proxy blocks connection</span></span>

<span data-ttu-id="6d572-131">Möglicherweise können Sie keine Ressourcen von Homebrew abrufen, wenn Sie das Programm nicht korrekt zur Verwendung Ihres Proxys konfiguriert haben.</span><span class="sxs-lookup"><span data-stu-id="6d572-131">You may be unable to get resources from Homebrew unless you have correctly configured it to use your proxy.</span></span> <span data-ttu-id="6d572-132">Führen Sie die [Anweisungen zur Proxykonfiguration für Homebrew](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy) aus.</span><span class="sxs-lookup"><span data-stu-id="6d572-132">Follow the [Homebrew proxy configuration instructions](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6d572-133">Wenn Sie sich hinter einem Proxy befinden, müssen `HTTP_PROXY` und `HTTPS_PROXY` so festgelegt sein, dass sie über die CLI eine Verbindung mit Azure-Diensten herstellen.</span><span class="sxs-lookup"><span data-stu-id="6d572-133">If you are behind a proxy, `HTTP_PROXY` and `HTTPS_PROXY` must be set to connect to Azure services with the CLI.</span></span>
> <span data-ttu-id="6d572-134">Wenn Sie nicht die Standardauthentifizierung verwenden, wird empfohlen, dass Sie diese Variablen in Ihrer Datei vom Typ `.bashrc` exportieren.</span><span class="sxs-lookup"><span data-stu-id="6d572-134">If you are not using basic auth, it's recommended to export these variables in your `.bashrc` file.</span></span>
> <span data-ttu-id="6d572-135">Berücksichtigen Sie dabei immer die Sicherheitsrichtlinien Ihres Unternehmens und die Anforderungen Ihres Systemadministrators.</span><span class="sxs-lookup"><span data-stu-id="6d572-135">Always follow your business' security policies and the requirements of your system administrator.</span></span>

<span data-ttu-id="6d572-136">Zum Abrufen der Bottle-Ressourcen von Homebrew muss Ihr Proxy HTTPS-Verbindungen mit den folgenden Adressen zulassen:</span><span class="sxs-lookup"><span data-stu-id="6d572-136">In order to get the bottle resources from Homebrew, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://formulae.brew.sh`
* `https://homebrew.bintray.com`

## <a name="update"></a><span data-ttu-id="6d572-137">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6d572-137">Update</span></span>

<span data-ttu-id="6d572-138">Die CLI wird regelmäßig mit Fehlerbehebungen, Verbesserungen, neuen Features und Vorschaufunktionen aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="6d572-138">The CLI is regularly updated with bug fixes, improvements, new features, and preview functionality.</span></span> <span data-ttu-id="6d572-139">Ein neues Release ist ungefähr alle zwei Wochen verfügbar.</span><span class="sxs-lookup"><span data-stu-id="6d572-139">A new release is available roughly every two weeks.</span></span> <span data-ttu-id="6d572-140">Aktualisieren Sie Ihre lokalen Repositoryinformationen, und upgraden Sie anschließend das Paket `azure-cli`.</span><span class="sxs-lookup"><span data-stu-id="6d572-140">Update your local repository information and then upgrade the `azure-cli` package.</span></span>

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="6d572-141">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="6d572-141">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="6d572-142">Verwenden Sie Homebrew, um das Paket `azure-cli` zu deinstallieren.</span><span class="sxs-lookup"><span data-stu-id="6d572-142">Use homebrew to uninstall the `azure-cli` package.</span></span>

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a><span data-ttu-id="6d572-143">Andere Installationsmethoden</span><span class="sxs-lookup"><span data-stu-id="6d572-143">Other installation methods</span></span>

<span data-ttu-id="6d572-144">Falls Sie die Azure-Befehlszeilenschnittstelle in Ihrer Umgebung nicht mithilfe von Homebrew installieren können, können Sie die manuelle Anleitung für Linux verwenden.</span><span class="sxs-lookup"><span data-stu-id="6d572-144">If you can't use homebrew to install the Azure CLI in your environment, it's possible to use the manual instructions for Linux.</span></span> <span data-ttu-id="6d572-145">Beachten Sie, dass dieser Prozess nicht offiziell mit macOS kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="6d572-145">Note that this process is not officially maintained to be compatible with macOS.</span></span> <span data-ttu-id="6d572-146">Es empfiehlt sich immer, einen Paket-Manager wie Homebrew zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="6d572-146">Using a package manager such as Homebrew is always recommended.</span></span> <span data-ttu-id="6d572-147">Verwenden Sie die manuelle Installationsmethode nur, wenn keine andere Option zur Verfügung steht.</span><span class="sxs-lookup"><span data-stu-id="6d572-147">Only use the manual installation method if you have no other option available.</span></span>

<span data-ttu-id="6d572-148">Die Anleitung für die manuelle Installation finden Sie unter [Manuelles Installieren der Azure CLI unter Linux](install-azure-cli-linux.md).</span><span class="sxs-lookup"><span data-stu-id="6d572-148">For the manual installation instructions, see [Install Azure CLI on Linux manually](install-azure-cli-linux.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="6d572-149">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="6d572-149">Next Steps</span></span>

<span data-ttu-id="6d572-150">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="6d572-150">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="6d572-151">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="6d572-151">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

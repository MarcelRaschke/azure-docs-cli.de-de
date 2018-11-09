---
title: Installieren der klassischen Azure CLI
description: Installieren der klassischen Azure CLI für Mac, Linux und Windows für das Starten von Azure-Diensten
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/11/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 78043f9c070626545030971dea2a8fd155ac76c2
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222462"
---
# <a name="install-the-azure-classic-cli"></a><span data-ttu-id="ae616-103">Installieren der klassischen Azure CLI</span><span class="sxs-lookup"><span data-stu-id="ae616-103">Install the Azure classic CLI</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ae616-104">In diesem Thema wird beschrieben, wie Sie die klassische Azure CLI installieren.</span><span class="sxs-lookup"><span data-stu-id="ae616-104">This topic describes how to install the Azure classic CLI.</span></span> <span data-ttu-id="ae616-105">Die klassische CLI ist veraltet und sollte nur mit dem klassischen Bereitstellungsmodell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="ae616-105">The classic CLI is deprecated and should only be used with the classic deployment model.</span></span>
> <span data-ttu-id="ae616-106">Verwenden Sie für alle anderen Bereitstellungen [die Azure CLI](/cli/azure).</span><span class="sxs-lookup"><span data-stu-id="ae616-106">For all other deployments, use [the Azure CLI](/cli/azure).</span></span>

<span data-ttu-id="ae616-107">Installieren Sie schnell die klassische Azure CLI, um eine Reihe von auf der Open-Source-Shell basierenden Befehlen zum Erstellen und Verwalten von Ressourcen in Microsoft Azure zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="ae616-107">Quickly install the Azure classic CLI to use a set of open-source shell-based commands for creating and managing resources in Microsoft Azure.</span></span> <span data-ttu-id="ae616-108">Zum Installieren dieser plattformübergreifenden Tools auf Ihrem Computer stehen Ihnen mehrere Optionen zur Verfügung:</span><span class="sxs-lookup"><span data-stu-id="ae616-108">You have several options to install these cross-platform tools on your computer:</span></span>

* <span data-ttu-id="ae616-109">**npm-Paket**: Führen Sie npm (den Paket-Manager für JavaScript) aus, um das Paket mit der klassischen Azure CLI auf Ihrer Linux-Distribution oder dem Betriebssystem zu installieren.</span><span class="sxs-lookup"><span data-stu-id="ae616-109">**npm package** - Run npm (the package manager for JavaScript) to install the Azure classic CLI package on your Linux distribution or OS.</span></span> <span data-ttu-id="ae616-110">Hierfür sind „Node.js“ und „npm“ erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae616-110">Requires node.js and npm.</span></span>
* <span data-ttu-id="ae616-111">**Installer**: Laden Sie ein Installationsprogramm für die einfache Installation unter macOS oder Windows herunter.</span><span class="sxs-lookup"><span data-stu-id="ae616-111">**Installer** - Download an installer for easy installation on macOS or Windows.</span></span>
* <span data-ttu-id="ae616-112">**Docker-Container**: Beginnen Sie mit der Verwendung der klassischen CLI in einem sofort betriebsbereiten Docker-Container.</span><span class="sxs-lookup"><span data-stu-id="ae616-112">**Docker container** - Start using the classic CLI in a ready-to-run Docker container.</span></span> <span data-ttu-id="ae616-113">Hierfür ist ein Docker-Host erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ae616-113">Requires a Docker host.</span></span>

<span data-ttu-id="ae616-114">Weitere Optionen und Hintergrundinformationen finden Sie im Projektrepository auf [GitHub](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="ae616-114">For more options and background, see the project repository on [GitHub](https://github.com/azure/azure-xplat-cli).</span></span>

<span data-ttu-id="ae616-115">Sobald die klassische Azure CLI installiert ist, stellen Sie mit `azure login` eine Verbindung her und führen die `azure`-Befehle in der Befehlszeilenschnittstelle (Bash, Terminal, Eingabeaufforderung usw.) aus, um mit Ihren Azure-Ressourcen zu arbeiten.</span><span class="sxs-lookup"><span data-stu-id="ae616-115">Once the Azure classic CLI is installed, connect with `azure login` and run the `azure` commands from your command-line interface (Bash, Terminal, Command prompt, and so on) to work with your Azure resources.</span></span>

## <a name="option-1-install-an-npm-package"></a><span data-ttu-id="ae616-116">Option 1: Installieren eines npm-Pakets</span><span class="sxs-lookup"><span data-stu-id="ae616-116">Option 1: Install an npm package</span></span>

<span data-ttu-id="ae616-117">Um die klassische CLI aus einem npm-Paket zu installieren, müssen Sie die aktuellen Versionen von [Node.js und npm](https://nodejs.org/en/download/package-manager/) herunterladen und installieren.</span><span class="sxs-lookup"><span data-stu-id="ae616-117">To install the classic CLI from an npm package, make sure you have downloaded and installed the [latest Node.js and npm](https://nodejs.org/en/download/package-manager/).</span></span> <span data-ttu-id="ae616-118">Führen Sie anschließend `npm install` aus, um das azure-cli-Paket zu installieren:</span><span class="sxs-lookup"><span data-stu-id="ae616-118">Then, run `npm install` to install the azure-cli package:</span></span>

```bash
npm install -g azure-cli
```

<span data-ttu-id="ae616-119">Bei Linux-Distributionen müssen Sie unter Umständen `sudo` wie folgt verwenden, um den `npm`-Befehl erfolgreich ausführen zu können:</span><span class="sxs-lookup"><span data-stu-id="ae616-119">On Linux distributions, you might need to use `sudo` to successfully run the `npm` command, as follows:</span></span>

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> <span data-ttu-id="ae616-120">Wenn Sie Node.js und npm auf Ihrem Betriebssystem installieren oder aktualisieren müssen, empfehlen wir Ihnen, Node.js-LTS-Version 4.x oder höher zu installieren.</span><span class="sxs-lookup"><span data-stu-id="ae616-120">If you need to install or update Node.js and npm on your OS, we recommend that you install Node.js LTS version 4.x or later.</span></span> <span data-ttu-id="ae616-121">Wenn Sie eine ältere Version verwenden, kommt es möglicherweise zu Fehlern bei der Installation.</span><span class="sxs-lookup"><span data-stu-id="ae616-121">If you use an older version, you might get installation errors.</span></span>

<span data-ttu-id="ae616-122">Falls Sie es vorziehen, können Sie auch aus den [GitHub-Releases](https://github.com/Azure/azure-xplat-cli/releases) eine TAR-Datei herunterladen.</span><span class="sxs-lookup"><span data-stu-id="ae616-122">If you prefer, you may also download a tar file from the [GitHub releases](https://github.com/Azure/azure-xplat-cli/releases).</span></span> <span data-ttu-id="ae616-123">Installieren Sie dann das heruntergeladene npm-Paket wie folgt (in Linux-Distributionen müssen Sie unter Umständen `sudo` verwenden):</span><span class="sxs-lookup"><span data-stu-id="ae616-123">Then, install the downloaded npm package as follows (on Linux distributions you might need to use `sudo`):</span></span>

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a><span data-ttu-id="ae616-124">Option 2: Verwenden eines Installers</span><span class="sxs-lookup"><span data-stu-id="ae616-124">Option 2: Use an installer</span></span>

<span data-ttu-id="ae616-125">Bei Verwendung eines Mac- oder Windows-Computers sind unter den [GitHub-Releases](https://github.com/Azure/azure-xplat-cli/releases) DMG- und MSI-Installer verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ae616-125">If you use a Mac or Windows computer, DMG and MSI installers are available from [GitHub releases](https://github.com/Azure/azure-xplat-cli/releases).</span></span>

> [!TIP]
> <span data-ttu-id="ae616-126">Unter Windows können Sie auch den [Webplattform-Installer](https://go.microsoft.com/?linkid=9828653) herunterladen, um die klassische CLI zu installieren.</span><span class="sxs-lookup"><span data-stu-id="ae616-126">On Windows, you can also download the [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) to install the classic CLI.</span></span> <span data-ttu-id="ae616-127">Dieser Installer bietet Ihnen die Möglichkeit, zusätzliche Azure SDK- und -Befehlszeilentools zu installieren.</span><span class="sxs-lookup"><span data-stu-id="ae616-127">This installer gives you the option to install additional Azure SDK and command-line tools.</span></span>

## <a name="option-3-use-a-docker-container"></a><span data-ttu-id="ae616-128">Option 3: Verwenden eines Docker-Containers</span><span class="sxs-lookup"><span data-stu-id="ae616-128">Option 3: Use a Docker container</span></span>

<span data-ttu-id="ae616-129">Wenn Sie Ihren Computer als [Docker](https://docs.docker.com/engine/understanding-docker/)-Host eingerichtet haben, können Sie die klassische Azure CLI in einem Docker-Container ausführen.</span><span class="sxs-lookup"><span data-stu-id="ae616-129">If you have set up your computer as a [Docker](https://docs.docker.com/engine/understanding-docker/) host, you can run the Azure classic CLI in a Docker container.</span></span> <span data-ttu-id="ae616-130">Führen Sie den folgenden Befehl aus (bei Linux-Distributionen müssen Sie unter Umständen `sudo` verwenden):</span><span class="sxs-lookup"><span data-stu-id="ae616-130">Run the following command (on Linux distributions you might need to use `sudo`):</span></span>

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-classic-cli-commands"></a><span data-ttu-id="ae616-131">Ausführen von Befehlen der klassischen Azure CLI</span><span class="sxs-lookup"><span data-stu-id="ae616-131">Run Azure classic CLI commands</span></span>

<span data-ttu-id="ae616-132">Nachdem die klassische Azure CLI installiert wurde, können Sie den Befehl `azure` in der Befehlszeilenschnittstelle (Bash, Terminal, Eingabeaufforderung usw.) ausführen.</span><span class="sxs-lookup"><span data-stu-id="ae616-132">After the classic CLI is installed, run the `azure` command from your command-line user interface (Bash, Terminal, Command prompt, and so on).</span></span> <span data-ttu-id="ae616-133">Um beispielsweise den Hilfebefehl auszuführen, geben Sie Folgendes ein:</span><span class="sxs-lookup"><span data-stu-id="ae616-133">For example, to run the help command, type the following:</span></span>

```azurecli-interactive
azure help
```

> [!NOTE]
> <span data-ttu-id="ae616-134">In einigen Linux-Distributionen erhalten Sie unter Umständen eine Fehlermeldung wie `/usr/bin/env: ‘node’: No such file or directory`.</span><span class="sxs-lookup"><span data-stu-id="ae616-134">On some Linux distributions, you may receive an error similar to `/usr/bin/env: ‘node’: No such file or directory`.</span></span> <span data-ttu-id="ae616-135">Dieser Fehler stammt von kürzlich durchgeführten Installationen von „Node.js“, die unter „/usr/bin/nodejs“ installiert sind.</span><span class="sxs-lookup"><span data-stu-id="ae616-135">This error comes from recent installations of Node.js being installed at /usr/bin/nodejs.</span></span> <span data-ttu-id="ae616-136">Erstellen Sie zum Beheben dieses Fehlers eine symbolische Verknüpfung mit „/usr/bin/node“, indem Sie den folgenden Befehl ausführen:</span><span class="sxs-lookup"><span data-stu-id="ae616-136">To fix it, create a symbolic link to /usr/bin/node by running this command:</span></span>

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

<span data-ttu-id="ae616-137">Geben Sie Folgendes ein, um die Version der installierten klassischen Azure CLI anzuzeigen:</span><span class="sxs-lookup"><span data-stu-id="ae616-137">To see the version of the Azure classic CLI installed, type the following:</span></span>

```azurecli-interactive
azure --version
```

> [!NOTE]
> <span data-ttu-id="ae616-138">Wenn Sie die klassische Azure CLI zum ersten Mal verwenden, werden Sie in einer Meldung gefragt, ob Sie Microsoft das Erfassen von Nutzungsinformationen erlauben möchten.</span><span class="sxs-lookup"><span data-stu-id="ae616-138">When you first use Azure classic CLI, you see a message asking if you want to allow Microsoft to collect usage information.</span></span> <span data-ttu-id="ae616-139">Die Teilnahme ist freiwillig.</span><span class="sxs-lookup"><span data-stu-id="ae616-139">Participation is voluntary.</span></span> <span data-ttu-id="ae616-140">Wenn Sie sich für die Teilnahme entscheiden, können Sie diese durch Ausführen von `azure telemetry --disable`jederzeit beenden.</span><span class="sxs-lookup"><span data-stu-id="ae616-140">If you choose to participate, you can stop at any time by running `azure telemetry --disable`.</span></span> <span data-ttu-id="ae616-141">Zum Aktivieren der Teilnahme können Sie jederzeit `azure telemetry --enable`ausführen.</span><span class="sxs-lookup"><span data-stu-id="ae616-141">To enable participation at any time, run `azure telemetry --enable`.</span></span>

## <a name="update-the-classic-cli"></a><span data-ttu-id="ae616-142">Aktualisieren der klassischen CLI</span><span class="sxs-lookup"><span data-stu-id="ae616-142">Update the classic CLI</span></span>

<span data-ttu-id="ae616-143">Microsoft veröffentlicht ggf. aktualisierte Versionen der klassischen Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="ae616-143">Microsoft may release updated versions of the Azure classic CLI.</span></span> <span data-ttu-id="ae616-144">Installieren Sie die klassische CLI erneut, indem Sie das Installationsprogramm für Ihr Betriebssystem verwenden, oder führen Sie den neuesten Docker-Container aus.</span><span class="sxs-lookup"><span data-stu-id="ae616-144">Reinstall the classic CLI using the installer for your operating system, or run the latest Docker container.</span></span> <span data-ttu-id="ae616-145">Falls Node.js und npm installiert sind, können Sie die Aktualisierung durchführen, indem Sie Folgendes eingeben (bei Linux-Distributionen müssen Sie unter Umständen `sudo` verwenden):</span><span class="sxs-lookup"><span data-stu-id="ae616-145">Or, if you have the latest Node.js and npm installed, update by typing the following (on Linux distributions you might need to use `sudo`).</span></span>

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a><span data-ttu-id="ae616-146">Aktivieren der Vervollständigung mit der TAB-Taste</span><span class="sxs-lookup"><span data-stu-id="ae616-146">Enable tab completion</span></span>

<span data-ttu-id="ae616-147">Die Vervollständigung mit der TAB-Taste für Befehle der klassischen CLI wird für Mac und Linux unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae616-147">Tab completion of classic CLI commands is supported for Mac and Linux.</span></span>

<span data-ttu-id="ae616-148">Für die Aktivierung in zsh führen Sie Folgendes aus:</span><span class="sxs-lookup"><span data-stu-id="ae616-148">To enable it in zsh, run:</span></span>

```bash
echo '. <(azure --completion)' >> .zshrc
```

<span data-ttu-id="ae616-149">Für die Aktivierung in bash führen Sie Folgendes aus:</span><span class="sxs-lookup"><span data-stu-id="ae616-149">To enable it in bash, run:</span></span>

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```

## <a name="next-steps"></a><span data-ttu-id="ae616-150">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="ae616-150">Next steps</span></span>

* <span data-ttu-id="ae616-151">Wenn Sie weitere Informationen zur klassischen Azure CLI erhalten, den Quellcode herunterladen, Probleme melden oder etwas zum Projekt beitragen möchten, hilft Ihnen der Artikel [GitHub repository for the Azure classic CLI](https://github.com/azure/azure-xplat-cli) (GitHub-Repository für die klassische Azure CLI) weiter.</span><span class="sxs-lookup"><span data-stu-id="ae616-151">To learn more about the Azure classic CLI, download source code, report problems, or contribute to the project, visit the [GitHub repository for the Azure classic CLI](https://github.com/azure/azure-xplat-cli).</span></span>

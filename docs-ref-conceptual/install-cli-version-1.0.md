---
title: Installieren von Azure CLI 1.0
description: Installieren von Azure CLI 1.0 für Mac, Linux und Windows für das Starten von Azure-Diensten
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/20/2017
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 5f185e02217d6a3b54a9c252825c0f3fed3ab09e
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967672"
---
# <a name="install-the-azure-cli-10"></a><span data-ttu-id="08e3f-103">Installieren von Azure CLI 1.0</span><span class="sxs-lookup"><span data-stu-id="08e3f-103">Install the Azure CLI 1.0</span></span>

> [!IMPORTANT]
> <span data-ttu-id="08e3f-104">Dieses Thema beschreibt, wie Sie die Azure CLI 1.0 installieren.</span><span class="sxs-lookup"><span data-stu-id="08e3f-104">This topic describes how to install the Azure CLI 1.0.</span></span> <span data-ttu-id="08e3f-105">Diese CLI ist veraltet und sollte nur als Unterstützung in Verbindung mit dem ASM-Modell (Azure Service Management, Azure-Dienstverwaltung) mit „klassischen“ Ressourcen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="08e3f-105">This CLI is deprecated and should only be used for support with the Azure Service Management (ASM) model with "classic" resources.</span></span>
> <span data-ttu-id="08e3f-106">Verwenden Sie für Azure Resource Manager-Bereitstellungen [Azure CLI 2.0](/cli/azure).</span><span class="sxs-lookup"><span data-stu-id="08e3f-106">For Azure Resource Manager deployments, use [Azure CLI 2.0](/cli/azure).</span></span>

<span data-ttu-id="08e3f-107">Installieren Sie schnell die Azure-Befehlszeilenschnittstelle (Azure CLI 1.0), um eine Reihe von auf der Shell basierenden Open-Source-Befehlen für das Erstellen und Verwalten von Ressourcen in Microsoft Azure zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="08e3f-107">Quickly install the Azure Command-Line Interface (Azure CLI 1.0) to use a set of open-source shell-based commands for creating and managing resources in Microsoft Azure.</span></span> <span data-ttu-id="08e3f-108">Zum Installieren dieser plattformübergreifenden Tools auf Ihrem Computer stehen Ihnen mehrere Optionen zur Verfügung:</span><span class="sxs-lookup"><span data-stu-id="08e3f-108">You have several options to install these cross-platform tools on your computer:</span></span>

* <span data-ttu-id="08e3f-109">**npm-Paket:** Führen Sie npm (den Paket-Manager für JavaScript) aus, um das neueste Azure CLI 1.0-Paket auf Ihrer Linux-Distribution oder dem Betriebssystem zu installieren.</span><span class="sxs-lookup"><span data-stu-id="08e3f-109">**npm package** - Run npm (the package manager for JavaScript) to install the latest Azure CLI 1.0 package on your Linux distribution or OS.</span></span> <span data-ttu-id="08e3f-110">Dafür sind Node.js und npm auf Ihrem Computer erforderlich.</span><span class="sxs-lookup"><span data-stu-id="08e3f-110">Requires node.js and npm on your computer.</span></span>
* <span data-ttu-id="08e3f-111">**Installer** : Laden Sie ein Installationsprogramm für die einfache Installation unter Mac OS oder Windows herunter.</span><span class="sxs-lookup"><span data-stu-id="08e3f-111">**Installer** - Download an installer for easy installation on Mac or Windows.</span></span>
* <span data-ttu-id="08e3f-112">**Docker-Container** : Beginnen Sie mit der Verwendung der neuesten Befehlszeilenschnittstelle in einem sofort betriebsbereiten Docker-Container.</span><span class="sxs-lookup"><span data-stu-id="08e3f-112">**Docker container** - Start using the latest CLI in a ready-to-run Docker container.</span></span> <span data-ttu-id="08e3f-113">Dazu benötigen Sie den Docker-Host auf Ihrem Computer.</span><span class="sxs-lookup"><span data-stu-id="08e3f-113">Requires Docker host on your computer.</span></span>

<span data-ttu-id="08e3f-114">Weitere Optionen und Hintergrundinformationen finden Sie im Projektrepository auf [GitHub](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="08e3f-114">For more options and background, see the project repository on [GitHub](https://github.com/azure/azure-xplat-cli).</span></span>

<span data-ttu-id="08e3f-115">Sobald Azure CLI 1.0 installiert ist, [verbinden Sie die Befehlszeilenschnittstelle mit Ihrem Azure-Abonnement](/cli/azure/authenticate-azure-cli), und führen Sie die **azure**-Befehle über die Befehlszeilenschnittstelle (Bash, Terminal, Eingabeaufforderung usw.) für die Arbeit mit Ihren Azure-Ressourcen aus.</span><span class="sxs-lookup"><span data-stu-id="08e3f-115">Once the Azure CLI 1.0 is installed, [connect it with your Azure subscription](/cli/azure/authenticate-azure-cli) and run the **azure** commands from your command-line interface (Bash, Terminal, Command prompt, and so on) to work with your Azure resources.</span></span>

## <a name="option-1-install-an-npm-package"></a><span data-ttu-id="08e3f-116">Option 1: Installieren eines npm-Pakets</span><span class="sxs-lookup"><span data-stu-id="08e3f-116">Option 1: Install an npm package</span></span>

<span data-ttu-id="08e3f-117">Um die CLI aus einem npm-Paket zu installieren, müssen Sie die aktuellen Versionen von [Node.js und npm](https://nodejs.org/en/download/package-manager/) herunterladen und installieren.</span><span class="sxs-lookup"><span data-stu-id="08e3f-117">To install the CLI from an npm package, make sure you have downloaded and installed the [latest Node.js and npm](https://nodejs.org/en/download/package-manager/).</span></span> <span data-ttu-id="08e3f-118">Führen Sie anschließend zum Installieren des Azure-CLI-Pakets **npm install** aus:</span><span class="sxs-lookup"><span data-stu-id="08e3f-118">Then, run **npm install** to install the azure-cli package:</span></span>

```bash
npm install -g azure-cli
```

<span data-ttu-id="08e3f-119">Bei Linux-Distributionen müssen Sie möglicherweise **sudo** wie folgt verwenden, um den Befehl **npm** erfolgreich ausführen zu können:</span><span class="sxs-lookup"><span data-stu-id="08e3f-119">On Linux distributions, you might need to use **sudo** to successfully run the **npm** command, as follows:</span></span>

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> <span data-ttu-id="08e3f-120">Falls Sie Node.js und npm für Ihre Linux-Distribution oder Ihr Betriebssystem installieren oder aktualisieren müssen, wird die Installation der aktuellsten LTS-Version von Node.js (4.x) empfohlen.</span><span class="sxs-lookup"><span data-stu-id="08e3f-120">If you need to install or update Node.js and npm on your Linux distribution or OS, we recommend that you install the most recent Node.js LTS version (4.x).</span></span> <span data-ttu-id="08e3f-121">Wenn Sie eine ältere Version verwenden, kommt es möglicherweise zu Fehlern bei der Installation.</span><span class="sxs-lookup"><span data-stu-id="08e3f-121">If you use an older version, you might get installation errors.</span></span>

<span data-ttu-id="08e3f-122">Falls gewünscht, laden Sie die neuesten Linux-[TAR-Datei][linux-installer] für das npm-Paket lokal herunter.</span><span class="sxs-lookup"><span data-stu-id="08e3f-122">If you prefer, download the latest Linux [tar file][linux-installer] for the npm package locally.</span></span> <span data-ttu-id="08e3f-123">Installieren Sie dann das heruntergeladene npm-Paket wie folgt (in Linux-Distributionen müssen Sie möglicherweise **sudo**verwenden):</span><span class="sxs-lookup"><span data-stu-id="08e3f-123">Then, install the downloaded npm package as follows (on Linux distributions you might need to use **sudo**):</span></span>

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a><span data-ttu-id="08e3f-124">Option 2: Verwenden eines Installers</span><span class="sxs-lookup"><span data-stu-id="08e3f-124">Option 2: Use an installer</span></span>

<span data-ttu-id="08e3f-125">Wenn Sie einen Mac- oder Windows-Computer verwenden, stehen die folgenden CLI-Installer zum Download zur Verfügung:</span><span class="sxs-lookup"><span data-stu-id="08e3f-125">If you use a Mac or Windows computer, the following CLI installers are available for download:</span></span>

* <span data-ttu-id="08e3f-126">[Mac OS X-Installer][mac-installer]</span><span class="sxs-lookup"><span data-stu-id="08e3f-126">[Mac OS X installer][mac-installer]</span></span>
* <span data-ttu-id="08e3f-127">[Windows-MSI][windows-installer]</span><span class="sxs-lookup"><span data-stu-id="08e3f-127">[Windows MSI][windows-installer]</span></span>

> [!TIP]
> <span data-ttu-id="08e3f-128">Unter Windows können Sie auch den [Webplattform-Installer](https://go.microsoft.com/?linkid=9828653) herunterladen, um die Befehlszeilenschnittstelle zu installieren.</span><span class="sxs-lookup"><span data-stu-id="08e3f-128">On Windows, you can also download the [Web Platform Installer](https://go.microsoft.com/?linkid=9828653) to install the CLI.</span></span> <span data-ttu-id="08e3f-129">Dieser Installer bietet Ihnen die Möglichkeit, nach der Installation der Befehlszeilenschnittstelle zusätzliche Azure SDK- und -Befehlszeilentools zu installieren.</span><span class="sxs-lookup"><span data-stu-id="08e3f-129">This installer gives you the option to install additional Azure SDK and command-line tools after installing the CLI.</span></span>

## <a name="option-3-use-a-docker-container"></a><span data-ttu-id="08e3f-130">Option 3: Verwenden eines Docker-Containers</span><span class="sxs-lookup"><span data-stu-id="08e3f-130">Option 3: Use a Docker container</span></span>

<span data-ttu-id="08e3f-131">Wenn Sie Ihren Computer als [Docker](https://docs.docker.com/engine/understanding-docker/)-Host eingerichtet haben, können Sie die neueste Azure CLI 1.0 in einem Docker-Container ausführen.</span><span class="sxs-lookup"><span data-stu-id="08e3f-131">If you have set up your computer as a [Docker](https://docs.docker.com/engine/understanding-docker/) host, you can run the latest Azure CLI 1.0 in a Docker container.</span></span> <span data-ttu-id="08e3f-132">Führen Sie den folgenden Befehl aus (bei Linux-Distributionen müssen Sie möglicherweise **sudo** verwenden):</span><span class="sxs-lookup"><span data-stu-id="08e3f-132">Run the following command (on Linux distributions you might need to use **sudo**):</span></span>

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-cli-10-commands"></a><span data-ttu-id="08e3f-133">Ausführen von Azure CLI 1.0-Befehlen</span><span class="sxs-lookup"><span data-stu-id="08e3f-133">Run Azure CLI 1.0 commands</span></span>

<span data-ttu-id="08e3f-134">Sobald Azure CLI 1.0 installiert ist, führen Sie den Befehl **azure** in der Befehlszeilenschnittstelle (Bash, Terminal, Eingabeaufforderung usw.) aus.</span><span class="sxs-lookup"><span data-stu-id="08e3f-134">After the Azure CLI 1.0 is installed, run the **azure** command from your command-line user interface (Bash, Terminal, Command prompt, and so on).</span></span> <span data-ttu-id="08e3f-135">Um beispielsweise den Hilfebefehl auszuführen, geben Sie Folgendes ein:</span><span class="sxs-lookup"><span data-stu-id="08e3f-135">For example, to run the help command, type the following:</span></span>

```azurecli
azure help
```

> [!NOTE]
> <span data-ttu-id="08e3f-136">In einigen Linux-Distributionen erhalten Sie unter Umständen eine Fehlermeldung wie `/usr/bin/env: ‘node’: No such file or directory`.</span><span class="sxs-lookup"><span data-stu-id="08e3f-136">On some Linux distributions, you may receive an error similar to `/usr/bin/env: ‘node’: No such file or directory`.</span></span> <span data-ttu-id="08e3f-137">Dieser Fehler stammt von kürzlich durchgeführten Installationen von „Node.js“, die unter „/usr/bin/nodejs“ installiert sind.</span><span class="sxs-lookup"><span data-stu-id="08e3f-137">This error comes from recent installations of Node.js being installed at /usr/bin/nodejs.</span></span> <span data-ttu-id="08e3f-138">Erstellen Sie zum Beheben dieses Fehlers eine symbolische Verknüpfung mit „/usr/bin/node“, indem Sie den folgenden Befehl ausführen:</span><span class="sxs-lookup"><span data-stu-id="08e3f-138">To fix it, create a symbolic link to /usr/bin/node by running this command:</span></span>

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

<span data-ttu-id="08e3f-139">Um die installierte Version von Azure CLI 1.0 anzuzeigen, geben Sie Folgendes ein:</span><span class="sxs-lookup"><span data-stu-id="08e3f-139">To see the version of the Azure CLI 1.0 you installed, type the following:</span></span>

```azurecli
azure --version
```

<span data-ttu-id="08e3f-140">Jetzt sind Sie soweit.</span><span class="sxs-lookup"><span data-stu-id="08e3f-140">Now you are ready!</span></span> <span data-ttu-id="08e3f-141">Um Zugriff auf alle CLI-Befehle für die Arbeit mit Ihren eigenen Ressourcen zu erhalten, [stellen Sie über die Azure-CLI eine Verbindung mit Ihrem Azure-Abonnement her](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="08e3f-141">To access all the CLI commands to work with your own resources, [connect to your Azure subscription from the Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="08e3f-142">Wenn Sie die Azure-CLI zum ersten Mal verwenden, werden Sie in einer Meldung gefragt, ob Sie Microsoft das Erfassen von Nutzungsinformationen erlauben möchten.</span><span class="sxs-lookup"><span data-stu-id="08e3f-142">When you first use Azure CLI, you see a message asking if you want to allow Microsoft to collect usage information.</span></span> <span data-ttu-id="08e3f-143">Die Teilnahme ist freiwillig.</span><span class="sxs-lookup"><span data-stu-id="08e3f-143">Participation is voluntary.</span></span> <span data-ttu-id="08e3f-144">Wenn Sie sich für die Teilnahme entscheiden, können Sie diese durch Ausführen von `azure telemetry --disable`jederzeit beenden.</span><span class="sxs-lookup"><span data-stu-id="08e3f-144">If you choose to participate, you can stop at any time by running `azure telemetry --disable`.</span></span> <span data-ttu-id="08e3f-145">Zum Aktivieren der Teilnahme können Sie jederzeit `azure telemetry --enable`ausführen.</span><span class="sxs-lookup"><span data-stu-id="08e3f-145">To enable participation at any time, run `azure telemetry --enable`.</span></span>

## <a name="update-the-cli"></a><span data-ttu-id="08e3f-146">Aktualisieren der CLI</span><span class="sxs-lookup"><span data-stu-id="08e3f-146">Update the CLI</span></span>

<span data-ttu-id="08e3f-147">Microsoft veröffentlicht regelmäßig aktualisierte Versionen der Azure-Befehlszeilenschnittstelle.</span><span class="sxs-lookup"><span data-stu-id="08e3f-147">Microsoft frequently releases updated versions of the Azure CLI.</span></span> <span data-ttu-id="08e3f-148">Installieren Sie die CLI erneut, indem Sie das Installationsprogramm für Ihr Betriebssystem verwenden, oder führen Sie den neuesten Docker-Container aus.</span><span class="sxs-lookup"><span data-stu-id="08e3f-148">Reinstall the CLI using the installer for your operating system, or run the latest Docker container.</span></span> <span data-ttu-id="08e3f-149">Oder wenn Node.js und npm installiert sind, aktualisieren Sie sie, indem Sie Folgendes eingeben (bei Linux-Distributionen müssen Sie möglicherweise **sudo**verwenden).</span><span class="sxs-lookup"><span data-stu-id="08e3f-149">Or, if you have the latest Node.js and npm installed, update by typing the following (on Linux distributions you might need to use **sudo**).</span></span>

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a><span data-ttu-id="08e3f-150">Aktivieren der Vervollständigung mit der TAB-Taste</span><span class="sxs-lookup"><span data-stu-id="08e3f-150">Enable tab completion</span></span>

<span data-ttu-id="08e3f-151">Die Vervollständigung mit der TAB-Taste für CLI-Befehle wird für Mac und Linux unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08e3f-151">Tab completion of CLI commands is supported for Mac and Linux.</span></span>

<span data-ttu-id="08e3f-152">Für die Aktivierung in zsh führen Sie Folgendes aus:</span><span class="sxs-lookup"><span data-stu-id="08e3f-152">To enable it in zsh, run:</span></span>

```bash
echo '. <(azure --completion)' >> .zshrc
```

<span data-ttu-id="08e3f-153">Für die Aktivierung in bash führen Sie Folgendes aus:</span><span class="sxs-lookup"><span data-stu-id="08e3f-153">To enable it in bash, run:</span></span>

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```

## <a name="next-steps"></a><span data-ttu-id="08e3f-154">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="08e3f-154">Next steps</span></span>

* <span data-ttu-id="08e3f-155">[Verbinden mit Ihrem Azure-Abonnement über die CLI](/cli/azure/authenticate-azure-cli) zum Erstellen und Verwalten von Azure-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="08e3f-155">[Connect from the CLI to your Azure subscription](/cli/azure/authenticate-azure-cli) to create and manage Azure resources.</span></span>
* <span data-ttu-id="08e3f-156">Wenn Sie weitere Informationen zur Azure-Befehlszeilenschnittstelle erhalten, den Quellcode herunterladen, Probleme melden oder etwas zum Projekt beitragen möchten, besuchen Sie die Webseite [GitHub repository for the Azure CLI](https://github.com/azure/azure-xplat-cli).</span><span class="sxs-lookup"><span data-stu-id="08e3f-156">To learn more about the Azure CLI, download source code, report problems, or contribute to the project, visit the [GitHub repository for the Azure CLI](https://github.com/azure/azure-xplat-cli).</span></span>
* <span data-ttu-id="08e3f-157">Wenn Sie Fragen zur Verwendung der Azure-CLI oder zu Azure haben, besuchen Sie die [Azure-Foren](https://social.msdn.microsoft.com/Forums/en-US/home?forum=azurescripting).</span><span class="sxs-lookup"><span data-stu-id="08e3f-157">If you have questions about using the Azure CLI, or Azure, visit the [Azure Forums](https://social.msdn.microsoft.com/Forums/en-US/home?forum=azurescripting).</span></span>

[mac-installer]: http://aka.ms/mac-azure-cli
[windows-installer]: http://aka.ms/webpi-azure-cli
[linux-installer]: http://aka.ms/linux-azure-cli
[cliasm]: /cli/azure/get-started-with-az-cli2
[cliarm]: ./virtual-machines/azure-cli-arm-commands.md

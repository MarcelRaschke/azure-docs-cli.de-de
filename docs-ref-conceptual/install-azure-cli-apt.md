---
title: Installieren der Azure CLI unter Linux mit apt
description: Installieren der Azure CLI mit dem apt-Paket-Manager
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/08/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: f22ada48502602cb4d9b502cb887412a6ddcf5cf
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516343"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="4566f-103">Installieren der Azure CLI mit apt</span><span class="sxs-lookup"><span data-stu-id="4566f-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="4566f-104">Wenn Sie eine Distribution mit `apt` verwenden (etwa Ubuntu oder Debian), steht ein x86_64-Paket für die Azure CLI zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="4566f-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's an x86_64 package available for the Azure CLI.</span></span> <span data-ttu-id="4566f-105">Dieses Paket wurde mit folgenden Produkten getestet und wird für diese unterstützt:</span><span class="sxs-lookup"><span data-stu-id="4566f-105">This package has been tested with and is supported for:</span></span>

* <span data-ttu-id="4566f-106">Ubuntu Trusty, Senial, Artful, Bionic und Disco</span><span class="sxs-lookup"><span data-stu-id="4566f-106">Ubuntu trusty, xenial, artful, bionic, and disco</span></span>
* <span data-ttu-id="4566f-107">Debian Wheezy, Jessie und Stretch</span><span class="sxs-lookup"><span data-stu-id="4566f-107">Debian wheezy, jessie, and stretch</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="4566f-108">Das Paket für die Azure CLI installiert einen eigenen Python-Interpreter und verwendet nicht die Python-Version des Systems.</span><span class="sxs-lookup"><span data-stu-id="4566f-108">The package for Azure CLI installs its own Python interpreter, and does not use the system Python.</span></span>

## <a name="install"></a><span data-ttu-id="4566f-109">Installieren</span><span class="sxs-lookup"><span data-stu-id="4566f-109">Install</span></span>

<span data-ttu-id="4566f-110">Wir bieten zwei Möglichkeiten zum Installieren der Azure-Befehlszeilenschnittstelle (Azure Command Line Interface, Azure CLI) mit Verteilungen, die `apt` unterstützen: Als All-in-One-Skript, das die Installationsbefehle für Sie ausführt, und mithilfe von Anweisungen, die Sie Schritt für Schritt selbst ausführen können.</span><span class="sxs-lookup"><span data-stu-id="4566f-110">We offer two ways to install the Azure CLI with distributions that support `apt`: As an all-in-one script that runs the install commands for you, and instructions that you can run as a step-by-step process on your own.</span></span>

### <a name="install-with-one-command"></a><span data-ttu-id="4566f-111">Installieren mit einem Befehl</span><span class="sxs-lookup"><span data-stu-id="4566f-111">Install with one command</span></span>

<span data-ttu-id="4566f-112">Wir bieten und pflegen ein Skript, das alle Installationsbefehle in einem Schritt ausführt.</span><span class="sxs-lookup"><span data-stu-id="4566f-112">We offer and maintain a script which runs all of the installation commands in one step.</span></span> <span data-ttu-id="4566f-113">Führen Sie das Skript mit `curl` aus, und leiten Sie es direkt an `bash` um, oder laden Sie das Skript in eine Datei herunter, und überprüfen Sie es vor dem Ausführen.</span><span class="sxs-lookup"><span data-stu-id="4566f-113">Run it by using `curl` and pipe directly to `bash`, or download the script to a file and inspect it before running.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4566f-114">Dieses Skript wurde nur für Ubuntu 16.04 und höher und Debian 8 und höher geprüft.</span><span class="sxs-lookup"><span data-stu-id="4566f-114">This script is only verified for Ubuntu 16.04+ and Debian 8+.</span></span> <span data-ttu-id="4566f-115">Bei anderen Verteilungen funktioniert es möglicherweise nicht.</span><span class="sxs-lookup"><span data-stu-id="4566f-115">It may not work on other distributions.</span></span>
> <span data-ttu-id="4566f-116">Wenn Sie eine abgeleitete Verteilung wie Linux Mint verwenden, folgen Sie den Anweisungen für die manuelle Installation, und führen Sie ggf. eine Problembehandlung durch.</span><span class="sxs-lookup"><span data-stu-id="4566f-116">If you're using a derived distribution such as Linux Mint, follow the manual install instructions and perform any necessary troubleshooting.</span></span>

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

### <a name="manual-install-instructions"></a><span data-ttu-id="4566f-117">Anweisungen für die manuelle Installation</span><span class="sxs-lookup"><span data-stu-id="4566f-117">Manual install instructions</span></span>

<span data-ttu-id="4566f-118">Falls Sie ein Skript nicht als Superuser ausführen möchten, führen Sie die folgenden Schritte zum manuellen Installieren der Azure CLI aus.</span><span class="sxs-lookup"><span data-stu-id="4566f-118">If you don't want to run a script as superuser, follow these manual steps to install the Azure CLI.</span></span>

1. <span data-ttu-id="4566f-119">Laden Sie die für die Installation erforderlichen Pakete herunter:</span><span class="sxs-lookup"><span data-stu-id="4566f-119">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gnupg
    ```

2. <span data-ttu-id="4566f-120">Laden Sie den Microsoft-Signaturschlüssel herunter, und installieren Sie ihn.</span><span class="sxs-lookup"><span data-stu-id="4566f-120">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="4566f-121">Fügen Sie das Azure CLI-Softwarerepository hinzu:</span><span class="sxs-lookup"><span data-stu-id="4566f-121">Add the Azure CLI software repository:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="4566f-122">Aktualisieren Sie die Repositoryinformationen, und installieren Sie das Paket `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="4566f-122">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

<span data-ttu-id="4566f-123">Führen Sie die Azure CLI mit dem Befehl `az` aus.</span><span class="sxs-lookup"><span data-stu-id="4566f-123">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="4566f-124">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="4566f-124">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="4566f-125">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="4566f-125">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="4566f-126">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="4566f-126">Troubleshooting</span></span>

<span data-ttu-id="4566f-127">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="4566f-127">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="4566f-128">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="4566f-128">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="4566f-129">„lsb_release“ gibt nicht die richtige Basisdistributionsversion zurück.</span><span class="sxs-lookup"><span data-stu-id="4566f-129">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="4566f-130">Einige von Ubuntu oder Debian abgeleiteten Distributionen wie Linux Mint geben über `lsb_release` unter Umständen nicht den richtigen Versionsnamen zurück.</span><span class="sxs-lookup"><span data-stu-id="4566f-130">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="4566f-131">Mit diesem Wert wird im Installationsprozess das zu installierende Pakete ermittelt.</span><span class="sxs-lookup"><span data-stu-id="4566f-131">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="4566f-132">Wenn Sie den Codenamen der Ubuntu- oder Debian-Version kennen, von der Ihre Distribution abgeleitet ist, können Sie beim [Hinzufügen des Repositorys](#set-release) den Wert `AZ_REPO` manuell festlegen.</span><span class="sxs-lookup"><span data-stu-id="4566f-132">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="4566f-133">Sehen Sie sich andernfalls Informationen dazu an, wie Sie für Ihre Distribution den Basisdistributions-Codenamen ermitteln, und legen Sie `AZ_REPO` auf den richtigen Wert fest.</span><span class="sxs-lookup"><span data-stu-id="4566f-133">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="4566f-134">Kein Paket für Ihre Distribution</span><span class="sxs-lookup"><span data-stu-id="4566f-134">No package for your distribution</span></span>

<span data-ttu-id="4566f-135">Manchmal dauert es nach der Veröffentlichung einer Distribution etwas, bis ein Azure CLI-Paket dafür zur Verfügung gestellt wird.</span><span class="sxs-lookup"><span data-stu-id="4566f-135">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="4566f-136">Die Azure CLI ist im Hinblick auf zukünftige Abhängigkeitsversionen resilient konzipiert und nutzt daher möglichst wenige dieser Abhängigkeiten.</span><span class="sxs-lookup"><span data-stu-id="4566f-136">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="4566f-137">Ist für Ihre Basisdistribution kein Paket verfügbar, verwenden Sie ein Paket für eine ältere Distribution.</span><span class="sxs-lookup"><span data-stu-id="4566f-137">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="4566f-138">Legen Sie dazu beim [Hinzufügen des Repositorys](#set-release) den Wert `AZ_REPO` manuell fest.</span><span class="sxs-lookup"><span data-stu-id="4566f-138">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="4566f-139">Verwenden Sie für Ubuntu-Distributionen das Repository `bionic` und für Debian-Distributionen `stretch`.</span><span class="sxs-lookup"><span data-stu-id="4566f-139">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="4566f-140">Distributionen, die vor Ubuntu Trusty und Debian Wheezy veröffentlicht wurden, werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4566f-140">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="4566f-141">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="4566f-141">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="4566f-142">Konfigurieren Sie `apt` explizit so, dass dieser Proxy immer verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="4566f-142">You may also want to explicitly configure `apt` to use this proxy at all times.</span></span> <span data-ttu-id="4566f-143">Stellen Sie sicher, dass die folgenden Zeilen in einer `apt`-Konfigurationsdatei in `/etc/apt/apt.conf.d/` erscheinen.</span><span class="sxs-lookup"><span data-stu-id="4566f-143">Make sure that the following lines appear in an `apt` configuration file in `/etc/apt/apt.conf.d/`.</span></span> <span data-ttu-id="4566f-144">Wir empfehlen, dass Sie Ihre vorhandene globale Konfigurationsdatei, eine vorhandene Proxykonfigurationsdatei, `40proxies` oder `99local` verwenden. Berücksichtigen Sie dabei jedoch die Verwaltungsanforderungen Ihres Systems.</span><span class="sxs-lookup"><span data-stu-id="4566f-144">We recommend using either your existing global configuration file, an existing proxy configuration file, `40proxies`, or `99local`, but follow your system administration requirements.</span></span>

```apt.conf
Acquire {
    http::proxy "http://[username]:[password]@[proxy]:[port]";
    https::proxy "https://[username]:[password]@[proxy]:[port]";
}
```

<span data-ttu-id="4566f-145">Wenn Ihr Proxy keine Standardauthentifizierung verwendet, __entfernen__ Sie den Teil `[username]:[password]@` des Proxy-URI.</span><span class="sxs-lookup"><span data-stu-id="4566f-145">If your proxy does not use basic auth, __remove__ the `[username]:[password]@` portion of the proxy URI.</span></span> <span data-ttu-id="4566f-146">Weitere Informationen zur Proxykonfiguration finden Sie in der offiziellen Ubuntu-Dokumentation:</span><span class="sxs-lookup"><span data-stu-id="4566f-146">If you require more information for proxy configuration, see the official Ubuntu documentation:</span></span>

* [<span data-ttu-id="4566f-147">apt.conf manpage</span><span class="sxs-lookup"><span data-stu-id="4566f-147">apt.conf manpage</span></span>](http://manpages.ubuntu.com/manpages/bionic/en/man5/apt.conf.5.html)
* [<span data-ttu-id="4566f-148">Ubuntu Wiki – apt-get howto</span><span class="sxs-lookup"><span data-stu-id="4566f-148">Ubuntu wiki - apt-get howto</span></span>](https://help.ubuntu.com/community/AptGet/Howto#Setting_up_apt-get_to_use_a_http-proxy)

<span data-ttu-id="4566f-149">Zum Abrufen des Microsoft-Signaturschlüssels und des Pakets von unserem Repository muss Ihr Proxy HTTPS-Verbindungen mit der folgenden Adresse zulassen:</span><span class="sxs-lookup"><span data-stu-id="4566f-149">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="4566f-150">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4566f-150">Update</span></span>

<span data-ttu-id="4566f-151">Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.</span><span class="sxs-lookup"><span data-stu-id="4566f-151">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="4566f-152">Durch diesen Befehl werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="4566f-152">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="4566f-153">Wenn Sie nur ein Upgrade für die CLI durchführen möchten, verwenden Sie `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="4566f-153">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="4566f-154">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="4566f-154">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="4566f-155">Deinstallieren Sie sie mit `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="4566f-155">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="4566f-156">Entfernen Sie die Azure CLI-Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren:</span><span class="sxs-lookup"><span data-stu-id="4566f-156">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="4566f-157">Entfernen Sie den Signaturschlüssel:</span><span class="sxs-lookup"><span data-stu-id="4566f-157">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. <span data-ttu-id="4566f-158">Entfernen Sie alle nicht benötigten Pakete:</span><span class="sxs-lookup"><span data-stu-id="4566f-158">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="4566f-159">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="4566f-159">Next Steps</span></span>

<span data-ttu-id="4566f-160">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="4566f-160">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="4566f-161">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="4566f-161">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

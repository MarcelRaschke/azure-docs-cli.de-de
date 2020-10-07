---
title: Installieren der Azure CLI unter Linux mit apt
description: Installieren der Azure CLI mit dem apt-Paket-Manager
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/29/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 242c634717cf964af718873ab9ecf84ff707db3d
ms.sourcegitcommit: aa44ec97af5c0e7558d254b3159f95921e22ff1c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/01/2020
ms.locfileid: "91625413"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="50817-103">Installieren der Azure CLI mit apt</span><span class="sxs-lookup"><span data-stu-id="50817-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="50817-104">Wenn Sie eine Distribution mit `apt` verwenden (etwa Ubuntu oder Debian), steht ein x86_64-Paket für die Azure CLI zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="50817-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's an x86_64 package available for the Azure CLI.</span></span> <span data-ttu-id="50817-105">Dieses Paket wurde mit folgenden Produkten getestet und wird für diese unterstützt:</span><span class="sxs-lookup"><span data-stu-id="50817-105">This package has been tested with and is supported for:</span></span>

* <span data-ttu-id="50817-106">Ubuntu Trusty, Xenial, Bionic, Eoan und Focal</span><span class="sxs-lookup"><span data-stu-id="50817-106">Ubuntu trusty, xenial, bionic, eoan and focal</span></span>
* <span data-ttu-id="50817-107">Debian Jessie, Stretch und Buster</span><span class="sxs-lookup"><span data-stu-id="50817-107">Debian jessie, stretch, and buster</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="50817-108">Das Paket für die Azure CLI installiert einen eigenen Python-Interpreter und verwendet nicht die Python-Version des Systems.</span><span class="sxs-lookup"><span data-stu-id="50817-108">The package for Azure CLI installs its own Python interpreter, and does not use the system Python.</span></span> 
>
> <span data-ttu-id="50817-109">Unter Ubuntu 20.04 (Focal) ist ein vom `focal/universe`-Repository bereitgestelltes `azure-cli`-Paket mit der Version `2.0.81` verfügbar.</span><span class="sxs-lookup"><span data-stu-id="50817-109">On Ubuntu 20.04 (Focal), there is an `azure-cli` package with version `2.0.81` provided by the `focal/universe` repository.</span></span> <span data-ttu-id="50817-110">Es ist veraltet und wird nicht empfohlen.</span><span class="sxs-lookup"><span data-stu-id="50817-110">It's outdated and not recommended.</span></span> <span data-ttu-id="50817-111">Wenn Sie es bereits installiert haben, entfernen Sie es zunächst durch Ausführen von `sudo apt remove azure-cli -y && sudo apt autoremove -y`, bevor Sie die folgenden Schritte zum Installieren des aktuellen `azure-cli`-Pakets ausführen.</span><span class="sxs-lookup"><span data-stu-id="50817-111">If you already installed it, please remove it first by running `sudo apt remove azure-cli -y && sudo apt autoremove -y` before following the below steps to install the latest `azure-cli` package.</span></span>

## <a name="install"></a><span data-ttu-id="50817-112">Installieren</span><span class="sxs-lookup"><span data-stu-id="50817-112">Install</span></span>

<span data-ttu-id="50817-113">Wir bieten zwei Möglichkeiten zum Installieren der Azure-Befehlszeilenschnittstelle (Azure Command Line Interface, Azure CLI) mit Verteilungen, die `apt` unterstützen: Als All-in-One-Skript, das die Installationsbefehle für Sie ausführt, und mithilfe von Anweisungen, die Sie Schritt für Schritt selbst ausführen können.</span><span class="sxs-lookup"><span data-stu-id="50817-113">We offer two ways to install the Azure CLI with distributions that support `apt`: As an all-in-one script that runs the install commands for you, and instructions that you can run as a step-by-step process on your own.</span></span>

### <a name="install-with-one-command"></a><span data-ttu-id="50817-114">Installieren mit einem Befehl</span><span class="sxs-lookup"><span data-stu-id="50817-114">Install with one command</span></span>

<span data-ttu-id="50817-115">Wir bieten und pflegen ein Skript, das alle Installationsbefehle in einem Schritt ausführt.</span><span class="sxs-lookup"><span data-stu-id="50817-115">We offer and maintain a script which runs all of the installation commands in one step.</span></span> <span data-ttu-id="50817-116">Führen Sie das Skript mit `curl` aus, und leiten Sie es direkt an `bash` um, oder laden Sie das Skript in eine Datei herunter, und überprüfen Sie es vor dem Ausführen.</span><span class="sxs-lookup"><span data-stu-id="50817-116">Run it by using `curl` and pipe directly to `bash`, or download the script to a file and inspect it before running.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="50817-117">Dieses Skript wurde nur für Ubuntu 16.04 und höher und Debian 8 und höher geprüft.</span><span class="sxs-lookup"><span data-stu-id="50817-117">This script is only verified for Ubuntu 16.04+ and Debian 8+.</span></span> <span data-ttu-id="50817-118">Bei anderen Verteilungen funktioniert es möglicherweise nicht.</span><span class="sxs-lookup"><span data-stu-id="50817-118">It may not work on other distributions.</span></span>
> <span data-ttu-id="50817-119">Wenn Sie eine abgeleitete Verteilung wie Linux Mint verwenden, folgen Sie den Anweisungen für die manuelle Installation, und führen Sie ggf. eine Problembehandlung durch.</span><span class="sxs-lookup"><span data-stu-id="50817-119">If you're using a derived distribution such as Linux Mint, follow the manual install instructions and perform any necessary troubleshooting.</span></span>

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

### <a name="manual-install-instructions"></a><span data-ttu-id="50817-120">Anweisungen für die manuelle Installation</span><span class="sxs-lookup"><span data-stu-id="50817-120">Manual install instructions</span></span>

<span data-ttu-id="50817-121">Falls Sie ein Skript nicht als Superuser ausführen möchten, oder falls das All-in-One-Skript fehlschlägt, führen Sie die folgenden Schritte zum Installieren der Azure CLI aus.</span><span class="sxs-lookup"><span data-stu-id="50817-121">If you don't want to run a script as superuser or the all-in-one script fails, follow these steps to install the Azure CLI.</span></span>

1. <span data-ttu-id="50817-122">Rufen Sie die für die Installation erforderlichen Pakete ab:</span><span class="sxs-lookup"><span data-stu-id="50817-122">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install ca-certificates curl apt-transport-https lsb-release gnupg
    ```

2. <span data-ttu-id="50817-123">Laden Sie den Microsoft-Signaturschlüssel herunter, und installieren Sie ihn.</span><span class="sxs-lookup"><span data-stu-id="50817-123">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc |
        gpg --dearmor |
        sudo tee /etc/apt/trusted.gpg.d/microsoft.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="50817-124">Fügen Sie das Azure CLI-Softwarerepository hinzu:</span><span class="sxs-lookup"><span data-stu-id="50817-124">Add the Azure CLI software repository:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" |
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="50817-125">Aktualisieren Sie die Repositoryinformationen, und installieren Sie das Paket `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="50817-125">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

<span data-ttu-id="50817-126">Führen Sie die Azure CLI mit dem Befehl `az` aus.</span><span class="sxs-lookup"><span data-stu-id="50817-126">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="50817-127">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="50817-127">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="50817-128">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="50817-128">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="50817-129">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="50817-129">Troubleshooting</span></span>

<span data-ttu-id="50817-130">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="50817-130">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="50817-131">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="50817-131">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="no-module-issue-on-ubuntu-2004-focalwsl"></a><span data-ttu-id="50817-132">Problem vom Typ „Kein Modul“ unter Ubuntu 20.04 (Focal)/WSL</span><span class="sxs-lookup"><span data-stu-id="50817-132">No module issue on Ubuntu 20.04 (Focal)/WSL</span></span>
<span data-ttu-id="50817-133">Wenn Sie `azure-cli` unter `Focal` installiert haben, ohne das Azure CLI-Softwarerepository in [Schritt 3](#set-release) der Anweisungen für die manuelle Installation hinzuzufügen oder unser [Skript](#install-with-one-command) zu verwenden, treten unter Umständen Probleme auf, etwa das Problem „Kein Modul mit dem Namen 'decorator' or 'antlr4'“. Das ist darauf zurückzuführen, dass es sich beim installierten Paket um das veraltete Paket `azure-cli 2.0.81` aus dem Repository `focal/universe` handelt.</span><span class="sxs-lookup"><span data-stu-id="50817-133">If you installed `azure-cli` on `Focal` without adding the Azure CLI software repository in [step 3](#set-release) of the manual install instructions or using our [script](#install-with-one-command), you may encounter issues such as no module named 'decorator' or 'antlr4' as the package you installed is the outdated `azure-cli 2.0.81` from the `focal/universe` repository.</span></span> <span data-ttu-id="50817-134">Entfernen Sie das Paket zuerst, indem Sie `sudo apt remove azure-cli -y && sudo apt autoremove -y` ausführen. Befolgen Sie anschließend die obigen [Anweisungen](#install) zum Installieren des aktuellen `azure-cli`-Pakets.</span><span class="sxs-lookup"><span data-stu-id="50817-134">Please remove it first by running `sudo apt remove azure-cli -y && sudo apt autoremove -y`, then follow the above [instructions](#install) to install the latest `azure-cli` package.</span></span>

### <a name="lsb_release-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="50817-135">„lsb_release“ gibt nicht die richtige Basisdistributionsversion zurück.</span><span class="sxs-lookup"><span data-stu-id="50817-135">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="50817-136">Einige von Ubuntu oder Debian abgeleiteten Distributionen wie Linux Mint geben über `lsb_release` unter Umständen nicht den richtigen Versionsnamen zurück.</span><span class="sxs-lookup"><span data-stu-id="50817-136">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="50817-137">Mit diesem Wert wird im Installationsprozess das zu installierende Pakete ermittelt.</span><span class="sxs-lookup"><span data-stu-id="50817-137">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="50817-138">Wenn Sie den Codenamen der Ubuntu- oder Debian-Version kennen, von der Ihre Distribution abgeleitet ist, können Sie beim [Hinzufügen des Repositorys](#set-release) den Wert `AZ_REPO` manuell festlegen.</span><span class="sxs-lookup"><span data-stu-id="50817-138">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="50817-139">Sehen Sie sich andernfalls Informationen dazu an, wie Sie für Ihre Distribution den Basisdistributions-Codenamen ermitteln, und legen Sie `AZ_REPO` auf den richtigen Wert fest.</span><span class="sxs-lookup"><span data-stu-id="50817-139">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="50817-140">Kein Paket für Ihre Distribution</span><span class="sxs-lookup"><span data-stu-id="50817-140">No package for your distribution</span></span>

<span data-ttu-id="50817-141">Manchmal dauert es nach der Veröffentlichung einer Distribution etwas, bis ein Azure CLI-Paket dafür zur Verfügung gestellt wird.</span><span class="sxs-lookup"><span data-stu-id="50817-141">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="50817-142">Die Azure CLI ist im Hinblick auf zukünftige Abhängigkeitsversionen resilient konzipiert und nutzt daher möglichst wenige dieser Abhängigkeiten.</span><span class="sxs-lookup"><span data-stu-id="50817-142">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="50817-143">Ist für Ihre Basisdistribution kein Paket verfügbar, verwenden Sie ein Paket für eine ältere Distribution.</span><span class="sxs-lookup"><span data-stu-id="50817-143">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="50817-144">Legen Sie dazu beim [Hinzufügen des Repositorys](#set-release) den Wert `AZ_REPO` manuell fest.</span><span class="sxs-lookup"><span data-stu-id="50817-144">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="50817-145">Verwenden Sie für Ubuntu-Distributionen das Repository `bionic` und für Debian-Distributionen `stretch`.</span><span class="sxs-lookup"><span data-stu-id="50817-145">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="50817-146">Distributionen, die vor Ubuntu Trusty und Debian Wheezy veröffentlicht wurden, werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50817-146">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="elementary-os-eos-fails-to-install-the-azure-cli"></a><span data-ttu-id="50817-147">Installation der Azure-Befehlszeilenschnittstelle durch EOS (Elementary OS) nicht möglich</span><span class="sxs-lookup"><span data-stu-id="50817-147">Elementary OS (EOS) fails to install the Azure CLI</span></span>

<span data-ttu-id="50817-148">Die Azure-Befehlszeilenschnittstelle kann von EOS nicht installiert werden, da `lsb_release` den Wert `HERA` (Name des EOS-Release) zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="50817-148">EOS fails to install the Azure cli because `lsb_release` returns `HERA`, which is the EOS release name.</span></span>  <span data-ttu-id="50817-149">Zur Lösung des Problems muss die Datei `/etc/apt/sources.list.d/azure-cli.list` korrigiert und `hera main` in `bionic main` geändert werden.</span><span class="sxs-lookup"><span data-stu-id="50817-149">The solution is to fix the file `/etc/apt/sources.list.d/azure-cli.list` and change `hera main` to `bionic main`.</span></span>

<span data-ttu-id="50817-150">Ursprünglicher Dateiinhalt:</span><span class="sxs-lookup"><span data-stu-id="50817-150">Original file contents:</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ hera main
```

<span data-ttu-id="50817-151">Geänderter Dateiinhalt:</span><span class="sxs-lookup"><span data-stu-id="50817-151">Modified file contents</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ bionic main
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="50817-152">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="50817-152">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="50817-153">Konfigurieren Sie `apt` explizit so, dass dieser Proxy immer verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="50817-153">You may also want to explicitly configure `apt` to use this proxy at all times.</span></span> <span data-ttu-id="50817-154">Stellen Sie sicher, dass die folgenden Zeilen in einer `apt`-Konfigurationsdatei in `/etc/apt/apt.conf.d/` erscheinen.</span><span class="sxs-lookup"><span data-stu-id="50817-154">Make sure that the following lines appear in an `apt` configuration file in `/etc/apt/apt.conf.d/`.</span></span> <span data-ttu-id="50817-155">Wir empfehlen, dass Sie Ihre vorhandene globale Konfigurationsdatei, eine vorhandene Proxykonfigurationsdatei, `40proxies` oder `99local` verwenden. Berücksichtigen Sie dabei jedoch die Verwaltungsanforderungen Ihres Systems.</span><span class="sxs-lookup"><span data-stu-id="50817-155">We recommend using either your existing global configuration file, an existing proxy configuration file, `40proxies`, or `99local`, but follow your system administration requirements.</span></span>

```apt.conf
Acquire {
    http::proxy "http://[username]:[password]@[proxy]:[port]";
    https::proxy "https://[username]:[password]@[proxy]:[port]";
}
```

<span data-ttu-id="50817-156">Wenn Ihr Proxy keine Standardauthentifizierung verwendet, __entfernen__ Sie den Teil `[username]:[password]@` des Proxy-URI.</span><span class="sxs-lookup"><span data-stu-id="50817-156">If your proxy does not use basic auth, __remove__ the `[username]:[password]@` portion of the proxy URI.</span></span> <span data-ttu-id="50817-157">Weitere Informationen zur Proxykonfiguration finden Sie in der offiziellen Ubuntu-Dokumentation:</span><span class="sxs-lookup"><span data-stu-id="50817-157">If you require more information for proxy configuration, see the official Ubuntu documentation:</span></span>

* [<span data-ttu-id="50817-158">apt.conf manpage</span><span class="sxs-lookup"><span data-stu-id="50817-158">apt.conf manpage</span></span>](http://manpages.ubuntu.com/manpages/bionic/en/man5/apt.conf.5.html)
* [<span data-ttu-id="50817-159">Ubuntu Wiki – apt-get howto</span><span class="sxs-lookup"><span data-stu-id="50817-159">Ubuntu wiki - apt-get howto</span></span>](https://help.ubuntu.com/community/AptGet/Howto#Setting_up_apt-get_to_use_a_http-proxy)

<span data-ttu-id="50817-160">Zum Abrufen des Microsoft-Signaturschlüssels und des Pakets von unserem Repository muss Ihr Proxy HTTPS-Verbindungen mit der folgenden Adresse zulassen:</span><span class="sxs-lookup"><span data-stu-id="50817-160">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="50817-161">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="50817-161">Update</span></span>
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="50817-162">Sie können auch `apt-get upgrade` zum Aktualisieren des CLI-Pakets verwenden.</span><span class="sxs-lookup"><span data-stu-id="50817-162">You can also use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="50817-163">Durch diesen Befehl werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="50817-163">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="50817-164">Wenn Sie nur ein Upgrade für die CLI durchführen möchten, verwenden Sie `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="50817-164">To upgrade the CLI only, use `apt-get install`.</span></span>
>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="50817-165">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="50817-165">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="50817-166">Deinstallieren Sie sie mit `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="50817-166">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="50817-167">Entfernen Sie die Azure CLI-Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren:</span><span class="sxs-lookup"><span data-stu-id="50817-167">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="50817-168">Wenn Sie keine anderen Pakete von Microsoft verwenden, entfernen Sie den Signaturschlüssel:</span><span class="sxs-lookup"><span data-stu-id="50817-168">If you use no other packages from Microsoft, remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.gpg
    ```

4. <span data-ttu-id="50817-169">Entfernen Sie alle nicht benötigten Pakete:</span><span class="sxs-lookup"><span data-stu-id="50817-169">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="50817-170">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="50817-170">Next Steps</span></span>

<span data-ttu-id="50817-171">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="50817-171">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="50817-172">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="50817-172">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

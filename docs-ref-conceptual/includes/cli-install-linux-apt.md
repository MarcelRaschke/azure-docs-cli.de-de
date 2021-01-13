---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/29/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: 31b6a6e1c4c987ea351ccebc5d5bf23313ed856f
ms.sourcegitcommit: 547d3db8a1469f11d33e738a82d96cb51de61bd6
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2021
ms.locfileid: "98147572"
---
## <a name="overview"></a><span data-ttu-id="81c72-101">Übersicht</span><span class="sxs-lookup"><span data-stu-id="81c72-101">Overview</span></span>

<span data-ttu-id="81c72-102">Der `apt`-Paket-Manager enthält ein x86_64-Paket für die Azure-Befehlszeilenschnittstelle (Azure CLI), die mit den folgenden Distributionen getestet wurde.</span><span class="sxs-lookup"><span data-stu-id="81c72-102">The `apt` package manager contains an x86_64 package for the Azure CLI that has been tested on the following distributions.</span></span>

| <span data-ttu-id="81c72-103">Distribution</span><span class="sxs-lookup"><span data-stu-id="81c72-103">Distribution</span></span> | <span data-ttu-id="81c72-104">Version</span><span class="sxs-lookup"><span data-stu-id="81c72-104">Version</span></span> |
|:-------------|:--------|
| <span data-ttu-id="81c72-105">Ubuntu</span><span class="sxs-lookup"><span data-stu-id="81c72-105">Ubuntu</span></span>       | <span data-ttu-id="81c72-106">14.04 LTS (Trusty Tahir), 16.04 LTS (Xenial Xerus), 18.04 LTS (Bionic Beaver), 20.04 LTS (Focal Fossa), 20.10 (Groovy Gorilla)</span><span class="sxs-lookup"><span data-stu-id="81c72-106">14.04 LTS (Trusty Tahir), 16.04 LTS (Xenial Xerus), 18.04 LTS (Bionic Beaver), 20.04 LTS (Focal Fossa), 20.10 (Groovy Gorilla)</span></span> |
| <span data-ttu-id="81c72-107">Debian</span><span class="sxs-lookup"><span data-stu-id="81c72-107">Debian</span></span>       | <span data-ttu-id="81c72-108">Debian 8 (Jessie), Debian 9 (Stretch), Debian 10 (Buster)</span><span class="sxs-lookup"><span data-stu-id="81c72-108">Debian 8 (Jessie), Debian 9 (Stretch), Debian 10 (Buster)</span></span> |

> [!WARNING]
> <span data-ttu-id="81c72-109">Ubuntu 20.04 (Focal Fossa) und 20.10 (Groovy Gorilla) enthalten ein `azure-cli`-Paket mit der Version `2.0.81`, das im `universe`-Repository verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="81c72-109">Ubuntu 20.04 (Focal Fossa) and 20.10 (Groovy Gorilla) include an `azure-cli` package with version `2.0.81` provided by the `universe` repository.</span></span> <span data-ttu-id="81c72-110">Dieses Paket ist veraltet und wird nicht empfohlen.</span><span class="sxs-lookup"><span data-stu-id="81c72-110">This package is outdated and not recommended.</span></span> <span data-ttu-id="81c72-111">Falls dieses Paket installiert ist, entfernen Sie es mit dem Befehl `sudo apt remove azure-cli -y && sudo apt autoremove -y`, bevor Sie fortfahren.</span><span class="sxs-lookup"><span data-stu-id="81c72-111">If this package is installed, remove the package before continuing by running the command `sudo apt remove azure-cli -y && sudo apt autoremove -y`.</span></span>

## <a name="installation-options"></a><span data-ttu-id="81c72-112">Installationsoptionen</span><span class="sxs-lookup"><span data-stu-id="81c72-112">Installation Options</span></span>

<span data-ttu-id="81c72-113">Zum Installieren der Azure CLI auf Ihrem System stehen zwei Optionen zur Auswahl.</span><span class="sxs-lookup"><span data-stu-id="81c72-113">There are two options to install the Azure CLI on your system.</span></span>  <span data-ttu-id="81c72-114">Sie können einen einzelnen Befehl ausführen, der ein Installationsskript herunterlädt und die Installationsbefehle für Sie ausführt.</span><span class="sxs-lookup"><span data-stu-id="81c72-114">First, you may execute a single command that will download an install script and run the install commands for you.</span></span>  <span data-ttu-id="81c72-115">Alternativ können Sie die Installationsbefehle selbst Schritt für Schritt ausführen.</span><span class="sxs-lookup"><span data-stu-id="81c72-115">Or if you prefer, you can execute the install commands yourself in a step-by-step process.</span></span>  <span data-ttu-id="81c72-116">Beide Methoden werden im Folgenden beschrieben.</span><span class="sxs-lookup"><span data-stu-id="81c72-116">Both methods are provided below.</span></span>

## <a name="option-1-install-with-one-command"></a><span data-ttu-id="81c72-117">Option 1: Installieren mit einem Befehl</span><span class="sxs-lookup"><span data-stu-id="81c72-117">Option 1: Install with one command</span></span>

<span data-ttu-id="81c72-118">Das Azure CLI-Team pflegt ein Skript, mit dem alle Installationsbefehle in einem Schritt ausgeführt werden können.</span><span class="sxs-lookup"><span data-stu-id="81c72-118">The Azure CLI team maintains a script to run all installation commands in one step.</span></span>  <span data-ttu-id="81c72-119">Dieses Skript wird über `curl` heruntergeladen und direkt an `bash` weitergeleitet, um die CLI zu installieren.</span><span class="sxs-lookup"><span data-stu-id="81c72-119">This script is downloaded via `curl` and piped directly to `bash` to install the CLI.</span></span>

<span data-ttu-id="81c72-120">Wenn Sie den Inhalt des Skripts vor der Ausführung überprüfen möchten, laden Sie es einfach mit `curl` herunter, und überprüfen Sie es in Ihrem bevorzugten Text-Editor.</span><span class="sxs-lookup"><span data-stu-id="81c72-120">If you wish to inspect the contents of the script yourself before executing, simply download the script first using `curl` and inspect it in your favorite text editor.</span></span>

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

## <a name="option-2-step-by-step-installation-instructions"></a><span data-ttu-id="81c72-121">Option 2: Schrittweise Installation</span><span class="sxs-lookup"><span data-stu-id="81c72-121">Option 2: Step-by-step installation instructions</span></span>

<span data-ttu-id="81c72-122">Wenn Sie die Installation der Azure CLI lieber Schritt für Schritt durchführen möchten, befolgen Sie die folgenden Schritte.</span><span class="sxs-lookup"><span data-stu-id="81c72-122">If you prefer a step-by-step installation process, complete the following steps to install the Azure CLI.</span></span>

1. <span data-ttu-id="81c72-123">Rufen Sie die für die Installation erforderlichen Pakete ab:</span><span class="sxs-lookup"><span data-stu-id="81c72-123">Get packages needed for the install process:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install ca-certificates curl apt-transport-https lsb-release gnupg
    ```

2. <span data-ttu-id="81c72-124">Laden Sie den Microsoft-Signaturschlüssel herunter, und installieren Sie ihn.</span><span class="sxs-lookup"><span data-stu-id="81c72-124">Download and install the Microsoft signing key:</span></span>

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc |
        gpg --dearmor |
        sudo tee /etc/apt/trusted.gpg.d/microsoft.gpg > /dev/null
    ```

3. <div id="set-release"/><span data-ttu-id="81c72-125">Fügen Sie das Azure CLI-Softwarerepository hinzu (überspringen Sie diesen Schritt bei ARM64-Linux-Distributionen):</span><span class="sxs-lookup"><span data-stu-id="81c72-125">Add the Azure CLI software repository (skip this step on ARM64 Linux distributions):</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" |
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. <span data-ttu-id="81c72-126">Aktualisieren Sie die Repositoryinformationen, und installieren Sie das Paket `azure-cli`:</span><span class="sxs-lookup"><span data-stu-id="81c72-126">Update repository information and install the `azure-cli` package:</span></span>

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

## <a name="sign-in-to-azure-with-the-azure-cli"></a><span data-ttu-id="81c72-127">Anmelden bei Azure mit der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="81c72-127">Sign in to Azure with the Azure CLI</span></span>

<span data-ttu-id="81c72-128">Führen Sie die Azure CLI mit dem Befehl `az` aus.</span><span class="sxs-lookup"><span data-stu-id="81c72-128">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="81c72-129">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="81c72-129">To sign in, use the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="81c72-130">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="81c72-130">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="81c72-131">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="81c72-131">Troubleshooting</span></span>

<span data-ttu-id="81c72-132">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="81c72-132">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="81c72-133">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="81c72-133">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="no-module-issue-on-ubuntu-2004-focalwsl"></a><span data-ttu-id="81c72-134">Problem vom Typ „Kein Modul“ unter Ubuntu 20.04 (Focal)/WSL</span><span class="sxs-lookup"><span data-stu-id="81c72-134">No module issue on Ubuntu 20.04 (Focal)/WSL</span></span>

<span data-ttu-id="81c72-135">Wenn Sie `azure-cli` unter `Focal` installiert haben, ohne das Azure CLI-Softwarerepository in [Schritt 3](#set-release) der Anweisungen für die manuelle Installation hinzuzufügen oder unser [Skript](#option-1-install-with-one-command) zu verwenden, treten unter Umständen Probleme auf, etwa das Problem „Kein Modul mit dem Namen 'decorator' or 'antlr4'“. Das ist darauf zurückzuführen, dass es sich beim installierten Paket um das veraltete Paket `azure-cli 2.0.81` aus dem Repository `focal/universe` handelt.</span><span class="sxs-lookup"><span data-stu-id="81c72-135">If you installed `azure-cli` on `Focal` without adding the Azure CLI software repository in [step 3](#set-release) of the manual install instructions or using our [script](#option-1-install-with-one-command), you may encounter issues such as no module named 'decorator' or 'antlr4' as the package you installed is the outdated `azure-cli 2.0.81` from the `focal/universe` repository.</span></span> <span data-ttu-id="81c72-136">Entfernen Sie das Paket zuerst, indem Sie `sudo apt remove azure-cli -y && sudo apt autoremove -y` ausführen. Befolgen Sie anschließend die obigen [Anweisungen](#install) zum Installieren des aktuellen `azure-cli`-Pakets.</span><span class="sxs-lookup"><span data-stu-id="81c72-136">Please remove it first by running `sudo apt remove azure-cli -y && sudo apt autoremove -y`, then follow the above [instructions](#install) to install the latest `azure-cli` package.</span></span>

### <a name="lsb_release-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="81c72-137">„lsb_release“ gibt nicht die richtige Basisdistributionsversion zurück.</span><span class="sxs-lookup"><span data-stu-id="81c72-137">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="81c72-138">Einige von Ubuntu oder Debian abgeleiteten Distributionen wie Linux Mint geben über `lsb_release` unter Umständen nicht den richtigen Versionsnamen zurück.</span><span class="sxs-lookup"><span data-stu-id="81c72-138">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="81c72-139">Mit diesem Wert wird im Installationsprozess das zu installierende Pakete ermittelt.</span><span class="sxs-lookup"><span data-stu-id="81c72-139">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="81c72-140">Wenn Sie den Codenamen der Ubuntu- oder Debian-Version kennen, von der Ihre Distribution abgeleitet ist, können Sie beim [Hinzufügen des Repositorys](#set-release) den Wert `AZ_REPO` manuell festlegen.</span><span class="sxs-lookup"><span data-stu-id="81c72-140">If you know the code name of the Ubuntu or Debian version your distribution is derived from, you can set the `AZ_REPO` value manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="81c72-141">Sehen Sie sich andernfalls Informationen dazu an, wie Sie für Ihre Distribution den Basisdistributions-Codenamen ermitteln, und legen Sie `AZ_REPO` auf den richtigen Wert fest.</span><span class="sxs-lookup"><span data-stu-id="81c72-141">Otherwise, look up information for your distribution on how to determine the base distribution code name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="81c72-142">Kein Paket für Ihre Distribution</span><span class="sxs-lookup"><span data-stu-id="81c72-142">No package for your distribution</span></span>

<span data-ttu-id="81c72-143">Manchmal dauert es nach der Veröffentlichung einer Distribution etwas, bis ein Azure CLI-Paket dafür zur Verfügung gestellt wird.</span><span class="sxs-lookup"><span data-stu-id="81c72-143">Sometimes it may be a while after a distribution is released before there's an Azure CLI package available for it.</span></span> <span data-ttu-id="81c72-144">Die Azure CLI ist im Hinblick auf zukünftige Abhängigkeitsversionen resilient konzipiert und nutzt daher möglichst wenige dieser Abhängigkeiten.</span><span class="sxs-lookup"><span data-stu-id="81c72-144">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="81c72-145">Ist für Ihre Basisdistribution kein Paket verfügbar, verwenden Sie ein Paket für eine ältere Distribution.</span><span class="sxs-lookup"><span data-stu-id="81c72-145">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="81c72-146">Legen Sie dazu beim [Hinzufügen des Repositorys](#set-release) den Wert `AZ_REPO` manuell fest.</span><span class="sxs-lookup"><span data-stu-id="81c72-146">To do this, set the value of `AZ_REPO` manually when [adding the repository](#set-release).</span></span> <span data-ttu-id="81c72-147">Verwenden Sie für Ubuntu-Distributionen das Repository `bionic` und für Debian-Distributionen `stretch`.</span><span class="sxs-lookup"><span data-stu-id="81c72-147">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="81c72-148">Distributionen, die vor Ubuntu Trusty und Debian Wheezy veröffentlicht wurden, werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="81c72-148">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="elementary-os-eos-fails-to-install-the-azure-cli"></a><span data-ttu-id="81c72-149">Installation der Azure-Befehlszeilenschnittstelle durch EOS (Elementary OS) nicht möglich</span><span class="sxs-lookup"><span data-stu-id="81c72-149">Elementary OS (EOS) fails to install the Azure CLI</span></span>

<span data-ttu-id="81c72-150">Die Azure-Befehlszeilenschnittstelle kann von EOS nicht installiert werden, da `lsb_release` den Wert `HERA` (Name des EOS-Release) zurückgibt.</span><span class="sxs-lookup"><span data-stu-id="81c72-150">EOS fails to install the Azure cli because `lsb_release` returns `HERA`, which is the EOS release name.</span></span>  <span data-ttu-id="81c72-151">Zur Lösung des Problems muss die Datei `/etc/apt/sources.list.d/azure-cli.list` korrigiert und `hera main` in `bionic main` geändert werden.</span><span class="sxs-lookup"><span data-stu-id="81c72-151">The solution is to fix the file `/etc/apt/sources.list.d/azure-cli.list` and change `hera main` to `bionic main`.</span></span>

<span data-ttu-id="81c72-152">Ursprünglicher Dateiinhalt:</span><span class="sxs-lookup"><span data-stu-id="81c72-152">Original file contents:</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ hera main
```

<span data-ttu-id="81c72-153">Geänderter Dateiinhalt:</span><span class="sxs-lookup"><span data-stu-id="81c72-153">Modified file contents</span></span>

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ bionic main
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="81c72-154">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="81c72-154">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="81c72-155">Konfigurieren Sie `apt` explizit so, dass dieser Proxy immer verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="81c72-155">You may also want to explicitly configure `apt` to use this proxy at all times.</span></span> <span data-ttu-id="81c72-156">Stellen Sie sicher, dass die folgenden Zeilen in einer `apt`-Konfigurationsdatei in `/etc/apt/apt.conf.d/` erscheinen.</span><span class="sxs-lookup"><span data-stu-id="81c72-156">Make sure that the following lines appear in an `apt` configuration file in `/etc/apt/apt.conf.d/`.</span></span> <span data-ttu-id="81c72-157">Wir empfehlen, dass Sie Ihre vorhandene globale Konfigurationsdatei, eine vorhandene Proxykonfigurationsdatei, `40proxies` oder `99local` verwenden. Berücksichtigen Sie dabei jedoch die Verwaltungsanforderungen Ihres Systems.</span><span class="sxs-lookup"><span data-stu-id="81c72-157">We recommend using either your existing global configuration file, an existing proxy configuration file, `40proxies`, or `99local`, but follow your system administration requirements.</span></span>

```apt.conf
Acquire {
    http::proxy "http://[username]:[password]@[proxy]:[port]";
    https::proxy "https://[username]:[password]@[proxy]:[port]";
}
```

<span data-ttu-id="81c72-158">Wenn Ihr Proxy keine Standardauthentifizierung verwendet, __entfernen__ Sie den Teil `[username]:[password]@` des Proxy-URI.</span><span class="sxs-lookup"><span data-stu-id="81c72-158">If your proxy does not use basic auth, __remove__ the `[username]:[password]@` portion of the proxy URI.</span></span> <span data-ttu-id="81c72-159">Weitere Informationen zur Proxykonfiguration finden Sie in der offiziellen Ubuntu-Dokumentation:</span><span class="sxs-lookup"><span data-stu-id="81c72-159">If you require more information for proxy configuration, see the official Ubuntu documentation:</span></span>

* [<span data-ttu-id="81c72-160">apt.conf manpage</span><span class="sxs-lookup"><span data-stu-id="81c72-160">apt.conf manpage</span></span>](http://manpages.ubuntu.com/manpages/bionic/en/man5/apt.conf.5.html)
* [<span data-ttu-id="81c72-161">Ubuntu Wiki – apt-get howto</span><span class="sxs-lookup"><span data-stu-id="81c72-161">Ubuntu wiki - apt-get howto</span></span>](https://help.ubuntu.com/community/AptGet/Howto#Setting_up_apt-get_to_use_a_http-proxy)

<span data-ttu-id="81c72-162">Zum Abrufen des Microsoft-Signaturschlüssels und des Pakets von unserem Repository muss Ihr Proxy HTTPS-Verbindungen mit der folgenden Adresse zulassen:</span><span class="sxs-lookup"><span data-stu-id="81c72-162">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="81c72-163">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="81c72-163">Update</span></span>
[!INCLUDE [az-upgrade](az-upgrade.md)]

<span data-ttu-id="81c72-164">Sie können auch `apt-get upgrade` zum Aktualisieren des CLI-Pakets verwenden.</span><span class="sxs-lookup"><span data-stu-id="81c72-164">You can also use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="81c72-165">Durch diesen Befehl werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="81c72-165">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="81c72-166">Wenn Sie nur ein Upgrade für die CLI durchführen möchten, verwenden Sie `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="81c72-166">To upgrade the CLI only, use `apt-get install`.</span></span>
>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="81c72-167">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="81c72-167">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. <span data-ttu-id="81c72-168">Deinstallieren Sie sie mit `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="81c72-168">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="81c72-169">Entfernen Sie die Azure CLI-Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren:</span><span class="sxs-lookup"><span data-stu-id="81c72-169">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="81c72-170">Wenn Sie keine anderen Pakete von Microsoft verwenden, entfernen Sie den Signaturschlüssel:</span><span class="sxs-lookup"><span data-stu-id="81c72-170">If you use no other packages from Microsoft, remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.gpg
    ```

4. <span data-ttu-id="81c72-171">Entfernen Sie alle nicht benötigten Pakete:</span><span class="sxs-lookup"><span data-stu-id="81c72-171">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

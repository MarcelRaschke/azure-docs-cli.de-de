---
title: Installieren der Azure CLI unter Linux mit apt
description: Installieren der Azure CLI mit dem apt-Paket-Manager
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/27/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 45e1e7468e5817d0138c9b87da83c5a5228e4965
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/19/2019
ms.locfileid: "56421931"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="7ea13-103">Installieren der Azure CLI mit apt</span><span class="sxs-lookup"><span data-stu-id="7ea13-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="7ea13-104">Wenn Sie eine Distribution mit `apt` verwenden (etwa Ubuntu oder Debian), steht ein 64-Bit-Paket für die Azure CLI zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="7ea13-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="7ea13-105">Dieses Paket wurde mit Folgendem getestet:</span><span class="sxs-lookup"><span data-stu-id="7ea13-105">This package has been tested with:</span></span>

* <span data-ttu-id="7ea13-106">Ubuntu Trusty, Xenial, Artful und Bionic</span><span class="sxs-lookup"><span data-stu-id="7ea13-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="7ea13-107">Debian Wheezy, Jessie und Stretch</span><span class="sxs-lookup"><span data-stu-id="7ea13-107">Debian wheezy, jessie, and stretch</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> <span data-ttu-id="7ea13-108">Das `.deb`-Paket für Azure CLI installiert einen eigenen Python-Interpreter und verwendet nicht die Python-Version des Systems. Daher ist eine lokale Python-Version nicht explizit erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7ea13-108">The `.deb` package for Azure CLI installs its own Python interpreter, and does not use the system Python, so there is no explicit requirement for a local Python version.</span></span>

## <a name="install"></a><span data-ttu-id="7ea13-109">Installieren</span><span class="sxs-lookup"><span data-stu-id="7ea13-109">Install</span></span>

1. <span data-ttu-id="7ea13-110">Installieren Sie die Pakete mit den erforderlichen Komponenten:</span><span class="sxs-lookup"><span data-stu-id="7ea13-110">Install prerequisite packages:</span></span>

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common dirmngr -y
    ```

2. <div id="set-release"/><span data-ttu-id="7ea13-111">Ändern Sie die Quellenliste:</span><span class="sxs-lookup"><span data-stu-id="7ea13-111">Modify your sources list:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

3. <div id="signingKey"/><span data-ttu-id="7ea13-112">Rufen Sie den Microsoft-Signaturschlüssel ab:</span><span class="sxs-lookup"><span data-stu-id="7ea13-112">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

4. <span data-ttu-id="7ea13-113">Installieren Sie die Befehlszeilenschnittstelle:</span><span class="sxs-lookup"><span data-stu-id="7ea13-113">Install the CLI:</span></span>

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="7ea13-114">Der Signaturschlüssel wurde im Mai 2018 aktualisiert und ersetzt.</span><span class="sxs-lookup"><span data-stu-id="7ea13-114">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="7ea13-115">Sollten Fehler beim Signieren auftreten, vergewissern Sie sich, dass Sie den [aktuellen Signaturschlüssel](#signingKey) besitzen.</span><span class="sxs-lookup"><span data-stu-id="7ea13-115">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>

<span data-ttu-id="7ea13-116">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="7ea13-116">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="7ea13-117">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="7ea13-117">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="7ea13-118">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="7ea13-118">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="7ea13-119">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="7ea13-119">Troubleshooting</span></span>

<span data-ttu-id="7ea13-120">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="7ea13-120">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="7ea13-121">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="7ea13-121">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="7ea13-122">„lsb_release“ gibt nicht die richtige Basisdistributionsversion zurück.</span><span class="sxs-lookup"><span data-stu-id="7ea13-122">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="7ea13-123">Einige von Ubuntu oder Debian abgeleiteten Distributionen wie Linux Mint geben über `lsb_release` unter Umständen nicht den richtigen Versionsnamen zurück.</span><span class="sxs-lookup"><span data-stu-id="7ea13-123">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="7ea13-124">Mit diesem Wert wird im Installationsprozess das zu installierende Pakete ermittelt.</span><span class="sxs-lookup"><span data-stu-id="7ea13-124">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="7ea13-125">Wenn Sie den Namen der Version kennen, von der Ihre Distribution abgeleitet ist, können Sie im [Installationsschritt 2](#set-release) den Wert `AZ_REPO` manuell festlegen.</span><span class="sxs-lookup"><span data-stu-id="7ea13-125">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 2](#set-release).</span></span> <span data-ttu-id="7ea13-126">Sehen Sie sich andernfalls Informationen dazu an, wie Sie für Ihre Distribution den Basisdistributionsnamen ermitteln, und legen Sie `AZ_REPO` auf den richtigen Wert fest.</span><span class="sxs-lookup"><span data-stu-id="7ea13-126">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="7ea13-127">Kein Paket für Ihre Distribution</span><span class="sxs-lookup"><span data-stu-id="7ea13-127">No package for your distribution</span></span>

<span data-ttu-id="7ea13-128">Manchmal dauert es nach der Veröffentlichung einer Ubuntu-Distribution etwas, bis ein Azure CLI-Paket dafür zur Verfügung gestellt wird.</span><span class="sxs-lookup"><span data-stu-id="7ea13-128">Sometimes it may be a while after an Ubuntu distribution is released before there's an Azure CLI package made available for it.</span></span> <span data-ttu-id="7ea13-129">Die Azure CLI ist im Hinblick auf zukünftige Abhängigkeitsversionen resilient konzipiert und nutzt daher möglichst wenige dieser Abhängigkeiten.</span><span class="sxs-lookup"><span data-stu-id="7ea13-129">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="7ea13-130">Ist für Ihre Basisdistribution kein Paket verfügbar, verwenden Sie ein Paket für eine ältere Distribution.</span><span class="sxs-lookup"><span data-stu-id="7ea13-130">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="7ea13-131">Legen Sie dazu im [Installationsschritt 1](#install-step-1) den Wert für `AZ_REPO` manuell fest.</span><span class="sxs-lookup"><span data-stu-id="7ea13-131">To do this, set the value of `AZ_REPO` manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="7ea13-132">Verwenden Sie für Ubuntu-Distributionen das Repository `bionic` und für Debian-Distributionen `stretch`.</span><span class="sxs-lookup"><span data-stu-id="7ea13-132">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="7ea13-133">Distributionen, die vor Ubuntu Trusty und Debian Wheezy veröffentlicht wurden, werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7ea13-133">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="7ea13-134">Fehler „No dirmngr“ beim Ausführen von „apt-key“</span><span class="sxs-lookup"><span data-stu-id="7ea13-134">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="7ea13-135">Beim Ausführen des Befehls `apt-key` wird unter Umständen eine Ausgabe wie die folgende angezeigt:</span><span class="sxs-lookup"><span data-stu-id="7ea13-135">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="7ea13-136">Dieser Fehler ist auf eine fehlende Komponente zurückzuführen, die von `apt-key` benötigt wird.</span><span class="sxs-lookup"><span data-stu-id="7ea13-136">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="7ea13-137">Das Problem lässt sich durch Installieren des Pakets `dirmngr` beheben.</span><span class="sxs-lookup"><span data-stu-id="7ea13-137">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

<span data-ttu-id="7ea13-138">Wenn Sie mit einem Windows-Subsystem für Linux (WSL) arbeiten, wird dieser Fehler auch für ältere Windows-Versionen als Windows 10 1809 angezeigt.</span><span class="sxs-lookup"><span data-stu-id="7ea13-138">If you are on Windows Subsystem for Linux (WSL), this error also appears on versions of Windows prior to Windows 10 1809.</span></span> <span data-ttu-id="7ea13-139">Aktualisieren Sie Ihre Version von Windows, um das Problem zu beheben.</span><span class="sxs-lookup"><span data-stu-id="7ea13-139">To resolve the issue, update your version of Windows.</span></span>

### <a name="apt-key-hangs"></a><span data-ttu-id="7ea13-140">Keine Reaktion von „apt-key“</span><span class="sxs-lookup"><span data-stu-id="7ea13-140">apt-key hangs</span></span>

<span data-ttu-id="7ea13-141">Wenn hinter einer Firewall ausgehende Verbindungen mit Port 11371 blockiert werden, hängt der Befehl `apt-key` unter Umständen auf unbestimmte Zeit.</span><span class="sxs-lookup"><span data-stu-id="7ea13-141">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span>
<span data-ttu-id="7ea13-142">Für Ihre Firewall ist möglicherweise ein HTTP-Proxy für ausgehende Verbindungen erforderlich:</span><span class="sxs-lookup"><span data-stu-id="7ea13-142">Your firewall may require an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

<span data-ttu-id="7ea13-143">Um zu ermitteln, ob ein Proxy eingerichtet ist, wenden Sie sich an Ihren Systemadministrator.</span><span class="sxs-lookup"><span data-stu-id="7ea13-143">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="7ea13-144">Wenn für den Proxy keine Anmeldung erforderlich ist, lassen Sie Benutzer und Kennwort weg.</span><span class="sxs-lookup"><span data-stu-id="7ea13-144">If your proxy does not require a login, then leave out the user and password information.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="7ea13-145">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7ea13-145">Update</span></span>

<span data-ttu-id="7ea13-146">Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.</span><span class="sxs-lookup"><span data-stu-id="7ea13-146">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="7ea13-147">Der Signaturschlüssel wurde im Mai 2018 aktualisiert und ersetzt.</span><span class="sxs-lookup"><span data-stu-id="7ea13-147">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="7ea13-148">Sollten Fehler beim Signieren auftreten, vergewissern Sie sich, dass Sie den [aktuellen Signaturschlüssel](#signingKey) besitzen.</span><span class="sxs-lookup"><span data-stu-id="7ea13-148">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="7ea13-149">Durch diesen Befehl werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="7ea13-149">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="7ea13-150">Wenn Sie nur ein Upgrade für die CLI durchführen möchten, verwenden Sie `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="7ea13-150">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="7ea13-151">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="7ea13-151">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="7ea13-152">Deinstallieren Sie sie mit `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="7ea13-152">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="7ea13-153">Entfernen Sie die Azure CLI-Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren:</span><span class="sxs-lookup"><span data-stu-id="7ea13-153">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="7ea13-154">Entfernen Sie den Signaturschlüssel:</span><span class="sxs-lookup"><span data-stu-id="7ea13-154">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. <span data-ttu-id="7ea13-155">Entfernen Sie alle nicht benötigten Pakete:</span><span class="sxs-lookup"><span data-stu-id="7ea13-155">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="7ea13-156">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="7ea13-156">Next Steps</span></span>

<span data-ttu-id="7ea13-157">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="7ea13-157">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="7ea13-158">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="7ea13-158">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

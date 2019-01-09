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
ms.openlocfilehash: 1973c933cbffa494cbe9c0749346450251feefcb
ms.sourcegitcommit: 9bd90875a324908ec7195fc4c4f63ebf124760f9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/02/2019
ms.locfileid: "53982585"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="f4cb0-103">Installieren der Azure CLI mit apt</span><span class="sxs-lookup"><span data-stu-id="f4cb0-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="f4cb0-104">Wenn Sie eine Distribution mit `apt` verwenden (etwa Ubuntu oder Debian), steht ein 64-Bit-Paket für die Azure CLI zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="f4cb0-105">Dieses Paket wurde mit Folgendem getestet:</span><span class="sxs-lookup"><span data-stu-id="f4cb0-105">This package has been tested with:</span></span>

* <span data-ttu-id="f4cb0-106">Ubuntu Trusty, Xenial, Artful und Bionic</span><span class="sxs-lookup"><span data-stu-id="f4cb0-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="f4cb0-107">Debian Wheezy, Jessie und Stretch</span><span class="sxs-lookup"><span data-stu-id="f4cb0-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="f4cb0-108">Installieren</span><span class="sxs-lookup"><span data-stu-id="f4cb0-108">Install</span></span>

1. <span data-ttu-id="f4cb0-109">Installieren Sie die Pakete mit den erforderlichen Komponenten:</span><span class="sxs-lookup"><span data-stu-id="f4cb0-109">Install prerequisite packages:</span></span>

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common dirmngr -y
    ```

2. <div id="set-release"/><span data-ttu-id="f4cb0-110">Ändern Sie die Quellenliste:</span><span class="sxs-lookup"><span data-stu-id="f4cb0-110">Modify your sources list:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

3. <div id="signingKey"/><span data-ttu-id="f4cb0-111">Rufen Sie den Microsoft-Signaturschlüssel ab:</span><span class="sxs-lookup"><span data-stu-id="f4cb0-111">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

4. <span data-ttu-id="f4cb0-112">Installieren Sie die Befehlszeilenschnittstelle:</span><span class="sxs-lookup"><span data-stu-id="f4cb0-112">Install the CLI:</span></span>

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="f4cb0-113">Der Signaturschlüssel wurde im Mai 2018 aktualisiert und ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-113">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="f4cb0-114">Sollten Fehler beim Signieren auftreten, vergewissern Sie sich, dass Sie den [aktuellen Signaturschlüssel](#signingKey) besitzen.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-114">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>

<span data-ttu-id="f4cb0-115">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-115">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="f4cb0-116">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-116">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="f4cb0-117">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f4cb0-117">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="f4cb0-118">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="f4cb0-118">Troubleshooting</span></span>

<span data-ttu-id="f4cb0-119">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-119">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="f4cb0-120">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="f4cb0-120">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="f4cb0-121">„lsb_release“ gibt nicht die richtige Basisdistributionsversion zurück.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-121">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="f4cb0-122">Einige von Ubuntu oder Debian abgeleiteten Distributionen wie Linux Mint geben über `lsb_release` unter Umständen nicht den richtigen Versionsnamen zurück.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-122">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="f4cb0-123">Mit diesem Wert wird im Installationsprozess das zu installierende Pakete ermittelt.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-123">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="f4cb0-124">Wenn Sie den Namen der Version kennen, von der Ihre Distribution abgeleitet ist, können Sie im [Installationsschritt 2](#set-release) den Wert `AZ_REPO` manuell festlegen.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-124">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 2](#set-release).</span></span> <span data-ttu-id="f4cb0-125">Sehen Sie sich andernfalls Informationen dazu an, wie Sie für Ihre Distribution den Basisdistributionsnamen ermitteln, und legen Sie `AZ_REPO` auf den richtigen Wert fest.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-125">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="f4cb0-126">Kein Paket für Ihre Distribution</span><span class="sxs-lookup"><span data-stu-id="f4cb0-126">No package for your distribution</span></span>

<span data-ttu-id="f4cb0-127">Manchmal dauert es nach der Veröffentlichung einer Ubuntu-Distribution etwas, bis ein Azure CLI-Paket dafür zur Verfügung gestellt wird.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-127">Sometimes it may be a while after an Ubuntu distribution is released before there's an Azure CLI package made available for it.</span></span> <span data-ttu-id="f4cb0-128">Die Azure CLI ist im Hinblick auf zukünftige Abhängigkeitsversionen resilient konzipiert und nutzt daher möglichst wenige dieser Abhängigkeiten.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-128">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="f4cb0-129">Ist für Ihre Basisdistribution kein Paket verfügbar, verwenden Sie ein Paket für eine ältere Distribution.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-129">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="f4cb0-130">Legen Sie dazu im [Installationsschritt 1](#install-step-1) den Wert für `AZ_REPO` manuell fest.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-130">To do this, set the value of `AZ_REPO` manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="f4cb0-131">Verwenden Sie für Ubuntu-Distributionen das Repository `bionic` und für Debian-Distributionen `stretch`.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-131">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="f4cb0-132">Distributionen, die vor Ubuntu Trusty und Debian Wheezy veröffentlicht wurden, werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-132">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="f4cb0-133">Fehler „No dirmngr“ beim Ausführen von „apt-key“</span><span class="sxs-lookup"><span data-stu-id="f4cb0-133">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="f4cb0-134">Beim Ausführen des Befehls `apt-key` wird unter Umständen eine Ausgabe wie die folgende angezeigt:</span><span class="sxs-lookup"><span data-stu-id="f4cb0-134">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="f4cb0-135">Dieser Fehler ist auf eine fehlende Komponente zurückzuführen, die von `apt-key` benötigt wird.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-135">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="f4cb0-136">Das Problem lässt sich durch Installieren des Pakets `dirmngr` beheben.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-136">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

<span data-ttu-id="f4cb0-137">Wenn Sie mit einem Windows-Subsystem für Linux (WSL) arbeiten, wird dieser Fehler auch für ältere Windows-Versionen als Windows 10 1809 angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-137">If you are on Windows Subsystem for Linux (WSL), this error also appears on versions of Windows prior to Windows 10 1809.</span></span> <span data-ttu-id="f4cb0-138">Aktualisieren Sie Ihre Version von Windows, um das Problem zu beheben.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-138">To resolve the issue, update your version of Windows.</span></span>

### <a name="apt-key-hangs"></a><span data-ttu-id="f4cb0-139">Keine Reaktion von „apt-key“</span><span class="sxs-lookup"><span data-stu-id="f4cb0-139">apt-key hangs</span></span>

<span data-ttu-id="f4cb0-140">Wenn hinter einer Firewall ausgehende Verbindungen mit Port 11371 blockiert werden, hängt der Befehl `apt-key` unter Umständen auf unbestimmte Zeit.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-140">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span>
<span data-ttu-id="f4cb0-141">Für Ihre Firewall ist möglicherweise ein HTTP-Proxy für ausgehende Verbindungen erforderlich:</span><span class="sxs-lookup"><span data-stu-id="f4cb0-141">Your firewall may require an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

<span data-ttu-id="f4cb0-142">Um zu ermitteln, ob ein Proxy eingerichtet ist, wenden Sie sich an Ihren Systemadministrator.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-142">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="f4cb0-143">Wenn für den Proxy keine Anmeldung erforderlich ist, lassen Sie Benutzer und Kennwort weg.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-143">If your proxy does not require a login, then leave out the user and password information.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="f4cb0-144">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f4cb0-144">Update</span></span>

<span data-ttu-id="f4cb0-145">Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-145">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="f4cb0-146">Der Signaturschlüssel wurde im Mai 2018 aktualisiert und ersetzt.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-146">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="f4cb0-147">Sollten Fehler beim Signieren auftreten, vergewissern Sie sich, dass Sie den [aktuellen Signaturschlüssel](#signingKey) besitzen.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-147">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="f4cb0-148">Durch diesen Befehl werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-148">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="f4cb0-149">Wenn Sie nur ein Upgrade für die CLI durchführen möchten, verwenden Sie `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-149">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="f4cb0-150">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="f4cb0-150">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="f4cb0-151">Deinstallieren Sie sie mit `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="f4cb0-151">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="f4cb0-152">Entfernen Sie die Azure CLI-Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren:</span><span class="sxs-lookup"><span data-stu-id="f4cb0-152">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="f4cb0-153">Entfernen Sie den Signaturschlüssel:</span><span class="sxs-lookup"><span data-stu-id="f4cb0-153">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. <span data-ttu-id="f4cb0-154">Entfernen Sie alle nicht benötigten Pakete:</span><span class="sxs-lookup"><span data-stu-id="f4cb0-154">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="f4cb0-155">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f4cb0-155">Next Steps</span></span>

<span data-ttu-id="f4cb0-156">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="f4cb0-156">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f4cb0-157">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="f4cb0-157">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

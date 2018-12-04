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
ms.devlang: azure-cli
ms.openlocfilehash: c33c3e75991979a72a7b82183dd88b87715907ae
ms.sourcegitcommit: a8aac038e6ede0b1b352ca6163a04b61ff4eed5b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/28/2018
ms.locfileid: "52450257"
---
# <a name="install-azure-cli-with-apt"></a><span data-ttu-id="75e32-103">Installieren der Azure CLI mit apt</span><span class="sxs-lookup"><span data-stu-id="75e32-103">Install Azure CLI with apt</span></span>

<span data-ttu-id="75e32-104">Wenn Sie eine Distribution mit `apt` verwenden (etwa Ubuntu oder Debian), steht ein 64-Bit-Paket für die Azure CLI zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="75e32-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there's a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="75e32-105">Dieses Paket wurde mit Folgendem getestet:</span><span class="sxs-lookup"><span data-stu-id="75e32-105">This package has been tested with:</span></span>

* <span data-ttu-id="75e32-106">Ubuntu Trusty, Xenial, Artful und Bionic</span><span class="sxs-lookup"><span data-stu-id="75e32-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="75e32-107">Debian Wheezy, Jessie und Stretch</span><span class="sxs-lookup"><span data-stu-id="75e32-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="75e32-108">Installieren</span><span class="sxs-lookup"><span data-stu-id="75e32-108">Install</span></span>

1. <div id="install-step-1"/><span data-ttu-id="75e32-109">Ändern Sie die Quellenliste:</span><span class="sxs-lookup"><span data-stu-id="75e32-109">Modify your sources list:</span></span>

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common -y
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <div id="signingKey"/><span data-ttu-id="75e32-110">Rufen Sie den Microsoft-Signaturschlüssel ab:</span><span class="sxs-lookup"><span data-stu-id="75e32-110">Get the Microsoft signing key:</span></span>

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

3. <span data-ttu-id="75e32-111">Installieren Sie die Befehlszeilenschnittstelle:</span><span class="sxs-lookup"><span data-stu-id="75e32-111">Install the CLI:</span></span>

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="75e32-112">Der Signaturschlüssel wurde im Mai 2018 aktualisiert und ersetzt.</span><span class="sxs-lookup"><span data-stu-id="75e32-112">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="75e32-113">Sollten Fehler beim Signieren auftreten, vergewissern Sie sich, dass Sie den [aktuellen Signaturschlüssel](#signingKey) besitzen.</span><span class="sxs-lookup"><span data-stu-id="75e32-113">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>

<span data-ttu-id="75e32-114">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="75e32-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="75e32-115">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="75e32-115">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="75e32-116">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="75e32-116">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="75e32-117">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="75e32-117">Troubleshooting</span></span>

<span data-ttu-id="75e32-118">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="75e32-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="75e32-119">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="75e32-119">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a><span data-ttu-id="75e32-120">„lsb_release“ gibt nicht die richtige Basisdistributionsversion zurück.</span><span class="sxs-lookup"><span data-stu-id="75e32-120">lsb_release does not return the correct base distribution version</span></span>

<span data-ttu-id="75e32-121">Einige von Ubuntu oder Debian abgeleiteten Distributionen wie Linux Mint geben über `lsb_release` unter Umständen nicht den richtigen Versionsnamen zurück.</span><span class="sxs-lookup"><span data-stu-id="75e32-121">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="75e32-122">Mit diesem Wert wird im Installationsprozess das zu installierende Pakete ermittelt.</span><span class="sxs-lookup"><span data-stu-id="75e32-122">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="75e32-123">Wenn Sie den Namen der Version kennen, von der Ihre Distribution abgeleitet ist, können Sie im [Installationsschritt 1](#install-step-1) den Wert `AZ_REPO` manuell festlegen.</span><span class="sxs-lookup"><span data-stu-id="75e32-123">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="75e32-124">Sehen Sie sich andernfalls Informationen dazu an, wie Sie für Ihre Distribution den Basisdistributionsnamen ermitteln, und legen Sie `AZ_REPO` auf den richtigen Wert fest.</span><span class="sxs-lookup"><span data-stu-id="75e32-124">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="no-package-for-your-distribution"></a><span data-ttu-id="75e32-125">Kein Paket für Ihre Distribution</span><span class="sxs-lookup"><span data-stu-id="75e32-125">No package for your distribution</span></span>

<span data-ttu-id="75e32-126">Manchmal dauert es nach der Veröffentlichung einer Ubuntu-Distribution etwas, bis ein Azure CLI-Paket dafür zur Verfügung gestellt wird.</span><span class="sxs-lookup"><span data-stu-id="75e32-126">Sometimes it may be a while after an Ubuntu distribution is released before there's an Azure CLI package made available for it.</span></span> <span data-ttu-id="75e32-127">Die Azure CLI ist im Hinblick auf zukünftige Abhängigkeitsversionen resilient konzipiert und nutzt daher möglichst wenige dieser Abhängigkeiten.</span><span class="sxs-lookup"><span data-stu-id="75e32-127">The Azure CLI designed to be resilient with regards to future versions of dependencies and rely on as few of them as possible.</span></span> <span data-ttu-id="75e32-128">Ist für Ihre Basisdistribution kein Paket verfügbar, verwenden Sie ein Paket für eine ältere Distribution.</span><span class="sxs-lookup"><span data-stu-id="75e32-128">If there's no package available for your base distribution, try a package for an earlier distribution.</span></span>

<span data-ttu-id="75e32-129">Legen Sie dazu im [Installationsschritt 1](#install-step-1) den Wert für `AZ_REPO` manuell fest.</span><span class="sxs-lookup"><span data-stu-id="75e32-129">To do this, set the value of `AZ_REPO` manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="75e32-130">Verwenden Sie für Ubuntu-Distributionen das Repository `bionic` und für Debian-Distributionen `stretch`.</span><span class="sxs-lookup"><span data-stu-id="75e32-130">For Ubuntu distributions use the `bionic` repository, and for Debian distributions use `stretch`.</span></span> <span data-ttu-id="75e32-131">Distributionen, die vor Ubuntu Trusty und Debian Wheezy veröffentlicht wurden, werden nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="75e32-131">Distributions released before Ubuntu Trusty and Debian Wheezy are not supported.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="75e32-132">Fehler „No dirmngr“ beim Ausführen von „apt-key“</span><span class="sxs-lookup"><span data-stu-id="75e32-132">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="75e32-133">Beim Ausführen des Befehls `apt-key` wird unter Umständen eine Ausgabe wie die folgende angezeigt:</span><span class="sxs-lookup"><span data-stu-id="75e32-133">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="75e32-134">Dieser Fehler ist auf eine fehlende Komponente zurückzuführen, die von `apt-key` benötigt wird.</span><span class="sxs-lookup"><span data-stu-id="75e32-134">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="75e32-135">Das Problem lässt sich durch Installieren des Pakets `dirmngr` beheben.</span><span class="sxs-lookup"><span data-stu-id="75e32-135">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="75e32-136">Keine Reaktion von „apt-key“</span><span class="sxs-lookup"><span data-stu-id="75e32-136">apt-key hangs</span></span>

<span data-ttu-id="75e32-137">Wenn hinter einer Firewall ausgehende Verbindungen mit Port 11371 blockiert werden, hängt der Befehl `apt-key` unter Umständen auf unbestimmte Zeit.</span><span class="sxs-lookup"><span data-stu-id="75e32-137">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span>
<span data-ttu-id="75e32-138">Für Ihre Firewall ist möglicherweise ein HTTP-Proxy für ausgehende Verbindungen erforderlich:</span><span class="sxs-lookup"><span data-stu-id="75e32-138">Your firewall may require an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

<span data-ttu-id="75e32-139">Um zu ermitteln, ob ein Proxy eingerichtet ist, wenden Sie sich an Ihren Systemadministrator.</span><span class="sxs-lookup"><span data-stu-id="75e32-139">To determine if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="75e32-140">Wenn für den Proxy keine Anmeldung erforderlich ist, lassen Sie Benutzer und Kennwort weg.</span><span class="sxs-lookup"><span data-stu-id="75e32-140">If your proxy does not require a login, then leave out the user and password information.</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="75e32-141">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="75e32-141">Update</span></span>

<span data-ttu-id="75e32-142">Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.</span><span class="sxs-lookup"><span data-stu-id="75e32-142">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="75e32-143">Der Signaturschlüssel wurde im Mai 2018 aktualisiert und ersetzt.</span><span class="sxs-lookup"><span data-stu-id="75e32-143">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="75e32-144">Sollten Fehler beim Signieren auftreten, vergewissern Sie sich, dass Sie den [aktuellen Signaturschlüssel](#signingKey) besitzen.</span><span class="sxs-lookup"><span data-stu-id="75e32-144">If you receive signing errors, make sure you have [the latest signing key](#signingKey).</span></span>
>
> [!NOTE]
> <span data-ttu-id="75e32-145">Durch diesen Befehl werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="75e32-145">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="75e32-146">Wenn Sie nur ein Upgrade für die CLI durchführen möchten, verwenden Sie `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="75e32-146">To upgrade the CLI only, use `apt-get install`.</span></span>
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="75e32-147">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="75e32-147">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="75e32-148">Deinstallieren Sie sie mit `apt-get remove`:</span><span class="sxs-lookup"><span data-stu-id="75e32-148">Uninstall with `apt-get remove`:</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="75e32-149">Entfernen Sie die Azure CLI-Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren:</span><span class="sxs-lookup"><span data-stu-id="75e32-149">If you don't plan to reinstall the CLI, remove the Azure CLI repository information:</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="75e32-150">Entfernen Sie den Signaturschlüssel:</span><span class="sxs-lookup"><span data-stu-id="75e32-150">Remove the signing key:</span></span>

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. <span data-ttu-id="75e32-151">Entfernen Sie alle nicht benötigten Pakete:</span><span class="sxs-lookup"><span data-stu-id="75e32-151">Remove any unneeded packages:</span></span>

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a><span data-ttu-id="75e32-152">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="75e32-152">Next Steps</span></span>

<span data-ttu-id="75e32-153">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="75e32-153">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="75e32-154">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="75e32-154">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

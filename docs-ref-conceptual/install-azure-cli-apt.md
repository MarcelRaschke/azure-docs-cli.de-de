---
title: Installieren der Azure CLI 2.0 unter Linux mit apt
description: Installieren der Azure CLI 2.0 mit dem apt-Paket-Manager
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/24/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 3f52f1545dc4bad44280c7e58ad17ec2302fd436
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439617"
---
# <a name="install-azure-cli-20-with-apt"></a><span data-ttu-id="210ea-103">Installieren der Azure CLI 2.0 mit apt</span><span class="sxs-lookup"><span data-stu-id="210ea-103">Install Azure CLI 2.0 with apt</span></span>

<span data-ttu-id="210ea-104">Wenn Sie eine Distribution mit `apt` verwenden (etwa Ubuntu oder Debian), steht ein 64-Bit-Paket für die Azure CLI zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="210ea-104">If you are running a distribution that comes with `apt`, such as Ubuntu or Debian, there is a 64-bit package available for the Azure CLI.</span></span> <span data-ttu-id="210ea-105">Dieses Paket wurde mit Folgendem getestet:</span><span class="sxs-lookup"><span data-stu-id="210ea-105">This package has been tested with:</span></span>

* <span data-ttu-id="210ea-106">Ubuntu Trusty, Xenial, Artful und Bionic</span><span class="sxs-lookup"><span data-stu-id="210ea-106">Ubuntu trusty, xenial, artful, and bionic</span></span>
* <span data-ttu-id="210ea-107">Debian Wheezy, Jessie und Stretch</span><span class="sxs-lookup"><span data-stu-id="210ea-107">Debian wheezy, jessie, and stretch</span></span>

## <a name="install"></a><span data-ttu-id="210ea-108">Installieren</span><span class="sxs-lookup"><span data-stu-id="210ea-108">Install</span></span>

1. <span data-ttu-id="210ea-109"><a name="install-step-1"/> Ändern Sie die Quellenliste:</span><span class="sxs-lookup"><span data-stu-id="210ea-109"><a name="install-step-1"/> Modify your sources list:</span></span>

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

2. <a name="signingKey"></a><span data-ttu-id="210ea-110">Rufen Sie den Microsoft-Signaturschlüssel ab:</span><span class="sxs-lookup"><span data-stu-id="210ea-110">Get the Microsoft signing key:</span></span>

   ```bash
   curl -L https://packages.microsoft.com/keys/microsoft.asc | sudo apt-key add -
   ```

3. <span data-ttu-id="210ea-111">Installieren Sie die Befehlszeilenschnittstelle:</span><span class="sxs-lookup"><span data-stu-id="210ea-111">Install the CLI:</span></span>

   ```bash
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > <span data-ttu-id="210ea-112">Der Signaturschlüssel wurde im Mai 2018 aktualisiert und ersetzt.</span><span class="sxs-lookup"><span data-stu-id="210ea-112">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="210ea-113">Falls Signaturschlüsselfehler auftreten, stellen Sie sicher, dass Sie den [aktuellen Signaturschlüssel](#signingKey) abgerufen haben.</span><span class="sxs-lookup"><span data-stu-id="210ea-113">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>

<span data-ttu-id="210ea-114">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="210ea-114">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="210ea-115">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="210ea-115">To log in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="210ea-116">Weitere Informationen zu verschiedenen Anmeldemethoden finden Sie unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="210ea-116">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="210ea-117">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="210ea-117">Troubleshooting</span></span>

<span data-ttu-id="210ea-118">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="210ea-118">Here are some common problems seen when installing with `apt`.</span></span> <span data-ttu-id="210ea-119">Sollte Ihr Problem hier nicht aufgeführt sein, [melden Sie es über GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="210ea-119">If your issue is not listed here, please [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="lsbrelease-fails-with-command-not-found"></a><span data-ttu-id="210ea-120">Bei „lsb_release“ tritt der Fehler „Der Befehl wurde nicht gefunden.“ auf.</span><span class="sxs-lookup"><span data-stu-id="210ea-120">lsb_release fails with "Command not found"</span></span>

<span data-ttu-id="210ea-121">Beim Ausführen des Befehls `lsb_release` wird unter Umständen eine Ausgabe wie die folgende angezeigt:</span><span class="sxs-lookup"><span data-stu-id="210ea-121">When running the `lsb_release` command, you may see output similar to the following error:</span></span>

```output
-bash: lsb_release: command not found
```

<span data-ttu-id="210ea-122">Fehlerursache: „lsb_release“ ist nicht installiert.</span><span class="sxs-lookup"><span data-stu-id="210ea-122">The error is due to lsb_release not being installed.</span></span> <span data-ttu-id="210ea-123">Das Problem lässt sich durch Installieren des Pakets `lsb-release` beheben.</span><span class="sxs-lookup"><span data-stu-id="210ea-123">You can resolve it by installing the `lsb-release` package.</span></span>

```bash
sudo apt-get install lsb-release
```

### <a name="lsbrelease-does-not-return-the-base-distribution-version"></a><span data-ttu-id="210ea-124">„lsb_release“ gibt nicht die Basisdistributionsversion zurück.</span><span class="sxs-lookup"><span data-stu-id="210ea-124">lsb_release does not return the base distribution version</span></span>

<span data-ttu-id="210ea-125">Einige von Ubuntu oder Debian abgeleiteten Distributionen wie Linux Mint geben über `lsb_release` unter Umständen nicht den richtigen Versionsnamen zurück.</span><span class="sxs-lookup"><span data-stu-id="210ea-125">Some Ubuntu- or Debian-derived distributions such as Linux Mint may not return the correct version name from `lsb_release`.</span></span> <span data-ttu-id="210ea-126">Mit diesem Wert wird im Installationsprozess das zu installierende Pakete ermittelt.</span><span class="sxs-lookup"><span data-stu-id="210ea-126">This value is used in the install process to determine the package to install.</span></span> <span data-ttu-id="210ea-127">Wenn Sie den Namen der Version kennen, von der Ihre Distribution abgeleitet ist, können Sie im [Installationsschritt 1](#install-step-1) den Wert `AZ_REPO` manuell festlegen.</span><span class="sxs-lookup"><span data-stu-id="210ea-127">If you know the name of the version your distribution is derived from, you can set the `AZ_REPO` value manually in [install step 1](#install-step-1).</span></span> <span data-ttu-id="210ea-128">Sehen Sie sich andernfalls Informationen dazu an, wie Sie für Ihre Distribution den Basisdistributionsnamen ermitteln, und legen Sie `AZ_REPO` auf den richtigen Wert fest.</span><span class="sxs-lookup"><span data-stu-id="210ea-128">Otherwise, look up information for your distribution on how to determine the base distribution name and set `AZ_REPO` to the correct value.</span></span>

### <a name="apt-key-fails-with-no-dirmngr"></a><span data-ttu-id="210ea-129">Fehler „No dirmngr“ beim Ausführen von „apt-key“</span><span class="sxs-lookup"><span data-stu-id="210ea-129">apt-key fails with "No dirmngr"</span></span>

<span data-ttu-id="210ea-130">Beim Ausführen des Befehls `apt-key` wird unter Umständen eine Ausgabe wie die folgende angezeigt:</span><span class="sxs-lookup"><span data-stu-id="210ea-130">When running the `apt-key` command, you may see output similar to the following error:</span></span>

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

<span data-ttu-id="210ea-131">Dieser Fehler ist auf eine fehlende Komponente zurückzuführen, die von `apt-key` benötigt wird.</span><span class="sxs-lookup"><span data-stu-id="210ea-131">The error is due to a missing component required by `apt-key`.</span></span> <span data-ttu-id="210ea-132">Das Problem lässt sich durch Installieren des Pakets `dirmngr` beheben.</span><span class="sxs-lookup"><span data-stu-id="210ea-132">You can resolve it by installing the `dirmngr` package.</span></span>

```bash
sudo apt-get install dirmngr
```

### <a name="apt-key-hangs"></a><span data-ttu-id="210ea-133">Keine Reaktion von „apt-key“</span><span class="sxs-lookup"><span data-stu-id="210ea-133">apt-key hangs</span></span>

<span data-ttu-id="210ea-134">Wenn hinter einer Firewall ausgehende Verbindungen mit Port 11371 blockiert werden, hängt der Befehl `apt-key` unter Umständen auf unbestimmte Zeit.</span><span class="sxs-lookup"><span data-stu-id="210ea-134">When behind a firewall blocking outgoing connections to port 11371, the `apt-key` command might hang indefinitely.</span></span> <span data-ttu-id="210ea-135">Für Ihre Firewall muss möglicherweise ein HTTP-Proxy für ausgehende Verbindungen verwendet werden:</span><span class="sxs-lookup"><span data-stu-id="210ea-135">Your firewall may require the use of an HTTP proxy for outgoing connections:</span></span>

```bash
sudo apt-key adv --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ --keyserver packages.microsoft.com --recv-keys 52E16F86FEE04B979B07E28DB02C46DF417A0893
```

<span data-ttu-id="210ea-136">Wenn Sie nicht wissen, ob ein Proxy eingerichtet ist, wenden Sie sich an Ihren Systemadministrator.</span><span class="sxs-lookup"><span data-stu-id="210ea-136">If you do not know if you have a proxy, contact your system administrator.</span></span> <span data-ttu-id="210ea-137">Wenn für den Proxy keine Anmeldung erforderlich ist, lassen Sie Benutzer, Kennwort und `@`-Token weg.</span><span class="sxs-lookup"><span data-stu-id="210ea-137">If your proxy does not require a login then leave out the user, password, and `@` token.</span></span>

## <a name="update"></a><span data-ttu-id="210ea-138">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="210ea-138">Update</span></span>

<span data-ttu-id="210ea-139">Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.</span><span class="sxs-lookup"><span data-stu-id="210ea-139">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> <span data-ttu-id="210ea-140">Der Signaturschlüssel wurde im Mai 2018 aktualisiert und ersetzt.</span><span class="sxs-lookup"><span data-stu-id="210ea-140">The signing key was updated in May 2018, and has been replaced.</span></span> <span data-ttu-id="210ea-141">Falls Signaturschlüsselfehler auftreten, stellen Sie sicher, dass Sie den [aktuellen Signaturschlüssel](#signingKey) abgerufen haben.</span><span class="sxs-lookup"><span data-stu-id="210ea-141">If you receive signing key errors, please ensure that you have [acquired the latest signing key](#signingKey).</span></span>
   
> [!NOTE]
> <span data-ttu-id="210ea-142">Durch diesen Befehl werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.</span><span class="sxs-lookup"><span data-stu-id="210ea-142">This command upgrades all of the installed packages on your system that have not had a dependency change.</span></span>
> <span data-ttu-id="210ea-143">Wenn Sie nur ein Upgrade für die CLI durchführen möchten, verwenden Sie `apt-get install`.</span><span class="sxs-lookup"><span data-stu-id="210ea-143">To upgrade the CLI only, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a><span data-ttu-id="210ea-144">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="210ea-144">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="210ea-145">Deinstallieren Sie sie mit `apt-get remove`.</span><span class="sxs-lookup"><span data-stu-id="210ea-145">Uninstall with `apt-get remove`.</span></span>

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. <span data-ttu-id="210ea-146">Entfernen Sie die Azure CLI-Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="210ea-146">If you do not plan to reinstall the CLI, remove the Azure CLI repository information.</span></span>

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. <span data-ttu-id="210ea-147">Entfernen Sie alle nicht benötigten Pakete.</span><span class="sxs-lookup"><span data-stu-id="210ea-147">Remove any unneeded packages.</span></span>

   ```bash
   sudo apt autoremove
   ```

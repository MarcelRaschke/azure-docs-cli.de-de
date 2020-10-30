---
title: Installieren der Azure CLI unter Linux mit zypper
description: Installieren der Azure CLI mit zypper
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/25/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: e501d05985b0483442ab11f78343d773fd7e55bf
ms.sourcegitcommit: 1187fb75b68426c46e84b3f294c509ee7b7da9be
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/27/2020
ms.locfileid: "92687098"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="37305-103">Installieren der Azure CLI mit zypper</span><span class="sxs-lookup"><span data-stu-id="37305-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="37305-104">Für Linux-Distributionen mit `zypper` wie openSUSE oder SLES ist ein Paket für die Azure CLI verfügbar.</span><span class="sxs-lookup"><span data-stu-id="37305-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="37305-105">Dieses Paket wurde mit openSUSE Leap 15.1 und SLES 15 getestet.</span><span class="sxs-lookup"><span data-stu-id="37305-105">This package has been tested with openSUSE Leap 15.1, and SLES 15.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="37305-106">Installieren</span><span class="sxs-lookup"><span data-stu-id="37305-106">Install</span></span>

1. <span data-ttu-id="37305-107">Installieren Sie `curl`:</span><span class="sxs-lookup"><span data-stu-id="37305-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="37305-108">Importieren Sie den Microsoft-Repositoryschlüssel:</span><span class="sxs-lookup"><span data-stu-id="37305-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="37305-109">Erstellen Sie lokale `azure-cli`-Repositoryinformationen:</span><span class="sxs-lookup"><span data-stu-id="37305-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="37305-110">Aktualisieren Sie den `zypper`-Paketindex, und führen Sie die Installation durch:</span><span class="sxs-lookup"><span data-stu-id="37305-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli azure-cli
   ```
   <span data-ttu-id="37305-111">2 eingeben, um die Installation fortzusetzen, indem einige Abhängigkeiten ignoriert werden.</span><span class="sxs-lookup"><span data-stu-id="37305-111">Input 2 to continue install by ignoring some of its dependencies.</span></span>

<span data-ttu-id="37305-112">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="37305-112">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="37305-113">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="37305-113">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="37305-114">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="37305-114">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="37305-115">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="37305-115">Troubleshooting</span></span>

<span data-ttu-id="37305-116">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `zypper` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="37305-116">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="37305-117">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="37305-117">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="notimplementederror-on-opensuse-15-vm"></a><span data-ttu-id="37305-118">NotImplementedError auf OpenSUSE 15-VM</span><span class="sxs-lookup"><span data-stu-id="37305-118">NotImplementedError on OpenSUSE 15 VM</span></span>
<span data-ttu-id="37305-119">Auf der OpenSUSE 15-VM ist die Azure CLI mit Version `2.0.45` vorinstalliert. Diese ist veraltet, und es treten Probleme mit `az login` auf.</span><span class="sxs-lookup"><span data-stu-id="37305-119">The OpenSUSE 15 VM has a pre-installed Azure CLI with version `2.0.45`, it's outdated and has issues with `az login`.</span></span> <span data-ttu-id="37305-120">Entfernen Sie sie zusammen mit den zugehörigen Abhängigkeiten, bevor Sie die [Installationsanweisungen](#install) zum Hinzufügen der aktuellen Azure CLI befolgen:</span><span class="sxs-lookup"><span data-stu-id="37305-120">Please remove it along with its dependencies before following the [Install](#install) instruction to add the latest Azure CLI:</span></span>
```bash
sudo zypper rm -y --clean-deps azure-cli
```

<span data-ttu-id="37305-121">Wenn Sie die Azure CLI aktualisiert haben, ohne die Abhängigkeiten von Version `2.0.45` zu entfernen, beeinträchtigen die alten Abhängigkeiten unter Umständen die aktuelle Version der Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="37305-121">If you updated Azure CLI without removing the dependencies of version `2.0.45`, its old dependencies may affect the latest version of Azure CLI.</span></span> <span data-ttu-id="37305-122">Sie müssen die alte Version wieder hinzufügen, um eine Verknüpfung mit ihren Abhängigkeiten herzustellen, und anschließend `azure-cli` zusammen mit den Abhängigkeiten entfernen:</span><span class="sxs-lookup"><span data-stu-id="37305-122">You need to add back the old version to link to its dependencies and then remove `azure-cli` along with its dependencies:</span></span>
```bash
# The package name may vary on different system version, run 'zypper --no-refresh info azure-cli' to check the source package format
sudo zypper install --oldpackage azure-cli-2.0.45-4.22.noarch

sudo zypper rm -y --clean-deps azure-cli
```


### <a name="install-on-sles-12-or-other-systems-without-python-36"></a><span data-ttu-id="37305-123">Installieren auf SLES 12 oder anderen Systemen ohne Python 3.6</span><span class="sxs-lookup"><span data-stu-id="37305-123">Install on SLES 12 or other systems without Python 3.6</span></span>

<span data-ttu-id="37305-124">Unter SLES 12 ist `3.4` das standardmäßige `python3`-Paket und wird von der Azure CLI nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="37305-124">On SLES 12, the default `python3` package is `3.4` and not supported by Azure CLI.</span></span> <span data-ttu-id="37305-125">Sie können zuerst die Schritte 1 bis 3 der [Installationsanweisungen](#install) ausführen, um das Repository `azure-cli` hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="37305-125">You can first follow step 1-3 of the [install instruction](#install) to add the `azure-cli` repository.</span></span> <span data-ttu-id="37305-126">Erstellen Sie dann eine höhere Version von `python3` aus der Quelle.</span><span class="sxs-lookup"><span data-stu-id="37305-126">Then build a higher version `python3` from source.</span></span> <span data-ttu-id="37305-127">Abschließend können Sie das Azure CLI-Paket herunterladen und ohne Abhängigkeit installieren.</span><span class="sxs-lookup"><span data-stu-id="37305-127">Finally, you can download the Azure CLI package and install it without dependency.</span></span>

<span data-ttu-id="37305-128">Sie können den folgenden Befehl verwenden, um die Azure CLI zu installieren. (Beachten Sie, dass Ihre vorhandene Python 3-Version von Python 3.6 überschrieben wird.)</span><span class="sxs-lookup"><span data-stu-id="37305-128">You can use the following one command to install Azure CLI (be aware that your existing Python 3 version will be overridden by Python 3.6):</span></span>
```bash
curl -sL https://azurecliprod.blob.core.windows.net/sles12_install.sh | sudo bash
```

<span data-ttu-id="37305-129">Alternativ können Sie Schritt für Schritt vorgehen:</span><span class="sxs-lookup"><span data-stu-id="37305-129">Or you can do it step by step:</span></span>

```bash
# !Please add azure-cli repository first following step 1-3 of the install instruction before running below commands
$ sudo zypper refresh
$ sudo zypper install -y gcc gcc-c++ make ncurses patch wget tar zlib-devel zlib openssl-devel
# Download Python source code
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
# Build Python
# Please be aware that with --prefix=/usr, the command will override the existing Python 3 version
$ $PYTHON_SRC_DIR/*/configure --prefix=/usr
$ make
$ sudo make install
# Download azure-cli package 
$ AZ_VERSION=$(zypper --no-refresh info azure-cli |grep Version | awk -F': ' '{print $2}' | awk '{$1=$1;print}')
$ wget https://packages.microsoft.com/yumrepos/azure-cli/azure-cli-$AZ_VERSION.x86_64.rpm
# Install without dependency
$ sudo rpm -ivh --nodeps azure-cli-$AZ_VERSION.x86_64.rpm
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="37305-130">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="37305-130">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="37305-131">Konfigurieren Sie `zypper` (über `yast2`) explizit so, dass dieser Proxy immer verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="37305-131">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="37305-132">Führen Sie hierfür den Befehl `yast2 proxy` als Superuser aus, und geben Sie die Informationen im Formular ein.</span><span class="sxs-lookup"><span data-stu-id="37305-132">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="37305-133">Wenn auf Ihrem System ein Fenster-Manager verfügbar ist, können Sie auch den Bereich `Network Services > Proxy` in `YaST Control Center` verwenden.</span><span class="sxs-lookup"><span data-stu-id="37305-133">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="37305-134">Details zur erweiterten Konfiguration oder weitere Informationen finden Sie in der [Dokumentation zur OpenSUSE-Proxykonfiguration](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html).</span><span class="sxs-lookup"><span data-stu-id="37305-134">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="37305-135">Zum Abrufen des Microsoft-Signaturschlüssels und des Pakets von unserem Repository muss Ihr Proxy HTTPS-Verbindungen mit den folgenden Adressen zulassen:</span><span class="sxs-lookup"><span data-stu-id="37305-135">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

### <a name="ssl-certificate-problem"></a><span data-ttu-id="37305-136">SSL-Zertifikatproblem</span><span class="sxs-lookup"><span data-stu-id="37305-136">SSL certificate problem</span></span>

<span data-ttu-id="37305-137">Wenn ein Zertifikat auf einem Computer beschädigt oder veraltet ist, erhalten Sie möglicherweise eine Fehlermeldung, die besagt, dass curl die Legitimität des Servers nicht verifizieren konnte und daher keine sichere Verbindung herstellen konnte.</span><span class="sxs-lookup"><span data-stu-id="37305-137">When a certificate is broken or outdated on a machine, you may receive an error indicating that curl failed to verify the legitimacy of the server and therefore could not establish a secure connection.</span></span>  <span data-ttu-id="37305-138">Aktualisieren Sie Ihr Zertifikat, um das Problem zu beheben.</span><span class="sxs-lookup"><span data-stu-id="37305-138">Update your certificate to correct the problem.</span></span>  

```bach
sudo zypper update-ca-certificates
```

## <a name="update"></a><span data-ttu-id="37305-139">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="37305-139">Update</span></span>

[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="37305-140">Sie können das Paket auch mit dem Befehl `zypper update` aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="37305-140">You can also update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="37305-141">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="37305-141">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="37305-142">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="37305-142">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="37305-143">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="37305-143">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="37305-144">Wenn Sie keine anderen Microsoft-Pakete verwenden, entfernen Sie den Microsoft-Signaturschlüssel.</span><span class="sxs-lookup"><span data-stu-id="37305-144">If you don't use other Microsoft packages, remove the Microsoft signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="37305-145">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="37305-145">Next Steps</span></span>

<span data-ttu-id="37305-146">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="37305-146">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="37305-147">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="37305-147">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
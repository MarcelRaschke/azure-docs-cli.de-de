---
title: Installieren der Azure CLI unter Linux mit zypper
description: Installieren der Azure CLI mit zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 7e5897fe545527aa2708432e0ad0cf626584c785
ms.sourcegitcommit: 0088160bdb1ea520724d3e1efe71a4a66f29753d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/19/2019
ms.locfileid: "75216876"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="518e4-103">Installieren der Azure CLI mit zypper</span><span class="sxs-lookup"><span data-stu-id="518e4-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="518e4-104">Für Linux-Distributionen mit `zypper` wie openSUSE oder SLES ist ein Paket für die Azure CLI verfügbar.</span><span class="sxs-lookup"><span data-stu-id="518e4-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="518e4-105">Dieses Paket wurde mit openSUSE Leap 15.1 und SLES 15 getestet.</span><span class="sxs-lookup"><span data-stu-id="518e4-105">This package has been tested with openSUSE Leap 15.1, and SLES 15.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="518e4-106">Installieren</span><span class="sxs-lookup"><span data-stu-id="518e4-106">Install</span></span>

1. <span data-ttu-id="518e4-107">Installieren Sie `curl`:</span><span class="sxs-lookup"><span data-stu-id="518e4-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="518e4-108">Importieren Sie den Microsoft-Repositoryschlüssel:</span><span class="sxs-lookup"><span data-stu-id="518e4-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="518e4-109">Erstellen Sie lokale `azure-cli`-Repositoryinformationen:</span><span class="sxs-lookup"><span data-stu-id="518e4-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="518e4-110">Aktualisieren Sie den `zypper`-Paketindex, und führen Sie die Installation durch:</span><span class="sxs-lookup"><span data-stu-id="518e4-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="518e4-111">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="518e4-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="518e4-112">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="518e4-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="518e4-113">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="518e4-113">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="518e4-114">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="518e4-114">Troubleshooting</span></span>

<span data-ttu-id="518e4-115">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `zypper` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="518e4-115">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="518e4-116">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="518e4-116">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-sles-12-or-other-other-systems-without-python-36"></a><span data-ttu-id="518e4-117">Installieren auf SLES 12 oder anderen Systemen ohne Python 3.6</span><span class="sxs-lookup"><span data-stu-id="518e4-117">Install on SLES 12 or other other systems without Python 3.6</span></span>

<span data-ttu-id="518e4-118">Auf SLES 12 ist das 3.4 das standardmäßige python3-Paket und wird von der Azure CLI nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="518e4-118">On SLES 12, the defualt python3 package is 3.4 and not supported by Azure CLI.</span></span> <span data-ttu-id="518e4-119">Sie können zuerst python3 mit einer höheren Version aus der Quelle erstellen.</span><span class="sxs-lookup"><span data-stu-id="518e4-119">You can first build a higher version python3 from source.</span></span> <span data-ttu-id="518e4-120">Anschließend können Sie das Azure CLI-Paket herunterladen und ohne Abhängigkeit installieren.</span><span class="sxs-lookup"><span data-stu-id="518e4-120">Then you can download the Azure CLI package and install it without dependency.</span></span>
```bash
$ sudo zypper install -y gcc gcc-c++ make ncurses patch wget tar zlib-devel zlib
# Download Python source code
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
# Build Python
$ $PYTHON_SRC_DIR/*/configure --with-ssl
$ make
$ sudo make install
#Download azure-cli package 
$ AZ_VERSION=$(zypper --no-refresh info azure-cli |grep Version | awk -F': ' '{print $2}' | awk '{$1=$1;print}')
$ wget https://packages.microsoft.com/yumrepos/azure-cli/azure-cli-$AZ_VERSION.x86_64.rpm
#Install without dependency
$ sudo rpm -ivh --nodeps azure-cli-$AZ_VERSION.x86_64.rpm
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="518e4-121">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="518e4-121">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="518e4-122">Konfigurieren Sie `zypper` (über `yast2`) explizit so, dass dieser Proxy immer verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="518e4-122">You may also want to explicitly configure `zypper` (via `yast2`) to use this proxy at all times.</span></span> <span data-ttu-id="518e4-123">Führen Sie hierfür den Befehl `yast2 proxy` als Superuser aus, und geben Sie die Informationen im Formular ein.</span><span class="sxs-lookup"><span data-stu-id="518e4-123">To do so, run the `yast2 proxy` command as superuser, and fill in the information presented in the form.</span></span> <span data-ttu-id="518e4-124">Wenn auf Ihrem System ein Fenster-Manager verfügbar ist, können Sie auch den Bereich `Network Services > Proxy` in `YaST Control Center` verwenden.</span><span class="sxs-lookup"><span data-stu-id="518e4-124">If you have a window manager available on your system, you can also use the `Network Services > Proxy` pane in the `YaST Control Center`.</span></span>

<span data-ttu-id="518e4-125">Details zur erweiterten Konfiguration oder weitere Informationen finden Sie in der [Dokumentation zur OpenSUSE-Proxykonfiguration](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html).</span><span class="sxs-lookup"><span data-stu-id="518e4-125">For advanced configuration or more information, see the [OpenSUSE Proxy configuration documentation](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html)</span></span>

<span data-ttu-id="518e4-126">Zum Abrufen des Microsoft-Signaturschlüssels und des Pakets von unserem Repository muss Ihr Proxy HTTPS-Verbindungen mit den folgenden Adressen zulassen:</span><span class="sxs-lookup"><span data-stu-id="518e4-126">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="518e4-127">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="518e4-127">Update</span></span>

<span data-ttu-id="518e4-128">Sie können das Paket mit dem Befehl `zypper update` aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="518e4-128">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="518e4-129">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="518e4-129">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="518e4-130">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="518e4-130">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="518e4-131">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="518e4-131">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="518e4-132">Wenn Sie keine anderen Microsoft-Pakete verwenden, entfernen Sie den Microsoft-Signaturschlüssel.</span><span class="sxs-lookup"><span data-stu-id="518e4-132">If you don't use other Microsoft packages, remove the Microsoft signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="518e4-133">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="518e4-133">Next Steps</span></span>

<span data-ttu-id="518e4-134">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="518e4-134">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="518e4-135">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="518e4-135">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

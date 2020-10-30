---
title: Installieren der Azure CLI unter Linux mit yum
description: Installieren der Azure CLI mit yum
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/25/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: fac9f37969ac23245568c521d5d3e50efa5c050d
ms.sourcegitcommit: 1187fb75b68426c46e84b3f294c509ee7b7da9be
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/27/2020
ms.locfileid: "92687063"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="db90c-103">Installieren der Azure CLI mit yum</span><span class="sxs-lookup"><span data-stu-id="db90c-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="db90c-104">Für Linux-Distributionen mit `yum` (etwa RHEL, Fedora oder CentOS) ist ein Paket für die Azure CLI verfügbar.</span><span class="sxs-lookup"><span data-stu-id="db90c-104">For Linux distributions with `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="db90c-105">Dieses Paket wurde mit RHEL 7.7, RHEL 8, Fedora 24 (und höher), CentOS 7 und CentOS 8 getestet.</span><span class="sxs-lookup"><span data-stu-id="db90c-105">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="db90c-106">Installieren</span><span class="sxs-lookup"><span data-stu-id="db90c-106">Install</span></span>

1. <span data-ttu-id="db90c-107">Importieren Sie den Microsoft-Repositoryschlüssel.</span><span class="sxs-lookup"><span data-stu-id="db90c-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="db90c-108">Erstellen Sie lokale `azure-cli`-Repositoryinformationen.</span><span class="sxs-lookup"><span data-stu-id="db90c-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="db90c-109">Installieren Sie mit dem Befehl `yum install`.</span><span class="sxs-lookup"><span data-stu-id="db90c-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="db90c-110">Führen Sie die Azure CLI mit dem Befehl `az` aus.</span><span class="sxs-lookup"><span data-stu-id="db90c-110">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="db90c-111">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="db90c-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="db90c-112">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="db90c-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="db90c-113">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="db90c-113">Troubleshooting</span></span>

<span data-ttu-id="db90c-114">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `yum` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="db90c-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="db90c-115">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="db90c-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="db90c-116">Installieren auf RHEL 7.6 oder anderen Systemen ohne Python 3</span><span class="sxs-lookup"><span data-stu-id="db90c-116">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="db90c-117">Führen Sie wenn möglich ein Upgrade Ihres Systems auf eine Version mit offizieller Unterstützung für `python 3.6+`-Pakete durch.</span><span class="sxs-lookup"><span data-stu-id="db90c-117">If you can, please upgrade your system to a version with official support for `python 3.6+` package.</span></span> <span data-ttu-id="db90c-118">Andernfalls müssen Sie zuerst ein `python3`-Paket und dann die Azure CLI ohne Abhängigkeit installieren.</span><span class="sxs-lookup"><span data-stu-id="db90c-118">Otherwise, you need to first install a `python3` package then install Azure CLI without dependency.</span></span> 

<span data-ttu-id="db90c-119">Sie können den folgenden Befehl verwenden, um die Azure CLI mit dem aus der Quelle erstellten `python 3.6`-Paket zu installieren:</span><span class="sxs-lookup"><span data-stu-id="db90c-119">You can use the following one command to install Azure CLI with `python 3.6` built from source:</span></span>
```bash
curl -sL https://azurecliprod.blob.core.windows.net/rhel7_6_install.sh | sudo bash
```
<span data-ttu-id="db90c-120">Sie können auch Schritt für Schritt vorgehen:</span><span class="sxs-lookup"><span data-stu-id="db90c-120">You can also do it step by step:</span></span>

<span data-ttu-id="db90c-121">Die Azure CLI erfordert zuerst `SSL 1.1+`, und Sie müssen `openssl 1.1` aus der Quelle erstellen, bevor Sie `python3` erstellen:</span><span class="sxs-lookup"><span data-stu-id="db90c-121">First, Azure CLI requires `SSL 1.1+` and you need to build `openssl 1.1` from source before building `python3`:</span></span>
```bash
$ sudo yum install gcc gcc-c++ make ncurses patch wget tar zlib zlib-devel -y
# build openssl from source
$ cd ~
$ wget https://www.openssl.org/source/openssl-1.1.1d.tar.gz
$ tar -xzf openssl-1.1.1d.tar.gz
$ cd openssl-1.1.1d
$ ./config --prefix=/usr/local/ssl --openssldir=/usr/local/ssl
$ make
$ sudo make install
# configure shared object lookup directory so that libssl.so.1.1 can be found
$ echo "/usr/local/ssl/lib" | sudo tee /etc/ld.so.conf.d/openssl-1.1.1d.conf
# reload config
$ sudo ldconfig -v
```

<span data-ttu-id="db90c-122">Erstellen Sie anschließend Python 3 aus der Quelle:</span><span class="sxs-lookup"><span data-stu-id="db90c-122">Then build Python 3 from source:</span></span>
```bash
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
$ cd $PYTHON_SRC_DIR/Python-$PYTHON_VERSION
$ ./configure --prefix=/usr --with-openssl=/usr/local/ssl
$ make
$ sudo make install
```

<span data-ttu-id="db90c-123">Führen Sie schließlich Schritt 1 und 2 der [Installationsanweisungen](#install) aus, um das Azure CLI-Repository hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="db90c-123">Finally, follow step 1 and 2 of the [install instruction](#install) to add Azure CLI repository.</span></span> <span data-ttu-id="db90c-124">Nun können Sie das Paket herunterladen und ohne Abhängigkeit installieren.</span><span class="sxs-lookup"><span data-stu-id="db90c-124">You can now download the package and install it without dependency.</span></span>
```bash
$ sudo yum install yum-utils -y
$ sudo yumdownloader azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="db90c-125">Als Alternative können Sie Python 3 auch über ein [zusätzliches Repository](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/) installieren.</span><span class="sxs-lookup"><span data-stu-id="db90c-125">As an alternative, you can also install Python 3 through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="db90c-126">Wenn Sie `python3` eingerichtet haben, aber weiterhin den Fehler `python3: command not found` erhalten, wenn Sie versuchen, die CLI auszuführen, müssen Sie sie bei dieser Vorgehensweise dem Pfad hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="db90c-126">Following this way, if you have set up `python3` but are still getting an error `python3: command not found` when trying to run the cli, you need to add it to your path.</span></span>
```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="db90c-127">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="db90c-127">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="db90c-128">Konfigurieren Sie `yum` explizit so, dass dieser Proxy immer verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="db90c-128">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="db90c-129">Stellen Sie sicher, dass die folgenden Zeilen im Abschnitt `[main]` von `/etc/yum.conf` erscheinen:</span><span class="sxs-lookup"><span data-stu-id="db90c-129">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="db90c-130">Zum Abrufen des Microsoft-Signaturschlüssels und des Pakets von unserem Repository muss Ihr Proxy HTTPS-Verbindungen mit der folgenden Adresse zulassen:</span><span class="sxs-lookup"><span data-stu-id="db90c-130">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="db90c-131">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="db90c-131">Update</span></span>

[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="db90c-132">Sie können die Azure CLI auch mit dem Befehl `yum update` aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="db90c-132">You can also update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="db90c-133">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="db90c-133">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="db90c-134">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="db90c-134">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="db90c-135">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="db90c-135">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="db90c-136">Wenn Sie keine anderen Microsoft-Pakete verwenden, entfernen Sie den Signaturschlüssel.</span><span class="sxs-lookup"><span data-stu-id="db90c-136">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="db90c-137">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="db90c-137">Next Steps</span></span>

<span data-ttu-id="db90c-138">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="db90c-138">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="db90c-139">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="db90c-139">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

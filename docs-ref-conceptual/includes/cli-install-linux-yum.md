---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: 6f121eff4f024da81dbf107fba5f5bd9d3b8aa0b
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744635"
---
## <a name="overview"></a><span data-ttu-id="2c28c-101">Übersicht</span><span class="sxs-lookup"><span data-stu-id="2c28c-101">Overview</span></span>

<span data-ttu-id="2c28c-102">Für Linux-Distributionen mit `yum` (etwa RHEL, Fedora oder CentOS) ist ein Paket für die Azure CLI verfügbar.</span><span class="sxs-lookup"><span data-stu-id="2c28c-102">For Linux distributions with `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="2c28c-103">Dieses Paket wurde mit RHEL 7.7, RHEL 8, Fedora 24 (und höher), CentOS 7 und CentOS 8 getestet.</span><span class="sxs-lookup"><span data-stu-id="2c28c-103">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="2c28c-104">Installieren</span><span class="sxs-lookup"><span data-stu-id="2c28c-104">Install</span></span>

1. <span data-ttu-id="2c28c-105">Importieren Sie den Microsoft-Repositoryschlüssel.</span><span class="sxs-lookup"><span data-stu-id="2c28c-105">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="2c28c-106">Erstellen Sie lokale `azure-cli`-Repositoryinformationen.</span><span class="sxs-lookup"><span data-stu-id="2c28c-106">Create local `azure-cli` repository information.</span></span>

   ```bash
   echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="2c28c-107">Installieren Sie mit dem Befehl `yum install`.</span><span class="sxs-lookup"><span data-stu-id="2c28c-107">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="2c28c-108">Führen Sie die Azure CLI mit dem Befehl `az` aus.</span><span class="sxs-lookup"><span data-stu-id="2c28c-108">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="2c28c-109">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="2c28c-109">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="2c28c-110">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="2c28c-110">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="2c28c-111">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="2c28c-111">Troubleshooting</span></span>

<span data-ttu-id="2c28c-112">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `yum` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="2c28c-112">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="2c28c-113">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="2c28c-113">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="2c28c-114">Installieren auf RHEL 7.6 oder anderen Systemen ohne Python 3</span><span class="sxs-lookup"><span data-stu-id="2c28c-114">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="2c28c-115">Führen Sie wenn möglich ein Upgrade Ihres Systems auf eine Version mit offizieller Unterstützung für `python 3.6+`-Pakete durch.</span><span class="sxs-lookup"><span data-stu-id="2c28c-115">If you can, please upgrade your system to a version with official support for `python 3.6+` package.</span></span> <span data-ttu-id="2c28c-116">Andernfalls müssen Sie zuerst ein `python3`-Paket und dann die Azure CLI ohne Abhängigkeit installieren.</span><span class="sxs-lookup"><span data-stu-id="2c28c-116">Otherwise, you need to first install a `python3` package then install Azure CLI without dependency.</span></span>

<span data-ttu-id="2c28c-117">Sie können den folgenden Befehl verwenden, um die Azure CLI mit dem aus der Quelle erstellten `python 3.6`-Paket zu installieren:</span><span class="sxs-lookup"><span data-stu-id="2c28c-117">You can use the following one command to install Azure CLI with `python 3.6` built from source:</span></span>

```bash
curl -sL https://azurecliprod.blob.core.windows.net/rhel7_6_install.sh | sudo bash
```

<span data-ttu-id="2c28c-118">Sie können auch Schritt für Schritt vorgehen:</span><span class="sxs-lookup"><span data-stu-id="2c28c-118">You can also do it step by step:</span></span>

<span data-ttu-id="2c28c-119">Die Azure CLI erfordert zuerst `SSL 1.1+`, und Sie müssen `openssl 1.1` aus der Quelle erstellen, bevor Sie `python3` erstellen:</span><span class="sxs-lookup"><span data-stu-id="2c28c-119">First, Azure CLI requires `SSL 1.1+` and you need to build `openssl 1.1` from source before building `python3`:</span></span>

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

<span data-ttu-id="2c28c-120">Erstellen Sie anschließend Python 3 aus der Quelle:</span><span class="sxs-lookup"><span data-stu-id="2c28c-120">Then build Python 3 from source:</span></span>

```bash
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
$ cd $PYTHON_SRC_DIR/Python-$PYTHON_VERSION
$ ./configure --prefix=/usr --with-openssl=/usr/local/ssl
$ make
$ sudo make install
```

<span data-ttu-id="2c28c-121">Führen Sie schließlich Schritt 1 und 2 der [Installationsanweisungen](#install) aus, um das Azure CLI-Repository hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="2c28c-121">Finally, follow step 1 and 2 of the [install instruction](#install) to add Azure CLI repository.</span></span> <span data-ttu-id="2c28c-122">Nun können Sie das Paket herunterladen und ohne Abhängigkeit installieren.</span><span class="sxs-lookup"><span data-stu-id="2c28c-122">You can now download the package and install it without dependency.</span></span>

```bash
$ sudo yum install yum-utils -y
$ sudo yumdownloader azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="2c28c-123">Als Alternative können Sie Python 3 auch über ein [zusätzliches Repository](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/) installieren.</span><span class="sxs-lookup"><span data-stu-id="2c28c-123">As an alternative, you can also install Python 3 through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="2c28c-124">Wenn Sie `python3` eingerichtet haben, aber weiterhin den Fehler `python3: command not found` erhalten, wenn Sie versuchen, die CLI auszuführen, müssen Sie sie bei dieser Vorgehensweise dem Pfad hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="2c28c-124">Following this way, if you have set up `python3` but are still getting an error `python3: command not found` when trying to run the cli, you need to add it to your path.</span></span>

```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="2c28c-125">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="2c28c-125">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="2c28c-126">Konfigurieren Sie `yum` explizit so, dass dieser Proxy immer verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="2c28c-126">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="2c28c-127">Stellen Sie sicher, dass die folgenden Zeilen im Abschnitt `[main]` von `/etc/yum.conf` erscheinen:</span><span class="sxs-lookup"><span data-stu-id="2c28c-127">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="2c28c-128">Zum Abrufen des Microsoft-Signaturschlüssels und des Pakets von unserem Repository muss Ihr Proxy HTTPS-Verbindungen mit der folgenden Adresse zulassen:</span><span class="sxs-lookup"><span data-stu-id="2c28c-128">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="2c28c-129">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2c28c-129">Update</span></span>

[!INCLUDE [az-upgrade](az-upgrade.md)]

<span data-ttu-id="2c28c-130">Sie können die Azure CLI auch mit dem Befehl `yum update` aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="2c28c-130">You can also update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="2c28c-131">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="2c28c-131">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. <span data-ttu-id="2c28c-132">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="2c28c-132">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="2c28c-133">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="2c28c-133">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="2c28c-134">Wenn Sie keine anderen Microsoft-Pakete verwenden, entfernen Sie den Signaturschlüssel.</span><span class="sxs-lookup"><span data-stu-id="2c28c-134">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

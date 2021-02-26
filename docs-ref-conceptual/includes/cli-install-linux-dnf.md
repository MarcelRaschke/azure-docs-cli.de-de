---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: c0de92ff9aed581d192d72ca920fafea8bbd192b
ms.sourcegitcommit: 594e9c620a6f74f5eaedf91a7f6a791e03a64c74
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/17/2021
ms.locfileid: "100631004"
---
## <a name="overview"></a><span data-ttu-id="e4b2a-101">Übersicht</span><span class="sxs-lookup"><span data-stu-id="e4b2a-101">Overview</span></span>

<span data-ttu-id="e4b2a-102">Für Linux-Distributionen mit `dnf` (etwa RHEL, Fedora oder CentOS) ist ein Paket für die Azure CLI verfügbar.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-102">For Linux distributions with `dnf` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="e4b2a-103">Dieses Paket wurde mit RHEL 7.7, RHEL 8, Fedora 24 (und höher), CentOS 7 und CentOS 8 getestet.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-103">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

> [!NOTE]
>
> <span data-ttu-id="e4b2a-104">Nutzen Sie bei Verwendung von Linux-Systemen, die den `dnf`-Paket-Manager nicht unterstützen, den `yum`-Paket-Manager.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-104">Use `yum` package manager if you are using Linux systems that don't support `dnf` package manager.</span></span>

## <a name="install"></a><span data-ttu-id="e4b2a-105">Installieren</span><span class="sxs-lookup"><span data-stu-id="e4b2a-105">Install</span></span>

1. <span data-ttu-id="e4b2a-106">Importieren Sie den Microsoft-Repositoryschlüssel.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-106">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="e4b2a-107">Erstellen Sie lokale `azure-cli`-Repositoryinformationen.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-107">Create local `azure-cli` repository information.</span></span>

   ```bash
   echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="e4b2a-108">Installieren Sie mit dem Befehl `dnf install`.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-108">Install with the `dnf install` command.</span></span>

   ```bash
   sudo dnf install azure-cli
   ```
 
<span data-ttu-id="e4b2a-109">Führen Sie die Azure CLI mit dem Befehl `az` aus.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-109">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="e4b2a-110">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-110">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>


[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="e4b2a-111">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e4b2a-111">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="e4b2a-112">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="e4b2a-112">Troubleshooting</span></span>

<span data-ttu-id="e4b2a-113">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `dnf` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-113">Here are some common problems seen when installing with `dnf`.</span></span> <span data-ttu-id="e4b2a-114">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="e4b2a-114">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="e4b2a-115">Installieren auf RHEL 7.6 oder anderen Systemen ohne Python 3</span><span class="sxs-lookup"><span data-stu-id="e4b2a-115">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="e4b2a-116">Führen Sie wenn möglich ein Upgrade Ihres Systems auf eine Version mit offizieller Unterstützung für `python 3.6+`-Pakete durch.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-116">If you can, please upgrade your system to a version with official support for `python 3.6+` package.</span></span> <span data-ttu-id="e4b2a-117">Andernfalls müssen Sie zuerst ein `python3`-Paket und dann die Azure CLI ohne Abhängigkeit installieren.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-117">Otherwise, you need to first install a `python3` package then install Azure CLI without dependency.</span></span>

<span data-ttu-id="e4b2a-118">Sie können den folgenden Befehl verwenden, um die Azure CLI mit dem aus der Quelle erstellten `python 3.6`-Paket zu installieren:</span><span class="sxs-lookup"><span data-stu-id="e4b2a-118">You can use the following one command to install Azure CLI with `python 3.6` built from source:</span></span>

```bash
curl -sL https://azurecliprod.blob.core.windows.net/rhel7_6_install.sh | sudo bash
```

<span data-ttu-id="e4b2a-119">Sie können auch Schritt für Schritt vorgehen:</span><span class="sxs-lookup"><span data-stu-id="e4b2a-119">You can also do it step by step:</span></span>

<span data-ttu-id="e4b2a-120">Die Azure CLI erfordert zuerst `SSL 1.1+`, und Sie müssen `openssl 1.1` aus der Quelle erstellen, bevor Sie `python3` erstellen:</span><span class="sxs-lookup"><span data-stu-id="e4b2a-120">First, Azure CLI requires `SSL 1.1+` and you need to build `openssl 1.1` from source before building `python3`:</span></span>

```bash
$ sudo dnf install gcc gcc-c++ make ncurses patch wget tar zlib zlib-devel -y
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

<span data-ttu-id="e4b2a-121">Erstellen Sie anschließend Python 3 aus der Quelle:</span><span class="sxs-lookup"><span data-stu-id="e4b2a-121">Then build Python 3 from source:</span></span>

```bash
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
$ cd $PYTHON_SRC_DIR/Python-$PYTHON_VERSION
$ ./configure --prefix=/usr --with-openssl=/usr/local/ssl
$ make
$ sudo make install
```

<span data-ttu-id="e4b2a-122">Führen Sie schließlich Schritt 1 und 2 der [Installationsanweisungen](#install) aus, um das Azure CLI-Repository hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-122">Finally, follow step 1 and 2 of the [install instruction](#install) to add Azure CLI repository.</span></span> <span data-ttu-id="e4b2a-123">Nun können Sie das Paket herunterladen und ohne Abhängigkeit installieren.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-123">You can now download the package and install it without dependency.</span></span>

> [!NOTE]
>
> <span data-ttu-id="e4b2a-124">Falls Sie das dnf-Download-Plug-In nicht installiert haben, wird beim Ausführen des unten angegebenen Codes der Fehler „Befehl nicht gefunden“ angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-124">In case you don't have the dnf download plugin installed, you will encounter command not found error on executing the below code.</span></span> <span data-ttu-id="e4b2a-125">Verwenden Sie `dnf install 'dnf-command(download)'` zum Installieren des dnf-Download-Plug-Ins.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-125">Use `dnf install 'dnf-command(download)'` to   install the dnf download plugin.</span></span>

```bash
$ sudo dnf download azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="e4b2a-126">Als Alternative können Sie Python 3 auch über ein [zusätzliches Repository](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/) installieren.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-126">As an alternative, you can also install Python 3 through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="e4b2a-127">Wenn Sie `python3` eingerichtet haben, aber weiterhin den Fehler `python3: command not found` erhalten, wenn Sie versuchen, die CLI auszuführen, müssen Sie sie bei dieser Vorgehensweise dem Pfad hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-127">Following this way, if you have set up `python3` but are still getting an error `python3: command not found` when trying to run the cli, you need to add it to your path.</span></span>

```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="e4b2a-128">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-128">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="e4b2a-129">Konfigurieren Sie `dnf` explizit so, dass dieser Proxy immer verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-129">You may also want to explicitly configure `dnf` to use this proxy at all times.</span></span> <span data-ttu-id="e4b2a-130">Stellen Sie sicher, dass die folgenden Zeilen im Abschnitt `[main]` von `/etc/dnf/dnf.conf` erscheinen:</span><span class="sxs-lookup"><span data-stu-id="e4b2a-130">Make sure that the following lines appear under the `[main]` section of `/etc/dnf/dnf.conf`:</span></span>

```dnf.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="e4b2a-131">Zum Abrufen des Microsoft-Signaturschlüssels und des Pakets von unserem Repository muss Ihr Proxy HTTPS-Verbindungen mit der folgenden Adresse zulassen:</span><span class="sxs-lookup"><span data-stu-id="e4b2a-131">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="e4b2a-132">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e4b2a-132">Update</span></span>

[!INCLUDE [az-upgrade](az-upgrade.md)]

<span data-ttu-id="e4b2a-133">Sie können die Azure CLI auch mit dem Befehl `dnf update` aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-133">You can also update the Azure CLI with the `dnf update` command.</span></span>

```bash
sudo dnf update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="e4b2a-134">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="e4b2a-134">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. <span data-ttu-id="e4b2a-135">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-135">Remove the package from your system.</span></span>

   ```bash
   sudo dnf remove azure-cli
   ```

2. <span data-ttu-id="e4b2a-136">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-136">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="e4b2a-137">Wenn Sie keine anderen Microsoft-Pakete verwenden, entfernen Sie den Signaturschlüssel.</span><span class="sxs-lookup"><span data-stu-id="e4b2a-137">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

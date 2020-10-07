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
ms.openlocfilehash: 08ef942ace04f018d52cf1f6f7b20dc344953485
ms.sourcegitcommit: aa44ec97af5c0e7558d254b3159f95921e22ff1c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/01/2020
ms.locfileid: "91625362"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="d8fe7-103">Installieren der Azure CLI mit yum</span><span class="sxs-lookup"><span data-stu-id="d8fe7-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="d8fe7-104">Für Linux-Distributionen mit `yum` (etwa RHEL, Fedora oder CentOS) ist ein Paket für die Azure CLI verfügbar.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-104">For Linux distributions with `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="d8fe7-105">Dieses Paket wurde mit RHEL 7.7, RHEL 8, Fedora 24 (und höher), CentOS 7 und CentOS 8 getestet.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-105">This package has been tested with RHEL 7.7, RHEL 8, Fedora 24 and higher, CentOS 7 and CentOS 8.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a><span data-ttu-id="d8fe7-106">Installieren</span><span class="sxs-lookup"><span data-stu-id="d8fe7-106">Install</span></span>

1. <span data-ttu-id="d8fe7-107">Importieren Sie den Microsoft-Repositoryschlüssel.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="d8fe7-108">Erstellen Sie lokale `azure-cli`-Repositoryinformationen.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="d8fe7-109">Installieren Sie mit dem Befehl `yum install`.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="d8fe7-110">Führen Sie die Azure CLI mit dem Befehl `az` aus.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-110">Run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="d8fe7-111">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="d8fe7-112">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d8fe7-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="d8fe7-113">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="d8fe7-113">Troubleshooting</span></span>

<span data-ttu-id="d8fe7-114">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `yum` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-114">Here are some common problems seen when installing with `yum`.</span></span> <span data-ttu-id="d8fe7-115">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="d8fe7-115">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a><span data-ttu-id="d8fe7-116">Installieren auf RHEL 7.6 oder anderen Systemen ohne Python 3</span><span class="sxs-lookup"><span data-stu-id="d8fe7-116">Install on RHEL 7.6 or other systems without Python 3</span></span>

<span data-ttu-id="d8fe7-117">Führen Sie wenn möglich ein Upgrade Ihres Systems auf eine Version mit offizieller Unterstützung für `python3`-Pakete durch.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-117">If you can, please upgrade your system to a version with official support for `python3` package.</span></span> <span data-ttu-id="d8fe7-118">Andernfalls müssen Sie zuerst ein `python3`-Paket installieren, um entweder [einen Buildvorgang aus der Quelle durchzuführen](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) oder über ein [zusätzliches Repository](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/) zu installieren.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-118">Otherwise, you need to first install a `python3` package, either [build from source](https://github.com/linux-on-ibm-z/docs/wiki/Building-Python-3.6.x) or install through some [additional repo](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/).</span></span> <span data-ttu-id="d8fe7-119">Anschließend können Sie das Paket herunterladen und ohne Abhängigkeit installieren.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-119">Then you can download the package and install it without dependency.</span></span>
```bash
$ sudo yum install yum-utils
$ sudo yumdownloader azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

<span data-ttu-id="d8fe7-120">Wenn Sie python3 eingerichtet haben, aber weiterhin den Fehler `python3: command not found` erhalten, wenn Sie versuchen, die CLI auszuführen, müssen Sie sie dem Pfad hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-120">If you have setup python3 but are still getting an error `python3: command not found` when trying to run the cli, you need to add it to your path.</span></span>
```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="d8fe7-121">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-121">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="d8fe7-122">Konfigurieren Sie `yum` explizit so, dass dieser Proxy immer verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-122">You may also want to explicitly configure `yum` to use this proxy at all times.</span></span> <span data-ttu-id="d8fe7-123">Stellen Sie sicher, dass die folgenden Zeilen im Abschnitt `[main]` von `/etc/yum.conf` erscheinen:</span><span class="sxs-lookup"><span data-stu-id="d8fe7-123">Make sure that the following lines appear under the `[main]` section of `/etc/yum.conf`:</span></span>

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

<span data-ttu-id="d8fe7-124">Zum Abrufen des Microsoft-Signaturschlüssels und des Pakets von unserem Repository muss Ihr Proxy HTTPS-Verbindungen mit der folgenden Adresse zulassen:</span><span class="sxs-lookup"><span data-stu-id="d8fe7-124">In order to get the Microsoft signing key and get the package from our repository, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a><span data-ttu-id="d8fe7-125">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d8fe7-125">Update</span></span>

[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="d8fe7-126">Sie können die Azure CLI auch mit dem Befehl `yum update` aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-126">You can also update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="d8fe7-127">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="d8fe7-127">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="d8fe7-128">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-128">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="d8fe7-129">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-129">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="d8fe7-130">Wenn Sie keine anderen Microsoft-Pakete verwenden, entfernen Sie den Signaturschlüssel.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-130">If you don't use any other Microsoft packages, remove the signing key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="d8fe7-131">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="d8fe7-131">Next Steps</span></span>

<span data-ttu-id="d8fe7-132">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="d8fe7-132">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="d8fe7-133">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="d8fe7-133">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)
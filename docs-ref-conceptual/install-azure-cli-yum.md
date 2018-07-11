---
title: Installieren der Azure CLI 2.0 unter Linux mit yum
description: Installieren der Azure CLI 2.0 mit yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7729077d9240f09e0ad93ad8ab154d1477d8c3fd
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439889"
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="fb77a-103">Installieren der Azure CLI 2.0 mit yum</span><span class="sxs-lookup"><span data-stu-id="fb77a-103">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="fb77a-104">Wenn Sie eine Distribution mit `yum` verwenden (etwa RHEL, Fedora oder CentOS), steht ein Paket für die Azure CLI zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="fb77a-104">If you are running a distribution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="fb77a-105">Dieses Paket wurde mit RHEL 7, Fedora 19 (und höher) und CentOS 7 getestet.</span><span class="sxs-lookup"><span data-stu-id="fb77a-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="fb77a-106">Installieren</span><span class="sxs-lookup"><span data-stu-id="fb77a-106">Install</span></span>

1. <span data-ttu-id="fb77a-107">Importieren Sie den Microsoft-Repositoryschlüssel.</span><span class="sxs-lookup"><span data-stu-id="fb77a-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="fb77a-108">Erstellen Sie lokale `azure-cli`-Repositoryinformationen.</span><span class="sxs-lookup"><span data-stu-id="fb77a-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="fb77a-109">Installieren Sie mit dem Befehl `yum install`.</span><span class="sxs-lookup"><span data-stu-id="fb77a-109">Install with the `yum install` command.</span></span> 

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="fb77a-110">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="fb77a-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="fb77a-111">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="fb77a-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="fb77a-112">Weitere Informationen zu verschiedenen Anmeldemethoden finden Sie unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="fb77a-112">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="fb77a-113">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="fb77a-113">Update</span></span>

<span data-ttu-id="fb77a-114">Aktualisieren Sie die Azure CLI mit dem Befehl `yum update`.</span><span class="sxs-lookup"><span data-stu-id="fb77a-114">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="fb77a-115">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="fb77a-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="fb77a-116">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="fb77a-116">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="fb77a-117">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="fb77a-117">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="fb77a-118">Entfernen Sie auch den Microsoft GPG-Signaturschlüssel, falls Sie die Repositoryinformationen entfernt haben.</span><span class="sxs-lookup"><span data-stu-id="fb77a-118">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

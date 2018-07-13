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
ms.openlocfilehash: 03276af8fc9640b6c74f7417ecdaecfe48762782
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967519"
---
# <a name="install-azure-cli-20-with-yum"></a><span data-ttu-id="d3ed9-103">Installieren der Azure CLI 2.0 mit yum</span><span class="sxs-lookup"><span data-stu-id="d3ed9-103">Install Azure CLI 2.0 with yum</span></span>

<span data-ttu-id="d3ed9-104">Wenn Sie eine Distribution mit `yum` verwenden (etwa RHEL, Fedora oder CentOS), steht ein Paket für die Azure CLI zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="d3ed9-104">If you are running a distribution that comes with `yum`, such as RHEL, Fedora, or CentOS, there is a package available for the Azure CLI.</span></span> <span data-ttu-id="d3ed9-105">Dieses Paket wurde mit RHEL 7, Fedora 19 (und höher) und CentOS 7 getestet.</span><span class="sxs-lookup"><span data-stu-id="d3ed9-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="d3ed9-106">Installieren</span><span class="sxs-lookup"><span data-stu-id="d3ed9-106">Install</span></span>

1. <span data-ttu-id="d3ed9-107">Importieren Sie den Microsoft-Repositoryschlüssel.</span><span class="sxs-lookup"><span data-stu-id="d3ed9-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="d3ed9-108">Erstellen Sie lokale `azure-cli`-Repositoryinformationen.</span><span class="sxs-lookup"><span data-stu-id="d3ed9-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="d3ed9-109">Installieren Sie mit dem Befehl `yum install`.</span><span class="sxs-lookup"><span data-stu-id="d3ed9-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="d3ed9-110">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="d3ed9-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="d3ed9-111">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="d3ed9-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="d3ed9-112">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d3ed9-112">To learn more about different authentication methods, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="d3ed9-113">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d3ed9-113">Update</span></span>

<span data-ttu-id="d3ed9-114">Aktualisieren Sie die Azure CLI mit dem Befehl `yum update`.</span><span class="sxs-lookup"><span data-stu-id="d3ed9-114">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="d3ed9-115">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="d3ed9-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="d3ed9-116">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="d3ed9-116">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="d3ed9-117">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="d3ed9-117">If you do not plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="d3ed9-118">Entfernen Sie auch den Microsoft GPG-Signaturschlüssel, falls Sie die Repositoryinformationen entfernt haben.</span><span class="sxs-lookup"><span data-stu-id="d3ed9-118">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

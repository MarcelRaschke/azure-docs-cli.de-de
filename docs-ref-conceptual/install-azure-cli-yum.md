---
title: Installieren der Azure CLI unter Linux mit yum
description: Installieren der Azure CLI mit yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 3747f276a30740602271477e154322cad45f190e
ms.sourcegitcommit: 6d9169ed547df151f99e5a3ac86578634486419a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/23/2018
ms.locfileid: "49652463"
---
# <a name="install-azure-cli-with-yum"></a><span data-ttu-id="b4d2e-103">Installieren der Azure CLI mit yum</span><span class="sxs-lookup"><span data-stu-id="b4d2e-103">Install Azure CLI with yum</span></span>

<span data-ttu-id="b4d2e-104">Für Linux-Distributionen mit `yum` (etwa RHEL, Fedora oder CentOS) ist ein Paket für die Azure CLI verfügbar.</span><span class="sxs-lookup"><span data-stu-id="b4d2e-104">For Linux distributions with  `yum` such as RHEL, Fedora, or CentOS, there's a package for the Azure CLI.</span></span> <span data-ttu-id="b4d2e-105">Dieses Paket wurde mit RHEL 7, Fedora 19 (und höher) und CentOS 7 getestet.</span><span class="sxs-lookup"><span data-stu-id="b4d2e-105">This package has been tested with RHEL 7, Fedora 19 and higher, and CentOS 7.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="b4d2e-106">Installieren</span><span class="sxs-lookup"><span data-stu-id="b4d2e-106">Install</span></span>

1. <span data-ttu-id="b4d2e-107">Importieren Sie den Microsoft-Repositoryschlüssel.</span><span class="sxs-lookup"><span data-stu-id="b4d2e-107">Import the Microsoft repository key.</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="b4d2e-108">Erstellen Sie lokale `azure-cli`-Repositoryinformationen.</span><span class="sxs-lookup"><span data-stu-id="b4d2e-108">Create local `azure-cli` repository information.</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="b4d2e-109">Installieren Sie mit dem Befehl `yum install`.</span><span class="sxs-lookup"><span data-stu-id="b4d2e-109">Install with the `yum install` command.</span></span>

   ```bash
   sudo yum install azure-cli
   ```

<span data-ttu-id="b4d2e-110">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="b4d2e-110">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="b4d2e-111">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="b4d2e-111">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="b4d2e-112">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="b4d2e-112">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="update"></a><span data-ttu-id="b4d2e-113">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b4d2e-113">Update</span></span>

<span data-ttu-id="b4d2e-114">Aktualisieren Sie die Azure CLI mit dem Befehl `yum update`.</span><span class="sxs-lookup"><span data-stu-id="b4d2e-114">Update the Azure CLI with the `yum update` command.</span></span>

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="b4d2e-115">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="b4d2e-115">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="b4d2e-116">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="b4d2e-116">Remove the package from your system.</span></span>

   ```bash
   sudo yum remove azure-cli
   ```

2. <span data-ttu-id="b4d2e-117">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="b4d2e-117">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. <span data-ttu-id="b4d2e-118">Entfernen Sie auch den Microsoft GPG-Signaturschlüssel, falls Sie die Repositoryinformationen entfernt haben.</span><span class="sxs-lookup"><span data-stu-id="b4d2e-118">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a><span data-ttu-id="b4d2e-119">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="b4d2e-119">Next Steps</span></span>

<span data-ttu-id="b4d2e-120">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="b4d2e-120">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="b4d2e-121">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="b4d2e-121">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

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
ms.devlang: azure-cli
ms.openlocfilehash: bb60b807df29833a74b1dab4def6f5ced58c8ffe
ms.sourcegitcommit: a8aac038e6ede0b1b352ca6163a04b61ff4eed5b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/28/2018
ms.locfileid: "52450274"
---
# <a name="install-azure-cli-with-zypper"></a><span data-ttu-id="f0b83-103">Installieren der Azure CLI mit zypper</span><span class="sxs-lookup"><span data-stu-id="f0b83-103">Install Azure CLI with zypper</span></span>

<span data-ttu-id="f0b83-104">Für Linux-Distributionen mit `zypper` wie openSUSE oder SLES ist ein Paket für die Azure CLI verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f0b83-104">For Linux distributions with `zypper`, such as openSUSE or SLES, there's a package available for the Azure CLI.</span></span> <span data-ttu-id="f0b83-105">Dieses Paket wurde mit openSUSE 42.2 und SLES 12 SP 2 getestet.</span><span class="sxs-lookup"><span data-stu-id="f0b83-105">This package has been tested with openSUSE 42.2 and SLES 12 SP 2.</span></span>

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a><span data-ttu-id="f0b83-106">Installieren</span><span class="sxs-lookup"><span data-stu-id="f0b83-106">Install</span></span>

1. <span data-ttu-id="f0b83-107">Installieren Sie `curl`:</span><span class="sxs-lookup"><span data-stu-id="f0b83-107">Install `curl`:</span></span>

   ```bash
   sudo zypper install -y curl
   ```

2. <span data-ttu-id="f0b83-108">Importieren Sie den Microsoft-Repositoryschlüssel:</span><span class="sxs-lookup"><span data-stu-id="f0b83-108">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. <span data-ttu-id="f0b83-109">Erstellen Sie lokale `azure-cli`-Repositoryinformationen:</span><span class="sxs-lookup"><span data-stu-id="f0b83-109">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. <span data-ttu-id="f0b83-110">Aktualisieren Sie den `zypper`-Paketindex, und führen Sie die Installation durch:</span><span class="sxs-lookup"><span data-stu-id="f0b83-110">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

<span data-ttu-id="f0b83-111">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="f0b83-111">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="f0b83-112">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="f0b83-112">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="f0b83-113">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="f0b83-113">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="f0b83-114">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="f0b83-114">Troubleshooting</span></span>

<span data-ttu-id="f0b83-115">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `zypper` auftreten können.</span><span class="sxs-lookup"><span data-stu-id="f0b83-115">Here are some common problems seen when installing with `zypper`.</span></span> <span data-ttu-id="f0b83-116">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="f0b83-116">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]


## <a name="update"></a><span data-ttu-id="f0b83-117">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f0b83-117">Update</span></span>

<span data-ttu-id="f0b83-118">Sie können das Paket mit dem Befehl `zypper update` aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="f0b83-118">You can update the package with the `zypper update` command.</span></span>

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a><span data-ttu-id="f0b83-119">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="f0b83-119">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. <span data-ttu-id="f0b83-120">Entfernen Sie das Paket aus Ihrem System.</span><span class="sxs-lookup"><span data-stu-id="f0b83-120">Remove the package from your system.</span></span>

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. <span data-ttu-id="f0b83-121">Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.</span><span class="sxs-lookup"><span data-stu-id="f0b83-121">If you don't plan to reinstall the CLI, remove the repository information.</span></span>

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. <span data-ttu-id="f0b83-122">Entfernen Sie auch den Microsoft GPG-Signaturschlüssel, falls Sie die Repositoryinformationen entfernt haben.</span><span class="sxs-lookup"><span data-stu-id="f0b83-122">If you removed the repository information, also remove the Microsoft GPG signature key.</span></span>

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
   ## <a name="next-steps"></a><span data-ttu-id="f0b83-123">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="f0b83-123">Next Steps</span></span>

<span data-ttu-id="f0b83-124">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="f0b83-124">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="f0b83-125">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="f0b83-125">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

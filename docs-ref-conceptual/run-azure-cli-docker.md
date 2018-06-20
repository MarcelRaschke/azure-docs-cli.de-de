---
title: Ausführen der Azure CLI 2.0 in einem Docker-Container
description: Ausführen eines Docker-Containers, der die Azure CLI 2.0 hostet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: d88dbcec947372aa154bce939edd99f65cd9480f
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2018
ms.locfileid: "32043719"
---
# <a name="run-azure-cli-20-in-a-docker-container"></a><span data-ttu-id="9dd8b-103">Ausführen der Azure CLI 2.0 in einem Docker-Container</span><span class="sxs-lookup"><span data-stu-id="9dd8b-103">Run Azure CLI 2.0 in a Docker container</span></span>

<span data-ttu-id="9dd8b-104">Mit Docker können Sie einen eigenständigen Linux-Container mit vorinstallierter Azure CLI 2.0 verwenden.</span><span class="sxs-lookup"><span data-stu-id="9dd8b-104">You can use Docker to run a standalone Linux container with the Azure CLI 2.0 pre-installed.</span></span> <span data-ttu-id="9dd8b-105">Docker ermöglicht einen schnellen Einstieg in eine Umgebung, in der Sie die CLI ausprobieren und somit testen können, ob sie für Sie geeignet ist. Eine Verwendung als Basisimage für Ihre eigene Bereitstellung ist ebenfalls möglich.</span><span class="sxs-lookup"><span data-stu-id="9dd8b-105">Docker lets you get started quickly with an environment where you can try out the CLI to decide if it's right for you, or use our image as a base for your own deployment.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="9dd8b-106">Ausführen in einem Docker-Container</span><span class="sxs-lookup"><span data-stu-id="9dd8b-106">Run in a Docker container</span></span>

<span data-ttu-id="9dd8b-107">Installieren Sie die CLI mit `docker run`.</span><span class="sxs-lookup"><span data-stu-id="9dd8b-107">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

<span data-ttu-id="9dd8b-108">Die CLI wird in dem Image als Befehl `az` in `/usr/local/bin` installiert.</span><span class="sxs-lookup"><span data-stu-id="9dd8b-108">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="9dd8b-109">Führen Sie den Befehl `az login` aus, um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="9dd8b-109">To log in, run the `az login` command.</span></span>

```azurecli
az login
```

<span data-ttu-id="9dd8b-110">Weitere Informationen zu verschiedenen Anmeldemethoden finden Sie unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="9dd8b-110">To learn more about different login methods, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="9dd8b-111">Wenn Sie die SSH-Schlüssel aus Ihrer Benutzerumgebung übernehmen möchten, können Sie `-v ${HOME}:/root` verwenden, um $HOME als `/root` bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="9dd8b-111">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

## <a name="update-docker-image"></a><span data-ttu-id="9dd8b-112">Aktualisieren des Docker-Images</span><span class="sxs-lookup"><span data-stu-id="9dd8b-112">Update Docker image</span></span>

<span data-ttu-id="9dd8b-113">Für die Aktualisierung mit Docker ist das Abrufen des neuen Images per Pull und das Neuerstellen vorhandener Container erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9dd8b-113">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="9dd8b-114">Aus diesem Grund sollten Sie die Verwendung eines Containers vermeiden, der die CLI als Datenspeicher hostet.</span><span class="sxs-lookup"><span data-stu-id="9dd8b-114">For this reason you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="9dd8b-115">Aktualisieren Sie Ihr lokales Image mit `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="9dd8b-115">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="9dd8b-116">Deinstallieren des Docker-Images</span><span class="sxs-lookup"><span data-stu-id="9dd8b-116">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="9dd8b-117">Entfernen Sie das CLI-Image, nachdem Sie alle Container angehalten haben, die das CLI-Image ausführen.</span><span class="sxs-lookup"><span data-stu-id="9dd8b-117">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```

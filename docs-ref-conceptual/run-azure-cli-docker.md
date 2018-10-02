---
title: Ausführen der Azure CLI in einem Docker-Container
description: Ausführen eines Docker-Containers, der die Azure CLI hostet
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 40e6865ce07b6ccb8e84a2666f0bcd6df3b5cfcf
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177758"
---
# <a name="run-azure-cli-in-a-docker-container"></a><span data-ttu-id="486cc-103">Ausführen der Azure CLI in einem Docker-Container</span><span class="sxs-lookup"><span data-stu-id="486cc-103">Run Azure CLI in a Docker container</span></span>

<span data-ttu-id="486cc-104">Mit Docker können Sie einen eigenständigen Linux-Container mit vorinstallierter Azure CLI verwenden.</span><span class="sxs-lookup"><span data-stu-id="486cc-104">You can use Docker to run a standalone Linux container with the Azure CLI pre-installed.</span></span> <span data-ttu-id="486cc-105">Docker ermöglicht Ihnen einen schnellen Einstieg mit einer isolierten Umgebung für die Ausführung der CLI.</span><span class="sxs-lookup"><span data-stu-id="486cc-105">Docker gets you started quickly with an isolated environment to run the CLI in.</span></span> <span data-ttu-id="486cc-106">Das Image kann auch als Grundlage für eigene Bereitstellungen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="486cc-106">The image can also be used as a base for your own deployments.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="486cc-107">Ausführen in einem Docker-Container</span><span class="sxs-lookup"><span data-stu-id="486cc-107">Run in a Docker container</span></span>

<span data-ttu-id="486cc-108">Installieren Sie die CLI mit `docker run`.</span><span class="sxs-lookup"><span data-stu-id="486cc-108">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="486cc-109">Wenn Sie die SSH-Schlüssel aus Ihrer Benutzerumgebung übernehmen möchten, verwenden Sie `-v ${HOME}/.ssh:/root/.ssh`, um Ihre SSH-Schlüssel in der Umgebung bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="486cc-109">If you want to pick up the SSH keys from your user environment, use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

<span data-ttu-id="486cc-110">Die CLI wird in dem Image als Befehl `az` in `/usr/local/bin` installiert.</span><span class="sxs-lookup"><span data-stu-id="486cc-110">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="486cc-111">Führen Sie den Befehl [az login](/cli/azure/reference-index#az-login) aus, um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="486cc-111">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="486cc-112">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="486cc-112">To learn more about different authentication methods, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="486cc-113">Aktualisieren des Docker-Images</span><span class="sxs-lookup"><span data-stu-id="486cc-113">Update Docker image</span></span>

<span data-ttu-id="486cc-114">Für die Aktualisierung mit Docker ist das Abrufen des neuen Images per Pull und das Neuerstellen vorhandener Container erforderlich.</span><span class="sxs-lookup"><span data-stu-id="486cc-114">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="486cc-115">Aus diesem Grund sollten Sie die Verwendung eines Containers vermeiden, der die CLI als Datenspeicher hostet.</span><span class="sxs-lookup"><span data-stu-id="486cc-115">For this reason, you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="486cc-116">Aktualisieren Sie Ihr lokales Image mit `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="486cc-116">Update your local image with `docker pull`.</span></span>

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="486cc-117">Deinstallieren des Docker-Images</span><span class="sxs-lookup"><span data-stu-id="486cc-117">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="486cc-118">Entfernen Sie das CLI-Image, nachdem Sie alle Container angehalten haben, die das CLI-Image ausführen.</span><span class="sxs-lookup"><span data-stu-id="486cc-118">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi microsoft/azure-cli
```

## <a name="next-steps"></a><span data-ttu-id="486cc-119">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="486cc-119">Next Steps</span></span>

<span data-ttu-id="486cc-120">Die Azure-Befehlszeilenschnittstelle ist nun verwendungsbereit. Machen Sie sich kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="486cc-120">Now that you're ready to use the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="486cc-121">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="486cc-121">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

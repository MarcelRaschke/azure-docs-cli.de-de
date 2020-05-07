---
title: Ausführen der Azure CLI in einem Docker-Container
description: Ausführen eines Docker-Containers, der die Azure CLI hostet
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/29/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 96a2bcf311cb504b08d44da3ea6033dbad9034b8
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2020
ms.locfileid: "77780042"
---
# <a name="run-azure-cli-in-a-docker-container"></a><span data-ttu-id="7dc14-103">Ausführen der Azure CLI in einem Docker-Container</span><span class="sxs-lookup"><span data-stu-id="7dc14-103">Run Azure CLI in a Docker container</span></span>

<span data-ttu-id="7dc14-104">Mit Docker können Sie einen eigenständigen Linux-Container mit vorinstallierter Azure CLI verwenden.</span><span class="sxs-lookup"><span data-stu-id="7dc14-104">You can use Docker to run a standalone Linux container with the Azure CLI pre-installed.</span></span> <span data-ttu-id="7dc14-105">Docker ermöglicht Ihnen einen schnellen Einstieg mit einer isolierten Umgebung für die Ausführung der CLI.</span><span class="sxs-lookup"><span data-stu-id="7dc14-105">Docker gets you started quickly with an isolated environment to run the CLI in.</span></span> <span data-ttu-id="7dc14-106">Das Image kann auch als Grundlage für eigene Bereitstellungen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="7dc14-106">The image can also be used as a base for your own deployments.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="7dc14-107">Ausführen in einem Docker-Container</span><span class="sxs-lookup"><span data-stu-id="7dc14-107">Run in a Docker container</span></span>

> [!NOTE]
> <span data-ttu-id="7dc14-108">Die Azure CLI wurde zur [Microsoft-Containerregistrierung](https://azure.microsoft.com/services/container-registry) migriert.</span><span class="sxs-lookup"><span data-stu-id="7dc14-108">The Azure CLI has migrated to [Microsoft Container Registry](https://azure.microsoft.com/services/container-registry).</span></span> <span data-ttu-id="7dc14-109">Vorhandene Tags in Docker Hub werden weiterhin unterstützt, neue Releases werden jedoch nur als „mcr.microsoft.com/azure-cli“ verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="7dc14-109">Existing tags on Docker Hub are still supported, but new releases will only be available as mcr.microsoft.com/azure-cli.</span></span>

<span data-ttu-id="7dc14-110">Installieren Sie die CLI mit `docker run`.</span><span class="sxs-lookup"><span data-stu-id="7dc14-110">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run -it mcr.microsoft.com/azure-cli
   ```

> [!NOTE]
> <span data-ttu-id="7dc14-111">Wenn Sie die SSH-Schlüssel aus Ihrer Benutzerumgebung übernehmen möchten, verwenden Sie `-v ${HOME}/.ssh:/root/.ssh`, um Ihre SSH-Schlüssel in der Umgebung bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="7dc14-111">If you want to pick up the SSH keys from your user environment, use `-v ${HOME}/.ssh:/root/.ssh` to mount your SSH keys in the environment.</span></span>
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh mcr.microsoft.com/azure-cli
> ```

<span data-ttu-id="7dc14-112">Die CLI wird in dem Image als Befehl `az` in `/usr/local/bin` installiert.</span><span class="sxs-lookup"><span data-stu-id="7dc14-112">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span> <span data-ttu-id="7dc14-113">Führen Sie den Befehl [az login](/cli/azure/reference-index#az-login) aus, um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="7dc14-113">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="7dc14-114">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="7dc14-114">To learn more about different authentication methods, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="update-docker-image"></a><span data-ttu-id="7dc14-115">Aktualisieren des Docker-Images</span><span class="sxs-lookup"><span data-stu-id="7dc14-115">Update Docker image</span></span>

<span data-ttu-id="7dc14-116">Für die Aktualisierung mit Docker ist das Abrufen des neuen Images per Pull und das Neuerstellen vorhandener Container erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7dc14-116">Updating with Docker requires both pulling the new image and re-creating any existing containers.</span></span> <span data-ttu-id="7dc14-117">Aus diesem Grund sollten Sie die Verwendung eines Containers vermeiden, der die CLI als Datenspeicher hostet.</span><span class="sxs-lookup"><span data-stu-id="7dc14-117">For this reason, you should try to avoid using a container that hosts the CLI as a data store.</span></span>

<span data-ttu-id="7dc14-118">Aktualisieren Sie Ihr lokales Image mit `docker pull`.</span><span class="sxs-lookup"><span data-stu-id="7dc14-118">Update your local image with `docker pull`.</span></span>

```bash
docker pull mcr.microsoft.com/azure-cli
```

## <a name="uninstall-docker-image"></a><span data-ttu-id="7dc14-119">Deinstallieren des Docker-Images</span><span class="sxs-lookup"><span data-stu-id="7dc14-119">Uninstall Docker image</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="7dc14-120">Entfernen Sie das CLI-Image, nachdem Sie alle Container angehalten haben, die das CLI-Image ausführen.</span><span class="sxs-lookup"><span data-stu-id="7dc14-120">After halting any containers running the CLI image, remove it.</span></span>

```bash
docker rmi mcr.microsoft.com/azure-cli
```

## <a name="next-steps"></a><span data-ttu-id="7dc14-121">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="7dc14-121">Next Steps</span></span>

<span data-ttu-id="7dc14-122">Die Azure-Befehlszeilenschnittstelle ist nun verwendungsbereit. Machen Sie sich kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="7dc14-122">Now that you're ready to use the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="7dc14-123">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="7dc14-123">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

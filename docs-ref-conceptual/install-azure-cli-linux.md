---
title: Manuelles Installieren der Azure CLI für Linux
description: Manuelles Installieren der Azure CLI unter Linux
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 12/15/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
zone_pivot_group_filename: azure/zone-pivot-groups.json
zone_pivot_groups: cli-linux-installation-method
ms.openlocfilehash: 03c7e7e4915f48dce70d2bc2cab16b4688f8b5fd
ms.sourcegitcommit: 594e9c620a6f74f5eaedf91a7f6a791e03a64c74
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/17/2021
ms.locfileid: "100631005"
---
# <a name="install-the-azure-cli-on-linux"></a><span data-ttu-id="19163-103">Installieren der Azure CLI unter Linux</span><span class="sxs-lookup"><span data-stu-id="19163-103">Install the Azure CLI on Linux</span></span>

<span data-ttu-id="19163-104">Es wird empfohlen, die Azure-Befehlszeilenschnittstelle (Azure CLI) über den Paket-Manager Ihrer Linux-Distribution zu installieren.</span><span class="sxs-lookup"><span data-stu-id="19163-104">It is recommended to install the Azure CLI using your Linux distribution's package manager.</span></span> <span data-ttu-id="19163-105">Wählen Sie den entsprechenden Paket-Manager für Ihre Distribution aus den obigen Optionen aus.</span><span class="sxs-lookup"><span data-stu-id="19163-105">Select the appropriate package manager for your distribution from the options above.</span></span>  <span data-ttu-id="19163-106">Wenn Sie nicht über einen der aufgelisteten Paket-Manager verfügen, können Sie die Azure CLI manuell installieren, indem Sie die Option *Installationsskript* auswählen.</span><span class="sxs-lookup"><span data-stu-id="19163-106">If you do not have one of the listed package managers, you may manually install the Azure CLI by selecting the *Install script* option.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

::: zone pivot="apt"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-apt.md)]

::: zone-end

::: zone pivot="dnf"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-dnf.md)]

::: zone-end

::: zone pivot="zypper"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-zypper.md)]

::: zone-end

::: zone pivot="script"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-script.md)]

::: zone-end

## <a name="next-steps"></a><span data-ttu-id="19163-107">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="19163-107">Next Steps</span></span>

<span data-ttu-id="19163-108">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="19163-108">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="19163-109">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="19163-109">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

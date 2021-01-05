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
ms.openlocfilehash: 3b6a3c9faa8424189bb5d4ffaeb17bdfc7de0d6d
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744658"
---
# <a name="install-the-azure-cli-on-linux"></a>Installieren der Azure CLI unter Linux

Es wird empfohlen, die Azure-Befehlszeilenschnittstelle (Azure CLI) über den Paket-Manager Ihrer Linux-Distribution zu installieren. Wählen Sie den entsprechenden Paket-Manager für Ihre Distribution aus den obigen Optionen aus.  Wenn Sie nicht über einen der aufgelisteten Paket-Manager verfügen, können Sie die Azure CLI manuell installieren, indem Sie die Option *Installationsskript* auswählen.

[!INCLUDE [current-version](includes/current-version.md)]

::: zone pivot="apt"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-apt.md)]

::: zone-end

::: zone pivot="yum"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-yum.md)]

::: zone-end

::: zone pivot="zypper"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-zypper.md)]

::: zone-end

::: zone pivot="script"

[!INCLUDE [cli-install-linux-apt](includes/cli-install-linux-script.md)]

::: zone-end

## <a name="next-steps"></a>Nächste Schritte

Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)
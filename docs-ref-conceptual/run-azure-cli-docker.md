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
ms.custom: devx-track-azurecli
ms.openlocfilehash: e75832866e63fb5315856d1b186ca9f1edf50afc
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2021
ms.locfileid: "105582123"
---
# <a name="run-azure-cli-in-a-docker-container"></a>Ausführen der Azure CLI in einem Docker-Container

Mit Docker können Sie einen eigenständigen Linux-Container mit vorinstallierter Azure CLI verwenden. Docker ermöglicht Ihnen einen schnellen Einstieg mit einer isolierten Umgebung für die Ausführung der CLI. Das Image kann auch als Grundlage für eigene Bereitstellungen verwendet werden.

## <a name="run-in-a-docker-container"></a>Ausführen in einem Docker-Container

> [!NOTE]
> Die Azure CLI wurde zur [Microsoft-Containerregistrierung](https://azure.microsoft.com/services/container-registry) migriert. Vorhandene Tags in Docker Hub werden weiterhin unterstützt, neue Releases werden jedoch nur als „mcr.microsoft.com/azure-cli“ verfügbar sein.

Installieren Sie die CLI mit `docker run`.

   ```bash
   docker run -it mcr.microsoft.com/azure-cli
   ```

> [!NOTE]
> Wenn Sie die SSH-Schlüssel aus Ihrer Benutzerumgebung übernehmen möchten, verwenden Sie `-v ${HOME}/.ssh:/root/.ssh`, um Ihre SSH-Schlüssel in der Umgebung bereitzustellen.
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh mcr.microsoft.com/azure-cli
> ```

Die CLI wird in dem Image als Befehl `az` in `/usr/local/bin` installiert. Führen Sie den Befehl [az login](/cli/azure/reference-index#az_login) aus, um sich anzumelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).

## <a name="update-docker-image"></a>Aktualisieren des Docker-Images

Für die Aktualisierung mit Docker ist das Abrufen des neuen Images per Pull und das Neuerstellen vorhandener Container erforderlich. Aus diesem Grund sollten Sie die Verwendung eines Containers vermeiden, der die CLI als Datenspeicher hostet.

Aktualisieren Sie Ihr lokales Image mit `docker pull`.

```bash
docker pull mcr.microsoft.com/azure-cli
```

## <a name="uninstall-docker-image"></a>Deinstallieren des Docker-Images

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Entfernen Sie das CLI-Image, nachdem Sie alle Container angehalten haben, die das CLI-Image ausführen.

```bash
docker rmi mcr.microsoft.com/azure-cli
```

## <a name="next-steps"></a>Nächste Schritte

Die Azure-Befehlszeilenschnittstelle ist nun verwendungsbereit. Machen Sie sich kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)
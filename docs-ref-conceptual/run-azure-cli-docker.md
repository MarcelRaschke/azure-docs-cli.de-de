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
ms.openlocfilehash: f22962717ec6a623dd69a266f660b67f2523b204
ms.sourcegitcommit: d93b0a2bcfb0d164ef90d6d4618f0552609a8ea6
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/20/2018
ms.locfileid: "46470030"
---
# <a name="run-azure-cli-20-in-a-docker-container"></a>Ausführen der Azure CLI 2.0 in einem Docker-Container

Mit Docker können Sie einen eigenständigen Linux-Container mit vorinstallierter Azure CLI 2.0 verwenden. Docker ermöglicht Ihnen einen schnellen Einstieg mit einer isolierten Umgebung für die Ausführung der CLI. Das Image kann auch als Grundlage für eigene Bereitstellungen verwendet werden.

## <a name="run-in-a-docker-container"></a>Ausführen in einem Docker-Container

Installieren Sie die CLI mit `docker run`.

   ```bash
   docker run -it microsoft/azure-cli
   ```

> [!NOTE]
> Wenn Sie die SSH-Schlüssel aus Ihrer Benutzerumgebung übernehmen möchten, verwenden Sie `-v ${HOME}/.ssh:/root/.ssh`, um Ihre SSH-Schlüssel in der Umgebung bereitzustellen.
>
> ```bash
> docker run -it -v ${HOME}/.ssh:/root/.ssh microsoft/azure-cli
> ```

Die CLI wird in dem Image als Befehl `az` in `/usr/local/bin` installiert. Führen Sie den Befehl [az login](/cli/azure/reference-index#az-login) aus, um sich anzumelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="update-docker-image"></a>Aktualisieren des Docker-Images

Für die Aktualisierung mit Docker ist das Abrufen des neuen Images per Pull und das Neuerstellen vorhandener Container erforderlich. Aus diesem Grund sollten Sie die Verwendung eines Containers vermeiden, der die CLI als Datenspeicher hostet.

Aktualisieren Sie Ihr lokales Image mit `docker pull`.

```bash
docker pull microsoft/azure-cli
```

## <a name="uninstall-docker-image"></a>Deinstallieren des Docker-Images

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Entfernen Sie das CLI-Image, nachdem Sie alle Container angehalten haben, die das CLI-Image ausführen.

```bash
docker rmi microsoft/azure-cli
```

## <a name="next-steps"></a>Nächste Schritte

Die Azure-Befehlszeilenschnittstelle ist nun verwendungsbereit. Machen Sie sich kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)

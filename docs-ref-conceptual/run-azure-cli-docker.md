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
# <a name="run-azure-cli-20-in-a-docker-container"></a>Ausführen der Azure CLI 2.0 in einem Docker-Container

Mit Docker können Sie einen eigenständigen Linux-Container mit vorinstallierter Azure CLI 2.0 verwenden. Docker ermöglicht einen schnellen Einstieg in eine Umgebung, in der Sie die CLI ausprobieren und somit testen können, ob sie für Sie geeignet ist. Eine Verwendung als Basisimage für Ihre eigene Bereitstellung ist ebenfalls möglich.

## <a name="run-in-a-docker-container"></a>Ausführen in einem Docker-Container

Installieren Sie die CLI mit `docker run`.

   ```bash
   docker run -it microsoft/azure-cli
   ```

Die CLI wird in dem Image als Befehl `az` in `/usr/local/bin` installiert. Führen Sie den Befehl `az login` aus, um sich anzumelden.

```azurecli
az login
```

Weitere Informationen zu verschiedenen Anmeldemethoden finden Sie unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md).

> [!NOTE]
> Wenn Sie die SSH-Schlüssel aus Ihrer Benutzerumgebung übernehmen möchten, können Sie `-v ${HOME}:/root` verwenden, um $HOME als `/root` bereitzustellen.

> ```bash
> docker run -it -v ${HOME}:/root microsoft/azure-cli
> ```

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

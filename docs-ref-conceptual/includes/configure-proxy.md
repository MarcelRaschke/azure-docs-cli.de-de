---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/28/2019
ms.topic: include
ms.prod: azure
ms.technology: azure-cli
ms.openlocfilehash: 676f33377a4e7122941bc789c51465b7f34aa1d3
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516265"
---
Wenn Sie aufgrund eines Proxys keine Verbindung mit einer externen Ressource herstellen können, stellen Sie sicher, dass Sie die Variablen `HTTP_PROXY` und `HTTPS_PROXY` in Ihrer Shell korrekt festgelegt haben. Wenden Sie sich an den Systemadministrator, um Informationen dazu zu erhalten, welche Hosts und Ports für diese Proxys verwendet werden müssen.

Diese Werte gelten für viele Linux-Programme, u. a. die Programme, die beim Installationsvorgang verwendet werden. Diese Werte legen Sie wie folgt fest:

```bash
# No auth
export HTTP_PROXY=http://[proxy]:[port]
export HTTPS_PROXY=https://[proxy]:[port]

# Basic auth
export HTTP_PROXY=http://[username]:[password]@[proxy]:[port]
export HTTPS_PROXY=https://[username]:[password]@[proxy]:[port]
```

> [!IMPORTANT]
> Wenn Sie sich hinter einem Proxy befinden, müssen diese Shellvariablen so festgelegt sein, dass sie mit der CLI eine Verbindung mit Azure-Diensten herstellen.
> Wenn Sie nicht die Standardauthentifizierung verwenden, wird empfohlen, dass Sie diese Variablen in Ihrer Datei vom Typ `.bashrc` exportieren.
> Berücksichtigen Sie dabei immer die Sicherheitsrichtlinien Ihres Unternehmens und die Anforderungen Ihres Systemadministrators.

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
<span data-ttu-id="054a5-101">Wenn Sie aufgrund eines Proxys keine Verbindung mit einer externen Ressource herstellen können, stellen Sie sicher, dass Sie die Variablen `HTTP_PROXY` und `HTTPS_PROXY` in Ihrer Shell korrekt festgelegt haben.</span><span class="sxs-lookup"><span data-stu-id="054a5-101">If you're unable to connect to an external resource due to a proxy, make sure that you've correctly set the `HTTP_PROXY` and `HTTPS_PROXY` variables in your shell.</span></span> <span data-ttu-id="054a5-102">Wenden Sie sich an den Systemadministrator, um Informationen dazu zu erhalten, welche Hosts und Ports für diese Proxys verwendet werden müssen.</span><span class="sxs-lookup"><span data-stu-id="054a5-102">You will need to contact your system administrator to know what host(s) and port(s) to use for these proxies.</span></span>

<span data-ttu-id="054a5-103">Diese Werte gelten für viele Linux-Programme, u. a. die Programme, die beim Installationsvorgang verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="054a5-103">These values are respected by many Linux programs, including those which are used in the install process.</span></span> <span data-ttu-id="054a5-104">Diese Werte legen Sie wie folgt fest:</span><span class="sxs-lookup"><span data-stu-id="054a5-104">To set these values:</span></span>

```bash
# No auth
export HTTP_PROXY=http://[proxy]:[port]
export HTTPS_PROXY=https://[proxy]:[port]

# Basic auth
export HTTP_PROXY=http://[username]:[password]@[proxy]:[port]
export HTTPS_PROXY=https://[username]:[password]@[proxy]:[port]
```

> [!IMPORTANT]
> <span data-ttu-id="054a5-105">Wenn Sie sich hinter einem Proxy befinden, müssen diese Shellvariablen so festgelegt sein, dass sie mit der CLI eine Verbindung mit Azure-Diensten herstellen.</span><span class="sxs-lookup"><span data-stu-id="054a5-105">If you are behind a proxy, these shell variables must be set to connect to Azure services with the CLI.</span></span>
> <span data-ttu-id="054a5-106">Wenn Sie nicht die Standardauthentifizierung verwenden, wird empfohlen, dass Sie diese Variablen in Ihrer Datei vom Typ `.bashrc` exportieren.</span><span class="sxs-lookup"><span data-stu-id="054a5-106">If you are not using basic auth, it's recommended to export these variables in your `.bashrc` file.</span></span>
> <span data-ttu-id="054a5-107">Berücksichtigen Sie dabei immer die Sicherheitsrichtlinien Ihres Unternehmens und die Anforderungen Ihres Systemadministrators.</span><span class="sxs-lookup"><span data-stu-id="054a5-107">Always follow your business' security policies and the requirements of your system administrator.</span></span>

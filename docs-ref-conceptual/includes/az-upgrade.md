---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/25/2020
ms.topic: include
ms.openlocfilehash: b931b465c8d4e7f6a507630a02f9fb7f06579a89
ms.sourcegitcommit: 19c24ebcd1e15ac23ca40ebc28b8c4804bd1327f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/14/2020
ms.locfileid: "92038419"
---
<span data-ttu-id="358ae-101">Die CLI bietet einen internen Befehl zum Aktualisieren auf die aktuelle Version:</span><span class="sxs-lookup"><span data-stu-id="358ae-101">The CLI provides an in-tool command to update to the latest version:</span></span>

```azurecli
az upgrade
```

> [!NOTE]
>
> <span data-ttu-id="358ae-102">Der Befehl `az upgrade` wurde in Version 2.11.0 hinzugefügt und funktioniert nicht mit Versionen vor 2.11.0.</span><span class="sxs-lookup"><span data-stu-id="358ae-102">The `az upgrade` command was added in version 2.11.0 and will not work with versions prior to 2.11.0.</span></span>
>
> <span data-ttu-id="358ae-103">Mit diesem Befehl werden auch alle installierten Erweiterungen standardmäßig aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="358ae-103">This command will also update all installed extensions by default.</span></span> <span data-ttu-id="358ae-104">Weitere `az upgrade`-Optionen finden Sie auf der [Referenzseite für Befehle](/cli/azure/reference-index#az_upgrade).</span><span class="sxs-lookup"><span data-stu-id="358ae-104">For more `az upgrade` options, please refer to the [command reference page](/cli/azure/reference-index#az_upgrade).</span></span>

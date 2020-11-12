---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: include
ms.openlocfilehash: 7aae9e9050306ee834858e528504ae87ff605fa0
ms.sourcegitcommit: 488d53525f1c647ea853d9227d95fdce35b9fb85
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/04/2020
ms.locfileid: "93331008"
---
1. <span data-ttu-id="73280-101">Führen Sie den Befehl `login` aus.</span><span class="sxs-lookup"><span data-stu-id="73280-101">Run the `login` command.</span></span>

    ```azurecli-interactive
    az login
    ```

    <span data-ttu-id="73280-102">Die CLI öffnet Ihren Standardbrowser, sofern sie dazu in der Lage ist, und lädt eine Azure-Anmeldeseite.</span><span class="sxs-lookup"><span data-stu-id="73280-102">If the CLI can open your default browser, it will do so and load an Azure sign-in page.</span></span>

    <span data-ttu-id="73280-103">Öffnen Sie andernfalls die Browserseite [https://aka.ms/devicelogin](https://aka.ms/devicelogin), und geben Sie den in Ihrem Terminal angezeigten Autorisierungscode ein.</span><span class="sxs-lookup"><span data-stu-id="73280-103">Otherwise, open a browser page at [https://aka.ms/devicelogin](https://aka.ms/devicelogin) and enter the  authorization code displayed in your terminal.</span></span>

    <span data-ttu-id="73280-104">Falls kein Webbrowser verfügbar ist oder nicht geöffnet werden kann, verwenden Sie den Gerätecodefluss mit **az login --use-device-code**.</span><span class="sxs-lookup"><span data-stu-id="73280-104">If no web browser is available or the web browser fails to open, use device code flow with **az login --use-device-code**.</span></span>

2. <span data-ttu-id="73280-105">Melden Sie sich im Browser mit Ihren Anmeldeinformationen an.</span><span class="sxs-lookup"><span data-stu-id="73280-105">Sign in with your account credentials in the browser.</span></span>

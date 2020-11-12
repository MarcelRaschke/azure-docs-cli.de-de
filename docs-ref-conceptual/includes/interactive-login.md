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
1. Führen Sie den Befehl `login` aus.

    ```azurecli-interactive
    az login
    ```

    Die CLI öffnet Ihren Standardbrowser, sofern sie dazu in der Lage ist, und lädt eine Azure-Anmeldeseite.

    Öffnen Sie andernfalls die Browserseite [https://aka.ms/devicelogin](https://aka.ms/devicelogin), und geben Sie den in Ihrem Terminal angezeigten Autorisierungscode ein.

    Falls kein Webbrowser verfügbar ist oder nicht geöffnet werden kann, verwenden Sie den Gerätecodefluss mit **az login --use-device-code**.

2. Melden Sie sich im Browser mit Ihren Anmeldeinformationen an.

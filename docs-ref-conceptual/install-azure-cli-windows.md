---
title: Installieren der Azure-Befehlszeilenschnittstelle für Windows
description: Installieren der Azure CLI unter Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: c65cff52211b4c77e32c2992cd71392c8b0e44d6
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177962"
---
# <a name="install-azure-cli-on-windows"></a>Installieren der Azure CLI unter Windows

Unter Windows wird die Azure CLI über eine MSI-Datei installiert. Dadurch können Sie über die Windows-Eingabeaufforderung (CMD) oder über PowerShell auf die CLI zugreifen.
Bei der Installation für ein Windows-Subsystem für Linux (WSL) sind Pakete für Ihre Linux-Distribution verfügbar. Die Liste der unterstützten Paket-Manager bzw. Informationen zur manuellen Installation unter WSL finden Sie auf der [Hauptseite für die Installation](install-azure-cli.md).

## <a name="install-or-update"></a>Installieren oder Aktualisieren

Das verteilbare MSI-Installationsprogramm wird zum Installieren, Aktualisieren und Deinstallieren des `az`-Befehls unter Windows verwendet.

> [!div class="nextstepaction"]
> [MSI-Installationsprogramm herunterladen](https://aka.ms/installazurecliwindows)

Wenn das Installationsprogramm fragt, ob Änderungen am Computer vorgenommen werden dürfen, klicken Sie auf „Ja“.

Sie können nun mit dem Befehl `az` über die Windows-Eingabeaufforderung oder PowerShell die Azure CLI ausführen. In PowerShell stehen einige Features zur Vervollständigung mit der TAB-TASTE zur Verfügung, die an der Windows-Eingabeaufforderung nicht verfügbar sind. Führen Sie den Befehl [az login](/cli/azure/reference-index#az-login) aus, um sich anzumelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Die Deinstallation kann durch erneutes Ausführen des MSI-Installationsprogramms oder durch Auswählen der Option „Deinstallieren“ ausgeführt werden.

> [!div class="nextstepaction"]
> [MSI-Installationsprogramm herunterladen](https://aka.ms/installazurecliwindows)

## <a name="next-steps"></a>Nächste Schritte

Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)

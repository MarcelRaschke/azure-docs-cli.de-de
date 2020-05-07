---
title: Installieren der Azure-Befehlszeilenschnittstelle für Windows
description: Installieren der Azure CLI unter Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 05/01/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c5e9118a04b0dc608309093866307fdc7083f591
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2020
ms.locfileid: "80417838"
---
# <a name="install-azure-cli-on-windows"></a>Installieren der Azure CLI unter Windows

Unter Windows wird die Azure CLI über eine MSI-Datei installiert. Dadurch können Sie über die Windows-Eingabeaufforderung (CMD) oder über PowerShell auf die CLI zugreifen.
Bei der Installation für ein Windows-Subsystem für Linux (WSL) sind Pakete für Ihre Linux-Distribution verfügbar. Die Liste der unterstützten Paket-Manager bzw. Informationen zur manuellen Installation unter WSL finden Sie auf der [Hauptseite für die Installation](install-azure-cli.md).

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a>Installieren oder Aktualisieren

Das verteilbare MSI-Installationsprogramm wird zum Installieren oder Aktualisieren der Azure-Befehlszeilenschnittstelle (Azure Command Line Interface, Azure CLI) unter Windows verwendet. Sie müssen keine aktuellen Versionen deinstallieren, bevor Sie das MSI-Installationsprogramm ausführen.

> [!div class="nextstepaction"]
> [MSI-Installationsprogramm herunterladen](https://aka.ms/installazurecliwindows)

Wenn das Installationsprogramm fragt, ob Änderungen am Computer vorgenommen werden dürfen, klicken Sie auf „Ja“.

Sie können die Azure-Befehlszeilenschnittstelle auch mithilfe von PowerShell installieren. Starten Sie PowerShell als Administrator, und führen Sie den folgenden Befehl aus:

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```
Dadurch wird die aktuelle Version der Azure-Befehlszeilenschnittstelle für Windows heruntergeladen und installiert. Haben Sie bereits eine Version installiert, wird diese aktualisiert. Nach Abschluss der Installation müssen Sie PowerShell erneut öffnen, damit die Azure-Befehlszeilenschnittstelle verwendet werden kann.

Sie können nun mit dem Befehl `az` über die Windows-Eingabeaufforderung oder PowerShell die Azure CLI ausführen. In PowerShell stehen einige Features zur Vervollständigung mit der TAB-TASTE zur Verfügung, die an der Windows-Eingabeaufforderung nicht verfügbar sind. Führen Sie den Befehl [az login](/cli/azure/reference-index#az-login) aus, um sich anzumelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation unter Windows auftreten können. Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="proxy-blocks-connection"></a>Der Proxy blockiert die Verbindung.

Wenn Sie das MSI-Installationsprogramm nicht herunterladen können, da Ihr Proxy die Verbindung blockiert, stellen Sie sicher, dass Sie den Proxy richtig konfiguriert haben. Für Windows 10 werden diese Einstellungen im Bereich `Settings > Network & Internet > Proxy` verwaltet. Wenden Sie sich an Ihren Systemadministrator, um Informationen zu den erforderlichen Einstellungen zu erhalten oder wenn Ihr Computer ggf. konfigurationsverwaltet ist oder ein erweitertes Setup erfordert.

> [!IMPORTANT]
> Diese Einstellungen sind auch erforderlich, damit Sie mit der CLI sowohl über PowerShell als auch über die Eingabeaufforderung auf Azure-Dienste zugreifen können. Führen Sie dazu in PowerShell den folgenden Befehl aus:
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

Zum Abrufen der MSI muss Ihr Proxy HTTPS-Verbindungen mit den folgenden Adressen zulassen:

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Sie deinstallieren die Azure-Befehlszeilenschnittstelle über die Liste „Apps und Features“ in Windows. Gehen Sie zum Deinstallieren wie folgt vor:

| Plattform | Instructions |
|---|---|
| Windows 10 | Start > Einstellungen > Apps |
| Windows 8<br/>Windows 7 | Start > Systemsteuerung > Programme > Programm deinstallieren |

Geben Sie auf diesem Bildschirm __Azure CLI__ in die Suchleiste des Programms ein. Das Programm zum Deinstallieren wird als __Microsoft CLI 2.0 for Azure__ angezeigt. Wählen Sie diese Anwendung aus, und klicken Sie dann auf die Schaltfläche `Uninstall`.

## <a name="next-steps"></a>Nächste Schritte

Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)

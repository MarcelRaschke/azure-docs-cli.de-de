---
title: Installieren der Azure-Befehlszeilenschnittstelle für Windows
description: Installieren der Azure CLI unter Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 09/25/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devx-track-azurecli
ms.openlocfilehash: e592f4e0787a8e4391e47dc45d1841ff415f24bb
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2021
ms.locfileid: "105581851"
---
# <a name="install-azure-cli-on-windows"></a>Installieren der Azure CLI unter Windows

Unter Windows wird die Azure CLI über eine MSI-Datei installiert. Dadurch können Sie über die Windows-Eingabeaufforderung (CMD) oder über PowerShell auf die CLI zugreifen.
Bei der Installation für ein Windows-Subsystem für Linux (WSL) sind Pakete für Ihre Linux-Distribution verfügbar. Die Liste der unterstützten Paket-Manager bzw. Informationen zur manuellen Installation unter WSL finden Sie auf der [Hauptseite für die Installation](install-azure-cli.md).

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a>Installieren oder Aktualisieren

Das verteilbare MSI-Installationsprogramm wird zum Installieren oder Aktualisieren der Azure-Befehlszeilenschnittstelle (Azure Command Line Interface, Azure CLI) unter Windows verwendet. Sie müssen aktuelle Versionen nicht deinstallieren, bevor Sie das MSI-Installationsprogramm verwenden, da mit der MSI-Datei vorhandene Versionen aktualisiert werden.

# <a name="microsoft-installer-msi"></a>[Microsoft Installer (MSI)](#tab/azure-cli)

Wenn das Installationsprogramm fragt, ob Änderungen am Computer vorgenommen werden dürfen, klicken Sie auf „Ja“.

### <a name="azure-cli-current-version"></a>Aktuelle Version der Azure CLI

Laden Sie die aktuelle Version der Azure CLI herunter, und installieren Sie sie.  Nach Abschluss der Installation müssen Sie alle aktiven Windows-Eingabeaufforderungen oder PowerShell-Fenster schließen und erneut öffnen, um die Azure CLI verwenden zu können.

> [!div class="nextstepaction"]
> [Aktuelle Version der Azure CLI](https://aka.ms/installazurecliwindows)

### <a name="azure-cli-beta-version"></a>Azure CLI-Betaversion

Die Betaversion der Azure CLI unterstützt alle Befehl und wird jeweils mit der aktuell veröffentlichen Version synchronisiert.  Anweisungen zur Installation finden Sie unter [Installieren der Azure CLI-Betaversion](install-azure-cli-beta.md). 

# <a name="microsoft-installer-msi-with-command"></a>[Microsoft Installer (MSI) mit Befehl](#tab/azure-powershell)

### <a name="powershell-command"></a>PowerShell-Befehl

Sie können die Azure-Befehlszeilenschnittstelle auch mithilfe von PowerShell installieren. Starten Sie PowerShell als Administrator, und führen Sie den folgenden Befehl aus:

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```

Dadurch wird die aktuelle Version der Azure-Befehlszeilenschnittstelle für Windows heruntergeladen und installiert. Haben Sie bereits eine Version installiert, wird die vorhandene Version vom Installationsprogramm aktualisiert. Nach Abschluss der Installation müssen Sie PowerShell erneut öffnen, damit die Azure-Befehlszeilenschnittstelle verwendet werden kann.

### <a name="azure-cli-command-for-update-only"></a>Azure CLI-Befehl (nur für die Aktualisierung)
[!INCLUDE [az upgrade](includes/az-upgrade.md)]

---

## <a name="run-the-azure-cli"></a>Ausführen der Azure CLI

Sie können nun mit dem Befehl `az` über die Windows-Eingabeaufforderung oder PowerShell die Azure CLI ausführen. In PowerShell stehen einige Features zur Vervollständigung mit der TAB-TASTE zur Verfügung, die an der Windows-Eingabeaufforderung nicht verfügbar sind. Führen Sie den Befehl [az login](/cli/azure/reference-index#az_login) aus, um sich anzumelden.

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
* `https://azcliprod.blob.core.windows.net/`

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Sie deinstallieren die Azure-Befehlszeilenschnittstelle über die Liste „Apps und Features“ in Windows. Gehen Sie zum Deinstallieren wie folgt vor:

| Plattform | Instructions |
|---|---|
| Windows 10 | Start > Einstellungen > Apps |
| Windows 8 und Windows 7 | Start > Systemsteuerung > Programme > Programm deinstallieren |

Geben Sie auf diesem Bildschirm __Azure CLI__ in die Suchleiste des Programms ein. Das Programm zum Deinstallieren wird als __Microsoft CLI 2.0 for Azure__ angezeigt. Wählen Sie diese Anwendung aus, und klicken Sie dann auf die Schaltfläche `Uninstall`.

## <a name="next-steps"></a>Nächste Schritte

Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)

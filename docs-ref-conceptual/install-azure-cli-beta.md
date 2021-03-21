---
title: Installieren der Azure CLI-Betaversion
description: Referenz zur Installation der Azure CLI-Betaversion
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/09/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: ccee5c30d625522525065f5cbd57637427d49b86
ms.sourcegitcommit: f9e23f29c59c6957d3df4d5ca2f4425093e6fd80
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2021
ms.locfileid: "103554931"
---
# <a name="install-azure-cli-beta-version"></a>Installieren der Azure CLI-Betaversion

Für die Azure-Befehlszeilenschnittstelle (Azure CLI) wurde eine neue Betaversion veröffentlicht, die mehr Sicherheit für Tokencache, Zugriffstoken und SSL-Zertifikate bietet.  Diese Betaversion kann in Windows-, macOS- und Linux-Umgebungen installiert werden und wird mit der jeweils neuesten Version synchronisiert.

> [!NOTE]
>
>  Mit dieser Version werden WICHTIGE ÄNDERUNGEN eingeführt.  Lesen Sie vor der Installation sorgfältig alle [Anmerkungen zur Version](/cli/azure/release-notes-azure-cli?tabs=azure-cli-beta).
>
> Die Betaversion garantiert keine Qualität auf Produktebene, daher sollte sie nicht in der Produktionsumgebung verwendet werden.

## <a name="understand-beta-changes"></a>Grundlegendes zu Änderungen in der Betaversion

### <a name="accesstokensjson-deprecation"></a>Eingestellte Unterstützung für `accessTokens.json`

Die aktuelle Azure CLI speichert die ADAL-Aktualisierungstoken und -Zugriffstoken in `~/.azure/accessToken.json`. Die Betaversion der Azure CLI verwendet MSAL und generiert `accessTokens.json` nicht mehr.  Die Token werden im freigegebenen Tokencache von MSAL namens `msal.cache` gespeichert. 

Der MSAL-Tokencache wird unter Windows, macOS und Linux mit einer Desktopumgebung verschlüsselt. Daher gibt es keinen direkten Zugriff auf den MSAL-Tokencache. Jeder vorhandene Workflow, der von `accessTokens.json` abhängt, funktioniert nicht mehr.

Im Folgenden finden Sie verschiedene Alternative, die Sie in Betracht ziehen können: 

#### <a name="calling-az-account-get-access-token"></a>Aufrufen von `az account get-access-token`

Sie können `az account get-access-token` manuell in einem Terminal aufrufen oder einen Teilprozess verwenden, um den Befehl mit einer anderen Programmiersprache aufzurufen. Standardmäßig gilt das zurückgegebene Token für das Standardabonnement bzw. den Standardmandanten, das bzw. der mit `az account show` angezeigt wird.

#### <a name="using-azureclicredential"></a>Verwenden von `AzureCliCredential`

Bei `AzureCliCredential` handelt es sich um einen Anmeldeinformationstyp in allen vorhandenen Programmiersprachen-SDKs. Intern wird ein Teilprozess zum Aufrufen von `az account get-access-token` verwendet, um ein Zugriffstoken von den aktuell angemeldeten CLI-Konten abzurufen. 

#### <a name="accessing-shared-msal-cache"></a>Zugreifen auf den freigegebenen MSAL-Cache

Erstanbieter-Apps können mit `SharedTokenCacheCredential` aus dem Azure Identity-SDK direkt auf den freigegebenen MSAL-Cache zugreifen.

## <a name="install-azure-cli-beta"></a>Installieren der Azure CLI-Betaversion

Azure CLI basiert auf [Python](https://www.python.org/). Die folgenden Python-Versionen werden unterstützt: 3.6, 3.7, 3.8. Unter Windows müssen Sie zuerst [Python installieren](https://www.python.org/downloads/windows/).

Die Azure CLI-Betaversion kann nur mit `pip` aus einem Microsoft-Repository installiert werden.  Verwenden Sie [Azure Cloud Shell](https://shell.azure.com), um die folgenden Befehle oder `python3` (abhängig von der Linux-Distribution oder der installierten Python-Version) auszuführen.

Um das Überschreiben der installierten Azure CLI zu vermeiden, empfiehlt es sich, die Betaversion in einer [virtuellen Umgebung](https://docs.python.org/3/tutorial/venv.html) zu installieren.

1. Erstellen einer virtuellen Umgebung

   Navigieren Sie zu dem Ordner, in dem Sie die virtuelle Umgebung erstellen möchten, und führen Sie dann Folgendes aus:

   ```bash
   python -m venv <env_name>
   ```

1. Aktivieren der virtuellen Umgebung

      ### <a name="windows-powershell"></a>[Windows PowerShell](#tab/powershell)

   ```powershell
   . .\$env\Scripts\Activate.ps1
   ```

   ### <a name="linuxmacos-bash"></a>[Linux/macOS: Bash](#tab/bash)

   ```bash
   . $env/bin/activate
   ```
   ---
   Diese Befehle können auch zum erneuten Aktivieren Ihrer virtuellen Umgebung verwendet werden.

1. Installieren der Azure CLI-Betaversion

   ```bash
   pip install --pre --extra-index-url https://azcliprod.blob.core.windows.net/beta/simple/ azure-cli
   ```

1. Deaktivieren der virtuellen Umgebung

   Nachdem Sie die Arbeit mit der Azure CLI-Betaversion abgeschlossen haben, können Sie das Terminalfenster schließen oder den Befehl `deactivate` verwenden.

   ```bash
   deactivate
   ```

## <a name="uninstall-azure-cli-beta"></a>Deinstallieren der Azure CLI-Betaversion

Um die Azure CLI-Betaversion zu deinstallieren, löschen Sie den Ordner in der virtuellen Umgebung.

### <a name="windows-powershell"></a>[Windows PowerShell](#tab/powershell)

```powershell
Remove-Item -Force -Recurse <env_name>
```

### <a name="linuxmacos-bash"></a>[Linux/macOS: Bash](#tab/bash)

```bash
rm -rf <env_name>
```

---

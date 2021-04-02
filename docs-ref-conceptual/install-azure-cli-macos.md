---
title: Installieren der Azure-Befehlszeilenschnittstelle für macOS
description: Installieren der Azure CLI unter macOS
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/25/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 665d6e5536282ad55eae6132c3925462f69fedf3
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2021
ms.locfileid: "105582089"
---
# <a name="install-azure-cli-on-macos"></a>Installieren der Azure CLI unter macOS

Bei Verwendung der macOS-Plattform können Sie die Azure CLI mit dem [Homebrew-Paket-Manager](https://brew.sh) installieren. Mit Homebrew können Sie Ihre CLI-Installation ganz einfach auf dem neuesten Stand halten. Das CLI-Paket wurde ab der macOS-Version 10.9 getestet.

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-with-homebrew"></a>Installieren mit Homebrew

Homebrew ist die einfachste Möglichkeit zum Verwalten der CLI-Installation. Homebrew bietet praktische Optionen zum Installieren, Aktualisieren und Deinstallieren.
Falls Homebrew auf Ihrem System nicht verfügbar ist, [installieren Sie Homebrew](https://docs.brew.sh/Installation.html), bevor Sie fortfahren.

Sie können die CLI installieren, indem Sie die Homebrew-Repositoryinformationen aktualisieren und dann den Befehl `install` ausführen:

```bash
brew update && brew install azure-cli
```

> [!IMPORTANT]
>
> Die Azure CLI weist eine Abhängigkeit vom Homebrew-Paket `python3` auf und installiert es.
> Die Azure CLI ist garantiert kompatibel mit der aktuellen Version von `python3`, die auf Homebrew veröffentlicht wurde.

Sie können dann die Azure CLI mit dem Befehl `az` ausführen. Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az_login), um sich anzumelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt finden Sie einige allgemeine Fehler, die zu Problemen bei der Homebrew-basierten CLI-Installation führen können. Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="completion-is-not-working"></a>Die Vervollständigung funktioniert nicht.

Die Homebrew-Formel der Azure CLI installiert eine Vervollständigungsdatei namens `az` im Verzeichnis für von Homebrew verwaltete Vervollständigungen (Standardspeicherort: `/usr/local/etc/bash_completion.d/`). Befolgen Sie zum Aktivieren der Vervollständigung [diese Anweisungen](https://docs.brew.sh/Shell-Completion) von Homebrew.

### <a name="unable-to-find-python-or-installed-packages"></a>Python und installierte Pakete können nicht gefunden werden.

Bei der Installation von Homebrew weichen die Versionen unter Umständen geringfügig voneinander ab, oder es liegt ein anderes Problem vor. Die CLI verwendet keine virtuelle Python-Umgebung und ist daher von der Ermittlung der installierten Python-Version abhängig. Sie können das Problem möglicherweise beheben, indem Sie die `python3`-Abhängigkeit installieren und über Homebrew neu verknüpfen.

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a>CLI-Version 1.x wird installiert.

Die Installation einer veralteten Version kann auf einen veralteten Homebrew-Cache zurückzuführen sein. Gehen Sie gemäß der [Aktualisierungsanleitung](#update) vor.

### <a name="proxy-blocks-connection"></a>Der Proxy blockiert die Verbindung.

Möglicherweise können Sie keine Ressourcen von Homebrew abrufen, wenn Sie das Programm nicht korrekt zur Verwendung Ihres Proxys konfiguriert haben. Führen Sie die [Anweisungen zur Proxykonfiguration für Homebrew](https://docs.brew.sh/Manpage#using-homebrew-behind-a-proxy) aus.

> [!IMPORTANT]
> Wenn Sie sich hinter einem Proxy befinden, müssen `HTTP_PROXY` und `HTTPS_PROXY` so festgelegt sein, dass sie über die CLI eine Verbindung mit Azure-Diensten herstellen.
> Wenn Sie nicht die Standardauthentifizierung verwenden, wird empfohlen, dass Sie diese Variablen in Ihrer Datei vom Typ `.bashrc` exportieren.
> Berücksichtigen Sie dabei immer die Sicherheitsrichtlinien Ihres Unternehmens und die Anforderungen Ihres Systemadministrators.

Zum Abrufen der Bottle-Ressourcen von Homebrew muss Ihr Proxy HTTPS-Verbindungen mit den folgenden Adressen zulassen:

* `https://formulae.brew.sh`
* `https://homebrew.bintray.com`

## <a name="update"></a>Aktualisieren

Die CLI wird regelmäßig mit Fehlerbehebungen, Verbesserungen, neuen Features und Vorschaufunktionen aktualisiert. Ein neues Release ist ungefähr alle drei Wochen verfügbar.

[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

Sie können Ihre lokalen Homebrew-Repositoryinformationen auch aktualisieren und anschließend ein Upgrade für das Paket `azure-cli` ausführen.

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Verwenden Sie Homebrew, um das Paket `azure-cli` zu deinstallieren.

```bash
brew uninstall azure-cli
```

## <a name="other-installation-methods"></a>Andere Installationsmethoden

Falls Sie die Azure-Befehlszeilenschnittstelle in Ihrer Umgebung nicht mithilfe von Homebrew installieren können, können Sie die manuelle Anleitung für Linux verwenden. Beachten Sie, dass dieser Prozess nicht offiziell mit macOS kompatibel ist. Es empfiehlt sich immer, einen Paket-Manager wie Homebrew zu verwenden. Verwenden Sie die manuelle Installationsmethode nur, wenn keine andere Option zur Verfügung steht.

Die Anleitung für die manuelle Installation finden Sie unter [Manuelles Installieren der Azure CLI unter Linux](install-azure-cli-linux.md).

## <a name="next-steps"></a>Nächste Schritte

Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)
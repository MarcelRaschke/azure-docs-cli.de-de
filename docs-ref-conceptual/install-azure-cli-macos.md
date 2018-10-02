---
title: Installieren der Azure-Befehlszeilenschnittstelle für macOS
description: Installieren der Azure CLI unter macOS
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 9eb816ef68d24d1dbbaaeb5fd4877580edbe87ad
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177656"
---
# <a name="install-azure-cli-on-macos"></a>Installieren der Azure CLI unter macOS

Bei Verwendung der macOS-Plattform können Sie die Azure CLI mit dem [Homebrew-Paket-Manager](https://brew.sh) installieren. Mit Homebrew können Sie Ihre CLI-Installation ganz einfach auf dem neuesten Stand halten. Das CLI-Paket wurde ab der macOS-Version 10.9 getestet.

## <a name="install"></a>Installieren

Homebrew ist die einfachste Möglichkeit zum Verwalten der CLI-Installation. Homebrew bietet praktische Optionen zum Installieren, Aktualisieren und Deinstallieren.
Falls Homebrew auf Ihrem System nicht verfügbar ist, [installieren Sie Homebrew](https://docs.brew.sh/Installation.html), bevor Sie fortfahren.

Sie können die CLI installieren, indem Sie die Homebrew-Repositoryinformationen aktualisieren und dann den Befehl `install` ausführen:

```bash
brew update && brew install azure-cli
```

Sie können dann die Azure CLI mit dem Befehl `az` ausführen. Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt finden Sie einige allgemeine Fehler, die zu Problemen bei der Homebrew-basierten CLI-Installation führen können. Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="unable-to-find-python-or-installed-packages"></a>Python und installierte Pakete können nicht gefunden werden.

Bei der Installation von Homebrew weichen die Versionen unter Umständen geringfügig voneinander ab, oder es liegt ein anderes Problem vor. Die CLI verwendet keine virtuelle Python-Umgebung und ist daher von der Ermittlung der installierten Python-Version abhängig. Sie können das Problem möglicherweise beheben, indem Sie die `python3`-Abhängigkeit installieren und über Homebrew neu verknüpfen.

```bash
brew update && brew install python3 && brew upgrade python3
brew link --overwrite python3
```

### <a name="cli-version-1x-is-installed"></a>CLI-Version 1.x wird installiert.

Die Installation einer veralteten Version kann auf einen veralteten Homebrew-Cache zurückzuführen sein. Gehen Sie gemäß der [Aktualisierungsanleitung](#Update) vor.

## <a name="update"></a>Aktualisieren

Die CLI wird regelmäßig mit Fehlerbehebungen, Verbesserungen, neuen Features und Vorschaufunktionen aktualisiert. Ein neues Release ist ungefähr alle zwei Wochen verfügbar. Aktualisieren Sie Ihre lokalen Repositoryinformationen, und upgraden Sie anschließend das Paket `azure-cli`.

```bash
brew update && brew upgrade azure-cli
```

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Verwenden Sie Homebrew, um das Paket `azure-cli` zu deinstallieren.

```bash
brew uninstall azure-cli
```

## <a name="next-steps"></a>Nächste Schritte

Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)

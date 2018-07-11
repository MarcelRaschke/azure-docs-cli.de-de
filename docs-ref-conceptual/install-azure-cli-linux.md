---
title: Manuelle Installation der Azure CLI 2.0 für Linux
description: Manuelle Installation der Azure CLI 2.0 unter Linux
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: dade772f178ed9fd321ff45727aea991acd6d311
ms.sourcegitcommit: 308f9eb433a05b814999ac404f63d181169fffeb
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/03/2018
ms.locfileid: "37439634"
---
# <a name="install-azure-cli-20-on-linux-manually"></a>Manuelle Installation der Azure CLI 2.0 unter Linux

Wenn in Ihrer Distribution kein Paket für die Azure CLI enthalten ist, können Sie die CLI durch Ausführen eines Installationsskripts jederzeit manuell installieren.

> [!NOTE]
> Es wird dringend empfohlen, einen Paket-Manager für die CLI zu verwenden. Ein Paket-Manager stellt sicher, dass Sie immer die neuesten Updates erhalten, und gewährleistet die Stabilität der CLI-Komponenten. Überprüfen Sie vor der manuellen Installation, ob ein Paket für Ihre Distribution verfügbar ist.

## <a name="prerequisites"></a>Voraussetzungen

Zum Installieren der CLI muss auf dem System folgende Software verfügbar sein:

* [Python 2.7 oder Python 3.x](https://www.python.org/downloads/)
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

## <a name="install-or-update"></a>Installieren oder Aktualisieren

Sie müssen eine vollständige Installation ausführen – unabhängig davon, ob die CLI installiert oder aktualisiert wird. Wenn alle erforderlichen Komponenten vorhanden sind, können Sie die CLI durch Ausführung von `curl` installieren.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

Alternativ können Sie das Skript herunterladen und lokal ausführen. Unter Umständen müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden. 

Sie können dann die Azure CLI mit dem Befehl `az` ausführen. Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Weitere Informationen zu verschiedenen Anmeldemethoden finden Sie unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt werden einige allgemeine Probleme beschrieben, die bei einer manuellen Installation auftreten können. Sollte Ihr Problem hier nicht aufgeführt sein, [melden Sie es über GitHub](https://github.com/Azure/azure-cli/issues).
### <a name="curl-object-moved-error"></a>curl-Fehler „Objekt verschoben“

Wenn Sie einen Fehler von `curl` im Zusammenhang mit dem `-L`-Parameter oder eine Fehlermeldung mit dem Text „Objekt verschoben“ erhalten, versuchen Sie, die vollständige URL anstatt der `aka.ms`-Umleitung zu verwenden:

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a>Der Befehl `az` wurde nicht gefunden.

Wenn Sie den Befehl nicht ausführen können, nachdem Sie die Installation durchgeführt und `bash` oder `zsh` verwendet haben, leeren Sie den Befehlshash-Cache Ihrer Shell. Ausführen

```bash
hash -r
```

Überprüfen Sie, ob das Problem behoben wurde.

Dieses Problem kann auch auftreten, wenn Sie die Shell nach der Installation nicht neu gestartet haben. Stellen Sie sicher, dass sich der Befehl `az` in `$PATH` befindet. Den Befehl `az` finden Sie hier:

```bash
<install path>/bin
```

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Sie können die CLI deinstallieren, indem Sie die Dateien direkt aus dem Verzeichnis löschen, das Sie bei der Installation ausgewählt haben. Das Standardinstallationsverzeichnis ist `$HOME`.

1. Entfernen Sie die installierten CLI-Dateien.

  ```bash
  rm -r <install location>/lib/azure-cli
  rm <install location>/bin/az
  ```
2. Ändern Sie die Datei `$HOME/.bash_profile`, indem Sie die folgende Zeile entfernen:

  ```text
  <install location>/lib/azure-cli/az.completion
  ```

3. Laden Sie bei Verwendung von `bash` oder `zsh` den Befehlscache Ihrer Shell neu.

  ```bash
  hash -r
  ```

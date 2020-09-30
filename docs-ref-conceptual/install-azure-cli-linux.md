---
title: Manuelles Installieren der Azure CLI für Linux
description: Manuelles Installieren der Azure CLI unter Linux
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 9f70e0eb4f518c8fbb7bf8803b93b8b8246d8791
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225659"
---
# <a name="install-azure-cli-on-linux-manually"></a>Manuelles Installieren der Azure CLI unter Linux

Ist kein Paket für die Azure CLI für Ihre Distribution vorhanden, installieren Sie die CLI manuell durch Ausführung eines Skripts.

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> Es wird dringend empfohlen, die CLI mit einem Paket-Manager zu installieren. Ein Paket-Manager stellt sicher, dass Sie immer die neuesten Updates erhalten, und gewährleistet die Stabilität der CLI-Komponenten. Überprüfen Sie vor der manuellen Installation, ob ein Paket für Ihre Distribution verfügbar ist.

## <a name="prerequisites"></a>Voraussetzungen

Die CLI benötigt die folgende Software:

* [Python 3.6.x, 3.7.x oder 3.8.x](https://www.python.org/downloads/). 
* [libffi](https://sourceware.org/libffi/)
* [OpenSSL 1.0.2](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> Die CLI unterstützt Python 2.7 seit Version `2.1.0` nicht mehr. Bei neuen Versionen wird die ordnungsgemäße Ausführung mit Python 2.7 nicht mehr garantiert.

## <a name="install-or-update"></a>Installieren oder Aktualisieren

Sowohl für die Installation als auch die Aktualisierung der CLI muss das Installationsskript erneut ausgeführt werden. Installieren Sie die CLI durch Ausführen von `curl`.

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

Das Skript kann auch heruntergeladen und lokal ausgeführt werden. Unter Umständen müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.

Sie können dann die Azure CLI mit dem Befehl `az` ausführen. Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt werden einige allgemeine Probleme beschrieben, die bei einer manuellen Installation auftreten können. Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).

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

### <a name="proxy-blocks-connection"></a>Der Proxy blockiert die Verbindung.

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

Zum Abrufen der Installationsskripts muss Ihr Proxy HTTPS-Verbindungen mit den folgenden Adressen zulassen:

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* Endpunkte, die vom Paket-Manager Ihrer Distribution (sofern vorhanden) für Core-Pakete verwendet werden

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

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

## <a name="next-steps"></a>Nächste Schritte

Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)
---
title: Installieren der klassischen Azure CLI
description: Installieren der klassischen Azure CLI für Mac, Linux und Windows für das Starten von Azure-Diensten
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 06/11/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 0cc1d7811223bf6f473c2c4516d0919306aa74c7
ms.sourcegitcommit: 7caa6673f65e61deb8d6def6386e4eb9acdac923
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/28/2020
ms.locfileid: "77779481"
---
# <a name="install-the-azure-classic-cli"></a>Installieren der klassischen Azure CLI

> [!IMPORTANT]
> In diesem Thema wird beschrieben, wie Sie die klassische Azure CLI installieren. Die klassische CLI ist veraltet und sollte nur mit dem klassischen Bereitstellungsmodell verwendet werden.
> Verwenden Sie für alle anderen Bereitstellungen [die Azure CLI](/cli/azure).

Installieren Sie schnell die klassische Azure CLI, um eine Reihe von auf der Open-Source-Shell basierenden Befehlen zum Erstellen und Verwalten von Ressourcen in Microsoft Azure zu verwenden. Zum Installieren dieser plattformübergreifenden Tools auf Ihrem Computer stehen Ihnen mehrere Optionen zur Verfügung:

* **npm-Paket**: Führen Sie npm (den Paket-Manager für JavaScript) aus, um das Paket mit der klassischen Azure CLI auf Ihrer Linux-Distribution oder dem Betriebssystem zu installieren. Hierfür sind „Node.js“ und „npm“ erforderlich.
* **Installer**: Laden Sie ein Installationsprogramm für die einfache Installation unter macOS oder Windows herunter.
* **Docker-Container**: Beginnen Sie mit der Verwendung der klassischen CLI in einem sofort betriebsbereiten Docker-Container. Hierfür ist ein Docker-Host erforderlich.

Weitere Optionen und Hintergrundinformationen finden Sie im Projektrepository auf [GitHub](https://github.com/azure/azure-xplat-cli).

Sobald die klassische Azure CLI installiert ist, stellen Sie mit `azure login` eine Verbindung her und führen die `azure`-Befehle in der Befehlszeilenschnittstelle (Bash, Terminal, Eingabeaufforderung usw.) aus, um mit Ihren Azure-Ressourcen zu arbeiten.

## <a name="option-1-install-an-npm-package"></a>Option 1: Installieren eines npm-Pakets

Um die klassische CLI aus einem npm-Paket zu installieren, müssen Sie die aktuellen Versionen von [Node.js und npm](https://nodejs.org/en/download/package-manager/) herunterladen und installieren. Führen Sie anschließend `npm install` aus, um das azure-cli-Paket zu installieren:

```bash
npm install -g azure-cli
```

Bei Linux-Distributionen müssen Sie unter Umständen `sudo` wie folgt verwenden, um den `npm`-Befehl erfolgreich ausführen zu können:

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> Wenn Sie Node.js und npm auf Ihrem Betriebssystem installieren oder aktualisieren müssen, empfehlen wir Ihnen, Node.js-LTS-Version 4.x oder höher zu installieren. Wenn Sie eine ältere Version verwenden, kommt es möglicherweise zu Fehlern bei der Installation.

Falls Sie es vorziehen, können Sie auch aus den [GitHub-Releases](https://github.com/Azure/azure-xplat-cli/releases) eine TAR-Datei herunterladen. Installieren Sie dann das heruntergeladene npm-Paket wie folgt (in Linux-Distributionen müssen Sie unter Umständen `sudo` verwenden):

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a>Option 2: Verwenden eines Installers

Bei Verwendung eines Mac- oder Windows-Computers sind unter den [GitHub-Releases](https://github.com/Azure/azure-xplat-cli/releases) DMG- und MSI-Installer verfügbar.

> [!TIP]
> Unter Windows können Sie auch den [Webplattform-Installer](https://go.microsoft.com/?linkid=9828653) herunterladen, um die klassische CLI zu installieren. Dieser Installer bietet Ihnen die Möglichkeit, zusätzliche Azure SDK- und -Befehlszeilentools zu installieren.

## <a name="option-3-use-a-docker-container"></a>Option 3: Verwenden eines Docker-Containers

Wenn Sie Ihren Computer als [Docker](https://docs.docker.com/engine/understanding-docker/)-Host eingerichtet haben, können Sie die klassische Azure CLI in einem Docker-Container ausführen. Führen Sie den folgenden Befehl aus (bei Linux-Distributionen müssen Sie unter Umständen `sudo` verwenden):

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-classic-cli-commands"></a>Ausführen von Befehlen der klassischen Azure CLI

Nachdem die klassische Azure CLI installiert wurde, können Sie den Befehl `azure` in der Befehlszeilenschnittstelle (Bash, Terminal, Eingabeaufforderung usw.) ausführen. Um beispielsweise den Hilfebefehl auszuführen, geben Sie Folgendes ein:

```azurecli-interactive
azure help
```

> [!NOTE]
> In einigen Linux-Distributionen erhalten Sie unter Umständen eine Fehlermeldung wie `/usr/bin/env: ‘node’: No such file or directory`. Dieser Fehler stammt von kürzlich durchgeführten Installationen von „Node.js“, die unter „/usr/bin/nodejs“ installiert sind. Erstellen Sie zum Beheben dieses Fehlers eine symbolische Verknüpfung mit „/usr/bin/node“, indem Sie den folgenden Befehl ausführen:

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

Geben Sie Folgendes ein, um die Version der installierten klassischen Azure CLI anzuzeigen:

```azurecli-interactive
azure --version
```

> [!NOTE]
> Wenn Sie die klassische Azure CLI zum ersten Mal verwenden, werden Sie in einer Meldung gefragt, ob Sie Microsoft das Erfassen von Nutzungsinformationen erlauben möchten. Die Teilnahme ist freiwillig. Wenn Sie sich für die Teilnahme entscheiden, können Sie diese durch Ausführen von `azure telemetry --disable`jederzeit beenden. Zum Aktivieren der Teilnahme können Sie jederzeit `azure telemetry --enable`ausführen.

## <a name="update-the-classic-cli"></a>Aktualisieren der klassischen CLI

Microsoft veröffentlicht ggf. aktualisierte Versionen der klassischen Azure CLI. Installieren Sie die klassische CLI erneut, indem Sie das Installationsprogramm für Ihr Betriebssystem verwenden, oder führen Sie den neuesten Docker-Container aus. Falls Node.js und npm installiert sind, können Sie die Aktualisierung durchführen, indem Sie Folgendes eingeben (bei Linux-Distributionen müssen Sie unter Umständen `sudo` verwenden):

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a>Aktivieren der Vervollständigung mit der TAB-Taste

Die Vervollständigung mit der TAB-Taste für Befehle der klassischen CLI wird für Mac und Linux unterstützt.

Für die Aktivierung in zsh führen Sie Folgendes aus:

```bash
echo '. <(azure --completion)' >> .zshrc
```

Für die Aktivierung in bash führen Sie Folgendes aus:

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```

## <a name="next-steps"></a>Nächste Schritte

* Wenn Sie weitere Informationen zur klassischen Azure CLI erhalten, den Quellcode herunterladen, Probleme melden oder etwas zum Projekt beitragen möchten, hilft Ihnen der Artikel [GitHub repository for the Azure classic CLI](https://github.com/azure/azure-xplat-cli) (GitHub-Repository für die klassische Azure CLI) weiter.

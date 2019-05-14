---
title: Installieren der Azure CLI unter Linux mit apt
description: Installieren der Azure CLI mit dem apt-Paket-Manager
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/08/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: af82eea3fd549cbca85699a3030a19bc82574b73
ms.sourcegitcommit: c65c69bd08fd6b7632ba60dc7c8e9f2b57a9d0b7
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/09/2019
ms.locfileid: "65476255"
---
# <a name="install-azure-cli-with-apt"></a>Installieren der Azure CLI mit apt

Wenn Sie eine Distribution mit `apt` verwenden (etwa Ubuntu oder Debian), steht ein x86_64-Paket für die Azure CLI zur Verfügung. Dieses Paket wurde mit folgenden Produkten getestet und wird für diese unterstützt:

* Ubuntu Trusty, Senial, Artful, Bionic und Disco
* Debian Wheezy, Jessie und Stretch

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> Das Paket für die Azure CLI installiert einen eigenen Python-Interpreter und verwendet nicht die Python-Version des Systems.

## <a name="install"></a>Installieren

Wir bieten zwei Möglichkeiten zum Installieren der Azure-Befehlszeilenschnittstelle (Azure Command Line Interface, Azure CLI) mit Verteilungen, die `apt` unterstützen: Als All-in-One-Skript, das die Installationsbefehle für Sie ausführt, und mithilfe von Anweisungen, die Sie Schritt für Schritt selbst ausführen können.

### <a name="install-with-one-command"></a>Installieren mit einem Befehl

Wir bieten und pflegen ein Skript, das alle Installationsbefehle in einem Schritt ausführt. Führen Sie das Skript mit `curl` aus, und leiten Sie es direkt an `bash` um, oder laden Sie das Skript in eine Datei herunter, und überprüfen Sie es vor dem Ausführen.

> [!IMPORTANT]
> Dieses Skript wurde nur für Ubuntu 16.04 und höher und Debian 8 und höher geprüft. Bei anderen Verteilungen funktioniert es möglicherweise nicht.
> Wenn Sie eine abgeleitete Verteilung wie Linux Mint verwenden, folgen Sie den Anweisungen für die manuelle Installation, und führen Sie ggf. eine Problembehandlung durch.

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

### <a name="manual-install-instructions"></a>Anweisungen für die manuelle Installation

Falls Sie ein Skript nicht als Superuser ausführen möchten, führen Sie die folgenden Schritte zum manuellen Installieren der Azure CLI aus.

1. Laden Sie die für die Installation erforderlichen Pakete herunter:

    ```bash
    sudo apt-get update
    sudo apt-get install curl apt-transport-https lsb-release gnupg
    ```

2. Laden Sie den Microsoft-Signaturschlüssel herunter, und installieren Sie ihn.

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
        gpg --dearmor | \
        sudo tee /etc/apt/trusted.gpg.d/microsoft.asc.gpg > /dev/null
    ```

3. <div id="set-release"/>Fügen Sie das Azure CLI-Softwarerepository hinzu:

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

4. Aktualisieren Sie die Repositoryinformationen, und installieren Sie das Paket `azure-cli`:

    ```bash
    sudo apt-get update
    sudo apt-get install azure-cli
    ```

Führen Sie die Azure CLI mit dem Befehl `az` aus. Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können. Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a>„lsb_release“ gibt nicht die richtige Basisdistributionsversion zurück.

Einige von Ubuntu oder Debian abgeleiteten Distributionen wie Linux Mint geben über `lsb_release` unter Umständen nicht den richtigen Versionsnamen zurück. Mit diesem Wert wird im Installationsprozess das zu installierende Pakete ermittelt. Wenn Sie den Codenamen der Ubuntu- oder Debian-Version kennen, von der Ihre Distribution abgeleitet ist, können Sie beim [Hinzufügen des Repositorys](#set-release) den Wert `AZ_REPO` manuell festlegen. Sehen Sie sich andernfalls Informationen dazu an, wie Sie für Ihre Distribution den Basisdistributions-Codenamen ermitteln, und legen Sie `AZ_REPO` auf den richtigen Wert fest.

### <a name="no-package-for-your-distribution"></a>Kein Paket für Ihre Distribution

Manchmal dauert es nach der Veröffentlichung einer Distribution etwas, bis ein Azure CLI-Paket dafür zur Verfügung gestellt wird. Die Azure CLI ist im Hinblick auf zukünftige Abhängigkeitsversionen resilient konzipiert und nutzt daher möglichst wenige dieser Abhängigkeiten. Ist für Ihre Basisdistribution kein Paket verfügbar, verwenden Sie ein Paket für eine ältere Distribution.

Legen Sie dazu beim [Hinzufügen des Repositorys](#set-release) den Wert `AZ_REPO` manuell fest. Verwenden Sie für Ubuntu-Distributionen das Repository `disco` und für Debian-Distributionen `stretch`. Distributionen, die vor Ubuntu Trusty und Debian Wheezy veröffentlicht wurden, werden nicht unterstützt.

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>Aktualisieren

Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> Durch diesen Befehl werden alle installierten Pakete auf Ihrem System aktualisiert, deren Abhängigkeiten nicht geändert wurden.
> Wenn Sie nur ein Upgrade für die CLI durchführen möchten, verwenden Sie `apt-get install`.
> 
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Deinstallieren Sie sie mit `apt-get remove`:

    ```bash
    sudo apt-get remove -y azure-cli
    ```

2. Entfernen Sie die Azure CLI-Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren:

   ```bash
   sudo rm /etc/apt/sources.list.d/azure-cli.list
   ```

3. Entfernen Sie den Signaturschlüssel:

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.asc.gpg
    ```

4. Entfernen Sie alle nicht benötigten Pakete:

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a>Nächste Schritte

Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)

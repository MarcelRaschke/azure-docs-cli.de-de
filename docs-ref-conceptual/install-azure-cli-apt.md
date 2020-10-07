---
title: Installieren der Azure CLI unter Linux mit apt
description: Installieren der Azure CLI mit dem apt-Paket-Manager
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/29/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 242c634717cf964af718873ab9ecf84ff707db3d
ms.sourcegitcommit: aa44ec97af5c0e7558d254b3159f95921e22ff1c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/01/2020
ms.locfileid: "91625413"
---
# <a name="install-azure-cli-with-apt"></a>Installieren der Azure CLI mit apt

Wenn Sie eine Distribution mit `apt` verwenden (etwa Ubuntu oder Debian), steht ein x86_64-Paket für die Azure CLI zur Verfügung. Dieses Paket wurde mit folgenden Produkten getestet und wird für diese unterstützt:

* Ubuntu Trusty, Xenial, Bionic, Eoan und Focal
* Debian Jessie, Stretch und Buster

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
>
> Das Paket für die Azure CLI installiert einen eigenen Python-Interpreter und verwendet nicht die Python-Version des Systems. 
>
> Unter Ubuntu 20.04 (Focal) ist ein vom `focal/universe`-Repository bereitgestelltes `azure-cli`-Paket mit der Version `2.0.81` verfügbar. Es ist veraltet und wird nicht empfohlen. Wenn Sie es bereits installiert haben, entfernen Sie es zunächst durch Ausführen von `sudo apt remove azure-cli -y && sudo apt autoremove -y`, bevor Sie die folgenden Schritte zum Installieren des aktuellen `azure-cli`-Pakets ausführen.

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

Falls Sie ein Skript nicht als Superuser ausführen möchten, oder falls das All-in-One-Skript fehlschlägt, führen Sie die folgenden Schritte zum Installieren der Azure CLI aus.

1. Rufen Sie die für die Installation erforderlichen Pakete ab:

    ```bash
    sudo apt-get update
    sudo apt-get install ca-certificates curl apt-transport-https lsb-release gnupg
    ```

2. Laden Sie den Microsoft-Signaturschlüssel herunter, und installieren Sie ihn.

    ```bash
    curl -sL https://packages.microsoft.com/keys/microsoft.asc |
        gpg --dearmor |
        sudo tee /etc/apt/trusted.gpg.d/microsoft.gpg > /dev/null
    ```

3. <div id="set-release"/>Fügen Sie das Azure CLI-Softwarerepository hinzu:

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" |
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

### <a name="no-module-issue-on-ubuntu-2004-focalwsl"></a>Problem vom Typ „Kein Modul“ unter Ubuntu 20.04 (Focal)/WSL
Wenn Sie `azure-cli` unter `Focal` installiert haben, ohne das Azure CLI-Softwarerepository in [Schritt 3](#set-release) der Anweisungen für die manuelle Installation hinzuzufügen oder unser [Skript](#install-with-one-command) zu verwenden, treten unter Umständen Probleme auf, etwa das Problem „Kein Modul mit dem Namen 'decorator' or 'antlr4'“. Das ist darauf zurückzuführen, dass es sich beim installierten Paket um das veraltete Paket `azure-cli 2.0.81` aus dem Repository `focal/universe` handelt. Entfernen Sie das Paket zuerst, indem Sie `sudo apt remove azure-cli -y && sudo apt autoremove -y` ausführen. Befolgen Sie anschließend die obigen [Anweisungen](#install) zum Installieren des aktuellen `azure-cli`-Pakets.

### <a name="lsb_release-does-not-return-the-correct-base-distribution-version"></a>„lsb_release“ gibt nicht die richtige Basisdistributionsversion zurück.

Einige von Ubuntu oder Debian abgeleiteten Distributionen wie Linux Mint geben über `lsb_release` unter Umständen nicht den richtigen Versionsnamen zurück. Mit diesem Wert wird im Installationsprozess das zu installierende Pakete ermittelt. Wenn Sie den Codenamen der Ubuntu- oder Debian-Version kennen, von der Ihre Distribution abgeleitet ist, können Sie beim [Hinzufügen des Repositorys](#set-release) den Wert `AZ_REPO` manuell festlegen. Sehen Sie sich andernfalls Informationen dazu an, wie Sie für Ihre Distribution den Basisdistributions-Codenamen ermitteln, und legen Sie `AZ_REPO` auf den richtigen Wert fest.

### <a name="no-package-for-your-distribution"></a>Kein Paket für Ihre Distribution

Manchmal dauert es nach der Veröffentlichung einer Distribution etwas, bis ein Azure CLI-Paket dafür zur Verfügung gestellt wird. Die Azure CLI ist im Hinblick auf zukünftige Abhängigkeitsversionen resilient konzipiert und nutzt daher möglichst wenige dieser Abhängigkeiten. Ist für Ihre Basisdistribution kein Paket verfügbar, verwenden Sie ein Paket für eine ältere Distribution.

Legen Sie dazu beim [Hinzufügen des Repositorys](#set-release) den Wert `AZ_REPO` manuell fest. Verwenden Sie für Ubuntu-Distributionen das Repository `bionic` und für Debian-Distributionen `stretch`. Distributionen, die vor Ubuntu Trusty und Debian Wheezy veröffentlicht wurden, werden nicht unterstützt.

### <a name="elementary-os-eos-fails-to-install-the-azure-cli"></a>Installation der Azure-Befehlszeilenschnittstelle durch EOS (Elementary OS) nicht möglich

Die Azure-Befehlszeilenschnittstelle kann von EOS nicht installiert werden, da `lsb_release` den Wert `HERA` (Name des EOS-Release) zurückgibt.  Zur Lösung des Problems muss die Datei `/etc/apt/sources.list.d/azure-cli.list` korrigiert und `hera main` in `bionic main` geändert werden.

Ursprünglicher Dateiinhalt:

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ hera main
```

Geänderter Dateiinhalt:

```
deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ bionic main
```

### <a name="proxy-blocks-connection"></a>Der Proxy blockiert die Verbindung.

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

Konfigurieren Sie `apt` explizit so, dass dieser Proxy immer verwendet wird. Stellen Sie sicher, dass die folgenden Zeilen in einer `apt`-Konfigurationsdatei in `/etc/apt/apt.conf.d/` erscheinen. Wir empfehlen, dass Sie Ihre vorhandene globale Konfigurationsdatei, eine vorhandene Proxykonfigurationsdatei, `40proxies` oder `99local` verwenden. Berücksichtigen Sie dabei jedoch die Verwaltungsanforderungen Ihres Systems.

```apt.conf
Acquire {
    http::proxy "http://[username]:[password]@[proxy]:[port]";
    https::proxy "https://[username]:[password]@[proxy]:[port]";
}
```

Wenn Ihr Proxy keine Standardauthentifizierung verwendet, __entfernen__ Sie den Teil `[username]:[password]@` des Proxy-URI. Weitere Informationen zur Proxykonfiguration finden Sie in der offiziellen Ubuntu-Dokumentation:

* [apt.conf manpage](http://manpages.ubuntu.com/manpages/bionic/en/man5/apt.conf.5.html)
* [Ubuntu Wiki – apt-get howto](https://help.ubuntu.com/community/AptGet/Howto#Setting_up_apt-get_to_use_a_http-proxy)

Zum Abrufen des Microsoft-Signaturschlüssels und des Pakets von unserem Repository muss Ihr Proxy HTTPS-Verbindungen mit der folgenden Adresse zulassen:

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>Aktualisieren
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

Sie können auch `apt-get upgrade` zum Aktualisieren des CLI-Pakets verwenden.

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

3. Wenn Sie keine anderen Pakete von Microsoft verwenden, entfernen Sie den Signaturschlüssel:

    ```bash
    sudo rm /etc/apt/trusted.gpg.d/microsoft.gpg
    ```

4. Entfernen Sie alle nicht benötigten Pakete:

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a>Nächste Schritte

Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)

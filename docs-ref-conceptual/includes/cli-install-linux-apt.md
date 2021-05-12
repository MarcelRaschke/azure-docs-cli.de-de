---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/29/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: 0738d79c9fc968d9b1000605c30ec30c6fa6eb3c
ms.sourcegitcommit: b76cc7c91ed21ae04b3463544ad46a749461cc6a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/25/2021
ms.locfileid: "107984475"
---
## <a name="overview"></a>Übersicht

Der `apt`-Paket-Manager enthält ein x86_64-Paket für die Azure-Befehlszeilenschnittstelle (Azure CLI), die mit den folgenden Distributionen getestet wurde.

| Distribution | Version |
|:-------------|:--------|
| Ubuntu       | 14.04 LTS (Trusty Tahir), 16.04 LTS (Xenial Xerus), 18.04 LTS (Bionic Beaver), 20.04 LTS (Focal Fossa), 20.10 (Groovy Gorilla) |
| Debian       | Debian 8 (Jessie), Debian 9 (Stretch), Debian 10 (Buster) |

> [!WARNING]
> Ubuntu 20.04 (Focal Fossa) und 20.10 (Groovy Gorilla) enthalten ein `azure-cli`-Paket mit der Version `2.0.81`, das im `universe`-Repository verfügbar ist. Dieses Paket ist veraltet und wird nicht empfohlen. Falls dieses Paket installiert ist, entfernen Sie es mit dem Befehl `sudo apt remove azure-cli -y && sudo apt autoremove -y`, bevor Sie fortfahren.
>
> Die ARM64-Architektur wird vom Deb-Paket `azure-cli` nicht unterstützt.

## <a name="installation-options"></a>Installationsoptionen

Zum Installieren der Azure CLI auf Ihrem System stehen zwei Optionen zur Auswahl.  Sie können einen einzelnen Befehl ausführen, der ein Installationsskript herunterlädt und die Installationsbefehle für Sie ausführt.  Alternativ können Sie die Installationsbefehle selbst Schritt für Schritt ausführen.  Beide Methoden werden im Folgenden beschrieben.

## <a name="option-1-install-with-one-command"></a>Option 1: Installieren mit einem Befehl

Das Azure CLI-Team pflegt ein Skript, mit dem alle Installationsbefehle in einem Schritt ausgeführt werden können.  Dieses Skript wird über `curl` heruntergeladen und direkt an `bash` weitergeleitet, um die CLI zu installieren.

Wenn Sie den Inhalt des Skripts vor der Ausführung überprüfen möchten, laden Sie es einfach mit `curl` herunter, und überprüfen Sie es in Ihrem bevorzugten Text-Editor.

```bash
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```

## <a name="option-2-step-by-step-installation-instructions"></a>Option 2: Schrittweise Installation

Wenn Sie die Installation der Azure CLI lieber Schritt für Schritt durchführen möchten, befolgen Sie die folgenden Schritte.

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

## <a name="sign-in-to-azure-with-the-azure-cli"></a>Anmelden bei Azure mit der Azure CLI

Führen Sie die Azure CLI mit dem Befehl `az` aus. Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az_login), um sich anzumelden.

[!INCLUDE [interactive-login](interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](../authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können. Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="no-module-issue-on-ubuntu-2004-focalwsl"></a>Problem vom Typ „Kein Modul“ unter Ubuntu 20.04 (Focal)/WSL

Wenn Sie `azure-cli` unter `Focal` installiert haben, ohne das Azure CLI-Softwarerepository in [Schritt 3](#set-release) der Anweisungen für die manuelle Installation hinzuzufügen oder unser [Skript](#option-1-install-with-one-command) zu verwenden, treten unter Umständen Probleme auf, etwa das Problem „Kein Modul mit dem Namen 'decorator' or 'antlr4'“. Das ist darauf zurückzuführen, dass es sich beim installierten Paket um das veraltete Paket `azure-cli 2.0.81` aus dem Repository `focal/universe` handelt. Entfernen Sie das Paket zuerst, indem Sie `sudo apt remove azure-cli -y && sudo apt autoremove -y` ausführen. Befolgen Sie anschließend die obigen [Anweisungen](#install) zum Installieren des aktuellen `azure-cli`-Pakets.

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

[!INCLUDE[configure-proxy](configure-proxy.md)]

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

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a>Aktualisieren
[!INCLUDE [az-upgrade](az-upgrade.md)]

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

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

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

---
title: Installieren der Azure CLI unter Linux mit apt
description: Installieren der Azure CLI mit dem apt-Paket-Manager
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/27/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 1973c933cbffa494cbe9c0749346450251feefcb
ms.sourcegitcommit: 9bd90875a324908ec7195fc4c4f63ebf124760f9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/02/2019
ms.locfileid: "53982585"
---
# <a name="install-azure-cli-with-apt"></a>Installieren der Azure CLI mit apt

Wenn Sie eine Distribution mit `apt` verwenden (etwa Ubuntu oder Debian), steht ein 64-Bit-Paket für die Azure CLI zur Verfügung. Dieses Paket wurde mit Folgendem getestet:

* Ubuntu Trusty, Xenial, Artful und Bionic
* Debian Wheezy, Jessie und Stretch

## <a name="install"></a>Installieren

1. Installieren Sie die Pakete mit den erforderlichen Komponenten:

    ```bash
    sudo apt-get install apt-transport-https lsb-release software-properties-common dirmngr -y
    ```

2. <div id="set-release"/>Ändern Sie die Quellenliste:

    ```bash
    AZ_REPO=$(lsb_release -cs)
    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
    ```

3. <div id="signingKey"/>Rufen Sie den Microsoft-Signaturschlüssel ab:

   ```bash
   sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
        --keyserver packages.microsoft.com \
        --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
   ```

4. Installieren Sie die Befehlszeilenschnittstelle:

   ```bash
   sudo apt-get update
   sudo apt-get install azure-cli
   ```

   > [!WARNING]
   > Der Signaturschlüssel wurde im Mai 2018 aktualisiert und ersetzt. Sollten Fehler beim Signieren auftreten, vergewissern Sie sich, dass Sie den [aktuellen Signaturschlüssel](#signingKey) besitzen.

Sie können dann die Azure CLI mit dem Befehl `az` ausführen. Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `apt` auftreten können. Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="lsbrelease-does-not-return-the-correct-base-distribution-version"></a>„lsb_release“ gibt nicht die richtige Basisdistributionsversion zurück.

Einige von Ubuntu oder Debian abgeleiteten Distributionen wie Linux Mint geben über `lsb_release` unter Umständen nicht den richtigen Versionsnamen zurück. Mit diesem Wert wird im Installationsprozess das zu installierende Pakete ermittelt. Wenn Sie den Namen der Version kennen, von der Ihre Distribution abgeleitet ist, können Sie im [Installationsschritt 2](#set-release) den Wert `AZ_REPO` manuell festlegen. Sehen Sie sich andernfalls Informationen dazu an, wie Sie für Ihre Distribution den Basisdistributionsnamen ermitteln, und legen Sie `AZ_REPO` auf den richtigen Wert fest.

### <a name="no-package-for-your-distribution"></a>Kein Paket für Ihre Distribution

Manchmal dauert es nach der Veröffentlichung einer Ubuntu-Distribution etwas, bis ein Azure CLI-Paket dafür zur Verfügung gestellt wird. Die Azure CLI ist im Hinblick auf zukünftige Abhängigkeitsversionen resilient konzipiert und nutzt daher möglichst wenige dieser Abhängigkeiten. Ist für Ihre Basisdistribution kein Paket verfügbar, verwenden Sie ein Paket für eine ältere Distribution.

Legen Sie dazu im [Installationsschritt 1](#install-step-1) den Wert für `AZ_REPO` manuell fest. Verwenden Sie für Ubuntu-Distributionen das Repository `bionic` und für Debian-Distributionen `stretch`. Distributionen, die vor Ubuntu Trusty und Debian Wheezy veröffentlicht wurden, werden nicht unterstützt.

### <a name="apt-key-fails-with-no-dirmngr"></a>Fehler „No dirmngr“ beim Ausführen von „apt-key“

Beim Ausführen des Befehls `apt-key` wird unter Umständen eine Ausgabe wie die folgende angezeigt:

```output
gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory
gpg: connecting dirmngr at '/tmp/apt-key-gpghome.kt5zo27tp1/S.dirmngr' failed: No such file or directory
gpg: keyserver receive failed: No dirmngr
```

Dieser Fehler ist auf eine fehlende Komponente zurückzuführen, die von `apt-key` benötigt wird. Das Problem lässt sich durch Installieren des Pakets `dirmngr` beheben.

```bash
sudo apt-get install dirmngr
```

Wenn Sie mit einem Windows-Subsystem für Linux (WSL) arbeiten, wird dieser Fehler auch für ältere Windows-Versionen als Windows 10 1809 angezeigt. Aktualisieren Sie Ihre Version von Windows, um das Problem zu beheben.

### <a name="apt-key-hangs"></a>Keine Reaktion von „apt-key“

Wenn hinter einer Firewall ausgehende Verbindungen mit Port 11371 blockiert werden, hängt der Befehl `apt-key` unter Umständen auf unbestimmte Zeit.
Für Ihre Firewall ist möglicherweise ein HTTP-Proxy für ausgehende Verbindungen erforderlich:

```bash
sudo apt-key --keyring /etc/apt/trusted.gpg.d/Microsoft.gpg adv \
    --keyserver-options http-proxy=http://<USER>:<PASSWORD>@<PROXY-HOST>:<PROXY-PORT>/ \
    --keyserver packages.microsoft.com \
    --recv-keys BC528686B50D79E339D3721CEB3E94ADBE1229CF
```

Um zu ermitteln, ob ein Proxy eingerichtet ist, wenden Sie sich an Ihren Systemadministrator. Wenn für den Proxy keine Anmeldung erforderlich ist, lassen Sie Benutzer und Kennwort weg.

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>Aktualisieren

Verwenden Sie `apt-get upgrade` zum Aktualisieren des CLI-Pakets.

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!WARNING]
> Der Signaturschlüssel wurde im Mai 2018 aktualisiert und ersetzt. Sollten Fehler beim Signieren auftreten, vergewissern Sie sich, dass Sie den [aktuellen Signaturschlüssel](#signingKey) besitzen.
>
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
    sudo rm /etc/apt/trusted.gpg.d/Microsoft.gpg
    ```

4. Entfernen Sie alle nicht benötigten Pakete:

   ```bash
   sudo apt autoremove
   ```

## <a name="next-steps"></a>Nächste Schritte

Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)

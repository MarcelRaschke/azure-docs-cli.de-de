---
title: Installieren der Azure CLI unter Linux mit zypper
description: Installieren der Azure CLI mit zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 84946fc0562e396ef296cbe8dede5e6a65cd6614
ms.sourcegitcommit: 5a29ce9c0a3d7b831f22b1a13b1ae2e239e5549f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/19/2019
ms.locfileid: "71143962"
---
# <a name="install-azure-cli-with-zypper"></a>Installieren der Azure CLI mit zypper

Für Linux-Distributionen mit `zypper` wie openSUSE oder SLES ist ein Paket für die Azure CLI verfügbar. Dieses Paket wurde mit openSUSE 42.2 und höher sowie mit SLES 12 SP 2 und höher getestet.

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a>Installieren

1. Installieren Sie `curl`:

   ```bash
   sudo zypper install -y curl
   ```

2. Importieren Sie den Microsoft-Repositoryschlüssel:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. Erstellen Sie lokale `azure-cli`-Repositoryinformationen:

   ```bash
   sudo zypper addrepo --name 'Azure CLI' --check https://packages.microsoft.com/yumrepos/azure-cli azure-cli
   ```

4. Aktualisieren Sie den `zypper`-Paketindex, und führen Sie die Installation durch:

   ```bash
   sudo zypper install --from azure-cli -y azure-cli
   ```

Sie können dann die Azure CLI mit dem Befehl `az` ausführen. Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `zypper` auftreten können. Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="proxy-blocks-connection"></a>Der Proxy blockiert die Verbindung.

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

Konfigurieren Sie `zypper` (über `yast2`) explizit so, dass dieser Proxy immer verwendet wird. Führen Sie hierfür den Befehl `yast2 proxy` als Superuser aus, und geben Sie die Informationen im Formular ein. Wenn auf Ihrem System ein Fenster-Manager verfügbar ist, können Sie auch den Bereich `Network Services > Proxy` in `YaST Control Center` verwenden.

Details zur erweiterten Konfiguration oder weitere Informationen finden Sie in der [Dokumentation zur OpenSUSE-Proxykonfiguration](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html).

Zum Abrufen des Microsoft-Signaturschlüssels und des Pakets von unserem Repository muss Ihr Proxy HTTPS-Verbindungen mit den folgenden Adressen zulassen:

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>Aktualisieren

Sie können das Paket mit dem Befehl `zypper update` aktualisieren.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Entfernen Sie das Paket aus Ihrem System.

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.

   ```bash
   sudo zypper removerepo azure-cli
   ```

3. Wenn Sie keine anderen Microsoft-Pakete verwenden, entfernen Sie den Microsoft-Signaturschlüssel.

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a>Nächste Schritte

Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)

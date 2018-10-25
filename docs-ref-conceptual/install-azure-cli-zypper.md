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
ms.devlang: azure-cli
ms.openlocfilehash: a73576a9caeb7d016f49bb1d90f1903cbd515c63
ms.sourcegitcommit: 6d9169ed547df151f99e5a3ac86578634486419a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/23/2018
ms.locfileid: "49652446"
---
# <a name="install-azure-cli-with-zypper"></a>Installieren der Azure CLI mit zypper

Für Linux-Distributionen mit `zypper` wie openSUSE oder SLES ist ein Paket für die Azure CLI verfügbar. Dieses Paket wurde mit openSUSE 42.2 und SLES 12 SP 2 getestet.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

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

3. Entfernen Sie auch den Microsoft GPG-Signaturschlüssel, falls Sie die Repositoryinformationen entfernt haben.

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```
   ## <a name="next-steps"></a>Nächste Schritte

Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.

> [!div class="nextstepaction"]
> [Erste Schritte mit Azure CLI 2.0](get-started-with-azure-cli.md)

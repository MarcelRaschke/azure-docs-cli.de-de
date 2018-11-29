---
title: Installieren der Azure CLI unter Linux mit yum
description: Installieren der Azure CLI mit yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7e2c7c5477c8d5a617875eeaed8e3d267d9bcf8c
ms.sourcegitcommit: a8aac038e6ede0b1b352ca6163a04b61ff4eed5b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/28/2018
ms.locfileid: "52450308"
---
# <a name="install-azure-cli-with-yum"></a>Installieren der Azure CLI mit yum

Für Linux-Distributionen mit `yum` (etwa RHEL, Fedora oder CentOS) ist ein Paket für die Azure CLI verfügbar. Dieses Paket wurde mit RHEL 7, Fedora 19 (und höher) und CentOS 7 getestet.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Installieren

1. Importieren Sie den Microsoft-Repositoryschlüssel.

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Erstellen Sie lokale `azure-cli`-Repositoryinformationen.

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. Installieren Sie mit dem Befehl `yum install`.

   ```bash
   sudo yum install azure-cli
   ```

Sie können dann die Azure CLI mit dem Befehl `az` ausführen. Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `yum` auftreten können. Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>Aktualisieren

Aktualisieren Sie die Azure CLI mit dem Befehl `yum update`.

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Entfernen Sie das Paket aus Ihrem System.

   ```bash
   sudo yum remove azure-cli
   ```

2. Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
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

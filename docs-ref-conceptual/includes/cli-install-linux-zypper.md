---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: include
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: d80970432a116656a33a3dc6c0d4909b4b92f312
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744636"
---
## <a name="overview"></a>Übersicht

Für Linux-Distributionen mit `zypper` wie openSUSE oder SLES ist ein Paket für die Azure CLI verfügbar. Dieses Paket wurde mit openSUSE Leap 15.1 und SLES 15 getestet.

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

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
   sudo zypper install --from azure-cli azure-cli
   ```

   2 eingeben, um die Installation fortzusetzen, indem einige Abhängigkeiten ignoriert werden.

Sie können dann die Azure CLI mit dem Befehl `az` ausführen. Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.

[!INCLUDE [interactive-login](interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](../authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `zypper` auftreten können. Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="notimplementederror-on-opensuse-15-vm"></a>NotImplementedError auf OpenSUSE 15-VM
Auf der OpenSUSE 15-VM ist die Azure CLI mit Version `2.0.45` vorinstalliert. Diese ist veraltet, und es treten Probleme mit `az login` auf. Entfernen Sie sie zusammen mit den zugehörigen Abhängigkeiten, bevor Sie die [Installationsanweisungen](#install) zum Hinzufügen der aktuellen Azure CLI befolgen:

```bash
sudo zypper rm -y --clean-deps azure-cli
```

Wenn Sie die Azure CLI aktualisiert haben, ohne die Abhängigkeiten von Version `2.0.45` zu entfernen, beeinträchtigen die alten Abhängigkeiten unter Umständen die aktuelle Version der Azure CLI. Sie müssen die alte Version wieder hinzufügen, um eine Verknüpfung mit ihren Abhängigkeiten herzustellen, und anschließend `azure-cli` zusammen mit den Abhängigkeiten entfernen:

```bash
# The package name may vary on different system version, run 'zypper --no-refresh info azure-cli' to check the source package format
sudo zypper install --oldpackage azure-cli-2.0.45-4.22.noarch

sudo zypper rm -y --clean-deps azure-cli
```

### <a name="install-on-sles-12-or-other-systems-without-python-36"></a>Installieren auf SLES 12 oder anderen Systemen ohne Python 3.6

Unter SLES 12 ist `3.4` das standardmäßige `python3`-Paket und wird von der Azure CLI nicht unterstützt. Sie können zuerst die Schritte 1 bis 3 der [Installationsanweisungen](#install) ausführen, um das Repository `azure-cli` hinzuzufügen. Erstellen Sie dann eine höhere Version von `python3` aus der Quelle. Abschließend können Sie das Azure CLI-Paket herunterladen und ohne Abhängigkeit installieren.

Sie können den folgenden Befehl verwenden, um die Azure CLI zu installieren. (Beachten Sie, dass Ihre vorhandene Python 3-Version von Python 3.6 überschrieben wird.)

```bash
curl -sL https://azurecliprod.blob.core.windows.net/sles12_install.sh | sudo bash
```

Alternativ können Sie Schritt für Schritt vorgehen:

```bash
# !Please add azure-cli repository first following step 1-3 of the install instruction before running below commands
$ sudo zypper refresh
$ sudo zypper install -y gcc gcc-c++ make ncurses patch wget tar zlib-devel zlib openssl-devel
# Download Python source code
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
# Build Python
# Please be aware that with --prefix=/usr, the command will override the existing Python 3 version
$ $PYTHON_SRC_DIR/*/configure --prefix=/usr
$ make
$ sudo make install
# Download azure-cli package 
$ AZ_VERSION=$(zypper --no-refresh info azure-cli |grep Version | awk -F': ' '{print $2}' | awk '{$1=$1;print}')
$ wget https://packages.microsoft.com/yumrepos/azure-cli/azure-cli-$AZ_VERSION.x86_64.rpm
# Install without dependency
$ sudo rpm -ivh --nodeps azure-cli-$AZ_VERSION.x86_64.rpm
```

### <a name="proxy-blocks-connection"></a>Der Proxy blockiert die Verbindung.

[!INCLUDE[configure-proxy](configure-proxy.md)]

Konfigurieren Sie `zypper` (über `yast2`) explizit so, dass dieser Proxy immer verwendet wird. Führen Sie hierfür den Befehl `yast2 proxy` als Superuser aus, und geben Sie die Informationen im Formular ein. Wenn auf Ihrem System ein Fenster-Manager verfügbar ist, können Sie auch den Bereich `Network Services > Proxy` in `YaST Control Center` verwenden.

Details zur erweiterten Konfiguration oder weitere Informationen finden Sie in der [Dokumentation zur OpenSUSE-Proxykonfiguration](https://www.suse.com/documentation/slms1/book_slms/data/sec_wy_config_updates_proxy.html).

Zum Abrufen des Microsoft-Signaturschlüssels und des Pakets von unserem Repository muss Ihr Proxy HTTPS-Verbindungen mit den folgenden Adressen zulassen:

* `https://packages.microsoft.com`
* `https://download.opensuse.org`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

### <a name="ssl-certificate-problem"></a>SSL-Zertifikatproblem

Wenn ein Zertifikat auf einem Computer beschädigt oder veraltet ist, erhalten Sie möglicherweise eine Fehlermeldung, die besagt, dass curl die Legitimität des Servers nicht verifizieren konnte und daher keine sichere Verbindung herstellen konnte.  Aktualisieren Sie Ihr Zertifikat, um das Problem zu beheben.  

```bach
sudo zypper update-ca-certificates
```

## <a name="update"></a>Aktualisieren

[!INCLUDE [az-upgrade](az-upgrade.md)]

Sie können das Paket auch mit dem Befehl `zypper update` aktualisieren.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

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

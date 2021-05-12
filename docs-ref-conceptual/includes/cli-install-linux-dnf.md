---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/24/2020
ms.topic: include
ms.custom: devx-track-azurecli
ms.openlocfilehash: 6044626c584eba4fd4ec55e11314cb89e20b3417
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2021
ms.locfileid: "105582687"
---
## <a name="overview"></a>Übersicht

Für Linux-Distributionen mit `dnf` (etwa RHEL, Fedora oder CentOS) ist ein Paket für die Azure CLI verfügbar. Dieses Paket wurde mit RHEL 7.7, RHEL 8, Fedora 24 (und höher), CentOS 7 und CentOS 8 getestet.

[!INCLUDE [current-version](current-version.md)]

[!INCLUDE [rpm-warning](rpm-warning.md)]

> [!NOTE]
>
> Nutzen Sie bei Verwendung von Linux-Systemen, die den `dnf`-Paket-Manager nicht unterstützen, den `yum`-Paket-Manager.

## <a name="install"></a>Installieren

1. Importieren Sie den Microsoft-Repositoryschlüssel.

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Erstellen Sie lokale `azure-cli`-Repositoryinformationen.

   ```bash
   echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" | sudo tee /etc/yum.repos.d/azure-cli.repo
   ```

3. Installieren Sie mit dem Befehl `dnf install`.

   ```bash
   sudo dnf install azure-cli
   ```
 
Führen Sie die Azure CLI mit dem Befehl `az` aus. Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az_login), um sich anzumelden.


[!INCLUDE [interactive-login](interactive-login.md)]

Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](../authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Problembehandlung

In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation mit `dnf` auftreten können. Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="install-on-rhel-76-or-other-systems-without-python-3"></a>Installieren auf RHEL 7.6 oder anderen Systemen ohne Python 3

Führen Sie wenn möglich ein Upgrade Ihres Systems auf eine Version mit offizieller Unterstützung für `python 3.6+`-Pakete durch. Andernfalls müssen Sie zuerst ein `python3`-Paket und dann die Azure CLI ohne Abhängigkeit installieren.

Sie können den folgenden Befehl verwenden, um die Azure CLI mit dem aus der Quelle erstellten `python 3.6`-Paket zu installieren:

```bash
curl -sL https://azurecliprod.blob.core.windows.net/rhel7_6_install.sh | sudo bash
```

Sie können auch Schritt für Schritt vorgehen:

Die Azure CLI erfordert zuerst `SSL 1.1+`, und Sie müssen `openssl 1.1` aus der Quelle erstellen, bevor Sie `python3` erstellen:

```bash
$ sudo dnf install gcc gcc-c++ make ncurses patch wget tar zlib zlib-devel -y
# build openssl from source
$ cd ~
$ wget https://www.openssl.org/source/openssl-1.1.1d.tar.gz
$ tar -xzf openssl-1.1.1d.tar.gz
$ cd openssl-1.1.1d
$ ./config --prefix=/usr/local/ssl --openssldir=/usr/local/ssl
$ make
$ sudo make install
# configure shared object lookup directory so that libssl.so.1.1 can be found
$ echo "/usr/local/ssl/lib" | sudo tee /etc/ld.so.conf.d/openssl-1.1.1d.conf
# reload config
$ sudo ldconfig -v
```

Erstellen Sie anschließend Python 3 aus der Quelle:

```bash
$ PYTHON_VERSION="3.6.9"
$ PYTHON_SRC_DIR=$(mktemp -d)
$ wget -qO- https://www.python.org/ftp/python/$PYTHON_VERSION/Python-$PYTHON_VERSION.tgz | tar -xz -C "$PYTHON_SRC_DIR"
$ cd $PYTHON_SRC_DIR/Python-$PYTHON_VERSION
$ ./configure --prefix=/usr --with-openssl=/usr/local/ssl
$ make
$ sudo make install
```

Führen Sie schließlich Schritt 1 und 2 der [Installationsanweisungen](#install) aus, um das Azure CLI-Repository hinzuzufügen. Nun können Sie das Paket herunterladen und ohne Abhängigkeit installieren.

> [!NOTE]
>
> Falls Sie das dnf-Download-Plug-In nicht installiert haben, wird beim Ausführen des unten angegebenen Codes der Fehler „Befehl nicht gefunden“ angezeigt. Verwenden Sie `dnf install 'dnf-command(download)'` zum Installieren des dnf-Download-Plug-Ins.

```bash
$ sudo dnf download azure-cli
$ sudo rpm -ivh --nodeps azure-cli-*.rpm
```

Als Alternative können Sie Python 3 auch über ein [zusätzliches Repository](https://developers.redhat.com/blog/2018/08/13/install-python3-rhel/) installieren. Wenn Sie `python3` eingerichtet haben, aber weiterhin den Fehler `python3: command not found` erhalten, wenn Sie versuchen, die CLI auszuführen, müssen Sie sie bei dieser Vorgehensweise dem Pfad hinzufügen.

```bash
$ scl enable rh-python36 bash
```

### <a name="proxy-blocks-connection"></a>Der Proxy blockiert die Verbindung.

[!INCLUDE[configure-proxy](configure-proxy.md)]

Konfigurieren Sie `dnf` explizit so, dass dieser Proxy immer verwendet wird. Stellen Sie sicher, dass die folgenden Zeilen im Abschnitt `[main]` von `/etc/dnf/dnf.conf` erscheinen:

```dnf.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

Zum Abrufen des Microsoft-Signaturschlüssels und des Pakets von unserem Repository muss Ihr Proxy HTTPS-Verbindungen mit der folgenden Adresse zulassen:

* `https://packages.microsoft.com`

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="update"></a>Aktualisieren

[!INCLUDE [az-upgrade](az-upgrade.md)]

Sie können die Azure CLI auch mit dem Befehl `dnf update` aktualisieren.

```bash
sudo dnf update azure-cli
```

## <a name="uninstall"></a>Deinstallieren

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

1. Entfernen Sie das Paket aus Ihrem System.

   ```bash
   sudo dnf remove azure-cli
   ```

2. Entfernen Sie die Repositoryinformationen, wenn Sie nicht planen, die CLI neu zu installieren.

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. Wenn Sie keine anderen Microsoft-Pakete verwenden, entfernen Sie den Signaturschlüssel.

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

---
title: Azure CLI-Aliaserweiterung
description: Verwenden der Azure CLI-Aliaserweiterung
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/07/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 576ed223887ff9a20cf5015d96ee4c949576d653
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/09/2020
ms.locfileid: "89562837"
---
# <a name="the-azure-cli-alias-extension"></a>Azure CLI-Aliaserweiterung

Dank der Aliaserweiterung können Benutzer mithilfe von vorhandenen Befehlen benutzerdefinierte Befehle für die Azure CLI definieren. Aliase ermöglichen die Verwendung von Verknüpfungen und vereinfachen dadurch Ihren Workflow. Aliase werden von der Jinja2-Vorlagenengine unterstützt und bieten daher sogar erweiterte Argumentverarbeitung.

> [!NOTE]
> Die Aliaserweiterung ist als öffentliche Vorschauversion verfügbar. Die Funktionen und das Konfigurationsdateiformat können sich ändern.

## <a name="install-the-alias-extension"></a>Installieren der Aliaserweiterung

Damit Sie die Aliaserweiterung verwenden können, ist mindestens Version **2.0.28** der Azure CLI erforderlich. Führen Sie zum Überprüfen der CLI-Version `az --version` aus. Falls Sie die Installation aktualisieren müssen, hilft Ihnen die Anleitung unter [Installieren der Azure CLI](./install-azure-cli.md) weiter.

Installieren Sie die Erweiterung mit dem Befehl [az extension add](/cli/azure/extension#az-extension-add).

```azurecli-interactive
az extension add --name alias
```

Überprüfen Sie die Installation der Erweiterung mithilfe von [az extension list](/cli/azure/extension#az-extension-list). Wenn die Aliaserweiterung ordnungsgemäß installiert wurde, ist sie in der Befehlsausgabe aufgeführt.

```azurecli-interactive
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```

## <a name="keep-the-extension-up-to-date"></a>Sicherstellen, dass die Erweiterung immer auf dem neuesten Stand ist

Die Aliaserweiterung befindet sich in der aktiven Entwicklung, und es werden regelmäßig neue Versionen veröffentlicht. Beim Aktualisieren der CLI werden keine neuen Versionen installiert. Installieren Sie die Updates für die Erweiterung mithilfe von [az extension update](/cli/azure/extension#az-extension-update).

```azurecli-interactive
az extension update --name alias
```

## <a name="manage-aliases-for-the-azure-cli"></a>Verwalten von Aliasen für die Azure CLI

Die Aliaserweiterung ermöglicht das Erstellen und Verwalten von Aliasen für andere CLI-Befehle. Führen Sie den Aliasbefehl mit `--help` aus, um alle verfügbaren Befehle und Parameterdetails anzuzeigen.

```azurecli-interactive
az alias --help
```

## <a name="create-simple-alias-commands"></a>Erstellen einfacher Aliasbefehle

Zum einen werden Aliase zum Kürzen vorhandener Befehlsgruppen oder Befehlsnamen verwendet. Beispielsweise können Sie die Befehlsgruppe `group` auf `rg` und den Befehl `list` auf `ls` verkürzen.

```azurecli-interactive
az alias create --name rg --command group
az alias create --name ls --command list
```

Diese neu definierten Aliase können nun anstelle ihrer Definition verwendet werden.

```azurecli-interactive
az rg list
az rg ls
az vm ls
```

Nehmen Sie `az` nicht in den Befehl auf.

Aliase können auch als Verknüpfungen für vollständige Befehle fungieren. Im nächsten Beispiel werden verfügbare Ressourcengruppen und ihre Speicherorte in der Tabellenausgabe aufgeführt:

```azurecli-interactive
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

`ls-groups` kann nun wie jeder andere CLI-Befehl ausgeführt werden.

```azurecli-interactive
az ls-groups
```

## <a name="create-an-alias-command-with-arguments"></a>Erstellen eines Aliasbefehls mit Argumenten

Sie können positionelle Argumente auch zu einem Aliasbefehl hinzufügen, indem Sie sie als `{{ arg_name }}` in den Aliasnamen aufnehmen. Das Leerzeichen in den Klammern ist erforderlich.

```azurecli-interactive
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

Das nächste Beispiel zeigt, wie Sie mithilfe von positionellen Argumenten die öffentliche IP-Adresse für einen virtuellen Computer abrufen.

```azurecli-interactive
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

Beim Ausführen dieses Befehls übergeben Sie Werte an die positionellen Argumente.

```azurecli-interactive
az get-vm-ip MyResourceGroup MyVM
```

Sie können in Aliasbefehlen auch Umgebungsvariablen verwenden, die zur Laufzeit ausgewertet werden. Im nächsten Beispiel wird der Alias `create-rg` hinzugefügt, der eine Ressourcengruppe in `eastus` erstellt und ein `owner`-Tag hinzufügt. Diesem Tag wird der Wert der lokalen Umgebungsvariablen `USER` zugewiesen.

```azurecli-interactive
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

Zum Registrieren der Umgebungsvariablen im Befehl des Alias muss das Dollarzeichen (`$`) mit Escapezeichen versehen werden.

## <a name="process-arguments-using-jinja2-templates"></a>Verarbeiten von Argumenten mithilfe von Jinja2-Vorlagen

Die Argumentersetzung in der Aliaserweiterung wird von [Jinja2](http://jinja.pocoo.org/docs/2.10/) durchgeführt. Jinja2-Vorlagen ermöglichen die Bearbeitung der Argumente.

Mit Jinja2-Vorlagen können Sie Aliase schreiben, die andere Argumenttypen akzeptieren als der zugrunde liegende Befehl. Beispielsweise können Sie einen Alias erstellen, der eine Speicher-URL übernimmt. Anschließend wird diese URL analysiert, um den Konto- und Containernamen an den Speicherbefehl zu übergeben.

```azurecli-interactive
az alias create \
    --name 'storage-ls {{ url }}' \
    --command "storage blob list
        --account-name {{ url.replace('https://', '').split('.')[0] }}
        --container-name {{ url.replace('https://', '').split('/')[1] }}"
```

Informationen zur Jinja2-Vorlagenengine finden Sie in der [Jinja2-Dokumentation](http://jinja.pocoo.org/docs/2.10/templates/).

## <a name="alias-configuration-file"></a>Aliaskonfigurationsdatei

Eine weitere Möglichkeit zum Erstellen und Ändern von Aliasen ist das Ändern der Aliaskonfigurationsdatei. Aliasbefehlsdefinitionen werden in eine Konfigurationsdatei unter `$AZURE_USER_CONFIG/alias` geschrieben. `AZURE_USER_CONFIG` hat standardmäßig den Wert `$HOME/.azure` (macOS und Linux) bzw. `%USERPROFILE%\.azure` (Windows). Die Aliaskonfigurationsdatei wird im INI-Konfigurationsdateiformat geschrieben. Das Format für Aliasbefehle lautet wie folgt:

```ini
[alias_name]
command = invoked_commands
```

Für Aliase, die positionelle Argumente enthalten, haben die Aliasbefehle das folgende Format:

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```

## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a>Erstellen eines Aliasbefehls mit Argumenten über die Aliaskonfigurationsdatei

Das nächste Beispiel zeigt einen Alias für einen Befehl mit Argumenten. Dieser Befehl ruft die öffentliche IP-Adresse für einen virtuellen Computer ab. Aliasbefehle müssen sich in einer Zeile befinden und alle Argumente im Aliasnamen verwenden.

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```

## <a name="uninstall-the-alias-extension"></a>Deinstallieren der Aliaserweiterung

Verwenden Sie zum Deinstallieren der Erweiterung den Befehl [az extension remove](/cli/azure/extension#az-extension-remove).

```azurecli-interactive
az extension remove --name alias
```

Falls Sie die Erweiterung aufgrund eines Fehlers oder eines anderen Problems deinstalliert haben, melden Sie das Problem über [GitHub](https://github.com/Azure/azure-cli-extensions/issues), damit wir eine Lösung bereitstellen können.

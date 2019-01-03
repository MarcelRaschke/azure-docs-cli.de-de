---
title: Erste Schritte mit der Azure CLI
description: Erste Schritte mit der Azure CLI durch das Erlernen der Befehlsgrundlagen.
keywords: Azure CLI, CLI Hilfe, Azure Hilfe, Abfrage, Automatisierung,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: a56ce4acf070c17d8deaec9674593ba930cca70f
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593607"
---
# <a name="get-started-with-azure-cli"></a>Erste Schritte mit der Azure CLI

Willkommen bei der Azure CLI! Die CLI ist ein Tool, das die schnelle und effiziente Verwendung von Azure-Diensten ermöglichen soll. Der Fokus liegt dabei auf der Automatisierung. Dieser Artikel stellt Features der CLI vor und enthält Links zu Ressourcen, die Sie dabei unterstützen, produktiv zu sein.

## <a name="install-or-run-in-azure-cloud-shell"></a>Installieren oder Ausführen in Azure Cloud Shell

Am einfachsten können Sie die Azure-Befehlszeilenschnittstelle in einer Azure Cloud Shell-Umgebung über Ihren Browser verwenden. Informationen zu Cloud Shell finden Sie unter [Schnellstart für Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).

Wenn Sie zur Installation der Befehlszeilenschnittstelle bereit sind, lesen Sie die [Installationsanweisungen](install-azure-cli.md).

## <a name="sign-in"></a>Anmelden

Bevor Sie CLI-Befehle mit einer lokalen Installation verwenden, müssen Sie sich mithilfe von [az login](/cli/azure/reference-index#az-login) anmelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Es gibt auch Wege, wie Sie sich nicht interaktiv anmelden können. Diese werden unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md) ausführlich beschrieben.

## <a name="common-commands"></a>Häufig verwendete Befehle

Die folgende Tabelle enthält einige allgemeine Befehle, die in der CLI verwendet werden, sowie Links zu ihrer Referenzdokumentation.

| Ressourcentyp | Azure CLI-Befehlsgruppe |
|---------------|-------------------------|
| [Ressourcengruppe](/azure/azure-resource-manager/resource-group-overview) | [az group](/cli/azure/group) |
| [Virtuelle Computer](/azure/virtual-machines) | [az vm](/cli/azure/vm) |
| [Speicherkonten](/azure/storage/common/storage-introduction) | [az storage account](/cli/azure/storage/account) |
| [Schlüsseltresor](/azure/key-vault/key-vault-whatis) | [az keyvault](/cli/azure/keyvault) |
| [Webanwendungen](/azure/app-service) | [az webapp](/cli/azure/webapp) |
| [SQL-Datenbanken](/azure/sql-database) | [az sql server](/cli/azure/sql/server) |
| [CosmosDB](/azure/cosmos-db) | [az cosmosdb](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a>Suchen von Befehlen

Befehle in der CLI werden als _Befehle_ von _Gruppen_ organisiert. Jede Gruppe stellt einen Azure-Dienst dar, und Befehle werden für diesen Dienst ausgeführt.

Suchen Sie Befehle mithilfe von [az find](/cli/azure/reference-index#az-find). Verwenden Sie den folgenden Befehl, um beispielsweise nach Befehlsnamen zu suchen, die `secret` enthalten:

```azurecli-interactive
az find -q secret
```

Verwenden Sie das Argument `--help`, um eine vollständige Liste der Befehle und Untergruppen einer Gruppe abzurufen. Geben Sie beispielsweise Folgendes ein, um die CLI-Befehle für die Verwendung mit Netzwerksicherheitsgruppen (NSGs) zu ermitteln:

```azurecli-interactive
az network nsg --help
```

Die CLI ermöglicht unter der Bash-Shell die Vervollständigung mit der TAB-TASTE.

## <a name="globally-available-arguments"></a>Global verfügbare Argumente

Es gibt einige Argumente, die für jeden Befehl verfügbar sind.

* `--help` gibt CLI-Referenzinformationen zu Befehlen und ihren Argumenten zurück und führt verfügbare Untergruppen und Befehle auf.
* `--output` ändert das Ausgabeformat. Verfügbare Ausgabeformate: `json`, `jsonc` (farbiger JSON-Code), `tsv` (per Tabulator getrennte Werte) und `table` (für Menschen lesbare ASCII-Tabellen). Die CLI gibt standardmäßig `json` aus. Weitere Informationen zu den verfügbaren Ausgabeformaten finden Sie unter [Ausgabeformate für die Azure CLI](format-output-azure-cli.md).
* `--query` verwendet die [JMESPath-Abfragesprache](http://jmespath.org/) zum Filtern der von Azure-Diensten zurückgegebenen Ausgabe. Weitere Informationen zu Abfragen finden Sie unter [Abfragen von Befehlsergebnissen mit der Azure CLI](query-azure-cli.md) und im [JMESPath-Tutorial](http://jmespath.org/tutorial.html).
* `--verbose` gibt Informationen zu Ressourcen, die in Azure während eines Vorgangs erstellt werden, und andere nützliche Informationen aus.
* `--debug` gibt noch mehr Informationen zu CLI-Vorgängen aus, die zum Debuggen verwendet werden. Wenn ein Fehler auftritt, stellen Sie beim Übermitteln eines Fehlerberichts die mit dem Flag `--debug` generierte Ausgabe bereit.

## <a name="interactive-mode"></a>Interaktiver Modus

Die CLI bietet einen interaktiven Modus, der automatisch Hilfeinformationen anzeigt und die Auswahl von Unterbefehlen vereinfacht. Sie wechseln mit dem Befehl [az interactive](/cli/azure/reference-index#az-interactive) in den interaktiven Modus.

```azurecli-interactive
az interactive
```

Weitere Informationen zum interaktiven Modus finden Sie unter [Azure CLI – Interaktiver Modus](interactive-azure-cli.md).

Darüber hinaus gibt es ein [Visual Studio Code-Plug-In](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli), das eine interaktive Benutzeroberfläche bereitstellt. Diese bietet unter anderem Funktionen wie AutoVervollständigen und die Anzeigen von Informationen beim Daraufzeigen.

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a>Lernen der CLI-Grundlagen mit Schnellstarts und Tutorials

Sehen Sie sich zu den ersten Schritten mit der Azure CLI ein ausführliches Tutorial an, in dem Sie lernen, wie Sie virtuelle Computer einrichten und die Funktionen der CLI zum Abfragen von Azure-Ressourcen nutzen.

> [!div class="nextstepaction"]
> [Erstellen von virtuellen Computern mit der Azure CLI](azure-cli-vm-tutorial.yml)

Es gibt auch Schnellstartanleitungen für andere beliebte Dienste.

* [Erstellen eines Speicherkontos mit der Azure-Befehlszeilenschnittstelle](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* [Transfer objects to/from Azure Blob storage using the CLI](/azure/storage/blobs/storage-quickstart-blobs-cli) (Übertragen von Objekten in/aus Azure Blob Storage mit der CLI)
* [Erstellen einer einzelnen Azure SQL-Datenbank mithilfe der Azure CLI](/azure/sql-database/sql-database-get-started-cli)
* [Erstellen eines Azure Database for MySQL-Servers mithilfe der Azure CLI](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [Erstellen einer Azure-Datenbank für PostgreSQL mithilfe der Azure-CLI](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [Erstellen einer Python-Web-App in Azure](/azure/app-service/app-service-web-get-started-python)
* [Ausführen eines benutzerdefinierten Image von Docker-Hubs in Azure-Web-Apps für Container](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a>Abgeben von Feedback

Ihr Feedback zur CLI hilft uns dabei, Verbesserungen vorzunehmen und Fehler zu beheben. Sie können [ein Problem auf Github melden](https://github.com/azure/azure-cli/issues) oder mit den integrierten Features der CLI und dem Befehl [az feedback](/cli/azure/reference-index#az-feedback) allgemeines Feedback hinterlassen.

```azurecli-interactive
az feedback
```

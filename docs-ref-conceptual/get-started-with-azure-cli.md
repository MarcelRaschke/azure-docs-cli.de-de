---
title: Erste Schritte mit Azure CLI 2.0
description: Erste Schritte mit der Azure CLI 2.0 durch Kennenlernen der Befehlsgrundlagen.
keywords: Azure CLI, CLI Hilfe, Azure Hilfe, Abfrage, Automatisierung,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: f45c3acfdb4edb82cde755472d240ae18d82aba2
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967740"
---
# <a name="get-started-with-azure-cli-20"></a>Erste Schritte mit Azure CLI 2.0

Willkommen bei der Azure CLI 2.0! Die CLI ist ein Tool, das die schnelle und effiziente Verwendung von Azure-Diensten ermöglichen soll. Der Fokus liegt dabei auf der Automatisierung. Dieser Artikel stellt Features der CLI vor und enthält Links zu Ressourcen, die Sie dabei unterstützen, produktiv zu sein.

## <a name="install-and-sign-in"></a>Installieren und Anmelden

[Installieren Sie die CLI](install-azure-cli.md), sofern noch nicht geschehen, oder probieren Sie [Azure Cloud Shell](/azure/cloud-shell/overview) aus.

Bevor Sie CLI-Befehle mit einer lokalen Installation verwenden, müssen Sie sich mithilfe von [az login](/cli/azure/reference-index#az-login) anmelden.

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Es gibt Methoden, sich nicht interaktiv anzumelden. Diese werden unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md) ausführlich beschrieben.

## <a name="common-commands"></a>Häufig verwendete Befehle

In der nachfolgenden Tabelle sind einige der in der CLI häufig verwendeten Befehle als Links zu den Dokumentationsseiten in der Referenz aufgeführt.
Alle Unterbefehle dieser Gruppen und ihre Dokumentation können in der Onlinereferenz oder mit dem Argument `--help` nachgeschlagen werden.

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

Befehle in der CLI werden als _Unterbefehle_ von _Gruppen_ bereitgestellt.
Jede Gruppe stellt einen von Azure bereitgestellten Dienst dar, und die Untergruppen unterteilen Befehle für diese Dienste in logische Gruppierungen.

Suchen Sie Befehle mithilfe von [az find](/cli/azure/reference-index#az-find). Verwenden Sie den folgenden Befehl, um beispielsweise nach Befehlsnamen zu suchen, die `secret` enthalten:

```azurecli-interactive
az find -q secret
```

Wenn Sie wissen, mit welcher Gruppe von Befehlen Sie arbeiten möchten, ist das Argument `--help` unter Umständen besser geeignet. Damit werden nicht nur detaillierte Informationen für einen Befehl, sondern – bei Verwendung mit einer Befehlsgruppe – alle verfügbaren Unterbefehle angezeigt. Beispielsweise können Sie bei Verwendung von Netzwerksicherheitsgruppen (NSGs) die verfügbaren Untergruppen und Befehle der NSGs ermitteln.

```azurecli-interactive
az network nsg --help
```

Die CLI ermöglicht unter der Bash-Shell die Vervollständigung mit der TAB-TASTE.

## <a name="globally-available-arguments"></a>Global verfügbare Argumente

Es gibt einige Argumente, die für jeden Befehl verfügbar sind.

* `--help` gibt CLI-Referenzinformationen zu Befehlen und ihren Argumenten zurück und führt verfügbare Untergruppen und Befehle auf.
* `--output` ändert das Ausgabeformat. Verfügbare Ausgabeformate: `json`, `jsonc` (farbiger JSON-Code), `tsv` (per Tabulator getrennte Werte) und `table` (für Menschen lesbare ASCII-Tabellen). Die CLI gibt standardmäßig `json` aus. Weitere Informationen zu den verfügbaren Ausgabeformaten finden Sie unter [Ausgabeformate für Azure CLI 2.0-Befehle](format-output-azure-cli.md).
* `--query` verwendet die [JMESPath-Abfragesprache](http://jmespath.org/) zum Filtern der von Azure-Diensten zurückgegebenen Ausgabe. Weitere Informationen zu Abfragen finden Sie unter [Verwenden von JMESPath-Abfragen mit Azure CLI 2.0](query-azure-cli.md) und im [JMESPath-Tutorial](http://jmespath.org/tutorial.html).
* `--verbose` gibt Informationen zu Ressourcen, die in Azure während eines Vorgangs erstellt werden, und andere nützliche Informationen aus.
* `--debug` gibt noch mehr Informationen zu CLI-Vorgängen aus, die zum Debuggen verwendet werden. Wenn ein Fehler auftritt, stellen Sie beim Übermitteln eines Fehlerberichts die mit dem Flag `--debug` generierte Ausgabe bereit.

## <a name="interactive-mode"></a>Interaktiver Modus

Die CLI bietet einen interaktiven Modus, der automatisch Hilfeinformationen anzeigt und die Auswahl von Unterbefehlen vereinfacht. Sie wechseln mit dem Befehl [az interactive](/cli/azure/reference-index#az-interactive) in den interaktiven Modus.

```azurecli-interactive
az interactive
```

Weitere Informationen zum interaktiven Modus finden Sie unter [Interaktive Azure CLI 2.0](interactive-azure-cli.md).

Darüber hinaus gibt es ein [Visual Studio Code-Plug-In](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli), das eine interaktive Benutzeroberfläche bereitstellt. Diese bietet unter anderem Funktionen wie AutoVervollständigen und die Anzeige von Informationen beim Daraufzeigen.

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a>Lernen der CLI-Grundlagen mit Schnellstarts und Tutorials

Sehen Sie sich für die ersten Schritte mit der Azure CLI 2.0 ein ausführliches Tutorial an, in dem Sie lernen, wie Sie virtuelle Computer einrichten und die Funktionen der CLI zum Abfragen von Azure-Ressourcen nutzen.

> [!div class="nextstepaction"]
> [Erstellen von virtuellen Computern mit der Azure CLI 2.0](azure-cli-vm-tutorial.yml)

Wenn Sie sich eher auf andere Dienste konzentrieren möchten, stehen verschiedene Schnellstartanleitungen für Azure-Dienste zur Verfügung, die die CLI nutzen.

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

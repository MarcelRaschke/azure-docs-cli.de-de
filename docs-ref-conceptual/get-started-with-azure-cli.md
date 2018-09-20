---
title: Erste Schritte mit Azure CLI 2.0
description: Erste Schritte mit der Azure CLI 2.0 durch Kennenlernen der Befehlsgrundlagen.
keywords: Azure CLI, CLI Hilfe, Azure Hilfe, Abfrage, Automatisierung,
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 165da295d187edf7dbc19a332670fd49d8f8bdd5
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388557"
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="a3e85-104">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="a3e85-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="a3e85-105">Willkommen bei der Azure CLI 2.0!</span><span class="sxs-lookup"><span data-stu-id="a3e85-105">Welcome to the Azure CLI 2.0!</span></span> <span data-ttu-id="a3e85-106">Die CLI ist ein Tool, das die schnelle und effiziente Verwendung von Azure-Diensten ermöglichen soll. Der Fokus liegt dabei auf der Automatisierung.</span><span class="sxs-lookup"><span data-stu-id="a3e85-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="a3e85-107">Dieser Artikel stellt Features der CLI vor und enthält Links zu Ressourcen, die Sie dabei unterstützen, produktiv zu sein.</span><span class="sxs-lookup"><span data-stu-id="a3e85-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-and-sign-in"></a><span data-ttu-id="a3e85-108">Installieren und Anmelden</span><span class="sxs-lookup"><span data-stu-id="a3e85-108">Install and sign in</span></span>

<span data-ttu-id="a3e85-109">[Installieren Sie die CLI](install-azure-cli.md), sofern noch nicht geschehen, oder probieren Sie [Azure Cloud Shell](/azure/cloud-shell/overview) aus.</span><span class="sxs-lookup"><span data-stu-id="a3e85-109">If you haven't already, [install the CLI](install-azure-cli.md) or try out the [Azure Cloud Shell](/azure/cloud-shell/overview).</span></span>

<span data-ttu-id="a3e85-110">Bevor Sie CLI-Befehle mit einer lokalen Installation verwenden, müssen Sie sich mithilfe von [az login](/cli/azure/reference-index#az-login) anmelden.</span><span class="sxs-lookup"><span data-stu-id="a3e85-110">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="a3e85-111">Es gibt Methoden, sich nicht interaktiv anzumelden. Diese werden unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md) ausführlich beschrieben.</span><span class="sxs-lookup"><span data-stu-id="a3e85-111">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="a3e85-112">Häufig verwendete Befehle</span><span class="sxs-lookup"><span data-stu-id="a3e85-112">Common commands</span></span>

<span data-ttu-id="a3e85-113">Die folgende Tabelle enthält einige allgemeine Befehle, die in der CLI verwendet werden, sowie Links zu ihrer Referenzdokumentation.</span><span class="sxs-lookup"><span data-stu-id="a3e85-113">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="a3e85-114">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a3e85-114">Resource type</span></span> | <span data-ttu-id="a3e85-115">Azure CLI-Befehlsgruppe</span><span class="sxs-lookup"><span data-stu-id="a3e85-115">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="a3e85-116">Ressourcengruppe</span><span class="sxs-lookup"><span data-stu-id="a3e85-116">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="a3e85-117">az group</span><span class="sxs-lookup"><span data-stu-id="a3e85-117">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="a3e85-118">Virtuelle Computer</span><span class="sxs-lookup"><span data-stu-id="a3e85-118">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="a3e85-119">az vm</span><span class="sxs-lookup"><span data-stu-id="a3e85-119">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="a3e85-120">Speicherkonten</span><span class="sxs-lookup"><span data-stu-id="a3e85-120">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="a3e85-121">az storage account</span><span class="sxs-lookup"><span data-stu-id="a3e85-121">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="a3e85-122">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="a3e85-122">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="a3e85-123">az keyvault</span><span class="sxs-lookup"><span data-stu-id="a3e85-123">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="a3e85-124">Webanwendungen</span><span class="sxs-lookup"><span data-stu-id="a3e85-124">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="a3e85-125">az webapp</span><span class="sxs-lookup"><span data-stu-id="a3e85-125">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="a3e85-126">SQL-Datenbanken</span><span class="sxs-lookup"><span data-stu-id="a3e85-126">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="a3e85-127">az sql server</span><span class="sxs-lookup"><span data-stu-id="a3e85-127">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="a3e85-128">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a3e85-128">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="a3e85-129">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="a3e85-129">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="a3e85-130">Suchen von Befehlen</span><span class="sxs-lookup"><span data-stu-id="a3e85-130">Finding commands</span></span>

<span data-ttu-id="a3e85-131">Befehle in der CLI werden als _Befehle_ von _Gruppen_ organisiert.</span><span class="sxs-lookup"><span data-stu-id="a3e85-131">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="a3e85-132">Jede Gruppe stellt einen Azure-Dienst dar, und Befehle werden für diesen Dienst ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="a3e85-132">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="a3e85-133">Suchen Sie Befehle mithilfe von [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="a3e85-133">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="a3e85-134">Verwenden Sie den folgenden Befehl, um beispielsweise nach Befehlsnamen zu suchen, die `secret` enthalten:</span><span class="sxs-lookup"><span data-stu-id="a3e85-134">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="a3e85-135">Verwenden Sie das Argument `--help`, um eine vollständige Liste der Befehle und Untergruppen einer Gruppe abzurufen.</span><span class="sxs-lookup"><span data-stu-id="a3e85-135">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="a3e85-136">Geben Sie beispielsweise Folgendes ein, um die CLI-Befehle für die Verwendung mit Netzwerksicherheitsgruppen (NSGs) zu ermitteln:</span><span class="sxs-lookup"><span data-stu-id="a3e85-136">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="a3e85-137">Die CLI ermöglicht unter der Bash-Shell die Vervollständigung mit der TAB-TASTE.</span><span class="sxs-lookup"><span data-stu-id="a3e85-137">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="a3e85-138">Global verfügbare Argumente</span><span class="sxs-lookup"><span data-stu-id="a3e85-138">Globally available arguments</span></span>

<span data-ttu-id="a3e85-139">Es gibt einige Argumente, die für jeden Befehl verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="a3e85-139">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="a3e85-140">`--help` gibt CLI-Referenzinformationen zu Befehlen und ihren Argumenten zurück und führt verfügbare Untergruppen und Befehle auf.</span><span class="sxs-lookup"><span data-stu-id="a3e85-140">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="a3e85-141">`--output` ändert das Ausgabeformat.</span><span class="sxs-lookup"><span data-stu-id="a3e85-141">`--output` changes the output format.</span></span> <span data-ttu-id="a3e85-142">Verfügbare Ausgabeformate: `json`, `jsonc` (farbiger JSON-Code), `tsv` (per Tabulator getrennte Werte) und `table` (für Menschen lesbare ASCII-Tabellen).</span><span class="sxs-lookup"><span data-stu-id="a3e85-142">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="a3e85-143">Die CLI gibt standardmäßig `json` aus.</span><span class="sxs-lookup"><span data-stu-id="a3e85-143">By default the CLI outputs `json`.</span></span> <span data-ttu-id="a3e85-144">Weitere Informationen zu den verfügbaren Ausgabeformaten finden Sie unter [Ausgabeformate für Azure CLI 2.0-Befehle](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="a3e85-144">To learn more about the available output formats, see [Output formats for Azure CLI 2.0](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="a3e85-145">`--query` verwendet die [JMESPath-Abfragesprache](http://jmespath.org/) zum Filtern der von Azure-Diensten zurückgegebenen Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="a3e85-145">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="a3e85-146">Weitere Informationen zu Abfragen finden Sie unter [Verwenden von JMESPath-Abfragen mit Azure CLI 2.0](query-azure-cli.md) und im [JMESPath-Tutorial](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="a3e85-146">To learn To learn more about queries, see [Query command results with Azure CLI 2.0](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="a3e85-147">`--verbose` gibt Informationen zu Ressourcen, die in Azure während eines Vorgangs erstellt werden, und andere nützliche Informationen aus.</span><span class="sxs-lookup"><span data-stu-id="a3e85-147">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="a3e85-148">`--debug` gibt noch mehr Informationen zu CLI-Vorgängen aus, die zum Debuggen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="a3e85-148">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="a3e85-149">Wenn ein Fehler auftritt, stellen Sie beim Übermitteln eines Fehlerberichts die mit dem Flag `--debug` generierte Ausgabe bereit.</span><span class="sxs-lookup"><span data-stu-id="a3e85-149">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="a3e85-150">Interaktiver Modus</span><span class="sxs-lookup"><span data-stu-id="a3e85-150">Interactive mode</span></span>

<span data-ttu-id="a3e85-151">Die CLI bietet einen interaktiven Modus, der automatisch Hilfeinformationen anzeigt und die Auswahl von Unterbefehlen vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="a3e85-151">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="a3e85-152">Sie wechseln mit dem Befehl [az interactive](/cli/azure/reference-index#az-interactive) in den interaktiven Modus.</span><span class="sxs-lookup"><span data-stu-id="a3e85-152">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="a3e85-153">Weitere Informationen zum interaktiven Modus finden Sie unter [Interaktive Azure CLI 2.0](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="a3e85-153">For more information on interactive mode, see [Azure CLI 2.0 Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="a3e85-154">Darüber hinaus gibt es ein [Visual Studio Code-Plug-In](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli), das eine interaktive Benutzeroberfläche bereitstellt. Diese bietet unter anderem Funktionen wie AutoVervollständigen und die Anzeigen von Informationen beim Daraufzeigen.</span><span class="sxs-lookup"><span data-stu-id="a3e85-154">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="a3e85-155">Lernen der CLI-Grundlagen mit Schnellstarts und Tutorials</span><span class="sxs-lookup"><span data-stu-id="a3e85-155">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="a3e85-156">Sehen Sie sich für die ersten Schritte mit der Azure CLI 2.0 ein ausführliches Tutorial an, in dem Sie lernen, wie Sie virtuelle Computer einrichten und die Funktionen der CLI zum Abfragen von Azure-Ressourcen nutzen.</span><span class="sxs-lookup"><span data-stu-id="a3e85-156">To get you started with the Azure CLI 2.0, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="a3e85-157">Erstellen von virtuellen Computern mit der Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="a3e85-157">Create virtual machines with the Azure CLI 2.0 tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="a3e85-158">Es gibt auch Schnellstartanleitungen für andere beliebte Dienste.</span><span class="sxs-lookup"><span data-stu-id="a3e85-158">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="a3e85-159">Erstellen eines Speicherkontos mit der Azure-Befehlszeilenschnittstelle</span><span class="sxs-lookup"><span data-stu-id="a3e85-159">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* <span data-ttu-id="a3e85-160">[Transfer objects to/from Azure Blob storage using the CLI](/azure/storage/blobs/storage-quickstart-blobs-cli) (Übertragen von Objekten in/aus Azure Blob Storage mit der CLI)</span><span class="sxs-lookup"><span data-stu-id="a3e85-160">[Transfer objects to/from Azure Blob storage using the CLI](/azure/storage/blobs/storage-quickstart-blobs-cli)</span></span>
* [<span data-ttu-id="a3e85-161">Erstellen einer einzelnen Azure SQL-Datenbank mithilfe der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="a3e85-161">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="a3e85-162">Erstellen eines Azure Database for MySQL-Servers mithilfe der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="a3e85-162">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="a3e85-163">Erstellen einer Azure-Datenbank für PostgreSQL mithilfe der Azure-CLI</span><span class="sxs-lookup"><span data-stu-id="a3e85-163">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="a3e85-164">Erstellen einer Python-Web-App in Azure</span><span class="sxs-lookup"><span data-stu-id="a3e85-164">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="a3e85-165">Ausführen eines benutzerdefinierten Image von Docker-Hubs in Azure-Web-Apps für Container</span><span class="sxs-lookup"><span data-stu-id="a3e85-165">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="a3e85-166">Abgeben von Feedback</span><span class="sxs-lookup"><span data-stu-id="a3e85-166">Give feedback</span></span>

<span data-ttu-id="a3e85-167">Ihr Feedback zur CLI hilft uns dabei, Verbesserungen vorzunehmen und Fehler zu beheben.</span><span class="sxs-lookup"><span data-stu-id="a3e85-167">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="a3e85-168">Sie können [ein Problem auf Github melden](https://github.com/azure/azure-cli/issues) oder mit den integrierten Features der CLI und dem Befehl [az feedback](/cli/azure/reference-index#az-feedback) allgemeines Feedback hinterlassen.</span><span class="sxs-lookup"><span data-stu-id="a3e85-168">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```

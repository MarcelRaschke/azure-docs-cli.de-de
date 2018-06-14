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
ms.openlocfilehash: dbb6233e8fed15b440282b8396d3b3bd056e80f7
ms.sourcegitcommit: 5c80e96e96f9608c92a94fa4a9c4afb25099f3fc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/13/2018
ms.locfileid: "35512936"
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="cf978-104">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="cf978-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="cf978-105">Willkommen bei der Azure CLI 2.0!</span><span class="sxs-lookup"><span data-stu-id="cf978-105">Welcome to the Azure CLI 2.0!</span></span> <span data-ttu-id="cf978-106">Die CLI ist ein Tool, das die schnelle und effiziente Verwendung von Azure-Diensten ermöglichen soll. Der Fokus liegt dabei auf der Automatisierung.</span><span class="sxs-lookup"><span data-stu-id="cf978-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="cf978-107">Dieser Artikel stellt Features der CLI vor und enthält Links zu Ressourcen, die Sie dabei unterstützen, produktiv zu sein.</span><span class="sxs-lookup"><span data-stu-id="cf978-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-and-log-in"></a><span data-ttu-id="cf978-108">Installieren und Anmelden</span><span class="sxs-lookup"><span data-stu-id="cf978-108">Install and log in</span></span>

<span data-ttu-id="cf978-109">[Installieren Sie die CLI](install-azure-cli.md), sofern noch nicht geschehen, oder probieren Sie [Azure Cloud Shell](/azure/cloud-shell/overview) aus.</span><span class="sxs-lookup"><span data-stu-id="cf978-109">If you haven't already, [install the CLI](install-azure-cli.md) or try out the [Azure Cloud Shell](/azure/cloud-shell/overview).</span></span>

<span data-ttu-id="cf978-110">Bevor Sie CLI-Befehle mit einer lokalen Installation verwenden, müssen Sie sich mithilfe von [az login](/cli/azure/reference-index#az-login) anmelden.</span><span class="sxs-lookup"><span data-stu-id="cf978-110">Before using any CLI commands with a local install, you need to log in with [az login](/cli/azure/reference-index#az-login).</span></span>

```azurecli
az login
```

<span data-ttu-id="cf978-111">Dieser Befehl fordert Sie dazu auf, sich mit einem Authentifizierungscode über eine Website anzumelden.</span><span class="sxs-lookup"><span data-stu-id="cf978-111">This command prompts you to log in with an authentication code via a website.</span></span> <span data-ttu-id="cf978-112">Es gibt Methoden, sich nicht interaktiv anzumelden. Diese werden unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md) ausführlich beschrieben.</span><span class="sxs-lookup"><span data-stu-id="cf978-112">There are ways to log in non-interactively, which are covered in detail in [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="cf978-113">Häufig verwendete Befehle</span><span class="sxs-lookup"><span data-stu-id="cf978-113">Common commands</span></span>

<span data-ttu-id="cf978-114">In der nachfolgenden Tabelle sind einige der in der CLI häufig verwendeten Befehle als Links zu den Dokumentationsseiten in der Referenz aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="cf978-114">This table lists a few of the common commands used in the CLI links out to their documentation pages in the reference.</span></span>
<span data-ttu-id="cf978-115">Alle Unterbefehle dieser Gruppen und ihre Dokumentation können in der Onlinereferenz oder mit dem Argument `--help` nachgeschlagen werden.</span><span class="sxs-lookup"><span data-stu-id="cf978-115">All subcommands of these groups and their documentation can be looked up in online reference or with the `--help` argument.</span></span>

| <span data-ttu-id="cf978-116">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cf978-116">Resource type</span></span> | <span data-ttu-id="cf978-117">Azure CLI-Befehlsgruppe</span><span class="sxs-lookup"><span data-stu-id="cf978-117">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="cf978-118">Ressourcengruppe</span><span class="sxs-lookup"><span data-stu-id="cf978-118">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="cf978-119">az group</span><span class="sxs-lookup"><span data-stu-id="cf978-119">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="cf978-120">Virtuelle Computer</span><span class="sxs-lookup"><span data-stu-id="cf978-120">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="cf978-121">az vm</span><span class="sxs-lookup"><span data-stu-id="cf978-121">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="cf978-122">Speicherkonten</span><span class="sxs-lookup"><span data-stu-id="cf978-122">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="cf978-123">az storage account</span><span class="sxs-lookup"><span data-stu-id="cf978-123">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="cf978-124">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="cf978-124">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="cf978-125">az keyvault</span><span class="sxs-lookup"><span data-stu-id="cf978-125">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="cf978-126">Webanwendungen</span><span class="sxs-lookup"><span data-stu-id="cf978-126">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="cf978-127">az webapp</span><span class="sxs-lookup"><span data-stu-id="cf978-127">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="cf978-128">SQL-Datenbanken</span><span class="sxs-lookup"><span data-stu-id="cf978-128">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="cf978-129">az sql server</span><span class="sxs-lookup"><span data-stu-id="cf978-129">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="cf978-130">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="cf978-130">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="cf978-131">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="cf978-131">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="cf978-132">Suchen von Befehlen</span><span class="sxs-lookup"><span data-stu-id="cf978-132">Finding commands</span></span>

<span data-ttu-id="cf978-133">Befehle in der CLI werden als _Unterbefehle_ von _Gruppen_ bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="cf978-133">Commands in the CLI are provided as _subcommands_ of _groups_.</span></span>
<span data-ttu-id="cf978-134">Jede Gruppe stellt einen von Azure bereitgestellten Dienst dar, und die Untergruppen unterteilen Befehle für diese Dienste in logische Gruppierungen.</span><span class="sxs-lookup"><span data-stu-id="cf978-134">Each group represents a service provided by Azure, and the subgroups divide commands for these services into logical groupings.</span></span>

<span data-ttu-id="cf978-135">Suchen Sie Befehle mithilfe von [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="cf978-135">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="cf978-136">Verwenden Sie den folgenden Befehl, um beispielsweise nach Befehlsnamen zu suchen, die `secret` enthalten:</span><span class="sxs-lookup"><span data-stu-id="cf978-136">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="cf978-137">Wenn Sie wissen, mit welcher Gruppe von Befehlen Sie arbeiten möchten, ist das Argument `--help` unter Umständen besser geeignet.</span><span class="sxs-lookup"><span data-stu-id="cf978-137">If you know which group of commands you want to work with, the `--help` argument may be a better choice.</span></span> <span data-ttu-id="cf978-138">Damit werden nicht nur detaillierte Informationen für einen Befehl, sondern – bei Verwendung mit einer Befehlsgruppe – alle verfügbaren Unterbefehle angezeigt.</span><span class="sxs-lookup"><span data-stu-id="cf978-138">This displays not just detailed information for a command, but when used with a command group, displays all of the available subcommands.</span></span> <span data-ttu-id="cf978-139">Beispielsweise können Sie bei Verwendung von Netzwerksicherheitsgruppen (NSGs) die verfügbaren Untergruppen und Befehle der NSGs ermitteln.</span><span class="sxs-lookup"><span data-stu-id="cf978-139">For example, when working with Network Security Groups (NSGs) you can find the available NSG subgroups and commands.</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="cf978-140">Die CLI ermöglicht unter der Bash-Shell die Vervollständigung mit der TAB-TASTE.</span><span class="sxs-lookup"><span data-stu-id="cf978-140">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="cf978-141">Global verfügbare Argumente</span><span class="sxs-lookup"><span data-stu-id="cf978-141">Globally available arguments</span></span>

<span data-ttu-id="cf978-142">Es gibt einige Argumente, die für jeden Befehl verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="cf978-142">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="cf978-143">`--help` gibt CLI-Referenzinformationen zu Befehlen und ihren Argumenten zurück und führt verfügbare Untergruppen und Befehle auf.</span><span class="sxs-lookup"><span data-stu-id="cf978-143">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="cf978-144">`--output` ändert das Ausgabeformat.</span><span class="sxs-lookup"><span data-stu-id="cf978-144">`--output` changes the output format.</span></span> <span data-ttu-id="cf978-145">Verfügbare Ausgabeformate: `json`, `jsonc` (farbiger JSON-Code), `tsv` (per Tabulator getrennte Werte) und `table` (für Menschen lesbare ASCII-Tabellen).</span><span class="sxs-lookup"><span data-stu-id="cf978-145">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="cf978-146">Die CLI gibt standardmäßig `json` aus.</span><span class="sxs-lookup"><span data-stu-id="cf978-146">By default the CLI outputs `json`.</span></span> <span data-ttu-id="cf978-147">Weitere Informationen zu den verfügbaren Ausgabeformaten finden Sie unter [Ausgabeformate für Azure CLI 2.0-Befehle](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="cf978-147">To learn more about the available output formats, see [Output formats for Azure CLI 2.0](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="cf978-148">`--query` verwendet die [JMESPath-Abfragesprache](http://jmespath.org/) zum Filtern der von Azure-Diensten zurückgegebenen Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="cf978-148">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="cf978-149">Weitere Informationen zu Abfragen finden Sie unter [Verwenden von JMESPath-Abfragen mit Azure CLI 2.0](query-azure-cli.md) und im [JMESPath-Tutorial](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="cf978-149">To learn To learn more about queries, see [Query command results with Azure CLI 2.0](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="cf978-150">`--verbose` gibt Informationen zu Ressourcen, die in Azure während eines Vorgangs erstellt werden, und andere nützliche Informationen aus.</span><span class="sxs-lookup"><span data-stu-id="cf978-150">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="cf978-151">`--debug` gibt noch mehr Informationen zu CLI-Vorgängen aus, die zum Debuggen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="cf978-151">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="cf978-152">Wenn ein Fehler auftritt, stellen Sie beim Übermitteln eines Fehlerberichts die mit dem Flag `--debug` generierte Ausgabe bereit.</span><span class="sxs-lookup"><span data-stu-id="cf978-152">If you encounter a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>


## <a name="interactive-mode"></a><span data-ttu-id="cf978-153">Interaktiver Modus</span><span class="sxs-lookup"><span data-stu-id="cf978-153">Interactive mode</span></span>

<span data-ttu-id="cf978-154">Die CLI bietet einen interaktiven Modus, der automatisch Hilfeinformationen anzeigt und die Auswahl von Unterbefehlen vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="cf978-154">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="cf978-155">Sie wechseln mit dem Befehl [az interactive](/cli/azure/reference-index#az-interactive) in den interaktiven Modus.</span><span class="sxs-lookup"><span data-stu-id="cf978-155">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="cf978-156">Weitere Informationen zum interaktiven Modus finden Sie unter [Interaktive Azure CLI 2.0](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="cf978-156">For more information on interactive mode, see [Azure CLI 2.0 Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="cf978-157">Darüber hinaus gibt es ein [Visual Studio Code-Plug-In](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli), das eine interaktive Benutzeroberfläche bereitstellt. Diese bietet unter anderem Funktionen wie AutoVervollständigen und die Anzeige von Informationen beim Daraufzeigen.</span><span class="sxs-lookup"><span data-stu-id="cf978-157">There is also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="cf978-158">Lernen der CLI-Grundlagen mit Schnellstarts und Tutorials</span><span class="sxs-lookup"><span data-stu-id="cf978-158">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="cf978-159">Sehen Sie sich für die ersten Schritte mit der Azure CLI 2.0 ein ausführliches Tutorial an, in dem Sie lernen, wie Sie virtuelle Computer einrichten und die Funktionen der CLI zum Abfragen von Azure-Ressourcen nutzen.</span><span class="sxs-lookup"><span data-stu-id="cf978-159">To get you started with the Azure CLI 2.0, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="cf978-160">Erstellen von virtuellen Computern mit der Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="cf978-160">Create virtual machines with the Azure CLI 2.0 tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="cf978-161">Wenn Sie sich eher auf andere Dienste konzentrieren möchten, stehen verschiedene Schnellstartanleitungen für Azure-Dienste zur Verfügung, die die CLI nutzen.</span><span class="sxs-lookup"><span data-stu-id="cf978-161">If you would rather focus on other services, there are a variety of quickstarts for Azure services that use the CLI.</span></span>

* [<span data-ttu-id="cf978-162">Erstellen eines Speicherkontos mit der Azure-Befehlszeilenschnittstelle</span><span class="sxs-lookup"><span data-stu-id="cf978-162">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* <span data-ttu-id="cf978-163">[Transfer objects to/from Azure Blob storage using the CLI](/azure/storage/blobs/storage-quickstart-blobs-cli) (Übertragen von Objekten in/aus Azure Blob Storage mit der CLI)</span><span class="sxs-lookup"><span data-stu-id="cf978-163">[Transfer objects to/from Azure Blob storage using the CLI](/azure/storage/blobs/storage-quickstart-blobs-cli)</span></span>
* [<span data-ttu-id="cf978-164">Erstellen einer einzelnen Azure SQL-Datenbank mithilfe der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="cf978-164">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="cf978-165">Erstellen eines Azure Database for MySQL-Servers mithilfe der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="cf978-165">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="cf978-166">Erstellen einer Azure-Datenbank für PostgreSQL mithilfe der Azure-CLI</span><span class="sxs-lookup"><span data-stu-id="cf978-166">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="cf978-167">Erstellen einer Python-Web-App in Azure</span><span class="sxs-lookup"><span data-stu-id="cf978-167">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="cf978-168">Ausführen eines benutzerdefinierten Image von Docker-Hubs in Azure-Web-Apps für Container</span><span class="sxs-lookup"><span data-stu-id="cf978-168">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="cf978-169">Abgeben von Feedback</span><span class="sxs-lookup"><span data-stu-id="cf978-169">Give feedback</span></span>

<span data-ttu-id="cf978-170">Ihr Feedback zur CLI hilft uns dabei, Verbesserungen vorzunehmen und Fehler zu beheben.</span><span class="sxs-lookup"><span data-stu-id="cf978-170">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="cf978-171">Sie können [ein Problem auf Github melden](https://github.com/azure/azure-cli/issues) oder mit den integrierten Features der CLI und dem Befehl [az feedback](/cli/azure/reference-index#az-feedback) allgemeines Feedback hinterlassen.</span><span class="sxs-lookup"><span data-stu-id="cf978-171">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```

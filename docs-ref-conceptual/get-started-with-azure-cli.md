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
# <a name="get-started-with-azure-cli"></a><span data-ttu-id="48362-104">Erste Schritte mit der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="48362-104">Get started with Azure CLI</span></span>

<span data-ttu-id="48362-105">Willkommen bei der Azure CLI!</span><span class="sxs-lookup"><span data-stu-id="48362-105">Welcome to the Azure CLI!</span></span> <span data-ttu-id="48362-106">Die CLI ist ein Tool, das die schnelle und effiziente Verwendung von Azure-Diensten ermöglichen soll. Der Fokus liegt dabei auf der Automatisierung.</span><span class="sxs-lookup"><span data-stu-id="48362-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="48362-107">Dieser Artikel stellt Features der CLI vor und enthält Links zu Ressourcen, die Sie dabei unterstützen, produktiv zu sein.</span><span class="sxs-lookup"><span data-stu-id="48362-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="48362-108">Installieren oder Ausführen in Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="48362-108">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="48362-109">Am einfachsten können Sie die Azure-Befehlszeilenschnittstelle in einer Azure Cloud Shell-Umgebung über Ihren Browser verwenden.</span><span class="sxs-lookup"><span data-stu-id="48362-109">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="48362-110">Informationen zu Cloud Shell finden Sie unter [Schnellstart für Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="48362-110">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="48362-111">Wenn Sie zur Installation der Befehlszeilenschnittstelle bereit sind, lesen Sie die [Installationsanweisungen](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="48362-111">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

## <a name="sign-in"></a><span data-ttu-id="48362-112">Anmelden</span><span class="sxs-lookup"><span data-stu-id="48362-112">Sign in</span></span>

<span data-ttu-id="48362-113">Bevor Sie CLI-Befehle mit einer lokalen Installation verwenden, müssen Sie sich mithilfe von [az login](/cli/azure/reference-index#az-login) anmelden.</span><span class="sxs-lookup"><span data-stu-id="48362-113">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="48362-114">Es gibt auch Wege, wie Sie sich nicht interaktiv anmelden können. Diese werden unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md) ausführlich beschrieben.</span><span class="sxs-lookup"><span data-stu-id="48362-114">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="48362-115">Häufig verwendete Befehle</span><span class="sxs-lookup"><span data-stu-id="48362-115">Common commands</span></span>

<span data-ttu-id="48362-116">Die folgende Tabelle enthält einige allgemeine Befehle, die in der CLI verwendet werden, sowie Links zu ihrer Referenzdokumentation.</span><span class="sxs-lookup"><span data-stu-id="48362-116">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="48362-117">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="48362-117">Resource type</span></span> | <span data-ttu-id="48362-118">Azure CLI-Befehlsgruppe</span><span class="sxs-lookup"><span data-stu-id="48362-118">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="48362-119">Ressourcengruppe</span><span class="sxs-lookup"><span data-stu-id="48362-119">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="48362-120">az group</span><span class="sxs-lookup"><span data-stu-id="48362-120">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="48362-121">Virtuelle Computer</span><span class="sxs-lookup"><span data-stu-id="48362-121">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="48362-122">az vm</span><span class="sxs-lookup"><span data-stu-id="48362-122">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="48362-123">Speicherkonten</span><span class="sxs-lookup"><span data-stu-id="48362-123">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="48362-124">az storage account</span><span class="sxs-lookup"><span data-stu-id="48362-124">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="48362-125">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="48362-125">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="48362-126">az keyvault</span><span class="sxs-lookup"><span data-stu-id="48362-126">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="48362-127">Webanwendungen</span><span class="sxs-lookup"><span data-stu-id="48362-127">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="48362-128">az webapp</span><span class="sxs-lookup"><span data-stu-id="48362-128">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="48362-129">SQL-Datenbanken</span><span class="sxs-lookup"><span data-stu-id="48362-129">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="48362-130">az sql server</span><span class="sxs-lookup"><span data-stu-id="48362-130">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="48362-131">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="48362-131">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="48362-132">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="48362-132">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="48362-133">Suchen von Befehlen</span><span class="sxs-lookup"><span data-stu-id="48362-133">Finding commands</span></span>

<span data-ttu-id="48362-134">Befehle in der CLI werden als _Befehle_ von _Gruppen_ organisiert.</span><span class="sxs-lookup"><span data-stu-id="48362-134">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="48362-135">Jede Gruppe stellt einen Azure-Dienst dar, und Befehle werden für diesen Dienst ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="48362-135">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="48362-136">Suchen Sie Befehle mithilfe von [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="48362-136">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="48362-137">Verwenden Sie den folgenden Befehl, um beispielsweise nach Befehlsnamen zu suchen, die `secret` enthalten:</span><span class="sxs-lookup"><span data-stu-id="48362-137">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="48362-138">Verwenden Sie das Argument `--help`, um eine vollständige Liste der Befehle und Untergruppen einer Gruppe abzurufen.</span><span class="sxs-lookup"><span data-stu-id="48362-138">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="48362-139">Geben Sie beispielsweise Folgendes ein, um die CLI-Befehle für die Verwendung mit Netzwerksicherheitsgruppen (NSGs) zu ermitteln:</span><span class="sxs-lookup"><span data-stu-id="48362-139">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="48362-140">Die CLI ermöglicht unter der Bash-Shell die Vervollständigung mit der TAB-TASTE.</span><span class="sxs-lookup"><span data-stu-id="48362-140">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="48362-141">Global verfügbare Argumente</span><span class="sxs-lookup"><span data-stu-id="48362-141">Globally available arguments</span></span>

<span data-ttu-id="48362-142">Es gibt einige Argumente, die für jeden Befehl verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="48362-142">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="48362-143">`--help` gibt CLI-Referenzinformationen zu Befehlen und ihren Argumenten zurück und führt verfügbare Untergruppen und Befehle auf.</span><span class="sxs-lookup"><span data-stu-id="48362-143">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="48362-144">`--output` ändert das Ausgabeformat.</span><span class="sxs-lookup"><span data-stu-id="48362-144">`--output` changes the output format.</span></span> <span data-ttu-id="48362-145">Verfügbare Ausgabeformate: `json`, `jsonc` (farbiger JSON-Code), `tsv` (per Tabulator getrennte Werte) und `table` (für Menschen lesbare ASCII-Tabellen).</span><span class="sxs-lookup"><span data-stu-id="48362-145">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="48362-146">Die CLI gibt standardmäßig `json` aus.</span><span class="sxs-lookup"><span data-stu-id="48362-146">By default the CLI outputs `json`.</span></span> <span data-ttu-id="48362-147">Weitere Informationen zu den verfügbaren Ausgabeformaten finden Sie unter [Ausgabeformate für die Azure CLI](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="48362-147">To learn more about the available output formats, see [Output formats for Azure CLI](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="48362-148">`--query` verwendet die [JMESPath-Abfragesprache](http://jmespath.org/) zum Filtern der von Azure-Diensten zurückgegebenen Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="48362-148">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="48362-149">Weitere Informationen zu Abfragen finden Sie unter [Abfragen von Befehlsergebnissen mit der Azure CLI](query-azure-cli.md) und im [JMESPath-Tutorial](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="48362-149">To learn To learn more about queries, see [Query command results with Azure CLI](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="48362-150">`--verbose` gibt Informationen zu Ressourcen, die in Azure während eines Vorgangs erstellt werden, und andere nützliche Informationen aus.</span><span class="sxs-lookup"><span data-stu-id="48362-150">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="48362-151">`--debug` gibt noch mehr Informationen zu CLI-Vorgängen aus, die zum Debuggen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="48362-151">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="48362-152">Wenn ein Fehler auftritt, stellen Sie beim Übermitteln eines Fehlerberichts die mit dem Flag `--debug` generierte Ausgabe bereit.</span><span class="sxs-lookup"><span data-stu-id="48362-152">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="48362-153">Interaktiver Modus</span><span class="sxs-lookup"><span data-stu-id="48362-153">Interactive mode</span></span>

<span data-ttu-id="48362-154">Die CLI bietet einen interaktiven Modus, der automatisch Hilfeinformationen anzeigt und die Auswahl von Unterbefehlen vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="48362-154">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="48362-155">Sie wechseln mit dem Befehl [az interactive](/cli/azure/reference-index#az-interactive) in den interaktiven Modus.</span><span class="sxs-lookup"><span data-stu-id="48362-155">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="48362-156">Weitere Informationen zum interaktiven Modus finden Sie unter [Azure CLI – Interaktiver Modus](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="48362-156">For more information on interactive mode, see [Azure CLI Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="48362-157">Darüber hinaus gibt es ein [Visual Studio Code-Plug-In](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli), das eine interaktive Benutzeroberfläche bereitstellt. Diese bietet unter anderem Funktionen wie AutoVervollständigen und die Anzeigen von Informationen beim Daraufzeigen.</span><span class="sxs-lookup"><span data-stu-id="48362-157">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="48362-158">Lernen der CLI-Grundlagen mit Schnellstarts und Tutorials</span><span class="sxs-lookup"><span data-stu-id="48362-158">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="48362-159">Sehen Sie sich zu den ersten Schritten mit der Azure CLI ein ausführliches Tutorial an, in dem Sie lernen, wie Sie virtuelle Computer einrichten und die Funktionen der CLI zum Abfragen von Azure-Ressourcen nutzen.</span><span class="sxs-lookup"><span data-stu-id="48362-159">To get you started with the Azure CLI, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="48362-160">Erstellen von virtuellen Computern mit der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="48362-160">Create virtual machines with the Azure CLI tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="48362-161">Es gibt auch Schnellstartanleitungen für andere beliebte Dienste.</span><span class="sxs-lookup"><span data-stu-id="48362-161">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="48362-162">Erstellen eines Speicherkontos mit der Azure-Befehlszeilenschnittstelle</span><span class="sxs-lookup"><span data-stu-id="48362-162">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* <span data-ttu-id="48362-163">[Transfer objects to/from Azure Blob storage using the CLI](/azure/storage/blobs/storage-quickstart-blobs-cli) (Übertragen von Objekten in/aus Azure Blob Storage mit der CLI)</span><span class="sxs-lookup"><span data-stu-id="48362-163">[Transfer objects to/from Azure Blob storage using the CLI](/azure/storage/blobs/storage-quickstart-blobs-cli)</span></span>
* [<span data-ttu-id="48362-164">Erstellen einer einzelnen Azure SQL-Datenbank mithilfe der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="48362-164">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="48362-165">Erstellen eines Azure Database for MySQL-Servers mithilfe der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="48362-165">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="48362-166">Erstellen einer Azure-Datenbank für PostgreSQL mithilfe der Azure-CLI</span><span class="sxs-lookup"><span data-stu-id="48362-166">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="48362-167">Erstellen einer Python-Web-App in Azure</span><span class="sxs-lookup"><span data-stu-id="48362-167">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="48362-168">Ausführen eines benutzerdefinierten Image von Docker-Hubs in Azure-Web-Apps für Container</span><span class="sxs-lookup"><span data-stu-id="48362-168">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="48362-169">Abgeben von Feedback</span><span class="sxs-lookup"><span data-stu-id="48362-169">Give feedback</span></span>

<span data-ttu-id="48362-170">Ihr Feedback zur CLI hilft uns dabei, Verbesserungen vorzunehmen und Fehler zu beheben.</span><span class="sxs-lookup"><span data-stu-id="48362-170">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="48362-171">Sie können [ein Problem auf Github melden](https://github.com/azure/azure-cli/issues) oder mit den integrierten Features der CLI und dem Befehl [az feedback](/cli/azure/reference-index#az-feedback) allgemeines Feedback hinterlassen.</span><span class="sxs-lookup"><span data-stu-id="48362-171">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```

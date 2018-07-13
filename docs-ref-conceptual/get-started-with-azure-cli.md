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
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="d2388-104">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="d2388-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="d2388-105">Willkommen bei der Azure CLI 2.0!</span><span class="sxs-lookup"><span data-stu-id="d2388-105">Welcome to the Azure CLI 2.0!</span></span> <span data-ttu-id="d2388-106">Die CLI ist ein Tool, das die schnelle und effiziente Verwendung von Azure-Diensten ermöglichen soll. Der Fokus liegt dabei auf der Automatisierung.</span><span class="sxs-lookup"><span data-stu-id="d2388-106">The CLI is a tool designed to get you working quickly and efficiently with Azure services, with an emphasis on automation.</span></span> <span data-ttu-id="d2388-107">Dieser Artikel stellt Features der CLI vor und enthält Links zu Ressourcen, die Sie dabei unterstützen, produktiv zu sein.</span><span class="sxs-lookup"><span data-stu-id="d2388-107">This article introduces features of the CLI and links out to resources that help you be productive.</span></span>

## <a name="install-and-sign-in"></a><span data-ttu-id="d2388-108">Installieren und Anmelden</span><span class="sxs-lookup"><span data-stu-id="d2388-108">Install and sign in</span></span>

<span data-ttu-id="d2388-109">[Installieren Sie die CLI](install-azure-cli.md), sofern noch nicht geschehen, oder probieren Sie [Azure Cloud Shell](/azure/cloud-shell/overview) aus.</span><span class="sxs-lookup"><span data-stu-id="d2388-109">If you haven't already, [install the CLI](install-azure-cli.md) or try out the [Azure Cloud Shell](/azure/cloud-shell/overview).</span></span>

<span data-ttu-id="d2388-110">Bevor Sie CLI-Befehle mit einer lokalen Installation verwenden, müssen Sie sich mithilfe von [az login](/cli/azure/reference-index#az-login) anmelden.</span><span class="sxs-lookup"><span data-stu-id="d2388-110">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="d2388-111">Es gibt Methoden, sich nicht interaktiv anzumelden. Diese werden unter [Anmelden mit Azure CLI 2.0](authenticate-azure-cli.md) ausführlich beschrieben.</span><span class="sxs-lookup"><span data-stu-id="d2388-111">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="d2388-112">Häufig verwendete Befehle</span><span class="sxs-lookup"><span data-stu-id="d2388-112">Common commands</span></span>

<span data-ttu-id="d2388-113">In der nachfolgenden Tabelle sind einige der in der CLI häufig verwendeten Befehle als Links zu den Dokumentationsseiten in der Referenz aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="d2388-113">This table lists a few of the common commands used in the CLI links out to their documentation pages in the reference.</span></span>
<span data-ttu-id="d2388-114">Alle Unterbefehle dieser Gruppen und ihre Dokumentation können in der Onlinereferenz oder mit dem Argument `--help` nachgeschlagen werden.</span><span class="sxs-lookup"><span data-stu-id="d2388-114">All subcommands of these groups and their documentation can be looked up in online reference or with the `--help` argument.</span></span>

| <span data-ttu-id="d2388-115">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d2388-115">Resource type</span></span> | <span data-ttu-id="d2388-116">Azure CLI-Befehlsgruppe</span><span class="sxs-lookup"><span data-stu-id="d2388-116">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="d2388-117">Ressourcengruppe</span><span class="sxs-lookup"><span data-stu-id="d2388-117">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="d2388-118">az group</span><span class="sxs-lookup"><span data-stu-id="d2388-118">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="d2388-119">Virtuelle Computer</span><span class="sxs-lookup"><span data-stu-id="d2388-119">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="d2388-120">az vm</span><span class="sxs-lookup"><span data-stu-id="d2388-120">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="d2388-121">Speicherkonten</span><span class="sxs-lookup"><span data-stu-id="d2388-121">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="d2388-122">az storage account</span><span class="sxs-lookup"><span data-stu-id="d2388-122">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="d2388-123">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="d2388-123">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="d2388-124">az keyvault</span><span class="sxs-lookup"><span data-stu-id="d2388-124">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="d2388-125">Webanwendungen</span><span class="sxs-lookup"><span data-stu-id="d2388-125">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="d2388-126">az webapp</span><span class="sxs-lookup"><span data-stu-id="d2388-126">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="d2388-127">SQL-Datenbanken</span><span class="sxs-lookup"><span data-stu-id="d2388-127">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="d2388-128">az sql server</span><span class="sxs-lookup"><span data-stu-id="d2388-128">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="d2388-129">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d2388-129">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="d2388-130">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="d2388-130">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="d2388-131">Suchen von Befehlen</span><span class="sxs-lookup"><span data-stu-id="d2388-131">Finding commands</span></span>

<span data-ttu-id="d2388-132">Befehle in der CLI werden als _Unterbefehle_ von _Gruppen_ bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="d2388-132">Commands in the CLI are provided as _subcommands_ of _groups_.</span></span>
<span data-ttu-id="d2388-133">Jede Gruppe stellt einen von Azure bereitgestellten Dienst dar, und die Untergruppen unterteilen Befehle für diese Dienste in logische Gruppierungen.</span><span class="sxs-lookup"><span data-stu-id="d2388-133">Each group represents a service provided by Azure, and the subgroups divide commands for these services into logical groupings.</span></span>

<span data-ttu-id="d2388-134">Suchen Sie Befehle mithilfe von [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="d2388-134">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="d2388-135">Verwenden Sie den folgenden Befehl, um beispielsweise nach Befehlsnamen zu suchen, die `secret` enthalten:</span><span class="sxs-lookup"><span data-stu-id="d2388-135">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find -q secret
```

<span data-ttu-id="d2388-136">Wenn Sie wissen, mit welcher Gruppe von Befehlen Sie arbeiten möchten, ist das Argument `--help` unter Umständen besser geeignet.</span><span class="sxs-lookup"><span data-stu-id="d2388-136">If you know which group of commands you want to work with, the `--help` argument may be a better choice.</span></span> <span data-ttu-id="d2388-137">Damit werden nicht nur detaillierte Informationen für einen Befehl, sondern – bei Verwendung mit einer Befehlsgruppe – alle verfügbaren Unterbefehle angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d2388-137">This displays not just detailed information for a command, but when used with a command group, displays all of the available subcommands.</span></span> <span data-ttu-id="d2388-138">Beispielsweise können Sie bei Verwendung von Netzwerksicherheitsgruppen (NSGs) die verfügbaren Untergruppen und Befehle der NSGs ermitteln.</span><span class="sxs-lookup"><span data-stu-id="d2388-138">For example, when working with Network Security Groups (NSGs) you can find the available NSG subgroups and commands.</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="d2388-139">Die CLI ermöglicht unter der Bash-Shell die Vervollständigung mit der TAB-TASTE.</span><span class="sxs-lookup"><span data-stu-id="d2388-139">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="d2388-140">Global verfügbare Argumente</span><span class="sxs-lookup"><span data-stu-id="d2388-140">Globally available arguments</span></span>

<span data-ttu-id="d2388-141">Es gibt einige Argumente, die für jeden Befehl verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="d2388-141">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="d2388-142">`--help` gibt CLI-Referenzinformationen zu Befehlen und ihren Argumenten zurück und führt verfügbare Untergruppen und Befehle auf.</span><span class="sxs-lookup"><span data-stu-id="d2388-142">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="d2388-143">`--output` ändert das Ausgabeformat.</span><span class="sxs-lookup"><span data-stu-id="d2388-143">`--output` changes the output format.</span></span> <span data-ttu-id="d2388-144">Verfügbare Ausgabeformate: `json`, `jsonc` (farbiger JSON-Code), `tsv` (per Tabulator getrennte Werte) und `table` (für Menschen lesbare ASCII-Tabellen).</span><span class="sxs-lookup"><span data-stu-id="d2388-144">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), and `table` (human-readable ASCII tables).</span></span> <span data-ttu-id="d2388-145">Die CLI gibt standardmäßig `json` aus.</span><span class="sxs-lookup"><span data-stu-id="d2388-145">By default the CLI outputs `json`.</span></span> <span data-ttu-id="d2388-146">Weitere Informationen zu den verfügbaren Ausgabeformaten finden Sie unter [Ausgabeformate für Azure CLI 2.0-Befehle](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d2388-146">To learn more about the available output formats, see [Output formats for Azure CLI 2.0](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="d2388-147">`--query` verwendet die [JMESPath-Abfragesprache](http://jmespath.org/) zum Filtern der von Azure-Diensten zurückgegebenen Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="d2388-147">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="d2388-148">Weitere Informationen zu Abfragen finden Sie unter [Verwenden von JMESPath-Abfragen mit Azure CLI 2.0](query-azure-cli.md) und im [JMESPath-Tutorial](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="d2388-148">To learn To learn more about queries, see [Query command results with Azure CLI 2.0](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="d2388-149">`--verbose` gibt Informationen zu Ressourcen, die in Azure während eines Vorgangs erstellt werden, und andere nützliche Informationen aus.</span><span class="sxs-lookup"><span data-stu-id="d2388-149">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="d2388-150">`--debug` gibt noch mehr Informationen zu CLI-Vorgängen aus, die zum Debuggen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="d2388-150">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="d2388-151">Wenn ein Fehler auftritt, stellen Sie beim Übermitteln eines Fehlerberichts die mit dem Flag `--debug` generierte Ausgabe bereit.</span><span class="sxs-lookup"><span data-stu-id="d2388-151">If you encounter a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="d2388-152">Interaktiver Modus</span><span class="sxs-lookup"><span data-stu-id="d2388-152">Interactive mode</span></span>

<span data-ttu-id="d2388-153">Die CLI bietet einen interaktiven Modus, der automatisch Hilfeinformationen anzeigt und die Auswahl von Unterbefehlen vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="d2388-153">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="d2388-154">Sie wechseln mit dem Befehl [az interactive](/cli/azure/reference-index#az-interactive) in den interaktiven Modus.</span><span class="sxs-lookup"><span data-stu-id="d2388-154">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="d2388-155">Weitere Informationen zum interaktiven Modus finden Sie unter [Interaktive Azure CLI 2.0](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d2388-155">For more information on interactive mode, see [Azure CLI 2.0 Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="d2388-156">Darüber hinaus gibt es ein [Visual Studio Code-Plug-In](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli), das eine interaktive Benutzeroberfläche bereitstellt. Diese bietet unter anderem Funktionen wie AutoVervollständigen und die Anzeige von Informationen beim Daraufzeigen.</span><span class="sxs-lookup"><span data-stu-id="d2388-156">There is also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="d2388-157">Lernen der CLI-Grundlagen mit Schnellstarts und Tutorials</span><span class="sxs-lookup"><span data-stu-id="d2388-157">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="d2388-158">Sehen Sie sich für die ersten Schritte mit der Azure CLI 2.0 ein ausführliches Tutorial an, in dem Sie lernen, wie Sie virtuelle Computer einrichten und die Funktionen der CLI zum Abfragen von Azure-Ressourcen nutzen.</span><span class="sxs-lookup"><span data-stu-id="d2388-158">To get you started with the Azure CLI 2.0, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="d2388-159">Erstellen von virtuellen Computern mit der Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="d2388-159">Create virtual machines with the Azure CLI 2.0 tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="d2388-160">Wenn Sie sich eher auf andere Dienste konzentrieren möchten, stehen verschiedene Schnellstartanleitungen für Azure-Dienste zur Verfügung, die die CLI nutzen.</span><span class="sxs-lookup"><span data-stu-id="d2388-160">If you would rather focus on other services, there are a variety of quickstarts for Azure services that use the CLI.</span></span>

* [<span data-ttu-id="d2388-161">Erstellen eines Speicherkontos mit der Azure-Befehlszeilenschnittstelle</span><span class="sxs-lookup"><span data-stu-id="d2388-161">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* <span data-ttu-id="d2388-162">[Transfer objects to/from Azure Blob storage using the CLI](/azure/storage/blobs/storage-quickstart-blobs-cli) (Übertragen von Objekten in/aus Azure Blob Storage mit der CLI)</span><span class="sxs-lookup"><span data-stu-id="d2388-162">[Transfer objects to/from Azure Blob storage using the CLI](/azure/storage/blobs/storage-quickstart-blobs-cli)</span></span>
* [<span data-ttu-id="d2388-163">Erstellen einer einzelnen Azure SQL-Datenbank mithilfe der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="d2388-163">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="d2388-164">Erstellen eines Azure Database for MySQL-Servers mithilfe der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="d2388-164">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="d2388-165">Erstellen einer Azure-Datenbank für PostgreSQL mithilfe der Azure-CLI</span><span class="sxs-lookup"><span data-stu-id="d2388-165">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="d2388-166">Erstellen einer Python-Web-App in Azure</span><span class="sxs-lookup"><span data-stu-id="d2388-166">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="d2388-167">Ausführen eines benutzerdefinierten Image von Docker-Hubs in Azure-Web-Apps für Container</span><span class="sxs-lookup"><span data-stu-id="d2388-167">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="d2388-168">Abgeben von Feedback</span><span class="sxs-lookup"><span data-stu-id="d2388-168">Give feedback</span></span>

<span data-ttu-id="d2388-169">Ihr Feedback zur CLI hilft uns dabei, Verbesserungen vorzunehmen und Fehler zu beheben.</span><span class="sxs-lookup"><span data-stu-id="d2388-169">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="d2388-170">Sie können [ein Problem auf Github melden](https://github.com/azure/azure-cli/issues) oder mit den integrierten Features der CLI und dem Befehl [az feedback](/cli/azure/reference-index#az-feedback) allgemeines Feedback hinterlassen.</span><span class="sxs-lookup"><span data-stu-id="d2388-170">You can [file an issue on Github](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```

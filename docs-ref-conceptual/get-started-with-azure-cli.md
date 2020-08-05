---
title: Erste Schritte mit der Azure CLI
description: Erste Schritte mit der Azure CLI durch das Erlernen der Befehlsgrundlagen.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/30/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: ffedd3d1fdbcba89106f2725b58ca62b11f4c27b
ms.sourcegitcommit: bf84dfb62e910ea246586481863bb43d09d07795
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/04/2020
ms.locfileid: "87551386"
---
# <a name="get-started-with-azure-cli"></a><span data-ttu-id="8037d-103">Erste Schritte mit der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="8037d-103">Get started with Azure CLI</span></span>

<span data-ttu-id="8037d-104">Willkommen bei der Azure CLI!</span><span class="sxs-lookup"><span data-stu-id="8037d-104">Welcome to the Azure CLI!</span></span>  <span data-ttu-id="8037d-105">Dieser Artikel bietet eine Einführung in die CLI und unterstützt Sie beim Ausführen allgemeiner Aufgaben.</span><span class="sxs-lookup"><span data-stu-id="8037d-105">This article introduces the CLI and helps you complete common tasks.</span></span>

> [!NOTE]
>
> <span data-ttu-id="8037d-106">In Skripts und auf der Microsoft-Dokumentationswebsite sind Azure CLI-Beispiele für die `bash`-Shell geschrieben.</span><span class="sxs-lookup"><span data-stu-id="8037d-106">In scripts and on the Microsoft documentation site, Azure CLI examples are written for the `bash` shell.</span></span> <span data-ttu-id="8037d-107">Einzeilige Beispiele können auf jeder Plattform ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="8037d-107">One-line examples will run on any platform.</span></span> <span data-ttu-id="8037d-108">Längere Beispiele mit Zeilenfortsetzungen (`\`) oder Variablenzuweisung müssen angepasst werden, damit sie in anderen Shells verwendet werden können (einschließlich PowerShell).</span><span class="sxs-lookup"><span data-stu-id="8037d-108">Longer examples which include line continuations (`\`) or variable assignment need to be modified to work on other shells, including PowerShell.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="8037d-109">Installieren oder Ausführen in Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="8037d-109">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="8037d-110">Am einfachsten können Sie die Azure-Befehlszeilenschnittstelle in einer Azure Cloud Shell-Umgebung über Ihren Browser verwenden.</span><span class="sxs-lookup"><span data-stu-id="8037d-110">The easiest way to get started with the Azure CLI is by running it in an Azure Cloud Shell environment through your browser.</span></span> <span data-ttu-id="8037d-111">Informationen zu Cloud Shell finden Sie unter [Schnellstart für Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="8037d-111">To learn about Cloud Shell, see  [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

<span data-ttu-id="8037d-112">Wenn Sie zur Installation der Befehlszeilenschnittstelle bereit sind, lesen Sie die [Installationsanweisungen](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="8037d-112">When you're ready to install the CLI, see the [installation instructions](install-azure-cli.md).</span></span>

<span data-ttu-id="8037d-113">Führen Sie nach der Erstinstallation der CLI `az --version` aus, um zu überprüfen, ob sie installiert wurde und die korrekte Version aufweist.</span><span class="sxs-lookup"><span data-stu-id="8037d-113">After installing the CLI for the first time, check that it's installed and you've got the correct version by running `az --version`.</span></span>

> [!NOTE]
> <span data-ttu-id="8037d-114">[Installieren Sie die klassische Azure CLI](install-classic-cli.md), wenn Sie das klassische Azure-Bereitstellungsmodell verwenden.</span><span class="sxs-lookup"><span data-stu-id="8037d-114">If you're using the Azure classic deployment model, [install the Azure classic CLI](install-classic-cli.md).</span></span>

## <a name="sign-in"></a><span data-ttu-id="8037d-115">Anmelden</span><span class="sxs-lookup"><span data-stu-id="8037d-115">Sign in</span></span>

<span data-ttu-id="8037d-116">Bevor Sie CLI-Befehle mit einer lokalen Installation verwenden, müssen Sie sich mithilfe von [az login](/cli/azure/reference-index#az-login) anmelden.</span><span class="sxs-lookup"><span data-stu-id="8037d-116">Before using any CLI commands with a local install, you need to sign in with [az login](/cli/azure/reference-index#az-login).</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="8037d-117">Nach der Anmeldung sehen Sie eine Liste der mit Ihrem Azure-Konto verknüpften Abonnements.</span><span class="sxs-lookup"><span data-stu-id="8037d-117">After logging in, you see a list of subscriptions associated with your Azure account.</span></span> <span data-ttu-id="8037d-118">Die Abonnementinformationen mit `isDefault: true` ist das momentan aktivierte Abonnement nach der Anmeldung.</span><span class="sxs-lookup"><span data-stu-id="8037d-118">The subscription information with `isDefault: true` is the currently activated subscription after logging in.</span></span> <span data-ttu-id="8037d-119">Zur Auswahl eines anderen Abonnements verwenden Sie den Befehl [az account set](/cli/azure/account#az-account-set) mit der ID des Abonnements, zu dem Sie wechseln möchten.</span><span class="sxs-lookup"><span data-stu-id="8037d-119">To select another subscription, use the [az account set](/cli/azure/account#az-account-set) command with the subscription ID to switch to.</span></span> <span data-ttu-id="8037d-120">Weitere Informationen zur Abonnementauswahl finden Sie unter [Verwenden mehrerer Azure-Abonnements](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="8037d-120">For more information about subscription selection, see [Use multiple Azure subscriptions](manage-azure-subscriptions-azure-cli.md).</span></span>

<span data-ttu-id="8037d-121">Es gibt auch Wege, wie Sie sich nicht interaktiv anmelden können. Diese werden unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md) ausführlich beschrieben.</span><span class="sxs-lookup"><span data-stu-id="8037d-121">There are ways to sign in non-interactively, which are covered in detail in [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="common-commands"></a><span data-ttu-id="8037d-122">Häufig verwendete Befehle</span><span class="sxs-lookup"><span data-stu-id="8037d-122">Common commands</span></span>

<span data-ttu-id="8037d-123">Die folgende Tabelle enthält einige allgemeine Befehle, die in der CLI verwendet werden, sowie Links zu ihrer Referenzdokumentation.</span><span class="sxs-lookup"><span data-stu-id="8037d-123">This table lists some common commands used in the CLI and links to their reference documentation.</span></span>

| <span data-ttu-id="8037d-124">Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8037d-124">Resource type</span></span> | <span data-ttu-id="8037d-125">Azure CLI-Befehlsgruppe</span><span class="sxs-lookup"><span data-stu-id="8037d-125">Azure CLI command group</span></span> |
|---------------|-------------------------|
| [<span data-ttu-id="8037d-126">Ressourcengruppe</span><span class="sxs-lookup"><span data-stu-id="8037d-126">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="8037d-127">az group</span><span class="sxs-lookup"><span data-stu-id="8037d-127">az group</span></span>](/cli/azure/group) |
| [<span data-ttu-id="8037d-128">Virtuelle Computer</span><span class="sxs-lookup"><span data-stu-id="8037d-128">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="8037d-129">az vm</span><span class="sxs-lookup"><span data-stu-id="8037d-129">az vm</span></span>](/cli/azure/vm) |
| [<span data-ttu-id="8037d-130">Speicherkonten</span><span class="sxs-lookup"><span data-stu-id="8037d-130">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="8037d-131">az storage account</span><span class="sxs-lookup"><span data-stu-id="8037d-131">az storage account</span></span>](/cli/azure/storage/account) |
| [<span data-ttu-id="8037d-132">Schlüsseltresor</span><span class="sxs-lookup"><span data-stu-id="8037d-132">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="8037d-133">az keyvault</span><span class="sxs-lookup"><span data-stu-id="8037d-133">az keyvault</span></span>](/cli/azure/keyvault) |
| [<span data-ttu-id="8037d-134">Webanwendungen</span><span class="sxs-lookup"><span data-stu-id="8037d-134">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="8037d-135">az webapp</span><span class="sxs-lookup"><span data-stu-id="8037d-135">az webapp</span></span>](/cli/azure/webapp) |
| [<span data-ttu-id="8037d-136">SQL-Datenbanken</span><span class="sxs-lookup"><span data-stu-id="8037d-136">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="8037d-137">az sql server</span><span class="sxs-lookup"><span data-stu-id="8037d-137">az sql server</span></span>](/cli/azure/sql/server) |
| [<span data-ttu-id="8037d-138">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8037d-138">CosmosDB</span></span>](/azure/cosmos-db) | [<span data-ttu-id="8037d-139">az cosmosdb</span><span class="sxs-lookup"><span data-stu-id="8037d-139">az cosmosdb</span></span>](/cli/azure/cosmosdb) |

## <a name="finding-commands"></a><span data-ttu-id="8037d-140">Suchen von Befehlen</span><span class="sxs-lookup"><span data-stu-id="8037d-140">Finding commands</span></span>

<span data-ttu-id="8037d-141">Befehle in der CLI werden als _Befehle_ von _Gruppen_ organisiert.</span><span class="sxs-lookup"><span data-stu-id="8037d-141">Commands in the CLI are organized as _commands_ of _groups_.</span></span> <span data-ttu-id="8037d-142">Jede Gruppe stellt einen Azure-Dienst dar, und Befehle werden für diesen Dienst ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="8037d-142">Each group represents an Azure service, and commands operate on that service.</span></span>

<span data-ttu-id="8037d-143">Suchen Sie Befehle mithilfe von [az find](/cli/azure/reference-index#az-find).</span><span class="sxs-lookup"><span data-stu-id="8037d-143">To search for commands, use [az find](/cli/azure/reference-index#az-find).</span></span> <span data-ttu-id="8037d-144">Verwenden Sie den folgenden Befehl, um beispielsweise nach Befehlsnamen zu suchen, die `secret` enthalten:</span><span class="sxs-lookup"><span data-stu-id="8037d-144">For example, to search for command names containing `secret`, use the following command:</span></span>

```azurecli-interactive
az find secret
```

<span data-ttu-id="8037d-145">Verwenden Sie das Argument `--help`, um eine vollständige Liste der Befehle und Untergruppen einer Gruppe abzurufen.</span><span class="sxs-lookup"><span data-stu-id="8037d-145">Use the `--help` argument to get a complete list of commands and subgroups of a group.</span></span> <span data-ttu-id="8037d-146">Geben Sie beispielsweise Folgendes ein, um die CLI-Befehle für die Verwendung mit Netzwerksicherheitsgruppen (NSGs) zu ermitteln:</span><span class="sxs-lookup"><span data-stu-id="8037d-146">For example, to find the CLI commands for working with Network Security Groups (NSGs):</span></span>

```azurecli-interactive
az network nsg --help
```

<span data-ttu-id="8037d-147">Die CLI ermöglicht unter der Bash-Shell die Vervollständigung mit der TAB-TASTE.</span><span class="sxs-lookup"><span data-stu-id="8037d-147">The CLI has full tab completion for commands under the bash shell.</span></span>

## <a name="globally-available-arguments"></a><span data-ttu-id="8037d-148">Global verfügbare Argumente</span><span class="sxs-lookup"><span data-stu-id="8037d-148">Globally available arguments</span></span>

<span data-ttu-id="8037d-149">Es gibt einige Argumente, die für jeden Befehl verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="8037d-149">There are some arguments that are available for every command.</span></span>

* <span data-ttu-id="8037d-150">`--help` gibt CLI-Referenzinformationen zu Befehlen und ihren Argumenten zurück und führt verfügbare Untergruppen und Befehle auf.</span><span class="sxs-lookup"><span data-stu-id="8037d-150">`--help` prints CLI reference information about commands and their arguments and lists available subgroups and commands.</span></span>
* <span data-ttu-id="8037d-151">`--output` ändert das Ausgabeformat.</span><span class="sxs-lookup"><span data-stu-id="8037d-151">`--output` changes the output format.</span></span> <span data-ttu-id="8037d-152">Verfügbare Ausgabeformate: `json`, `jsonc` (farbiger JSON-Code), `tsv` (per Tabulator getrennte Werte), `table` (für Menschen lesbare ASCII-Tabellen) und `yaml`.</span><span class="sxs-lookup"><span data-stu-id="8037d-152">The available output formats are `json`, `jsonc` (colorized JSON), `tsv` (Tab-Separated Values), `table` (human-readable ASCII tables), and `yaml`.</span></span> <span data-ttu-id="8037d-153">Die CLI gibt standardmäßig `json` aus.</span><span class="sxs-lookup"><span data-stu-id="8037d-153">By default the CLI outputs `json`.</span></span> <span data-ttu-id="8037d-154">Weitere Informationen zu den verfügbaren Ausgabeformaten finden Sie unter [Ausgabeformate für die Azure CLI](format-output-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="8037d-154">To learn more about the available output formats, see [Output formats for Azure CLI](format-output-azure-cli.md).</span></span>
* <span data-ttu-id="8037d-155">`--query` verwendet die [JMESPath-Abfragesprache](http://jmespath.org/) zum Filtern der von Azure-Diensten zurückgegebenen Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="8037d-155">`--query` uses the [JMESPath query language](http://jmespath.org/) to filter the output returned from Azure services.</span></span> <span data-ttu-id="8037d-156">Weitere Informationen zu Abfragen finden Sie unter [Abfragen von Befehlsergebnissen mit der Azure CLI](query-azure-cli.md) und im [JMESPath-Tutorial](http://jmespath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="8037d-156">To learn more about queries, see [Query command results with Azure CLI](query-azure-cli.md) and the [JMESPath tutorial](http://jmespath.org/tutorial.html).</span></span>
* <span data-ttu-id="8037d-157">`--verbose` gibt Informationen zu Ressourcen, die in Azure während eines Vorgangs erstellt werden, und andere nützliche Informationen aus.</span><span class="sxs-lookup"><span data-stu-id="8037d-157">`--verbose` prints information about resources created in Azure during an operation, and other useful information.</span></span>
* <span data-ttu-id="8037d-158">`--debug` gibt noch mehr Informationen zu CLI-Vorgängen aus, die zum Debuggen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="8037d-158">`--debug` prints even more information about CLI operations, used for debugging purposes.</span></span> <span data-ttu-id="8037d-159">Wenn ein Fehler auftritt, stellen Sie beim Übermitteln eines Fehlerberichts die mit dem Flag `--debug` generierte Ausgabe bereit.</span><span class="sxs-lookup"><span data-stu-id="8037d-159">If you find a bug, provide output generated with the `--debug` flag on when submitting a bug report.</span></span>

## <a name="interactive-mode"></a><span data-ttu-id="8037d-160">Interaktiver Modus</span><span class="sxs-lookup"><span data-stu-id="8037d-160">Interactive mode</span></span>

<span data-ttu-id="8037d-161">Die CLI bietet einen interaktiven Modus, der automatisch Hilfeinformationen anzeigt und die Auswahl von Unterbefehlen vereinfacht.</span><span class="sxs-lookup"><span data-stu-id="8037d-161">The CLI offers an interactive mode that automatically displays help information and makes it easier to select subcommands.</span></span> <span data-ttu-id="8037d-162">Sie wechseln mit dem Befehl [az interactive](/cli/azure/reference-index#az-interactive) in den interaktiven Modus.</span><span class="sxs-lookup"><span data-stu-id="8037d-162">You enter interactive mode with the [az interactive](/cli/azure/reference-index#az-interactive) command.</span></span>

```azurecli-interactive
az interactive
```

<span data-ttu-id="8037d-163">Weitere Informationen zum interaktiven Modus finden Sie unter [Azure CLI – Interaktiver Modus](interactive-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="8037d-163">For more information on interactive mode, see [Azure CLI Interactive Mode](interactive-azure-cli.md).</span></span>

<span data-ttu-id="8037d-164">Darüber hinaus gibt es ein [Visual Studio Code-Plug-In](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli), das eine interaktive Benutzeroberfläche bereitstellt. Diese bietet unter anderem Funktionen wie AutoVervollständigen und die Anzeigen von Informationen beim Daraufzeigen.</span><span class="sxs-lookup"><span data-stu-id="8037d-164">There's also a [Visual Studio Code plugin](https://marketplace.visualstudio.com/items?itemName=ms-vscode.azurecli) that offers an interactive experience, including autocomplete and mouse-over documentation.</span></span>

## <a name="learn-cli-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="8037d-165">Lernen der CLI-Grundlagen mit Schnellstarts und Tutorials</span><span class="sxs-lookup"><span data-stu-id="8037d-165">Learn CLI basics with quickstarts and tutorials</span></span>

<span data-ttu-id="8037d-166">Sehen Sie sich zu den ersten Schritten mit der Azure CLI ein ausführliches Tutorial an, in dem Sie lernen, wie Sie virtuelle Computer einrichten und die Funktionen der CLI zum Abfragen von Azure-Ressourcen nutzen.</span><span class="sxs-lookup"><span data-stu-id="8037d-166">To get you started with the Azure CLI, try an in-depth tutorial for setting up virtual machines and using the power of the CLI to query Azure resources.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="8037d-167">Erstellen von virtuellen Computern mit der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="8037d-167">Create virtual machines with the Azure CLI tutorial</span></span>](azure-cli-vm-tutorial.yml)

<span data-ttu-id="8037d-168">Es gibt auch Schnellstartanleitungen für andere beliebte Dienste.</span><span class="sxs-lookup"><span data-stu-id="8037d-168">There are also quickstarts for other popular services.</span></span>

* [<span data-ttu-id="8037d-169">Erstellen eines Speicherkontos mit der Azure-Befehlszeilenschnittstelle</span><span class="sxs-lookup"><span data-stu-id="8037d-169">Create a storage account using the Azure CLI</span></span>](/azure/storage/common/storage-quickstart-create-storage-account-cli)
* <span data-ttu-id="8037d-170">[Transfer objects to/from Azure Blob storage using the CLI](/azure/storage/blobs/storage-quickstart-blobs-cli) (Übertragen von Objekten in/aus Azure Blob Storage mit der CLI)</span><span class="sxs-lookup"><span data-stu-id="8037d-170">[Transfer objects to/from Azure Blob storage using the CLI](/azure/storage/blobs/storage-quickstart-blobs-cli)</span></span>
* [<span data-ttu-id="8037d-171">Erstellen einer einzelnen Azure SQL-Datenbank mithilfe der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="8037d-171">Create a single Azure SQL database using the Azure CLI</span></span>](/azure/sql-database/sql-database-get-started-cli)
* [<span data-ttu-id="8037d-172">Erstellen eines Azure Database for MySQL-Servers mithilfe der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="8037d-172">Create an Azure Database for MySQL server using the Azure CLI</span></span>](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli)
* [<span data-ttu-id="8037d-173">Erstellen einer Azure-Datenbank für PostgreSQL mithilfe der Azure-CLI</span><span class="sxs-lookup"><span data-stu-id="8037d-173">Create an Azure Database for PostgreSQL using the Azure CLI</span></span>](/azure/postgresql/quickstart-create-server-database-azure-cli)
* [<span data-ttu-id="8037d-174">Erstellen einer Python-Web-App in Azure</span><span class="sxs-lookup"><span data-stu-id="8037d-174">Create a Python web app in Azure</span></span>](/azure/app-service/app-service-web-get-started-python)
* [<span data-ttu-id="8037d-175">Ausführen eines benutzerdefinierten Image von Docker-Hubs in Azure-Web-Apps für Container</span><span class="sxs-lookup"><span data-stu-id="8037d-175">Run a custom Docker Hub image in Azure Web Apps for Containers</span></span>](/azure/app-service/containers/quickstart-custom-docker-image)

## <a name="give-feedback"></a><span data-ttu-id="8037d-176">Abgeben von Feedback</span><span class="sxs-lookup"><span data-stu-id="8037d-176">Give feedback</span></span>

<span data-ttu-id="8037d-177">Ihr Feedback zur CLI hilft uns dabei, Verbesserungen vorzunehmen und Fehler zu beheben.</span><span class="sxs-lookup"><span data-stu-id="8037d-177">We welcome your feedback for the CLI to help us make improvements and resolve bugs.</span></span> <span data-ttu-id="8037d-178">Sie können [ein Problem auf GitHub melden](https://github.com/azure/azure-cli/issues) oder mit den integrierten Features der CLI und dem Befehl [az feedback](/cli/azure/reference-index#az-feedback) allgemeines Feedback hinterlassen.</span><span class="sxs-lookup"><span data-stu-id="8037d-178">You can [file an issue on GitHub](https://github.com/azure/azure-cli/issues) or use the built-in features of the CLI to leave general feedback with the [az feedback](/cli/azure/reference-index#az-feedback) command.</span></span>

```azurecli-interactive
az feedback
```

## <a name="see-also"></a><span data-ttu-id="8037d-179">Weitere Informationen</span><span class="sxs-lookup"><span data-stu-id="8037d-179">See also</span></span>

* [<span data-ttu-id="8037d-180">Dienste, die von der Azure CLI verwaltet werden können</span><span class="sxs-lookup"><span data-stu-id="8037d-180">Services the Azure CLI can manage</span></span>](azure-services-the-azure-cli-can-manage.md)
* [<span data-ttu-id="8037d-181">Vollständige Liste mit Befehlsreferenzen für die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="8037d-181">Full command reference list for the Azure CLI</span></span>](/cli/azure/reference-index)
* [<span data-ttu-id="8037d-182">Beliebte Artikel zur Verwendung der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="8037d-182">Popular articles on using the Azure CLI</span></span>](popular-articles-using-the-azure-cli.md)

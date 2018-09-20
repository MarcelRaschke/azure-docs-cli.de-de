---
title: Übersicht über Azure CLI 2.0
description: Enthält eine Übersicht über Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 55c5ea3ad69df60d211cc076e3570e9f07040af7
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388387"
---
# <a name="azure-cli-20"></a><span data-ttu-id="0d2db-103">Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="0d2db-103">Azure CLI 2.0</span></span>

<span data-ttu-id="0d2db-104">Die Azure CLI 2.0 ist die plattformübergreifende Befehlszeilenumgebung von Microsoft zum Verwalten von Azure-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="0d2db-104">The Azure CLI 2.0 is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="0d2db-105">Sie können sie in Ihrem Browser mit [Azure Cloud Shell](/azure/cloud-shell/overview) verwenden oder unter macOS, Linux oder Windows [installieren](install-azure-cli.md) und über die Befehlszeile ausführen.</span><span class="sxs-lookup"><span data-stu-id="0d2db-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="0d2db-106">Der Einstieg in die Azure CLI 2.0 ist einfach, und sie eignet sich am besten für die Erstellung von Automatisierungsskripts für Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="0d2db-106">Azure CLI 2.0 is simple to get started with, and best used for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="0d2db-107">Mit Azure CLI 2.0 können Sie VMs in Azure erstellen, indem Sie einfach den folgenden Befehl eingeben:</span><span class="sxs-lookup"><span data-stu-id="0d2db-107">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a><span data-ttu-id="0d2db-108">Ausführen oder Installieren</span><span class="sxs-lookup"><span data-stu-id="0d2db-108">Run or Install</span></span>

<span data-ttu-id="0d2db-109">Sie können die CLI lokal installieren oder im Browser mit Azure Cloud Shell oder in einem Docker-Container ausführen.</span><span class="sxs-lookup"><span data-stu-id="0d2db-109">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span>

* <span data-ttu-id="0d2db-110">Informationen zum Ausführen im Browser mit Azure Cloud Shell finden Sie unter [Schnellstart für Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) oder [Schnellstartanleitung für PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="0d2db-110">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="0d2db-111">Informationen zur Installation der Azure CLI finden Sie unter [Installieren der Azure CLI 2.0](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0d2db-111">To install the CLI, see [Install the Azure CLI 2.0](install-azure-cli.md).</span></span>
* <span data-ttu-id="0d2db-112">Informationen zur Ausführung als Docker-Container finden Sie unter [Ausführen der Azure CLI 2.0 in einem Docker-Container](run-azure-cli-docker.md).</span><span class="sxs-lookup"><span data-stu-id="0d2db-112">To run as a Docker container, see [Run Azure CLI 2.0 in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="get-started"></a><span data-ttu-id="0d2db-113">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="0d2db-113">Get started</span></span>

<span data-ttu-id="0d2db-114">Lesen Sie den Artikel mit den [ersten Schritten](get-started-with-azure-cli.md), um mehr über die Grundlagen der CLI zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="0d2db-114">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="0d2db-115">Die folgenden Beispiele zeigen einige allgemeine Anwendungsfälle:</span><span class="sxs-lookup"><span data-stu-id="0d2db-115">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="0d2db-116">Virtuelle Linux-Computer</span><span class="sxs-lookup"><span data-stu-id="0d2db-116">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="0d2db-117">Virtuelle Windows-Computer</span><span class="sxs-lookup"><span data-stu-id="0d2db-117">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="0d2db-118">Web-Apps</span><span class="sxs-lookup"><span data-stu-id="0d2db-118">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="0d2db-119">SQL-Datenbank</span><span class="sxs-lookup"><span data-stu-id="0d2db-119">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="0d2db-120">Außerdem ist eine ausführliche [Referenz](/cli/azure/reference-index) verfügbar, in der dokumentiert ist, wie Sie die einzelnen Azure CLI 2.0-Befehle verwenden.</span><span class="sxs-lookup"><span data-stu-id="0d2db-120">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

> [!NOTE]
> <span data-ttu-id="0d2db-121">Falls Sie die vorherige Version der CLI (Azure CLI 1.0) nutzen, können Sie sie weiterverwenden.</span><span class="sxs-lookup"><span data-stu-id="0d2db-121">If you use the previous version of the CLI (Azure CLI 1.0), you can continue to use it.</span></span>
> <span data-ttu-id="0d2db-122">Das beste Ergebnis erzielen Sie jedoch, wenn Sie ein Update auf die aktuelle Version der Azure CLI 2.0 ausführen.</span><span class="sxs-lookup"><span data-stu-id="0d2db-122">However, we recommend updating to use the latest version of Azure CLI 2.0 for the best experience.</span></span>
> <span data-ttu-id="0d2db-123">Beachten Sie bei der Verwendung beider CLIs Folgendes: `azure` ist die alte CLI (Azure-CLI), und `az` ist die neue CLI (Azure CLI 2.0).</span><span class="sxs-lookup"><span data-stu-id="0d2db-123">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>

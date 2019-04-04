---
title: Übersicht über die Azure CLI
description: Übersicht über die Azure-Befehlszeilenschnittstelle (CLI)
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 3b9589c769a90e82c35aa64c583dffdac4e4f063
ms.sourcegitcommit: 1987a39809f9865034b27130e56f30b2bd1eb72c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/19/2019
ms.locfileid: "56421982"
---
# <a name="azure-command-line-interface-cli"></a><span data-ttu-id="65805-103">Azure-Befehlszeilenschnittstelle (CLI)</span><span class="sxs-lookup"><span data-stu-id="65805-103">Azure Command-Line Interface (CLI)</span></span>

<span data-ttu-id="65805-104">Die Azure-Befehlszeilenschnittstelle (CLI) ist die plattformübergreifende Befehlszeilenumgebung von Microsoft zum Verwalten von Azure-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="65805-104">The Azure command-line interface (CLI) is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="65805-105">Sie können sie in Ihrem Browser mit [Azure Cloud Shell](/azure/cloud-shell/overview) verwenden oder unter macOS, Linux oder Windows [installieren](install-azure-cli.md) und über die Befehlszeile ausführen.</span><span class="sxs-lookup"><span data-stu-id="65805-105">Use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="65805-106">Der Einstieg in die Azure CLI ist einfach, und sie eignet sich am besten für die Erstellung von Automatisierungsskripts für Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="65805-106">The Azure CLI is easy to get started with, and best used for building automation scripts that work with the Azure Resource Manager.</span></span>
<span data-ttu-id="65805-107">Mit der Azure CLI können Sie VMs in Azure erstellen, indem Sie einfach den folgenden Befehl eingeben:</span><span class="sxs-lookup"><span data-stu-id="65805-107">Using the Azure CLI, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

> [!NOTE]
>
> <span data-ttu-id="65805-108">In Skripts und auf der Microsoft-Dokumentationswebsite sind Azure CLI-Beispiele für die `bash`-Shell geschrieben.</span><span class="sxs-lookup"><span data-stu-id="65805-108">In scripts and on the Microsoft documentation site, Azure CLI examples are written for the `bash` shell.</span></span> <span data-ttu-id="65805-109">Einzeilige Beispiele können auf jeder Plattform ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="65805-109">One-line examples will run on any platform.</span></span> <span data-ttu-id="65805-110">Längere Beispiele mit Zeilenfortsetzungen (`\`) oder Variablenzuweisung müssen angepasst werden, damit sie in anderen Shells verwendet werden können (einschließlich PowerShell).</span><span class="sxs-lookup"><span data-stu-id="65805-110">Longer examples which include line continuations (`\`) or variable assignment need to be modified to work on other shells, including PowerShell.</span></span>

## <a name="run-or-install"></a><span data-ttu-id="65805-111">Ausführen oder Installieren</span><span class="sxs-lookup"><span data-stu-id="65805-111">Run or Install</span></span>

<span data-ttu-id="65805-112">Sie können die CLI lokal installieren oder im Browser mit Azure Cloud Shell oder in einem Docker-Container ausführen.</span><span class="sxs-lookup"><span data-stu-id="65805-112">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span> <span data-ttu-id="65805-113">Führen Sie zum Abrufen der aktuellen Version der CLI `az --version` aus.</span><span class="sxs-lookup"><span data-stu-id="65805-113">To get the current version of the CLI, run `az --version`.</span></span>

* <span data-ttu-id="65805-114">Informationen zum Ausführen im Browser mit Azure Cloud Shell finden Sie unter [Schnellstart für Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) oder [Schnellstartanleitung für PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="65805-114">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="65805-115">Informationen zur Installation der Azure CLI finden Sie unter [Installieren der Azure CLI](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="65805-115">To install the CLI, see [Install the Azure CLI](install-azure-cli.md).</span></span>
* <span data-ttu-id="65805-116">Informationen zur Ausführung als Docker-Container finden Sie unter [Ausführen der Azure CLI in einem Docker-Container](run-azure-cli-docker.md).</span><span class="sxs-lookup"><span data-stu-id="65805-116">To run as a Docker container, see [Run Azure CLI in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="65805-117">Erweitern Ihrer Fähigkeiten mit Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="65805-117">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="65805-118">Verwalten von virtuellen Computern mit der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="65805-118">Manage virtual machines with the Azure CLI</span></span>](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [<span data-ttu-id="65805-119">Steuern der Azure-Dienste mit der Befehlszeilenschnittstelle</span><span class="sxs-lookup"><span data-stu-id="65805-119">Control Azure services with the CLI</span></span>](/learn/modules/control-azure-services-with-cli/)
- [<span data-ttu-id="65805-120">Mehr interaktives Lernen...</span><span class="sxs-lookup"><span data-stu-id="65805-120">More interactive learning...</span></span>](/learn/browse/?products=azure-clis)

## <a name="get-started"></a><span data-ttu-id="65805-121">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="65805-121">Get started</span></span>

<span data-ttu-id="65805-122">Lesen Sie den Artikel mit den [ersten Schritten](get-started-with-azure-cli.md), um mehr über die Grundlagen der CLI zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="65805-122">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="65805-123">Die folgenden Beispiele zeigen einige allgemeine Anwendungsfälle:</span><span class="sxs-lookup"><span data-stu-id="65805-123">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="65805-124">Virtuelle Linux-Computer</span><span class="sxs-lookup"><span data-stu-id="65805-124">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="65805-125">Virtuelle Windows-Computer</span><span class="sxs-lookup"><span data-stu-id="65805-125">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="65805-126">Web-Apps</span><span class="sxs-lookup"><span data-stu-id="65805-126">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="65805-127">SQL-Datenbank</span><span class="sxs-lookup"><span data-stu-id="65805-127">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="65805-128">Außerdem ist eine ausführliche [Referenz](/cli/azure/reference-index) verfügbar, in der dokumentiert ist, wie Sie die einzelnen Azure CLI-Befehle verwenden.</span><span class="sxs-lookup"><span data-stu-id="65805-128">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI command.</span></span>

> [!NOTE]
> <span data-ttu-id="65805-129">Falls Sie die vorherige Version der CLI (klassische Azure CLI) nutzen, können Sie sie weiterverwenden.</span><span class="sxs-lookup"><span data-stu-id="65805-129">If you use the previous version of the CLI (Azure classic CLI), you can continue to use it.</span></span>
> <span data-ttu-id="65805-130">Das beste Ergebnis erzielen Sie aber, wenn Sie ein Update auf die aktuelle Version der Azure CLI durchführen.</span><span class="sxs-lookup"><span data-stu-id="65805-130">However, we recommend updating to use the latest version of the Azure CLI for the best experience.</span></span>
> <span data-ttu-id="65805-131">Wenn Sie beide CLIs verwenden, sollten Sie daran denken, dass `azure` die klassische CLI und `az` die aktuellste CLI ist.</span><span class="sxs-lookup"><span data-stu-id="65805-131">If you use both CLIs, remember that `azure` is the classic CLI and that `az` is the most recent CLI.</span></span>

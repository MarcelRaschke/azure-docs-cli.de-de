---
title: Übersicht über die Azure CLI
description: Enthält eine Übersicht über die Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 8ab8435f2d8337f63a73aef39472646dc8ebcd74
ms.sourcegitcommit: 0d6b08048b5b35bf0bb3d7b91ff567adbaab2a8b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/07/2018
ms.locfileid: "51222292"
---
# <a name="azure-cli"></a><span data-ttu-id="fe948-103">Azure-Befehlszeilenschnittstelle</span><span class="sxs-lookup"><span data-stu-id="fe948-103">Azure CLI</span></span>

<span data-ttu-id="fe948-104">Die Azure CLI ist die plattformübergreifende Befehlszeilenumgebung von Microsoft zum Verwalten von Azure-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="fe948-104">The Azure CLI is Microsoft's cross-platform command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="fe948-105">Sie können sie in Ihrem Browser mit [Azure Cloud Shell](/azure/cloud-shell/overview) verwenden oder unter macOS, Linux oder Windows [installieren](install-azure-cli.md) und über die Befehlszeile ausführen.</span><span class="sxs-lookup"><span data-stu-id="fe948-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="fe948-106">Der Einstieg in die Azure CLI ist einfach, und sie eignet sich am besten für die Erstellung von Automatisierungsskripts für Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="fe948-106">The Azure CLI is simple to get started with, and best used for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="fe948-107">Mit der Azure CLI können Sie VMs in Azure erstellen, indem Sie einfach den folgenden Befehl eingeben:</span><span class="sxs-lookup"><span data-stu-id="fe948-107">Using the Azure CLI, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

> [!NOTE]
>
> <span data-ttu-id="fe948-108">In Skripts und auf der Microsoft-Dokumentationswebsite sind Azure CLI-Beispiele für die `bash`-Shell geschrieben.</span><span class="sxs-lookup"><span data-stu-id="fe948-108">In scripts and on the Microsoft documentation site, Azure CLI examples are written for the `bash` shell.</span></span> <span data-ttu-id="fe948-109">Einzeilige Beispiele können auf jeder Plattform ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="fe948-109">One-line examples will run on any platform.</span></span> <span data-ttu-id="fe948-110">Längere oder kompliziertere Beispiele mit Zeilenfortsetzungen (`\`) oder Variablenzuweisung müssen angepasst werden, damit sie in anderen Shells verwendet werden können (einschließlich PowerShell).</span><span class="sxs-lookup"><span data-stu-id="fe948-110">Longer or more complicated examples which include line continutions (`\`) or variable assignment will need to be modified to work on other shells, including PowerShell.</span></span>

## <a name="run-or-install"></a><span data-ttu-id="fe948-111">Ausführen oder Installieren</span><span class="sxs-lookup"><span data-stu-id="fe948-111">Run or Install</span></span>

<span data-ttu-id="fe948-112">Sie können die CLI lokal installieren oder im Browser mit Azure Cloud Shell oder in einem Docker-Container ausführen.</span><span class="sxs-lookup"><span data-stu-id="fe948-112">You can install the CLI locally, run it in the browser with Azure Cloud Shell, or run in a Docker container.</span></span>

* <span data-ttu-id="fe948-113">Informationen zum Ausführen im Browser mit Azure Cloud Shell finden Sie unter [Schnellstart für Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) oder [Schnellstartanleitung für PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span><span class="sxs-lookup"><span data-stu-id="fe948-113">To run in your browser with Azure Cloud Shell, see [Quickstart for Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) or [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="fe948-114">Informationen zur Installation der Azure CLI finden Sie unter [Installieren der Azure CLI](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="fe948-114">To install the CLI, see [Install the Azure CLI](install-azure-cli.md).</span></span>
* <span data-ttu-id="fe948-115">Informationen zur Ausführung als Docker-Container finden Sie unter [Ausführen der Azure CLI in einem Docker-Container](run-azure-cli-docker.md).</span><span class="sxs-lookup"><span data-stu-id="fe948-115">To run as a Docker container, see [Run Azure CLI in a Docker Container](run-azure-cli-docker.md)</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="fe948-116">Erweitern Ihrer Fähigkeiten mit Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="fe948-116">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="fe948-117">Verwalten von virtuellen Computern mit der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="fe948-117">Manage virtual machines with the Azure CLI</span></span>](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [<span data-ttu-id="fe948-118">Steuern der Azure-Dienste mit der Befehlszeilenschnittstelle</span><span class="sxs-lookup"><span data-stu-id="fe948-118">Control Azure services with the CLI</span></span>](/learn/modules/control-azure-services-with-cli/)
- [<span data-ttu-id="fe948-119">Mehr interaktives Lernen...</span><span class="sxs-lookup"><span data-stu-id="fe948-119">More interactive learning...</span></span>](/learn/browse/?products=azure-clis)

## <a name="get-started"></a><span data-ttu-id="fe948-120">Erste Schritte</span><span class="sxs-lookup"><span data-stu-id="fe948-120">Get started</span></span>

<span data-ttu-id="fe948-121">Lesen Sie den Artikel mit den [ersten Schritten](get-started-with-azure-cli.md), um mehr über die Grundlagen der CLI zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="fe948-121">Read the [Get Started](get-started-with-azure-cli.md) article to learn the CLI basics.</span></span> <span data-ttu-id="fe948-122">Die folgenden Beispiele zeigen einige allgemeine Anwendungsfälle:</span><span class="sxs-lookup"><span data-stu-id="fe948-122">The following samples demonstrate some common uses cases:</span></span>

- [<span data-ttu-id="fe948-123">Virtuelle Linux-Computer</span><span class="sxs-lookup"><span data-stu-id="fe948-123">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="fe948-124">Virtuelle Windows-Computer</span><span class="sxs-lookup"><span data-stu-id="fe948-124">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="fe948-125">Web-Apps</span><span class="sxs-lookup"><span data-stu-id="fe948-125">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="fe948-126">SQL-Datenbank</span><span class="sxs-lookup"><span data-stu-id="fe948-126">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="fe948-127">Außerdem ist eine ausführliche [Referenz](/cli/azure/reference-index) verfügbar, in der dokumentiert ist, wie Sie die einzelnen Azure CLI-Befehle verwenden.</span><span class="sxs-lookup"><span data-stu-id="fe948-127">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI command.</span></span>

> [!NOTE]
> <span data-ttu-id="fe948-128">Falls Sie die vorherige Version der CLI (klassische Azure CLI) nutzen, können Sie sie weiterverwenden.</span><span class="sxs-lookup"><span data-stu-id="fe948-128">If you use the previous version of the CLI (Azure classic CLI), you can continue to use it.</span></span>
> <span data-ttu-id="fe948-129">Das beste Ergebnis erzielen Sie aber, wenn Sie ein Update auf die aktuelle Version der Azure CLI durchführen.</span><span class="sxs-lookup"><span data-stu-id="fe948-129">However, we recommend updating to use the latest version of the Azure CLI for the best experience.</span></span>
> <span data-ttu-id="fe948-130">Wenn Sie beide CLIs verwenden, sollten Sie daran denken, dass `azure` die klassische CLI und `az` die aktuellste CLI ist.</span><span class="sxs-lookup"><span data-stu-id="fe948-130">If you use both CLIs, remember that `azure` is the classic CLI and that `az` is the most recent CLI.</span></span>

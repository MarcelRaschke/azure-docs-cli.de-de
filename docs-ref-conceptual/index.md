---
title: Azure CLI 2.0
description: Enthält eine Übersicht über Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: ffa435f8c6ee5aa82d2efe2e09d7bcb1f1dc434b
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967689"
---
# <a name="azure-cli-20"></a><span data-ttu-id="c5756-103">Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="c5756-103">Azure CLI 2.0</span></span>

<span data-ttu-id="c5756-104">Die Azure CLI 2.0 ist die plattformübergreifende Befehlszeilenumgebung von Microsoft zum Verwalten von Azure-Ressourcen.</span><span class="sxs-lookup"><span data-stu-id="c5756-104">The Azure CLI 2.0 is Microsoft's cross-platform command line experience for managing Azure resources.</span></span>
<span data-ttu-id="c5756-105">Sie können sie in Ihrem Browser mit [Azure Cloud Shell](/azure/cloud-shell/overview) verwenden oder unter macOS, Linux oder Windows [installieren](install-azure-cli.md) und über die Befehlszeile ausführen.</span><span class="sxs-lookup"><span data-stu-id="c5756-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or [install](install-azure-cli.md) it on macOS, Linux, or Windows and run it from the command line.</span></span>

<span data-ttu-id="c5756-106">Azure CLI 2.0 ist für die Verwaltung von Azure-Ressourcen über die Befehlszeile sowie die Erstellung von Automatisierungsskripts für Azure Resource Manager optimiert.</span><span class="sxs-lookup"><span data-stu-id="c5756-106">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="c5756-107">Mit Azure CLI 2.0 können Sie VMs in Azure erstellen, indem Sie einfach den folgenden Befehl eingeben:</span><span class="sxs-lookup"><span data-stu-id="c5756-107">Using the Azure CLI 2.0, you can create VMs within Azure as easily as typing the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

<span data-ttu-id="c5756-108">Führen Sie die CLI mithilfe von [Cloud Shell](/azure/cloud-shell/overview) in Ihrem Browser aus, oder [installieren](install-azure-cli.md) Sie sie unter macOS, Linux oder Windows.</span><span class="sxs-lookup"><span data-stu-id="c5756-108">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the CLI in your browser, or [install](install-azure-cli.md) it on macOS, Linux, or Windows.</span></span>
<span data-ttu-id="c5756-109">Lesen Sie den Artikel mit den [ersten Schritten](get-started-with-azure-cli.md), um mit der Verwendung der CLI zu beginnen.</span><span class="sxs-lookup"><span data-stu-id="c5756-109">Read the [Get Started](get-started-with-azure-cli.md) article to begin using the CLI.</span></span>
<span data-ttu-id="c5756-110">Informationen zur neuesten Version finden Sie in den [Versionshinweisen](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="c5756-110">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

<span data-ttu-id="c5756-111">Die folgenden Beispiele erleichtern Ihnen den Einstieg in allgemeine Aufgaben in Azure CLI 2.0:</span><span class="sxs-lookup"><span data-stu-id="c5756-111">The following samples help you get started with common tasks in Azure CLI 2.0:</span></span>

- [<span data-ttu-id="c5756-112">Virtuelle Linux-Computer</span><span class="sxs-lookup"><span data-stu-id="c5756-112">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="c5756-113">Virtuelle Windows-Computer</span><span class="sxs-lookup"><span data-stu-id="c5756-113">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="c5756-114">Web-Apps</span><span class="sxs-lookup"><span data-stu-id="c5756-114">Web Apps</span></span>](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [<span data-ttu-id="c5756-115">SQL-Datenbank</span><span class="sxs-lookup"><span data-stu-id="c5756-115">SQL Database</span></span>](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

<span data-ttu-id="c5756-116">Außerdem ist eine ausführliche [Referenz](/cli/azure/reference-index) verfügbar, in der dokumentiert ist, wie Sie die einzelnen Azure CLI 2.0-Befehle verwenden.</span><span class="sxs-lookup"><span data-stu-id="c5756-116">A detailed [reference](/cli/azure/reference-index) is also available that documents how to use each individual Azure CLI 2.0 command.</span></span>

<span data-ttu-id="c5756-117">Führen Sie jetzt die [ersten Schritte](get-started-with-azure-cli.md) mit Azure CLI 2.0 aus.</span><span class="sxs-lookup"><span data-stu-id="c5756-117">[Get started](get-started-with-azure-cli.md) with Azure CLI 2.0 now.</span></span>

> [!NOTE]
> <span data-ttu-id="c5756-118">Falls Sie die vorherige Version der CLI (Azure CLI 1.0) nutzen, können Sie sie weiterverwenden.</span><span class="sxs-lookup"><span data-stu-id="c5756-118">If you use the previous version of the CLI (Azure CLI 1.0), you can continue to use it.</span></span>
> <span data-ttu-id="c5756-119">Das beste Ergebnis erzielen Sie jedoch, wenn Sie ein Update auf die aktuelle Version der Azure CLI 2.0 ausführen.</span><span class="sxs-lookup"><span data-stu-id="c5756-119">However, we recommend updating to use the latest version of Azure CLI 2.0 for the best experience.</span></span>
> <span data-ttu-id="c5756-120">Beachten Sie bei der Verwendung beider CLIs Folgendes: `azure` ist die alte CLI (Azure-CLI), und `az` ist die neue CLI (Azure CLI 2.0).</span><span class="sxs-lookup"><span data-stu-id="c5756-120">If you use both CLIs, remember that `azure` is the old CLI - Azure CLI, and that `az` is the new CLI - Azure CLI 2.0.</span></span>

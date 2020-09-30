---
title: Azure CLI-Referenzen für Azure Data Share
description: Landing Page der Azure CLI-Referenzen für Azure Data Share
services: data-share
author: dbradish-microsoft
manager: barbkess
ms.service: data-share
ms.devlang: azurecli
ms.topic: reference
ms.date: 05/27/2020
ms.author: dbradish
ms.custom: devx-track-azurecli
ms.openlocfilehash: 5d6ed2fae3988bbf43a83d40b10a3dc37ad25dad
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225846"
---
# <a name="azure-cli-for-azure-data-share"></a><span data-ttu-id="effeb-103">Azure CLI für Azure Data Share</span><span class="sxs-lookup"><span data-stu-id="effeb-103">Azure CLI for Azure Data Share</span></span>

<span data-ttu-id="effeb-104">Die Azure-Befehlszeilenschnittstelle ([Azure CLI](./what-is-azure-cli.md)) setzt sich aus Befehlen zum Erstellen und Verwalten von Azure-Ressourcen zusammen.</span><span class="sxs-lookup"><span data-stu-id="effeb-104">The Azure Command Line Interface ([Azure CLI](./what-is-azure-cli.md)) is a set of commands used to create and manage Azure resources.</span></span>  <span data-ttu-id="effeb-105">Sie ist in vielen Azure-Diensten verfügbar, darunter auch Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="effeb-105">It is available across many Azure services including Azure Data Share.</span></span>  <span data-ttu-id="effeb-106">Es stehen mehr als 65 verschiedene Befehle für Data Share bereit.</span><span class="sxs-lookup"><span data-stu-id="effeb-106">There are over 65 different commands for data share!</span></span>  <span data-ttu-id="effeb-107">Mithilfe dieser Befehle können Sie den Dienst effektiv über eine Befehlszeile nutzen.</span><span class="sxs-lookup"><span data-stu-id="effeb-107">These commands give you the ability to work effectively with the service from a command line.</span></span>

## <a name="references-for-data-share"></a><span data-ttu-id="effeb-108">Referenzen für Data Share</span><span class="sxs-lookup"><span data-stu-id="effeb-108">References for Data Share</span></span>

<span data-ttu-id="effeb-109">Alle Azure CLI-Befehle für Azure Data Share sind derzeit Erweiterungen der Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="effeb-109">All Azure CLI commands for Azure Data Share are currently extensions to the Azure CLI.</span></span>  <span data-ttu-id="effeb-110">Eine Erweiterung ermöglicht Ihnen den Zugriff auf experimentelle und vorab veröffentlichte Befehle.</span><span class="sxs-lookup"><span data-stu-id="effeb-110">An extension gives you access to experimental and pre-release commands.</span></span>  <span data-ttu-id="effeb-111">Weitere Informationen zu Erweiterungen finden Sie unter [Verwenden von Erweiterungen mit der Azure CLI](./azure-cli-extensions-overview.md).</span><span class="sxs-lookup"><span data-stu-id="effeb-111">Find out more about extension references in [Use extensions with Azure CLI](./azure-cli-extensions-overview.md).</span></span>

|<span data-ttu-id="effeb-112">Azure CLI-Referenz</span><span class="sxs-lookup"><span data-stu-id="effeb-112">Azure CLI Reference</span></span> |<span data-ttu-id="effeb-113">BESCHREIBUNG</span><span class="sxs-lookup"><span data-stu-id="effeb-113">Description</span></span>
|-|-|-|
| [<span data-ttu-id="effeb-114">az datashare</span><span class="sxs-lookup"><span data-stu-id="effeb-114">az datashare</span></span>](/cli/azure/ext/datashare/datashare) | <span data-ttu-id="effeb-115">Alle Befehle zum Verwalten von Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="effeb-115">All commands to manage Azure Data Share.</span></span>
| [<span data-ttu-id="effeb-116">az datashare account</span><span class="sxs-lookup"><span data-stu-id="effeb-116">az datashare account</span></span>](/cli/azure/ext/datashare/datashare/account) | <span data-ttu-id="effeb-117">Befehle zum Verwalten von Azure Data Share-Konten.</span><span class="sxs-lookup"><span data-stu-id="effeb-117">Commands to manage Azure Data Share accounts.</span></span>
| [<span data-ttu-id="effeb-118">az datashare consumer</span><span class="sxs-lookup"><span data-stu-id="effeb-118">az datashare consumer</span></span>](/cli/azure/ext/datashare/datashare/consumer) | <span data-ttu-id="effeb-119">Befehle für Consumer zum Verwalten von Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="effeb-119">Commands for consumers to manage Azure Data Share.</span></span>
| [<span data-ttu-id="effeb-120">az datashare dataset</span><span class="sxs-lookup"><span data-stu-id="effeb-120">az datashare dataset</span></span>](/cli/azure/ext/datashare/datashare/dataset) | <span data-ttu-id="effeb-121">Befehle für Anbieter zum Verwalten von Azure Data Share-Datasets.</span><span class="sxs-lookup"><span data-stu-id="effeb-121">Commands for providers to manage Azure Data Share datasets.</span></span>
| [<span data-ttu-id="effeb-122">az datashare invitation</span><span class="sxs-lookup"><span data-stu-id="effeb-122">az datashare invitation</span></span>](/cli/azure/ext/datashare/datashare/invitation) | <span data-ttu-id="effeb-123">Befehle für Consumer zum Verwalten von Azure Data Share-Einladungen.</span><span class="sxs-lookup"><span data-stu-id="effeb-123">Commands for consumers to manage Azure Data Share invitations.</span></span>
| [<span data-ttu-id="effeb-124">az datashare provider-share-subscription</span><span class="sxs-lookup"><span data-stu-id="effeb-124">az datashare provider-share-subscription</span></span>](/cli/azure/ext/datashare/datashare/provider-share-subscription) | <span data-ttu-id="effeb-125">Befehle für Anbieter zum Verwalten von Azure Data Share-Abonnements.</span><span class="sxs-lookup"><span data-stu-id="effeb-125">Commands for providers to manage Azure Data Share subscriptions.</span></span>
| [<span data-ttu-id="effeb-126">az datashare synchronization</span><span class="sxs-lookup"><span data-stu-id="effeb-126">az datashare synchronization</span></span>](/cli/azure/ext/datashare/datashare/synchronization)  | <span data-ttu-id="effeb-127">Befehle zum Verwalten der Azure Data Share-Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="effeb-127">Commands to manage Azure Data Share synchronization.</span></span>
| [<span data-ttu-id="effeb-128">az datashare synchronization-setting</span><span class="sxs-lookup"><span data-stu-id="effeb-128">az datashare synchronization-setting</span></span>](/cli/azure/ext/datashare/datashare/synchronization-setting)  | <span data-ttu-id="effeb-129">Befehle für Anbieter zum Verwalten von Azure Data Share-Synchronisierungseinstellungen.</span><span class="sxs-lookup"><span data-stu-id="effeb-129">Commands for providers to manage Azure Data Share synchronization settings.</span></span>

## <a name="reference-examples"></a><span data-ttu-id="effeb-130">Referenzbeispiele</span><span class="sxs-lookup"><span data-stu-id="effeb-130">Reference examples</span></span>

<span data-ttu-id="effeb-131">Es stehen Beispiele für jede Azure CLI-Referenz bereit.</span><span class="sxs-lookup"><span data-stu-id="effeb-131">Examples are provided with every Azure CLI reference.</span></span> <span data-ttu-id="effeb-132">Sie können diese Aufgaben zwar auch über das Azure-Portal ausführen, doch ist zur Verwendung der Azure CLI nur eine einzige Befehlszeile erforderlich.</span><span class="sxs-lookup"><span data-stu-id="effeb-132">Although you can also complete these tasks through the Azure portal, using the Azure CLI requires a single command line.</span></span>  <span data-ttu-id="effeb-133">Nachfolgend sehen Sie einige Codeblöcke, die Ihnen eine Vorstellung davon geben, wie einfach die Azure CLI zu verwenden ist.</span><span class="sxs-lookup"><span data-stu-id="effeb-133">Here are a few code blocks to give you an idea of how easy it is to use the Azure CLI.</span></span>

<span data-ttu-id="effeb-134">Zum Arbeiten mit Azure Data Share benötigen Sie zunächst eine Ressourcengruppe.</span><span class="sxs-lookup"><span data-stu-id="effeb-134">To work with Azure Data Share, you'll first need a resource group.</span></span>  <span data-ttu-id="effeb-135">Azure-Ressourcengruppen können auf einfache Weise mit der Azure CLI erstellt und verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="effeb-135">Azure resource groups are simple to create and manage with the Azure CLI.</span></span>  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

<span data-ttu-id="effeb-136">Genauso einfach kann ein Data Share-Konto erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="effeb-136">It is as straightforward to create a data share account.</span></span>

```azurecli
#create a data share account
az datashare account create --location "West US 2" --tags tag1=Red tag2=White --name MyAccount --resource-group MyResourceGroup
```

## <a name="see-also"></a><span data-ttu-id="effeb-137">Weitere Informationen</span><span class="sxs-lookup"><span data-stu-id="effeb-137">See also</span></span>

* <span data-ttu-id="effeb-138">Unter [Erste Schritte mit der Azure CLI](./get-started-with-azure-cli.md) erhalten Sie Informationen zur Installation und Anmeldung.</span><span class="sxs-lookup"><span data-stu-id="effeb-138">[Get started with Azure CLI](./get-started-with-azure-cli.md) to learn about installation and sign in.</span></span>

* <span data-ttu-id="effeb-139">Entdecken Sie weitere [Befehle](/cli/azure/reference-index) und [Erweiterungen](./azure-cli-extensions-list.md) in der Azure CLI-Dokumentation.</span><span class="sxs-lookup"><span data-stu-id="effeb-139">Discover additional [core](/cli/azure/reference-index) and [extension](./azure-cli-extensions-list.md) references in the Azure CLI documentation.</span></span>
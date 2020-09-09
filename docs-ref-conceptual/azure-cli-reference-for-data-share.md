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
ms.openlocfilehash: e8d834864b2d967beb18e9cd304b922db859ef09
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/09/2020
ms.locfileid: "89562769"
---
# <a name="azure-cli-for-azure-data-share"></a><span data-ttu-id="cf4ec-103">Azure CLI für Azure Data Share</span><span class="sxs-lookup"><span data-stu-id="cf4ec-103">Azure CLI for Azure Data Share</span></span>

<span data-ttu-id="cf4ec-104">Die Azure-Befehlszeilenschnittstelle ([Azure CLI](/cli/azure/what-is-azure-cli)) setzt sich aus Befehlen zum Erstellen und Verwalten von Azure-Ressourcen zusammen.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-104">The Azure Command Line Interface ([Azure CLI](/cli/azure/what-is-azure-cli)) is a set of commands used to create and manage Azure resources.</span></span>  <span data-ttu-id="cf4ec-105">Sie ist in vielen Azure-Diensten verfügbar, darunter auch Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-105">It is available across many Azure services including Azure Data Share.</span></span>  <span data-ttu-id="cf4ec-106">Es stehen mehr als 65 verschiedene Befehle für Data Share bereit.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-106">There are over 65 different commands for data share!</span></span>  <span data-ttu-id="cf4ec-107">Mithilfe dieser Befehle können Sie den Dienst effektiv über eine Befehlszeile nutzen.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-107">These commands give you the ability to work effectively with the service from a command line.</span></span>

## <a name="references-for-data-share"></a><span data-ttu-id="cf4ec-108">Referenzen für Data Share</span><span class="sxs-lookup"><span data-stu-id="cf4ec-108">References for Data Share</span></span>

<span data-ttu-id="cf4ec-109">Alle Azure CLI-Befehle für Azure Data Share sind derzeit Erweiterungen der Azure CLI.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-109">All Azure CLI commands for Azure Data Share are currently extensions to the Azure CLI.</span></span>  <span data-ttu-id="cf4ec-110">Eine Erweiterung ermöglicht Ihnen den Zugriff auf experimentelle und vorab veröffentlichte Befehle.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-110">An extension gives you access to experimental and pre-release commands.</span></span>  <span data-ttu-id="cf4ec-111">Weitere Informationen zu Erweiterungen finden Sie unter [Verwenden von Erweiterungen mit der Azure CLI](/cli/azure/azure-cli-extensions-overview).</span><span class="sxs-lookup"><span data-stu-id="cf4ec-111">Find out more about extension references in [Use extensions with Azure CLI](/cli/azure/azure-cli-extensions-overview).</span></span>

|<span data-ttu-id="cf4ec-112">Azure CLI-Referenz</span><span class="sxs-lookup"><span data-stu-id="cf4ec-112">Azure CLI Reference</span></span> |<span data-ttu-id="cf4ec-113">BESCHREIBUNG</span><span class="sxs-lookup"><span data-stu-id="cf4ec-113">Description</span></span>
|-|-|-|
| [<span data-ttu-id="cf4ec-114">az datashare</span><span class="sxs-lookup"><span data-stu-id="cf4ec-114">az datashare</span></span>](/cli/azure/ext/datashare/datashare) | <span data-ttu-id="cf4ec-115">Alle Befehle zum Verwalten von Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-115">All commands to manage Azure Data Share.</span></span>
| [<span data-ttu-id="cf4ec-116">az datashare account</span><span class="sxs-lookup"><span data-stu-id="cf4ec-116">az datashare account</span></span>](/cli/azure/ext/datashare/datashare/account) | <span data-ttu-id="cf4ec-117">Befehle zum Verwalten von Azure Data Share-Konten.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-117">Commands to manage Azure Data Share accounts.</span></span>
| [<span data-ttu-id="cf4ec-118">az datashare consumer</span><span class="sxs-lookup"><span data-stu-id="cf4ec-118">az datashare consumer</span></span>](/cli/azure/ext/datashare/datashare/consumer) | <span data-ttu-id="cf4ec-119">Befehle für Consumer zum Verwalten von Azure Data Share.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-119">Commands for consumers to manage Azure Data Share.</span></span>
| [<span data-ttu-id="cf4ec-120">az datashare dataset</span><span class="sxs-lookup"><span data-stu-id="cf4ec-120">az datashare dataset</span></span>](/cli/azure/ext/datashare/datashare/dataset) | <span data-ttu-id="cf4ec-121">Befehle für Anbieter zum Verwalten von Azure Data Share-Datasets.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-121">Commands for providers to manage Azure Data Share datasets.</span></span>
| [<span data-ttu-id="cf4ec-122">az datashare invitation</span><span class="sxs-lookup"><span data-stu-id="cf4ec-122">az datashare invitation</span></span>](/cli/azure/ext/datashare/datashare/invitation) | <span data-ttu-id="cf4ec-123">Befehle für Consumer zum Verwalten von Azure Data Share-Einladungen.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-123">Commands for consumers to manage Azure Data Share invitations.</span></span>
| [<span data-ttu-id="cf4ec-124">az datashare provider-share-subscription</span><span class="sxs-lookup"><span data-stu-id="cf4ec-124">az datashare provider-share-subscription</span></span>](/cli/azure/ext/datashare/datashare/provider-share-subscription) | <span data-ttu-id="cf4ec-125">Befehle für Anbieter zum Verwalten von Azure Data Share-Abonnements.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-125">Commands for providers to manage Azure Data Share subscriptions.</span></span>
| [<span data-ttu-id="cf4ec-126">az datashare synchronization</span><span class="sxs-lookup"><span data-stu-id="cf4ec-126">az datashare synchronization</span></span>](/cli/azure/ext/datashare/datashare/synchronization)  | <span data-ttu-id="cf4ec-127">Befehle zum Verwalten der Azure Data Share-Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-127">Commands to manage Azure Data Share synchronization.</span></span>
| [<span data-ttu-id="cf4ec-128">az datashare synchronization-setting</span><span class="sxs-lookup"><span data-stu-id="cf4ec-128">az datashare synchronization-setting</span></span>](/cli/azure/ext/datashare/datashare/synchronization-setting)  | <span data-ttu-id="cf4ec-129">Befehle für Anbieter zum Verwalten von Azure Data Share-Synchronisierungseinstellungen.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-129">Commands for providers to manage Azure Data Share synchronization settings.</span></span>

## <a name="reference-examples"></a><span data-ttu-id="cf4ec-130">Referenzbeispiele</span><span class="sxs-lookup"><span data-stu-id="cf4ec-130">Reference examples</span></span>

<span data-ttu-id="cf4ec-131">Es stehen Beispiele für jede Azure CLI-Referenz bereit.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-131">Examples are provided with every Azure CLI reference.</span></span> <span data-ttu-id="cf4ec-132">Sie können diese Aufgaben zwar auch über das Azure-Portal ausführen, doch ist zur Verwendung der Azure CLI nur eine einzige Befehlszeile erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-132">Although you can also complete these tasks through the Azure portal, using the Azure CLI requires a single command line.</span></span>  <span data-ttu-id="cf4ec-133">Nachfolgend sehen Sie einige Codeblöcke, die Ihnen eine Vorstellung davon geben, wie einfach die Azure CLI zu verwenden ist.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-133">Here are a few code blocks to give you an idea of how easy it is to use the Azure CLI.</span></span>

<span data-ttu-id="cf4ec-134">Zum Arbeiten mit Azure Data Share benötigen Sie zunächst eine Ressourcengruppe.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-134">To work with Azure Data Share, you'll first need a resource group.</span></span>  <span data-ttu-id="cf4ec-135">Azure-Ressourcengruppen können auf einfache Weise mit der Azure CLI erstellt und verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-135">Azure resource groups are simple to create and manage with the Azure CLI.</span></span>  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

<span data-ttu-id="cf4ec-136">Genauso einfach kann ein Data Share-Konto erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-136">It is as straightforward to create a data share account.</span></span>

```azurecli
#create a data share account
az datashare account create --location "West US 2" --tags tag1=Red tag2=White --name MyAccount --resource-group MyResourceGroup
```

## <a name="see-also"></a><span data-ttu-id="cf4ec-137">Weitere Informationen</span><span class="sxs-lookup"><span data-stu-id="cf4ec-137">See also</span></span>

* <span data-ttu-id="cf4ec-138">Unter [Erste Schritte mit der Azure CLI](/cli/azure/get-started-with-azure-cli) erhalten Sie Informationen zur Installation und Anmeldung.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-138">[Get started with Azure CLI](/cli/azure/get-started-with-azure-cli) to learn about installation and sign in.</span></span>

* <span data-ttu-id="cf4ec-139">Entdecken Sie weitere [Befehle](/cli/azure/reference-index) und [Erweiterungen](/cli/azure/azure-cli-extensions-list) in der Azure CLI-Dokumentation.</span><span class="sxs-lookup"><span data-stu-id="cf4ec-139">Discover additional [core](/cli/azure/reference-index) and [extension](/cli/azure/azure-cli-extensions-list) references in the Azure CLI documentation.</span></span>

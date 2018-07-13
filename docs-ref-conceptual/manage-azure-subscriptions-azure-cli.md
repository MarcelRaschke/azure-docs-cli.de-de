---
title: Verwalten von Azure-Abonnements mit Azure CLI
description: Verwalten Sie Azure-Abonnements mit Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/15/2018
ms.topic: conceptual
ms.produdct: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: active-directory
ms.openlocfilehash: f5fdfba785d849b1fd4f5919870ec9c341bb9c7d
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967808"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="244f6-103">Verwalten mehrerer Azure-Abonnements</span><span class="sxs-lookup"><span data-stu-id="244f6-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="244f6-104">Die meisten Azure-Benutzer verwenden nur ein einzelnes Abonnement.</span><span class="sxs-lookup"><span data-stu-id="244f6-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="244f6-105">Wenn Sie allerdings mehreren Organisationen angehören oder Ihre Organisation den Zugriff auf bestimmte Ressourcen über Gruppierungen aufgeteilt hat, besitzen Sie möglicherweise mehrere Abonnements in Azure.</span><span class="sxs-lookup"><span data-stu-id="244f6-105">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="244f6-106">Mit der CLI lassen sich mehrere Abonnements problemlos verwalten. Dazu wird entweder ein globales Abonnement für alle Befehle festgelegt oder ein Abonnement pro Befehl ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="244f6-106">Multiple subscriptions can be easily managed with the CLI either by setting a global subscription for all commands, or selecting a subscription on a per-command basis.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="244f6-107">Mandanten, Benutzer und Abonnements</span><span class="sxs-lookup"><span data-stu-id="244f6-107">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="244f6-108">Möglicherweise sind Sie sich nicht ganz über den Unterschied zwischen Mandanten, Benutzern und Abonnements in Azure im Klaren.</span><span class="sxs-lookup"><span data-stu-id="244f6-108">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="244f6-109">Ein _Mandant_ ist die Azure Active Directory-Entität, die eine gesamte Organisation umfasst.</span><span class="sxs-lookup"><span data-stu-id="244f6-109">A _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="244f6-110">Dieser Mandant hat mindestens ein _Abonnement_ und einen _Benutzer_.</span><span class="sxs-lookup"><span data-stu-id="244f6-110">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="244f6-111">Ein Benutzer ist eine Person und nur einem einzelnen Mandanten zugeordnet: der Organisation, der er angehört.</span><span class="sxs-lookup"><span data-stu-id="244f6-111">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="244f6-112">Benutzer sind Konten, die sich bei Azure anmelden, um Ressourcen bereitzustellen oder zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="244f6-112">Users are those accounts which sign in to Azure to provision and use resources.</span></span>
<span data-ttu-id="244f6-113">Ein Benutzer hat möglicherweise Zugriff auf mehrere _Abonnements_. Hierbei handelt es sich um die Vereinbarungen mit Microsoft, die die Verwendung von Clouddiensten wie Azure regeln.</span><span class="sxs-lookup"><span data-stu-id="244f6-113">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="244f6-114">Jede Ressource ist einem Abonnement zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="244f6-114">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="244f6-115">Weitere Informationen zu den Unterschieden zwischen Mandanten, Benutzern und Abonnements finden Sie im [Microsoft Azure-Glossar](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="244f6-115">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="244f6-116">Informationen zum Hinzufügen eines neuen Abonnements zu Ihrem Azure Active Directory-Mandanten finden Sie unter [Hinzufügen eines Azure-Abonnements zu Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="244f6-116">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="244f6-117">Bei der Verwendung mehrerer Mandanten müssen Sie sich unter Umständen bei einem bestimmten Mandanten anmelden.</span><span class="sxs-lookup"><span data-stu-id="244f6-117">When working with multiple tenants, you may need to sign in to a specific tenant.</span></span> <span data-ttu-id="244f6-118">Informationen dazu finden Sie unter [Anmelden mit Azure CLI](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="244f6-118">To do this, see [Sign in with Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="work-with-multiple-subscriptions"></a><span data-ttu-id="244f6-119">Verwenden mehrerer Abonnements</span><span class="sxs-lookup"><span data-stu-id="244f6-119">Work with multiple subscriptions</span></span>

<span data-ttu-id="244f6-120">Für den Zugriff auf die Ressourcen in einem Abonnement müssen Sie Ihr aktives Abonnement wechseln.</span><span class="sxs-lookup"><span data-stu-id="244f6-120">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="244f6-121">Der Wechsel Ihres Abonnements kann mit [az account set](/cli/azure/account#az-account-set) für alle Azure CLI-Befehle erfolgen oder mit dem `--subscription`-Argument für einzelne Befehle durchgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="244f6-121">Switching your subscription can be done for all Azure CLI commands with [az account set](/cli/azure/account#az-account-set), or done on a per-command basis by using the `--subscription` argument.</span></span>

<span data-ttu-id="244f6-122">Zunächst benötigen Sie eine Liste Ihrer verfügbaren Abonnements.</span><span class="sxs-lookup"><span data-stu-id="244f6-122">To start, you will need a list of your available subscriptions.</span></span> <span data-ttu-id="244f6-123">Rufen Sie diese mit dem Befehl [az account list](/cli/azure/account#az-account-list) ab:</span><span class="sxs-lookup"><span data-stu-id="244f6-123">To get it, use the [az account list](/cli/azure/account#az-account-list) command:</span></span>

```azurecli-interactive
az account list --output table
```

<span data-ttu-id="244f6-124">Für eine globale Änderung des aktiven Abonnements verwenden Sie `az account set` zusammen mit der Abonnement-ID oder dem Abonnementnamen:</span><span class="sxs-lookup"><span data-stu-id="244f6-124">To change the active subscription globally, use `az account set` along with either the subscription ID or subscription name:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="244f6-125">Zum Ausführen des Befehls für ein bestimmtes Abonnement verwenden Sie nur das Argument `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="244f6-125">To use a specific subscription for a command, just use the `--subscription` argument.</span></span> <span data-ttu-id="244f6-126">Mit diesem Argument kann entweder eine Abonnement-ID oder ein Abonnementname verwendet werden:</span><span class="sxs-lookup"><span data-stu-id="244f6-126">This argument takes either a subscription ID or subscription name:</span></span>

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```

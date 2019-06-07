---
title: Verwalten von Azure-Abonnements mit der Azure CLI
description: Verwalten Sie Azure-Abonnements mit der Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.product: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 37ef0c1d7cca90c99aa6f832c6dc6dc29a1806a3
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516205"
---
# <a name="use-multiple-azure-subscriptions"></a><span data-ttu-id="045e2-103">Verwenden mehrerer Azure-Abonnements</span><span class="sxs-lookup"><span data-stu-id="045e2-103">Use multiple Azure subscriptions</span></span>

<span data-ttu-id="045e2-104">Die meisten Azure-Benutzer verwenden nur ein einzelnes Abonnement.</span><span class="sxs-lookup"><span data-stu-id="045e2-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="045e2-105">Wenn Sie allerdings mehreren Organisationen angehören oder Ihre Organisation den Zugriff auf bestimmte Ressourcen über Gruppierungen aufgeteilt hat, besitzen Sie möglicherweise mehrere Abonnements in Azure.</span><span class="sxs-lookup"><span data-stu-id="045e2-105">However, if you are part of more than one organization or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="045e2-106">Die CLI unterstützt sowohl die globale Auswahl eines Abonnements als auch die Auswahl per Befehl.</span><span class="sxs-lookup"><span data-stu-id="045e2-106">The CLI supports selecting a subscription both globally and per command.</span></span>

<span data-ttu-id="045e2-107">Ausführliche Informationen zu Abonnements, der Abrechnung und der Kostenverwaltung finden Sie in der [Dokumentation zur Abrechnungs- und Kostenverwaltung in Azure](/azure/billing/).</span><span class="sxs-lookup"><span data-stu-id="045e2-107">For detailed information on subscriptions, billing, and cost management, see the [billing and cost management documentation](/azure/billing/).</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="045e2-108">Mandanten, Benutzer und Abonnements</span><span class="sxs-lookup"><span data-stu-id="045e2-108">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="045e2-109">Möglicherweise sind Sie sich nicht ganz über den Unterschied zwischen Mandanten, Benutzern und Abonnements in Azure im Klaren.</span><span class="sxs-lookup"><span data-stu-id="045e2-109">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="045e2-110">Ein _Mandant_ ist die Azure Active Directory-Entität, die eine gesamte Organisation umfasst.</span><span class="sxs-lookup"><span data-stu-id="045e2-110">A _tenant_ is the Azure Active Directory entity that encompasses a whole organization.</span></span> <span data-ttu-id="045e2-111">Dieser Mandant hat mindestens ein _Abonnement_ und einen _Benutzer_.</span><span class="sxs-lookup"><span data-stu-id="045e2-111">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="045e2-112">Ein Benutzer ist eine Person und nur einem einzelnen Mandanten zugeordnet: der Organisation, der er angehört.</span><span class="sxs-lookup"><span data-stu-id="045e2-112">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="045e2-113">Benutzer sind Konten, die sich bei Azure anmelden, um Ressourcen zu erstellen, zu verwalten und zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="045e2-113">Users are those accounts that sign in to Azure to create, manage, and use resources.</span></span>
<span data-ttu-id="045e2-114">Ein Benutzer hat möglicherweise Zugriff auf mehrere _Abonnements_. Hierbei handelt es sich um die Vereinbarungen mit Microsoft, die die Verwendung von Clouddiensten wie Azure regeln.</span><span class="sxs-lookup"><span data-stu-id="045e2-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="045e2-115">Jede Ressource ist einem Abonnement zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="045e2-115">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="045e2-116">Weitere Informationen zu den Unterschieden zwischen Mandanten, Benutzern und Abonnements finden Sie im [Microsoft Azure-Glossar](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="045e2-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="045e2-117">Informationen zum Hinzufügen eines neuen Abonnements zu Ihrem Azure Active Directory-Mandanten finden Sie unter [Hinzufügen eines Azure-Abonnements zu Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="045e2-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="045e2-118">Informationen zum Anmelden bei einem bestimmten Mandanten finden Sie unter [Anmelden mit Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="045e2-118">To learn how to sign in to a specific tenant, see [Sign in with Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="change-the-active-subscription"></a><span data-ttu-id="045e2-119">Ändern des aktiven Abonnements</span><span class="sxs-lookup"><span data-stu-id="045e2-119">Change the active subscription</span></span>

<span data-ttu-id="045e2-120">Wechseln Sie für den Zugriff auf die Ressourcen eines Abonnements Ihr aktives Abonnement, oder verwenden Sie das Argument `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="045e2-120">To access the resources for a subscription, switch your active subscription or use the `--subscription` argument.</span></span> <span data-ttu-id="045e2-121">Der Wechsel Ihres Abonnements für alle Befehle wird mit [az account set](/cli/azure/account#az-account-set) ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="045e2-121">Switching your subscription for all commands is done with [az account set](/cli/azure/account#az-account-set).</span></span>

<span data-ttu-id="045e2-122">So wechseln Sie Ihr aktives Abonnement:</span><span class="sxs-lookup"><span data-stu-id="045e2-122">To switch your active subscription:</span></span>

1. <span data-ttu-id="045e2-123">Rufen Sie eine Liste Ihrer Abonnements mithilfe des Befehls [az account list](/cli/azure/account#az-account-list) ab.</span><span class="sxs-lookup"><span data-stu-id="045e2-123">Get a list of your subscriptions with the [az account list](/cli/azure/account#az-account-list) command:</span></span>

    ```azurecli-interactive
    az account list --output table
    ```
2. <span data-ttu-id="045e2-124">Verwenden Sie `az account set` mit der ID oder dem Namen des Abonnements, zu dem Sie wechseln möchten.</span><span class="sxs-lookup"><span data-stu-id="045e2-124">Use `az account set` with the subscription ID or name you want to switch to.</span></span>

    ```azurecli-interactive
    az account set --subscription "My Demos"
    ```

<span data-ttu-id="045e2-125">Wenn Sie nur einen Befehl mit einem anderen Abonnement ausführen möchten, verwenden Sie das Argument `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="045e2-125">To run only a single command with a different subscription, use the `--subscription` argument.</span></span> <span data-ttu-id="045e2-126">Mit diesem Argument kann entweder eine Abonnement-ID oder ein Abonnementname verwendet werden:</span><span class="sxs-lookup"><span data-stu-id="045e2-126">This argument takes either a subscription ID or subscription name:</span></span>

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```

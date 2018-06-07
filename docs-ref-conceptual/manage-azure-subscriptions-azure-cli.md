---
title: Verwalten von Azure-Abonnements mit Azure CLI 2.0
description: Es wird beschrieben, wie Sie Azure-Abonnements mit Azure CLI 2.0 unter Linux, MacOS oder Windows verwalten.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/30/2017
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: active-directory
ms.openlocfilehash: 5a27eed40e0666f6a5e57a23ac369d92c3b01dab
ms.sourcegitcommit: 38549f60d76d4b6b65d180367e83749769fe6e43
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/04/2018
ms.locfileid: "34703025"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="bd0d0-103">Verwalten mehrerer Azure-Abonnements</span><span class="sxs-lookup"><span data-stu-id="bd0d0-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="bd0d0-104">Die meisten Azure-Benutzer verwenden nur ein einzelnes Abonnement.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="bd0d0-105">Wenn Sie allerdings mehreren Organisationen angehören oder Ihre Organisation den Zugriff auf bestimmte Ressourcen über Gruppierungen aufgeteilt hat, besitzen Sie möglicherweise mehrere Abonnements in Azure.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-105">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="bd0d0-106">Mehrere Abonnements lassen sich problemlos über die Befehlszeilenschnittstelle verwalten, und Vorgänge können durch Auswählen eines Abonnements ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-106">Multiple subscriptions can be easily managed with the CLI, and operations can be performed by selecting a subscription.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="bd0d0-107">Mandanten, Benutzer und Abonnements</span><span class="sxs-lookup"><span data-stu-id="bd0d0-107">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="bd0d0-108">Möglicherweise sind Sie sich nicht ganz über den Unterschied zwischen Mandanten, Benutzern und Abonnements in Azure im Klaren.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-108">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="bd0d0-109">Ein _Mandant_ ist ganz allgemein die Azure Active Directory-Entität, die eine gesamte Organisation umfasst.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-109">In general, a _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="bd0d0-110">Dieser Mandant hat mindestens ein _Abonnement_ und einen _Benutzer_.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-110">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="bd0d0-111">Ein Benutzer ist eine Person und nur einem einzelnen Mandanten zugeordnet: der Organisation, der er angehört.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-111">A user is an individual, and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="bd0d0-112">Benutzer sind Konten, die sich bei Azure anmelden, um Ressourcen bereitzustellen oder zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-112">Users are those accounts which log in to Azure to provision and use resources.</span></span> <span data-ttu-id="bd0d0-113">Ein Benutzer hat möglicherweise Zugriff auf mehrere _Abonnements_. Hierbei handelt es sich um die Vereinbarungen mit Microsoft, die die Verwendung von Clouddiensten wie Azure regeln.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-113">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="bd0d0-114">Jede Ressource ist einem Abonnement zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-114">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="bd0d0-115">Weitere Informationen zu den Unterschieden zwischen Mandanten, Benutzern und Abonnements finden Sie im [Microsoft Azure-Glossar](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="bd0d0-115">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>
<span data-ttu-id="bd0d0-116">Informationen zum Hinzufügen eines neuen Abonnements zu Ihrem Azure Active Directory-Mandanten finden Sie unter [Hinzufügen eines Azure-Abonnements zu Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="bd0d0-116">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="bd0d0-117">Bei der Verwendung mehrerer Mandanten müssen Sie sich unter Umständen bei einem bestimmten Mandanten anmelden.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-117">When working with multiple tenants, you may need to log into a specific tenant.</span></span> <span data-ttu-id="bd0d0-118">Informationen dazu finden Sie unter [Anmelden mit Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="bd0d0-118">To do this, see [Log in with Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="working-with-multiple-subscriptions"></a><span data-ttu-id="bd0d0-119">Verwenden mehrerer Abonnements</span><span class="sxs-lookup"><span data-stu-id="bd0d0-119">Working with multiple subscriptions</span></span>

<span data-ttu-id="bd0d0-120">Für den Zugriff auf die Ressourcen in einem Abonnement müssen Sie Ihr aktives Abonnement wechseln.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-120">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="bd0d0-121">Alle Aufgaben im Zusammenhang mit Abonnements werden über den Befehl `az account` ausgeführt. Dieser verweist nicht auf Ihr individuelles Konto, sondern auf den Servicevertrag, den ein Abonnement darstellt.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-121">All work with subscriptions is done through the `az account` command, which refers to the service agreement that a subscription represents and not your individual account.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

<span data-ttu-id="bd0d0-122">Wenn Sie mit Ihren verfügbaren Abonnements arbeiten möchten, rufen Sie zunächst eine Liste mit den verfügbaren Abonnements in Ihrem Konto ab:</span><span class="sxs-lookup"><span data-stu-id="bd0d0-122">To start working with your available subscriptions, get a list of those available in your account:</span></span>

```azurecli-interactive
az account list --output table
```

```Output
Name                                         CloudName    SubscriptionId                        State     IsDefault
-------------------------------------------  -----------  ------------------------------------  --------  -----------
My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
```

<span data-ttu-id="bd0d0-123">Das aktive Abonnement können Sie mit `az account set` wechseln:</span><span class="sxs-lookup"><span data-stu-id="bd0d0-123">In order to change the active subscription, you can use `az account set`:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="bd0d0-124">Verwenden Sie zum Auswählen des Abonnements entweder die Abonnement-ID oder den Namen des Abonnements.</span><span class="sxs-lookup"><span data-stu-id="bd0d0-124">You can use either the subscription ID or the subscription name to select the subscription.</span></span>

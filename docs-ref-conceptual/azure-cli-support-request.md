---
title: Erstellen einer Azure-Supportanfrage über die Azure CLI
description: Hier erfahren Sie, wie Sie die Azure CLI-Befehle vom Typ „az support“ verwenden, um Azure-Supportanfragen zu erstellen, zu aktualisieren und zu verwalten.
author: dbradish-microsoft
ms.author: dbradish
ms.service: azure-supportability
ms.topic: how-to
ms.date: 02/12/2021
ms.custom: template-how-to
ms.openlocfilehash: 446fe0d3a6d7c726167d07e8eb5f4cfa2321d9b7
ms.sourcegitcommit: 594e9c620a6f74f5eaedf91a7f6a791e03a64c74
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/17/2021
ms.locfileid: "100631165"
---
# <a name="create-an-azure-support-request-in-azure-cli"></a><span data-ttu-id="a79b5-103">Erstellen einer Azure-Supportanfrage über die Azure CLI</span><span class="sxs-lookup"><span data-stu-id="a79b5-103">Create an Azure support request in Azure CLI</span></span>

<span data-ttu-id="a79b5-104">Mit der Azure CLI können Sie Azure-Supporttickets erstellen und verwalten.</span><span class="sxs-lookup"><span data-stu-id="a79b5-104">The Azure CLI enables you to create and manage Azure support tickets.</span></span>

- <span data-ttu-id="a79b5-105">Öffnen Sie ein Supportticket zum Thema Technik, Abrechnung, Abonnementverwaltung oder Abonnement- und Dienstgrenzwerte (Kontingent).</span><span class="sxs-lookup"><span data-stu-id="a79b5-105">Open a technical, billing, subscription management, or subscription and service limits (quota) support ticket.</span></span>
- <span data-ttu-id="a79b5-106">Rufen Sie eine Liste mit Supporttickets und ausführlichen Informationen zu den einzelnen Tickets ab.</span><span class="sxs-lookup"><span data-stu-id="a79b5-106">Get a list of support tickets and detailed information about each ticket.</span></span> <span data-ttu-id="a79b5-107">Grenzen Sie Ihre Suche nach Supporttickets anhand des Status oder Erstellungsdatums ein.</span><span class="sxs-lookup"><span data-stu-id="a79b5-107">Narrow your search for support tickets by status or created date.</span></span>
- <span data-ttu-id="a79b5-108">Aktualisieren Sie den Schweregrad, den Ticketstatus und die Kontaktinformationen für ein Supportticket.</span><span class="sxs-lookup"><span data-stu-id="a79b5-108">Update severity, ticket status, and contact information for a support ticket.</span></span>
- <span data-ttu-id="a79b5-109">Fügen Sie einem Supportticket ein neues Kommunikationselement hinzu, oder rufen Sie alle Kommunikationselemente für ein Supportticket ab.</span><span class="sxs-lookup"><span data-stu-id="a79b5-109">Add a new communication to a support ticket or get a list of all communications for a support ticket.</span></span> <span data-ttu-id="a79b5-110">Grenzen Sie die Suche nach Kommunikationslisten anhand des Erstellungsdatums oder Kommunikationstyps ein.</span><span class="sxs-lookup"><span data-stu-id="a79b5-110">Narrow your search of communication lists by created date or communication type.</span></span>

<span data-ttu-id="a79b5-111">Um eine Supportanfrage erstellen zu können, müssen Sie ein [Besitzer](/azure/role-based-access-control/built-in-roles#owner) oder [Mitwirkender](/azure/role-based-access-control/built-in-roles#contributor) sein, oder Ihnen muss die Rolle [Mitwirkender für Supportanfragen](/azure/role-based-access-control/built-in-roles#support-request-contributor) auf Abonnementebene zugewiesen sein.</span><span class="sxs-lookup"><span data-stu-id="a79b5-111">To create a support request, you must be an [Owner](/azure/role-based-access-control/built-in-roles#owner) or [Contributor](/azure/role-based-access-control/built-in-roles#contributor), or be assigned to the [Support Request Contributor](/azure/role-based-access-control/built-in-roles#support-request-contributor) role at the subscription level.</span></span> <span data-ttu-id="a79b5-112">Zum Erstellen einer Supportanfrage ohne Abonnement, z. B. in einem Azure Active Directory-Szenario, müssen Sie ein [Administrator](/azure/active-directory/roles/permissions-reference) sein.</span><span class="sxs-lookup"><span data-stu-id="a79b5-112">To create a support request without a subscription, such as an Azure Active Directory scenario, you must be an [Admin](/azure/active-directory/roles/permissions-reference).</span></span>

[!INCLUDE [azure-cli-prepare-your-environment.md](includes/azure-cli-prepare-your-environment.md)]

## <a name="create-a-support-ticket"></a><span data-ttu-id="a79b5-113">Erstellen ein Supporttickets</span><span class="sxs-lookup"><span data-stu-id="a79b5-113">Create a support ticket</span></span>

1. <span data-ttu-id="a79b5-114">Zum Abrufen einer Liste von Diensten verwenden Sie den Befehl [az support services list](/cli/azure/ext/support/support/services#ext_support_az_support_services_list):</span><span class="sxs-lookup"><span data-stu-id="a79b5-114">To obtain a list of services, use the [az support services list](/cli/azure/ext/support/support/services#ext_support_az_support_services_list) command:</span></span>

   ```azurecli
   az support services list --output table
   ```

   <span data-ttu-id="a79b5-115">Suchen Sie in diesem Beispiel den Wert für **Virtueller Computer mit Windows**. Er lautet **6f16735c-b0ae-b275-ad3a-03479cfa1396**.</span><span class="sxs-lookup"><span data-stu-id="a79b5-115">For this example, find the value for **Virtual Machine running Windows**, which is **6f16735c-b0ae-b275-ad3a-03479cfa1396**.</span></span>

1. <span data-ttu-id="a79b5-116">Führen Sie den Befehl [az support services problem-classifications list](/cli/azure/ext/support/support/services/problem-classifications#ext_support_az_support_services_problem_classifications_list) aus, um den Problemtyp und den Problemuntertyp abzurufen, der Ihr Problem beschreibt:</span><span class="sxs-lookup"><span data-stu-id="a79b5-116">To get the problem type and problem subtype that describes your problem, run the [az support services problem-classifications list](/cli/azure/ext/support/support/services/problem-classifications#ext_support_az_support_services_problem_classifications_list) command:</span></span>

   ```azurecli
   az support services problem-classifications list --service-name 6f16735c-b0ae-b275-ad3a-03479cfa1396 --output table
   ```

   <span data-ttu-id="a79b5-117">Suchen Sie in diesem Beispiel nach **Es kann keine Verbindung mit meinem virtuellen Computer hergestellt werden/Ich habe ein Problem mit meiner öffentlichen IP-Adresse**.</span><span class="sxs-lookup"><span data-stu-id="a79b5-117">For this example, find **Cannot connect to my VM / I have an issue with my public IP**.</span></span> <span data-ttu-id="a79b5-118">Dieser Typ hat den Wert **e5c307e3-50ff-5dc9-c8ae-7d35051f88c9**.</span><span class="sxs-lookup"><span data-stu-id="a79b5-118">That type has a value of **e5c307e3-50ff-5dc9-c8ae-7d35051f88c9**.</span></span>

1. <span data-ttu-id="a79b5-119">Erstellen Sie mit dem Befehl [az support tickets create](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_create) ein Ticket:</span><span class="sxs-lookup"><span data-stu-id="a79b5-119">Create a ticket by using the [az support tickets create](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_create) command:</span></span>

   ```azurecli
   az support tickets create --ticket-name "VM012" --title "Issue with public IP" \
      --description "This ticket involves a public IP address of a VM." \
      --problem-classification e5c307e3-50ff-5dc9-c8ae-7d35051f88c9 \
      --severity minimal --contact-first-name Kenneth --contact-last-name Liew \
      --contact-method email --contact-email Kenneth.Liew@Contoso.com \
      --contact-country US --contact-language English --contact-timezone "Pacific Standard Time"
   ```

<span data-ttu-id="a79b5-120">Ein Supporttechniker setzt sich mit Ihnen mithilfe der von Ihnen angeführten Methode in Verbindung.</span><span class="sxs-lookup"><span data-stu-id="a79b5-120">A support engineer will contact you using the method you indicated.</span></span> <span data-ttu-id="a79b5-121">Informationen zur anfänglichen Reaktionszeit finden Sie unter [Supportumfang und Reaktionszeiten](/support/plans/response/).</span><span class="sxs-lookup"><span data-stu-id="a79b5-121">For information about initial response times, see [Support scope and responsiveness](/support/plans/response/).</span></span>

## <a name="manage-support-tickets"></a><span data-ttu-id="a79b5-122">Verwalten von Supporttickets</span><span class="sxs-lookup"><span data-stu-id="a79b5-122">Manage support tickets</span></span>

<span data-ttu-id="a79b5-123">Führen Sie zum Anzeigen der Supporttickets für Ihr aktuelles Abonnement den Befehl [az support tickets list](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_list) aus:</span><span class="sxs-lookup"><span data-stu-id="a79b5-123">To see your support tickets for your current subscription, run the [az support tickets list](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_list) command:</span></span>

```azurecli
az support tickets list
```

<span data-ttu-id="a79b5-124">Wenn Sie Supporttickets in einem anderen Abonnement anzeigen möchten, führen Sie den Befehl [az account set](/cli/azure/account#az_account_set) zum Ändern des aktuellen Abonnements und anschließend den entsprechenden Befehl aus.</span><span class="sxs-lookup"><span data-stu-id="a79b5-124">To see support tickets in another subscription, run the [az account set](/cli/azure/account#az_account_set) command to change your current subscription, and then run the command.</span></span>

<span data-ttu-id="a79b5-125">Sie können ein Ticket auch mithilfe des Befehls [az support tickets update](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_update) aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="a79b5-125">You can also update a ticket by using the [az support tickets update](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_update) command:</span></span>

```azurecli
az support tickets update --ticket-name VM012 --severity moderate
```

## <a name="communicate-about-your-ticket"></a><span data-ttu-id="a79b5-126">Ticketbezogene Kommunikation</span><span class="sxs-lookup"><span data-stu-id="a79b5-126">Communicate about your ticket</span></span>

<span data-ttu-id="a79b5-127">Sie können ein mit der Azure CLI erstelltes Supportticket nicht löschen.</span><span class="sxs-lookup"><span data-stu-id="a79b5-127">You can't delete a support ticket created by using Azure CLI.</span></span> <span data-ttu-id="a79b5-128">Senden Sie stattdessen eine Nachricht, um ein Ticket zu schließen.</span><span class="sxs-lookup"><span data-stu-id="a79b5-128">Instead, send a message to close a ticket.</span></span> <span data-ttu-id="a79b5-129">Wenn Sie eine geschlossene Supportanfrage erneut öffnen müssen, erstellen Sie eine neue Nachricht. Dadurch wird die Anfrage automatisch erneut geöffnet.</span><span class="sxs-lookup"><span data-stu-id="a79b5-129">If you need to reopen a closed support request, create a new message, which automatically reopens the request.</span></span>

<span data-ttu-id="a79b5-130">Führen Sie für ticketbezogene Kommunikation den Befehl [az support tickets communications create](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_create) aus:</span><span class="sxs-lookup"><span data-stu-id="a79b5-130">To communicate about your ticket, run the [az support tickets communications create](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_create) command:</span></span>

```azurecli
az support tickets communications create --ticket-name VM012 \
    --communication-name "VM Delay" \
    --communication-body "Delaying VM fixes due to scheduling on our end." \
    --communication-subject "Delaying VM fixes due to scheduling on our end."
```

<span data-ttu-id="a79b5-131">Verwenden Sie zum Anzeigen der gesamten Ticketkommunikation den Befehl [az support tickets communications list](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_list):</span><span class="sxs-lookup"><span data-stu-id="a79b5-131">To see all the communications for a ticket, use the [az support tickets communications list](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_list) command:</span></span>

```azurecli
az support tickets communications list --ticket-name VM012
```

<span data-ttu-id="a79b5-132">Dieser Befehl enthält den Parameter `--filters` zum Einschränken der Antworten.</span><span class="sxs-lookup"><span data-stu-id="a79b5-132">This command offers a `--filters` parameter to narrow your responses.</span></span>

```azurecli
az support tickets communications list --ticket-name VM012 \
    --filters "communicationType eq 'Web'"
```

## <a name="next-steps"></a><span data-ttu-id="a79b5-133">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="a79b5-133">Next steps</span></span>

- [<span data-ttu-id="a79b5-134">Häufig gestellte Fragen zum Azure-Support</span><span class="sxs-lookup"><span data-stu-id="a79b5-134">Azure Support FAQs</span></span>](/support/faq/)
- [<span data-ttu-id="a79b5-135">Supportumfang und Reaktionszeiten</span><span class="sxs-lookup"><span data-stu-id="a79b5-135">Azure severity and levels</span></span>](/support/plans/response/)
- [<span data-ttu-id="a79b5-136">Gewusst wie: Erstellen einer Azure-Supportanfrage</span><span class="sxs-lookup"><span data-stu-id="a79b5-136">How to create a support ticket via Azure portal</span></span>](/azure/azure-portal/supportability/how-to-create-azure-support-request)

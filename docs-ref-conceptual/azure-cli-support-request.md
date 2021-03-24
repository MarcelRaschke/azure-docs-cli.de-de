---
title: Erstellen einer Azure-Supportanfrage über die Azure CLI
description: Hier erfahren Sie, wie Sie die Azure CLI-Befehle vom Typ „az support“ verwenden, um Azure-Supportanfragen zu erstellen, zu aktualisieren und zu verwalten.
author: dbradish-microsoft
ms.author: dbradish
ms.service: azure-supportability
ms.topic: how-to
ms.date: 02/12/2021
ms.custom: template-how-to
ms.openlocfilehash: 297b8b65973a7d2b3d377a56865f1cbdd42e08f2
ms.sourcegitcommit: 936ec07eb1c56e24d8000cc24a2a0e05102e0cf4
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2021
ms.locfileid: "104911123"
---
# <a name="create-an-azure-support-request-in-azure-cli"></a>Erstellen einer Azure-Supportanfrage über die Azure CLI

Mit der Azure CLI können Sie Azure-Supporttickets erstellen und verwalten.

- Öffnen Sie ein Supportticket zum Thema Technik, Abrechnung, Abonnementverwaltung oder Abonnement- und Dienstgrenzwerte (Kontingent).
- Rufen Sie eine Liste mit Supporttickets und ausführlichen Informationen zu den einzelnen Tickets ab. Grenzen Sie Ihre Suche nach Supporttickets anhand des Status oder Erstellungsdatums ein.
- Aktualisieren Sie den Schweregrad, den Ticketstatus und die Kontaktinformationen für ein Supportticket.
- Fügen Sie einem Supportticket ein neues Kommunikationselement hinzu, oder rufen Sie alle Kommunikationselemente für ein Supportticket ab. Grenzen Sie die Suche nach Kommunikationslisten anhand des Erstellungsdatums oder Kommunikationstyps ein.

Um eine Supportanfrage erstellen zu können, müssen Sie ein [Besitzer](/azure/role-based-access-control/built-in-roles#owner) oder [Mitwirkender](/azure/role-based-access-control/built-in-roles#contributor) sein, oder Ihnen muss die Rolle [Mitwirkender für Supportanfragen](/azure/role-based-access-control/built-in-roles#support-request-contributor) auf Abonnementebene zugewiesen sein. Zum Erstellen einer Supportanfrage ohne Abonnement, z. B. in einem Azure Active Directory-Szenario, müssen Sie ein [Administrator](/azure/active-directory/roles/permissions-reference) sein.

[!INCLUDE [azure-cli-prepare-your-environment.md](includes/azure-cli-prepare-your-environment.md)]

## <a name="create-a-support-ticket"></a>Erstellen ein Supporttickets

1. Zum Abrufen einer Liste von Diensten verwenden Sie den Befehl [az support services list](/cli/azure/ext/support/support/services#ext_support_az_support_services_list):

   ```azurecli
   az support services list --output table
   ```

   Suchen Sie in diesem Beispiel den Wert für **Virtueller Computer mit Windows**. Er lautet **6f16735c-b0ae-b275-ad3a-03479cfa1396**.

1. Führen Sie den Befehl [az support services problem-classifications list](/cli/azure/ext/support/support/services/problem-classifications#ext_support_az_support_services_problem_classifications_list) aus, um den Problemtyp und den Problemuntertyp abzurufen, der Ihr Problem beschreibt:

   ```azurecli
   az support services problem-classifications list --service-name 6f16735c-b0ae-b275-ad3a-03479cfa1396 --output table
   ```

   Suchen Sie in diesem Beispiel nach **Es kann keine Verbindung mit meinem virtuellen Computer hergestellt werden/Ich habe ein Problem mit meiner öffentlichen IP-Adresse**. Dieser Typ hat den Wert **e5c307e3-50ff-5dc9-c8ae-7d35051f88c9**.

1. Erstellen Sie mit dem Befehl [az support tickets create](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_create) ein Ticket:

   ```azurecli
   az support tickets create --ticket-name "VM012" --title "Issue with public IP" \
      --description "This ticket involves a public IP address of a VM." \
      --problem-classification e5c307e3-50ff-5dc9-c8ae-7d35051f88c9 \
      --severity minimal --contact-first-name Kenneth --contact-last-name Liew \
      --contact-method email --contact-email Kenneth.Liew@Contoso.com \
      --contact-country US --contact-language English --contact-timezone "Pacific Standard Time"
   ```

Ein Supporttechniker setzt sich mit Ihnen mithilfe der von Ihnen angeführten Methode in Verbindung. Informationen zur anfänglichen Reaktionszeit finden Sie unter [Supportumfang und Reaktionszeiten](/support/plans/response/).

## <a name="manage-support-tickets"></a>Verwalten von Supporttickets

Führen Sie zum Anzeigen der Supporttickets für Ihr aktuelles Abonnement den Befehl [az support tickets list](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_list) aus:

```azurecli
az support tickets list
```

Wenn Sie Supporttickets in einem anderen Abonnement anzeigen möchten, führen Sie den Befehl [az account set](/cli/azure/account#az_account_set) zum Ändern des aktuellen Abonnements und anschließend den entsprechenden Befehl aus.

Sie können ein Ticket auch mithilfe des Befehls [az support tickets update](/cli/azure/ext/support/support/tickets#ext_support_az_support_tickets_update) aktualisieren:

```azurecli
az support tickets update --ticket-name VM012 --severity moderate
```

## <a name="communicate-about-your-ticket"></a>Ticketbezogene Kommunikation

Sie können ein mit der Azure CLI erstelltes Supportticket nicht löschen. Senden Sie stattdessen eine Nachricht, um ein Ticket zu schließen. Wenn Sie eine geschlossene Supportanfrage erneut öffnen müssen, erstellen Sie eine neue Nachricht. Dadurch wird die Anfrage automatisch erneut geöffnet.

Führen Sie für ticketbezogene Kommunikation den Befehl [az support tickets communications create](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_create) aus:

```azurecli
az support tickets communications create --ticket-name VM012 \
    --communication-name "VM Delay" \
    --communication-body "Delaying VM fixes due to scheduling on our end." \
    --communication-subject "Delaying VM fixes due to scheduling on our end."
```

Verwenden Sie zum Anzeigen der gesamten Ticketkommunikation den Befehl [az support tickets communications list](/cli/azure/ext/support/support/tickets/communications#ext_support_az_support_tickets_communications_list):

```azurecli
az support tickets communications list --ticket-name VM012
```

Dieser Befehl enthält den Parameter `--filters` zum Einschränken der Antworten.

```azurecli
az support tickets communications list --ticket-name VM012 \
    --filters "communicationType eq 'Web'"
```

## <a name="next-steps"></a>Nächste Schritte

- [Häufig gestellte Fragen zum Azure-Support](https://azure.microsoft.com/support/faq/)
- [Supportumfang und Reaktionszeiten](https://azure.microsoft.com/support/plans/response/)
- [Gewusst wie: Erstellen einer Azure-Supportanfrage](/azure/azure-portal/supportability/how-to-create-azure-support-request)

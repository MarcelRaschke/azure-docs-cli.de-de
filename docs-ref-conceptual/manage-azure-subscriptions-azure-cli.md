---
title: Verwalten von Azure-Abonnements mit der Azure CLI
description: Verwalten Sie Azure-Abonnements mit der Azure CLI.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: dad217dff159baa39bd1361258fb308eea872564
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2020
ms.locfileid: "77780059"
---
# <a name="use-multiple-azure-subscriptions"></a>Verwenden mehrerer Azure-Abonnements

Die meisten Azure-Benutzer verwenden nur ein einzelnes Abonnement. Wenn Sie allerdings mehreren Organisationen angehören oder Ihre Organisation den Zugriff auf bestimmte Ressourcen über Gruppierungen aufgeteilt hat, besitzen Sie möglicherweise mehrere Abonnements in Azure. Die CLI unterstützt sowohl die globale Auswahl eines Abonnements als auch die Auswahl per Befehl.

Ausführliche Informationen zu Abonnements, der Abrechnung und der Kostenverwaltung finden Sie in der [Dokumentation zur Abrechnungs- und Kostenverwaltung in Azure](/azure/billing/).

## <a name="tenants-users-and-subscriptions"></a>Mandanten, Benutzer und Abonnements

Möglicherweise sind Sie sich nicht ganz über den Unterschied zwischen Mandanten, Benutzern und Abonnements in Azure im Klaren. Ein _Mandant_ ist die Azure Active Directory-Entität, die eine gesamte Organisation umfasst. Dieser Mandant hat mindestens ein _Abonnement_ und einen _Benutzer_. Ein Benutzer ist eine Person und nur einem einzelnen Mandanten zugeordnet: der Organisation, der er angehört. Benutzer sind Konten, die sich bei Azure anmelden, um Ressourcen zu erstellen, zu verwalten und zu verwenden.
Ein Benutzer hat möglicherweise Zugriff auf mehrere _Abonnements_. Hierbei handelt es sich um die Vereinbarungen mit Microsoft, die die Verwendung von Clouddiensten wie Azure regeln. Jede Ressource ist einem Abonnement zugeordnet.

Weitere Informationen zu den Unterschieden zwischen Mandanten, Benutzern und Abonnements finden Sie im [Microsoft Azure-Glossar](/azure/azure-glossary-cloud-terminology).  Informationen zum Hinzufügen eines neuen Abonnements zu Ihrem Azure Active Directory-Mandanten finden Sie unter [Hinzufügen eines Azure-Abonnements zu Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
Informationen zum Anmelden bei einem bestimmten Mandanten finden Sie unter [Anmelden mit Azure CLI 2.0](/cli/azure/authenticate-azure-cli).

## <a name="change-the-active-subscription"></a>Ändern des aktiven Abonnements

Wechseln Sie für den Zugriff auf die Ressourcen eines Abonnements Ihr aktives Abonnement, oder verwenden Sie das Argument `--subscription`. Der Wechsel Ihres Abonnements für alle Befehle wird mit [az account set](/cli/azure/account#az-account-set) ausgeführt.

So wechseln Sie Ihr aktives Abonnement:

1. Rufen Sie eine Liste Ihrer Abonnements mithilfe des Befehls [az account list](/cli/azure/account#az-account-list) ab.

    ```azurecli-interactive
    az account list --output table
    ```
2. Verwenden Sie `az account set` mit der ID oder dem Namen des Abonnements, zu dem Sie wechseln möchten.

    ```azurecli-interactive
    az account set --subscription "My Demos"
    ```

Wenn Sie nur einen Befehl mit einem anderen Abonnement ausführen möchten, verwenden Sie das Argument `--subscription`. Mit diesem Argument kann entweder eine Abonnement-ID oder ein Abonnementname verwendet werden:

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```

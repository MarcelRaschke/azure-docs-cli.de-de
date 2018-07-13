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
# <a name="manage-multiple-azure-subscriptions"></a>Verwalten mehrerer Azure-Abonnements

Die meisten Azure-Benutzer verwenden nur ein einzelnes Abonnement. Wenn Sie allerdings mehreren Organisationen angehören oder Ihre Organisation den Zugriff auf bestimmte Ressourcen über Gruppierungen aufgeteilt hat, besitzen Sie möglicherweise mehrere Abonnements in Azure. Mit der CLI lassen sich mehrere Abonnements problemlos verwalten. Dazu wird entweder ein globales Abonnement für alle Befehle festgelegt oder ein Abonnement pro Befehl ausgewählt.

## <a name="tenants-users-and-subscriptions"></a>Mandanten, Benutzer und Abonnements

Möglicherweise sind Sie sich nicht ganz über den Unterschied zwischen Mandanten, Benutzern und Abonnements in Azure im Klaren. Ein _Mandant_ ist die Azure Active Directory-Entität, die eine gesamte Organisation umfasst. Dieser Mandant hat mindestens ein _Abonnement_ und einen _Benutzer_. Ein Benutzer ist eine Person und nur einem einzelnen Mandanten zugeordnet: der Organisation, der er angehört. Benutzer sind Konten, die sich bei Azure anmelden, um Ressourcen bereitzustellen oder zu verwenden.
Ein Benutzer hat möglicherweise Zugriff auf mehrere _Abonnements_. Hierbei handelt es sich um die Vereinbarungen mit Microsoft, die die Verwendung von Clouddiensten wie Azure regeln. Jede Ressource ist einem Abonnement zugeordnet.

Weitere Informationen zu den Unterschieden zwischen Mandanten, Benutzern und Abonnements finden Sie im [Microsoft Azure-Glossar](/azure/azure-glossary-cloud-terminology).  Informationen zum Hinzufügen eines neuen Abonnements zu Ihrem Azure Active Directory-Mandanten finden Sie unter [Hinzufügen eines Azure-Abonnements zu Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
Bei der Verwendung mehrerer Mandanten müssen Sie sich unter Umständen bei einem bestimmten Mandanten anmelden. Informationen dazu finden Sie unter [Anmelden mit Azure CLI](/cli/azure/authenticate-azure-cli).

## <a name="work-with-multiple-subscriptions"></a>Verwenden mehrerer Abonnements

Für den Zugriff auf die Ressourcen in einem Abonnement müssen Sie Ihr aktives Abonnement wechseln. Der Wechsel Ihres Abonnements kann mit [az account set](/cli/azure/account#az-account-set) für alle Azure CLI-Befehle erfolgen oder mit dem `--subscription`-Argument für einzelne Befehle durchgeführt werden.

Zunächst benötigen Sie eine Liste Ihrer verfügbaren Abonnements. Rufen Sie diese mit dem Befehl [az account list](/cli/azure/account#az-account-list) ab:

```azurecli-interactive
az account list --output table
```

Für eine globale Änderung des aktiven Abonnements verwenden Sie `az account set` zusammen mit der Abonnement-ID oder dem Abonnementnamen:

```azurecli-interactive
az account set --subscription "My Demos"
```

Zum Ausführen des Befehls für ein bestimmtes Abonnement verwenden Sie nur das Argument `--subscription`. Mit diesem Argument kann entweder eine Abonnement-ID oder ein Abonnementname verwendet werden:

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```

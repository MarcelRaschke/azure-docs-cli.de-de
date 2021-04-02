---
title: Verwalten von Azure-Abonnements mit der Azure CLI
description: Hier erfahren Sie mehr über Azure-Mandanten, -Benutzer und -Abonnements. Verwenden Sie die Azure CLI, um Ihre Abonnements zu verwalten, Verwaltungsgruppen zu erstellen und Abonnements zu sperren.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/29/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: a2a4467bc25fb8da8ced0c7b8cb6c4db9eb35e64
ms.sourcegitcommit: 8bff8b2ce4492ab99ad39390e4c802fb4f4425c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2021
ms.locfileid: "105581834"
---
# <a name="use-azure-subscriptions-with-azure-cli"></a>Verwenden von Azure-Abonnements mit der Azure CLI

Sie verfügen möglicherweise über mehrere Abonnements in Azure. Sie können mehreren Organisationen angehören, oder Ihre Organisation teilt unter Umständen den Zugriff auf bestimmte Ressourcen gruppierungsübergreifend auf. Die Azure CLI unterstützt sowohl die globale Auswahl eines Abonnements als auch die Auswahl per Befehl.

Ausführliche Informationen zu Abonnements, der Abrechnung und der Kostenverwaltung finden Sie in der [Dokumentation zur Abrechnungs- und Kostenverwaltung in Azure](/azure/billing/).

## <a name="tenants-users-and-subscriptions"></a>Mandanten, Benutzer und Abonnements

Ein _Mandant_ ist die Azure Active Directory-Entität, die eine gesamte Organisation umfasst. Ein Mandant verfügt über mindestens ein _Abonnement_ und mindestens einen _Benutzer_. Ein Benutzer ist eine Person und nur einem einzelnen Mandanten zugeordnet: der Organisation, der er angehört. Benutzer sind Konten, die sich bei Azure anmelden, um Ressourcen zu erstellen, zu verwalten und zu verwenden. Ein Benutzer hat möglicherweise Zugriff auf mehrere _Abonnements_. Hierbei handelt es sich um die Vereinbarungen mit Microsoft, die die Verwendung von Clouddiensten wie Azure regeln. Jede Ressource ist einem Abonnement zugeordnet.

* Weitere Informationen zu den Unterschieden zwischen Mandanten, Benutzern und Abonnements finden Sie im [Microsoft Azure-Glossar](/azure/azure-glossary-cloud-terminology).
* Informationen zum Hinzufügen eines neuen Abonnements zu Ihrem Azure Active Directory-Mandanten finden Sie unter [Zuordnen oder Hinzufügen eines Azure-Abonnements zu Ihrem Azure Active Directory-Mandanten](/azure/active-directory/active-directory-how-subscriptions-associated-directory).
* Informationen zum Anmelden bei einem bestimmten Mandanten finden Sie unter [Anmelden mit der Azure CLI](./authenticate-azure-cli.md).

## <a name="commands-in-a-subscription"></a>Befehle in einem Abonnement

Viele Azure CLI Befehle werden im Kontext eines Abonnements ausgeführt. Sie können jederzeit angeben, in welchem Abonnement Sie arbeiten möchten. Verwenden Sie dazu den Parameter **subscription** in Ihrem Befehl. Dieser Parameter ist optional. Wenn Sie kein Abonnement angeben, verwendet der Befehl das aktuelle, aktive Abonnement.

Führen Sie zum Anzeigen des derzeit verwendeten Abonnements den Befehl [az account show](/cli/azure/account#az_account_show) aus:

```azurecli
az account show --output table
```

> [!TIP]
> Der Parameter `--output` ist ein globaler Parameter und für alle Befehle verfügbar. Mit dem Wert **table** wird die Ausgabe in einem benutzerfreundlichen Format angezeigt. Weitere Informationen finden Sie unter [Ausgabeformate für Azure CLI-Befehle](/cli/azure/format-output-azure-cli).

Abonnements enthalten Ressourcengruppen. Eine Azure-Ressourcengruppe ist ein Container, der verwandte Ressourcen für eine Azure-Lösung enthält. Wenn Ihr Befehl mit Ressourcen im aktiven Abonnement funktioniert, muss `--subscription` nicht angegeben werden.

Mit dem folgenden Befehl wird ein Speicherkonto in der angegebenen Ressourcengruppe erstellt:

```azurecli
az storage account create --resource-group StorageGroups --name storage136 \
    --location eastus --sku Standard_LRS
```

Ist die Speichergruppe nicht Teil Ihres aktuellen aktiven Abonnements, tritt bei diesem Befehl ein Fehler auf.

Ändern Sie ggf. das aktive Abonnement wie im nächsten Abschnitt beschrieben, oder geben Sie das Abonnement im Befehl an:

```azurecli
az storage account create --resource-group StorageGroups --subscription "My Demos" \
    --name storage136 --location eastus --sku Standard_LRS
```

## <a name="change-the-active-subscription"></a>Ändern des aktiven Abonnements

Sie können das aktive Abonnement mithilfe des Befehls [az account set](/cli/azure/account#az_account_set) ändern.

Rufen Sie eine Liste Ihrer Abonnements mithilfe des Befehls [az account list](/cli/azure/account#az_account_list) ab.

```azurecli
az account list --output table
```

Mit diesem Befehl werden alle Abonnements aufgelistet, auf die Sie zugreifen können. Ihr aktives Abonnement ist in der Spalte `IsDefault` durch `True` gekennzeichnet. Wenn ein erwartetes Abonnement nicht angezeigt wird, fügen Sie den Parameter `--refresh` hinzu, um die aktuelle Liste der Abonnements zu erhalten.

Um zu einem anderen Abonnement zu wechseln, verwenden Sie [az account set](/cli/azure/account#az_account_set) mit der ID oder dem Namen des gewünschten Abonnements.

```azurecli
az account set --subscription "My Demos"
```

Ihre Abonnements verfügen sowohl über einen Namen als auch über eine ID (GUID). Beides kann für diese Befehle verwendet werden. Verwenden Sie Anführungszeichen für einen Namen mit Leerzeichen.

Wenn Sie den Befehl [az account list](/cli/azure/account#az_account_list) erneut ausführen, wird in der Spalte `IsDefault` ihr aktuelles aktives Abonnement angezeigt.

## <a name="create-management-groups"></a>Erstellen von Verwaltungsgruppen

Azure-Verwaltungsgruppen enthalten Abonnements. Verwaltungsgruppen ermöglichen die Verwaltung des Zugriffs, der Richtlinien und der Compliance für diese Abonnements. Weitere Informationen finden Sie unter [Was sind Azure-Verwaltungsgruppen?](/azure/governance/management-groups/overview).

Verwenden Sie die Befehle vom Typ [az account management-group](/cli/azure/account/management-group) zum Erstellen und Verwalten von Verwaltungsgruppen.

Mithilfe des Befehls [az account management-group create](/cli/azure/account/management-group#az_account_management_group_create) können Sie eine Verwaltungsgruppe für mehrere Abonnements erstellen:

```azurecli
az account management-group create --name Contoso01
```

Verwenden Sie zum Anzeigen aller Verwaltungsgruppen den Befehl [az account management-group list](/cli/azure/account/management-group#az_account_management_group_list):

```azurecli
az account management-group list
```

Fügen Sie mithilfe des Befehls [az account management-group subscription add](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_add) Abonnements zur neuen Gruppe hinzu:

```azurecli
az account management-group subscription add --name Contoso01 --subscription "My Demos"
az account management-group subscription add --name Contoso01 --subscription "My Second Demos"
```

Verwenden Sie zum Entfernen eines Abonnements den Befehl [az account management-group subscription remove](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_remove):

```azurecli
az account management-group subscription remove --name Contoso01 --subscription "My Demos"
```

Führen Sie zum Entfernen einer Verwaltungsgruppe den Befehl [az account management-group delete](/cli/azure/account/management-group#az_account_management_group_delete) aus:

```azurecli
az account management-group delete --name Contoso01
```

Durch das Entfernen eines Abonnements oder das Löschen einer Verwaltungsgruppe wird ein Abonnement nicht gelöscht oder deaktiviert.

## <a name="set-a-subscription-lock"></a>Festlegen einer Abonnementsperre

Als Administrator müssen Sie ein Abonnement möglicherweise sperren, um zu verhindern, dass Benutzer es löschen oder ändern. Weitere Informationen finden Sie unter [Sperren von Ressourcen, um unerwartete Änderungen zu verhindern](/azure/azure-resource-manager/management/lock-resources).

Verwenden Sie in Azure CLI die Befehle vom Typ [az account lock](/cli/azure/account/lock). Beispielsweise kann der Befehl [az account lock create](/cli/azure/account/lock#az_account_lock_create) Benutzer am Löschen eines Abonnements hindern:

```azurecli
az account lock create --name "Cannot delete subscription" --lock-type CanNotDelete
```

> [!NOTE]
> Sie müssen über die entsprechenden Berechtigungen verfügen, um Sperren erstellen oder ändern zu können.

Verwenden Sie zum Anzeigen der aktuellen Sperren für Ihr Abonnement den Befehl [az account lock list](/cli/azure/account/lock#az_account_lock_list):

```azurecli
az account lock list --output table
```

Wenn Sie ein Konto als schreibgeschützt festlegen, ähnelt das Ergebnis dem Zuweisen von Berechtigungen der Rolle „Leser“ für alle Benutzer. Weitere Informationen zum Festlegen von Berechtigungen für einzelne Benutzer und Rollen finden Sie unter [Hinzufügen oder Entfernen von Azure-Rollenzuweisungen mithilfe der Azure-Befehlszeilenschnittstelle](/azure/role-based-access-control/role-assignments-cli).

Verwenden Sie zum Anzeigen der Details für eine Sperre den Befehl [az account lock show](/cli/azure/account/lock#az_account_lock_show):

```azurecli
az account lock show --name "Cannot delete subscription"
```

Sie können eine Sperre mithilfe des Befehls [az account lock delete](/cli/azure/account/lock#az_account_lock_delete) entfernen:

```azurecli
az account lock delete --name "Cannot delete subscription"
```

## <a name="see-also"></a>Siehe auch

* [Microsoft Azure-Glossar: Ein Wörterbuch der Cloudterminologie auf der Azure Platform](/azure/azure-glossary-cloud-terminology)
* [Zuordnen oder Hinzufügen eines Azure-Abonnements zu Ihrem Azure Active Directory-Mandanten](/azure/active-directory/active-directory-how-subscriptions-associated-directory)
* [Anmelden mit der Azure CLI](./authenticate-azure-cli.md)

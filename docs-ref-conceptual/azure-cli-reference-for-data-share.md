---
title: Azure CLI-Referenzen für Azure Data Share
description: Landing Page der Azure CLI-Referenzen für Azure Data Share
services: data-share
author: dbradish-microsoft
manager: barbkess
ms.service: data-share
ms.devlang: azurecli
ms.topic: reference
ms.date: 04/09/2021
ms.author: dbradish
ms.custom: devx-track-azurecli
ms.openlocfilehash: 7dda5b73452b9e8da905c88209189c14d83b0b81
ms.sourcegitcommit: f11f08a8b571d9909044693a8dc52c0cf2e9b2bc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/19/2021
ms.locfileid: "107711081"
---
# <a name="azure-cli-for-azure-data-share"></a>Azure CLI für Azure Data Share

Die Azure-Befehlszeilenschnittstelle ([Azure CLI](./what-is-azure-cli.md)) setzt sich aus Befehlen zum Erstellen und Verwalten von Azure-Ressourcen für zahlreiche Azure-Dienste zusammen. Für Azure Data Share sind über 65 verschiedene Befehle verfügbar, mit denen Sie den Dienst effektiv über eine Befehlszeile verwenden können.

## <a name="references-for-data-share"></a>Referenzen für Data Share

Alle Azure CLI-Befehle für [Azure Data Share](/azure/data-share/) sind derzeit in einer Erweiterung des Azure CLI-Kerns enthalten. Eine Datenfreigabeerweiterung ermöglicht Ihnen den Zugriff auf experimentelle und vorab veröffentlichte Befehle und wird automatisch installiert, wenn Sie zum ersten Mal einen Befehl vom Typ `az datashare` ausführen. Weitere Informationen zu Azure CLI-Erweiterungen finden Sie unter [Verwenden von Erweiterungen mit der Azure CLI](./azure-cli-extensions-overview.md).

|Azure CLI-Referenz |BESCHREIBUNG
|-|-|
| [az datashare](/cli/azure/datashare) | Alle Befehle zum Verwalten von Azure Data Share.
| [az datashare account](/cli/azure/datashare/account) | Befehle zum Verwalten von Azure Data Share-Konten.
| [az datashare consumer](/cli/azure/datashare/consumer) | Befehle für Consumer zum Verwalten von Azure Data Share.
| [az datashare dataset](/cli/azure/datashare/dataset) | Befehle für Anbieter zum Verwalten von Azure Data Share-Datasets.
| [az datashare invitation](/cli/azure/datashare/invitation) | Befehle für Consumer zum Verwalten von Azure Data Share-Einladungen.
| [az datashare provider-share-subscription](/cli/azure/datashare/provider-share-subscription) | Befehle für Anbieter zum Verwalten von Azure Data Share-Abonnements.
| [az datashare synchronization](/cli/azure/datashare/synchronization) | Befehle zum Verwalten der Azure Data Share-Synchronisierung.
| [az datashare synchronization-setting](/cli/azure/datashare/synchronization-setting) | Befehle für Anbieter zum Verwalten von Azure Data Share-Synchronisierungseinstellungen.

## <a name="reference-examples"></a>Referenzbeispiele

Es stehen Beispiele für jede Azure CLI-Referenz bereit. Sie können diese Aufgaben zwar auch über das Azure-Portal ausführen, aber zur Verwendung der Azure CLI ist eine Befehlszeile erforderlich. Nachfolgend sehen Sie einige Codeblöcke, die Ihnen eine Vorstellung davon geben, wie einfach die Azure CLI zu verwenden ist.

Zum Arbeiten mit Azure Data Share benötigen Sie zunächst eine Ressourcengruppe. Azure-Ressourcengruppen können auf einfache Weise mit der Azure CLI erstellt und verwaltet werden.  

```azurecli
#create a resource group
az group create --location westus --name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

Die Erstellung eines Datenfreigabekontos ist ebenfalls ganz einfach.

```azurecli
#create a data share account
az datashare account create --location westus --tags tag1=Red tag2=White --name MyAccount --resource-group MyResourceGroup
```

## <a name="see-also"></a>Weitere Informationen

* Unter [Erste Schritte mit der Azure CLI](./get-started-with-azure-cli.md) erhalten Sie Informationen zur Installation und Anmeldung.

* Entdecken Sie weitere [Befehle](/cli/azure/reference-index) und [Erweiterungen](./azure-cli-extensions-list.md) in der Azure CLI-Dokumentation.

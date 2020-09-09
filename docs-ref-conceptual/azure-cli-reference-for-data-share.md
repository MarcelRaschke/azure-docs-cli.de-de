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
# <a name="azure-cli-for-azure-data-share"></a>Azure CLI für Azure Data Share

Die Azure-Befehlszeilenschnittstelle ([Azure CLI](/cli/azure/what-is-azure-cli)) setzt sich aus Befehlen zum Erstellen und Verwalten von Azure-Ressourcen zusammen.  Sie ist in vielen Azure-Diensten verfügbar, darunter auch Azure Data Share.  Es stehen mehr als 65 verschiedene Befehle für Data Share bereit.  Mithilfe dieser Befehle können Sie den Dienst effektiv über eine Befehlszeile nutzen.

## <a name="references-for-data-share"></a>Referenzen für Data Share

Alle Azure CLI-Befehle für Azure Data Share sind derzeit Erweiterungen der Azure CLI.  Eine Erweiterung ermöglicht Ihnen den Zugriff auf experimentelle und vorab veröffentlichte Befehle.  Weitere Informationen zu Erweiterungen finden Sie unter [Verwenden von Erweiterungen mit der Azure CLI](/cli/azure/azure-cli-extensions-overview).

|Azure CLI-Referenz |BESCHREIBUNG
|-|-|-|
| [az datashare](/cli/azure/ext/datashare/datashare) | Alle Befehle zum Verwalten von Azure Data Share.
| [az datashare account](/cli/azure/ext/datashare/datashare/account) | Befehle zum Verwalten von Azure Data Share-Konten.
| [az datashare consumer](/cli/azure/ext/datashare/datashare/consumer) | Befehle für Consumer zum Verwalten von Azure Data Share.
| [az datashare dataset](/cli/azure/ext/datashare/datashare/dataset) | Befehle für Anbieter zum Verwalten von Azure Data Share-Datasets.
| [az datashare invitation](/cli/azure/ext/datashare/datashare/invitation) | Befehle für Consumer zum Verwalten von Azure Data Share-Einladungen.
| [az datashare provider-share-subscription](/cli/azure/ext/datashare/datashare/provider-share-subscription) | Befehle für Anbieter zum Verwalten von Azure Data Share-Abonnements.
| [az datashare synchronization](/cli/azure/ext/datashare/datashare/synchronization)  | Befehle zum Verwalten der Azure Data Share-Synchronisierung.
| [az datashare synchronization-setting](/cli/azure/ext/datashare/datashare/synchronization-setting)  | Befehle für Anbieter zum Verwalten von Azure Data Share-Synchronisierungseinstellungen.

## <a name="reference-examples"></a>Referenzbeispiele

Es stehen Beispiele für jede Azure CLI-Referenz bereit. Sie können diese Aufgaben zwar auch über das Azure-Portal ausführen, doch ist zur Verwendung der Azure CLI nur eine einzige Befehlszeile erforderlich.  Nachfolgend sehen Sie einige Codeblöcke, die Ihnen eine Vorstellung davon geben, wie einfach die Azure CLI zu verwenden ist.

Zum Arbeiten mit Azure Data Share benötigen Sie zunächst eine Ressourcengruppe.  Azure-Ressourcengruppen können auf einfache Weise mit der Azure CLI erstellt und verwaltet werden.  

```azurecli
#create a resource group
az group create -location westus -name MyResourceGroup
```

```azurecli
#get a list of resource groups for a subscription
az group list --subscription MySubscription --output table
```

Genauso einfach kann ein Data Share-Konto erstellt werden.

```azurecli
#create a data share account
az datashare account create --location "West US 2" --tags tag1=Red tag2=White --name MyAccount --resource-group MyResourceGroup
```

## <a name="see-also"></a>Weitere Informationen

* Unter [Erste Schritte mit der Azure CLI](/cli/azure/get-started-with-azure-cli) erhalten Sie Informationen zur Installation und Anmeldung.

* Entdecken Sie weitere [Befehle](/cli/azure/reference-index) und [Erweiterungen](/cli/azure/azure-cli-extensions-list) in der Azure CLI-Dokumentation.

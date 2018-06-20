---
title: Azure CLI 2.0
description: Enthält eine Übersicht über Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 9b6f7a5c79033c0b0bec2bf8b56eb40831484f1a
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/18/2018
ms.locfileid: "34306249"
---
# <a name="azure-cli-20"></a>Azure CLI 2.0

Die Azure CLI 2.0 ist die plattformübergreifende Befehlszeilenumgebung von Microsoft zum Verwalten von Azure-Ressourcen.
Sie können sie in Ihrem Browser mit [Azure Cloud Shell](/azure/cloud-shell/overview) verwenden oder unter macOS, Linux oder Windows [installieren](install-azure-cli.md) und über die Befehlszeile ausführen.

Azure CLI 2.0 ist für die Verwaltung von Azure-Ressourcen über die Befehlszeile sowie die Erstellung von Automatisierungsskripts für Azure Resource Manager optimiert. Mit Azure CLI 2.0 können Sie VMs in Azure erstellen, indem Sie einfach den folgenden Befehl eingeben:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

Führen Sie die CLI mithilfe von [Cloud Shell](/azure/cloud-shell/overview) in Ihrem Browser aus, oder [installieren](install-azure-cli.md) Sie sie unter macOS, Linux oder Windows.
Lesen Sie den Artikel mit den [ersten Schritten](get-started-with-azure-cli.md), um mit der Verwendung der CLI zu beginnen.
Informationen zur neuesten Version finden Sie in den [Versionshinweisen](release-notes-azure-cli.md).

Die folgenden Beispiele erleichtern Ihnen den Einstieg in allgemeine Aufgaben in Azure CLI 2.0:
- [Virtuelle Linux-Computer](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- Interaktiv: [Erstellen virtueller Linux-Computer](https://docs.microsoft.com/learn/azure-cli-2-0/index)
- [Virtuelle Windows-Computer](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Web-Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [SQL-Datenbank](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Außerdem ist eine ausführliche [Referenz](/cli/azure/reference-index) verfügbar, in der dokumentiert ist, wie Sie die einzelnen Azure CLI 2.0-Befehle verwenden.

Führen Sie jetzt die [ersten Schritte](get-started-with-azure-cli.md) mit Azure CLI 2.0 aus.

> [!NOTE]
> Falls Sie die vorherige Version der CLI (Azure CLI 1.0) nutzen, können Sie sie weiterverwenden.
> Das beste Ergebnis erzielen Sie jedoch, wenn Sie ein Update auf die aktuelle Version der Azure CLI 2.0 ausführen.
> Beachten Sie bei der Verwendung beider CLIs Folgendes: `azure` ist die alte CLI (Azure-CLI), und `az` ist die neue CLI (Azure CLI 2.0).

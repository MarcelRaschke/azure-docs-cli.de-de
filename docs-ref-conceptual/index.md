---
title: Übersicht über Azure CLI 2.0
description: Enthält eine Übersicht über Azure CLI 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 55c5ea3ad69df60d211cc076e3570e9f07040af7
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388387"
---
# <a name="azure-cli-20"></a>Azure CLI 2.0

Die Azure CLI 2.0 ist die plattformübergreifende Befehlszeilenumgebung von Microsoft zum Verwalten von Azure-Ressourcen.
Sie können sie in Ihrem Browser mit [Azure Cloud Shell](/azure/cloud-shell/overview) verwenden oder unter macOS, Linux oder Windows [installieren](install-azure-cli.md) und über die Befehlszeile ausführen.

Der Einstieg in die Azure CLI 2.0 ist einfach, und sie eignet sich am besten für die Erstellung von Automatisierungsskripts für Azure Resource Manager. Mit Azure CLI 2.0 können Sie VMs in Azure erstellen, indem Sie einfach den folgenden Befehl eingeben:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a>Ausführen oder Installieren

Sie können die CLI lokal installieren oder im Browser mit Azure Cloud Shell oder in einem Docker-Container ausführen.

* Informationen zum Ausführen im Browser mit Azure Cloud Shell finden Sie unter [Schnellstart für Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) oder [Schnellstartanleitung für PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).
* Informationen zur Installation der Azure CLI finden Sie unter [Installieren der Azure CLI 2.0](install-azure-cli.md).
* Informationen zur Ausführung als Docker-Container finden Sie unter [Ausführen der Azure CLI 2.0 in einem Docker-Container](run-azure-cli-docker.md).

## <a name="get-started"></a>Erste Schritte

Lesen Sie den Artikel mit den [ersten Schritten](get-started-with-azure-cli.md), um mehr über die Grundlagen der CLI zu erfahren. Die folgenden Beispiele zeigen einige allgemeine Anwendungsfälle:

- [Virtuelle Linux-Computer](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Virtuelle Windows-Computer](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Web-Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [SQL-Datenbank](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Außerdem ist eine ausführliche [Referenz](/cli/azure/reference-index) verfügbar, in der dokumentiert ist, wie Sie die einzelnen Azure CLI 2.0-Befehle verwenden.

> [!NOTE]
> Falls Sie die vorherige Version der CLI (Azure CLI 1.0) nutzen, können Sie sie weiterverwenden.
> Das beste Ergebnis erzielen Sie jedoch, wenn Sie ein Update auf die aktuelle Version der Azure CLI 2.0 ausführen.
> Beachten Sie bei der Verwendung beider CLIs Folgendes: `azure` ist die alte CLI (Azure-CLI), und `az` ist die neue CLI (Azure CLI 2.0).

---
title: Übersicht über die Azure CLI
description: Enthält eine Übersicht über die Azure CLI.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 047a953a0ab8ccaf145d56e4d774d2bf9852ed6f
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177724"
---
# <a name="azure-cli"></a>Azure CLI

Die Azure CLI ist die plattformübergreifende Befehlszeilenumgebung von Microsoft zum Verwalten von Azure-Ressourcen.
Sie können sie in Ihrem Browser mit [Azure Cloud Shell](/azure/cloud-shell/overview) verwenden oder unter macOS, Linux oder Windows [installieren](install-azure-cli.md) und über die Befehlszeile ausführen.

Der Einstieg in die Azure CLI ist einfach, und sie eignet sich am besten für die Erstellung von Automatisierungsskripts für Azure Resource Manager. Mit der Azure CLI können Sie VMs in Azure erstellen, indem Sie einfach den folgenden Befehl eingeben:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS
```

## <a name="run-or-install"></a>Ausführen oder Installieren

Sie können die CLI lokal installieren oder im Browser mit Azure Cloud Shell oder in einem Docker-Container ausführen.

* Informationen zum Ausführen im Browser mit Azure Cloud Shell finden Sie unter [Schnellstart für Bash in Azure Cloud Shell](/azure/cloud-shell/quickstart) oder [Schnellstartanleitung für PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).
* Informationen zur Installation der Azure CLI finden Sie unter [Installieren der Azure CLI](install-azure-cli.md).
* Informationen zur Ausführung als Docker-Container finden Sie unter [Ausführen der Azure CLI in einem Docker-Container](run-azure-cli-docker.md).

## <a name="build-your-skills-with-microsoft-learn"></a>Erweitern Ihrer Fähigkeiten mit Microsoft Learn

- [Verwalten von virtuellen Computern mit der Azure CLI](/learn/modules/manage-virtual-machines-with-azure-cli/)
- [Steuern der Azure-Dienste mit der Befehlszeilenschnittstelle](/learn/modules/control-azure-services-with-cli/)
- [Mehr interaktives Lernen...](/learn/browse/?products=azure-clis)

## <a name="get-started"></a>Erste Schritte

Lesen Sie den Artikel mit den [ersten Schritten](get-started-with-azure-cli.md), um mehr über die Grundlagen der CLI zu erfahren. Die folgenden Beispiele zeigen einige allgemeine Anwendungsfälle:

- [Virtuelle Linux-Computer](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Virtuelle Windows-Computer](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [Web-Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)
- [SQL-Datenbank](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json)

Außerdem ist eine ausführliche [Referenz](/cli/azure/reference-index) verfügbar, in der dokumentiert ist, wie Sie die einzelnen Azure CLI-Befehle verwenden.

> [!NOTE]
> Falls Sie die vorherige Version der CLI (klassische Azure CLI) nutzen, können Sie sie weiterverwenden.
> Das beste Ergebnis erzielen Sie aber, wenn Sie ein Update auf die aktuelle Version der Azure CLI durchführen.
> Wenn Sie beide CLIs verwenden, sollten Sie daran denken, dass `azure` die klassische CLI und `az` die aktuellste CLI ist.

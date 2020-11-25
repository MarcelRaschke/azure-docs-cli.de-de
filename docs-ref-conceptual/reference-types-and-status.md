---
title: Azure CLI-Verweistypen
description: Eine Erläuterung der Verweistypen und des Verweisstatus
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/19/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: ff77011db5a64e7c541dc67f2b2564301bfeebfb
ms.sourcegitcommit: 6996f3d05d73f528a95b61fdce1422eee3c7a580
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/25/2020
ms.locfileid: "95870150"
---
# <a name="overview-azure-cli-reference-types-and-status"></a>Übersicht: Azure CLI-Verweistypen und -status

Die Azure CLI verfügt über verschiedene Verweistypen, die manchmal synonym als Verweisstatus bezeichnet werden.  In diesem Artikel wird der Unterschied zwischen einem Azure CLI-Typ und einem Status erläutert. Außerdem finden Sie hier Informationen zur Verwendung beider Optionen.

## <a name="azure-cli-syntax-components"></a>Komponenten der Azure CLI-Syntax

Die Azure CLI-Syntax ist eine Kombination aus Verweisen, Befehlen und Parametern.  Der **gesamte Verweisbefehl** wird häufig als **Befehl** bezeichnet.

| Azure-Dienst | Verweis | Subdienst für den Verweis | Get-Help | Vollständiger Verweisbefehl | Parameterbeispiele
|-|-|-|-|-|-|
| Azure CLI | [az configure](/cli/azure/reference-index#az-configure) | | | az configure | --defaults, --list-default, --scope
| Azure-Netzwerk | [az network](/cli/azure/network) | application-gateway | create | [az network application-gateway create](/cli/azure/network/application-gateway#az-network-application-gateway-create) | --name, --resource-group, --capacity
| Azure DevOps Server | [az pipelines](/cli/azure/pipelines) | Agent | list | [az pipelines agent list](/cli/azure/pipelines/agent) | --pool-id, --agent-name, --demands

## <a name="reference-types"></a>Verweistypen

Ein Verweistyp gibt Aufschluss darüber, ob der Verweisbefehl Teil des primären Azure CLI-Diensts ist oder ob es sich um ein optionales Add-on handelt.  Es gibt zwei Arten von Azure CLI-Verweisbefehlen: **Kern** und **Erweiterung**.

|         | Core  | Durchwahl
|-|-|-|
| **Referenzen** | Teil des primären Azure CLI-Diensts | Optionale Verweisbefehle, die installiert werden müssen
| **Installieren** | Gemeinsam mit dem [MSI-Installationsprogramm]() | Einzeln mit [az extension add]()|
| **Veröffentlicht** | Nach einem Zeitplan | Wenn neue Features oder Updates verfügbar werden
| **Status** | Kann „Allgemein verfügbar“, „Public Preview“ oder „Experimentell“ lauten. | Allgemein verfügbar, Vorschauversion oder experimentell

Alle Azure CLI-Verweise können unter Windows, macOS und Linux sowie in Docker und Azure Cloud Shell ausgeführt werden.

### <a name="core"></a>Core

Azure CLI-Verweise, die als ständiger Teil der CLI veröffentlicht wurden, werden als **Kernverweise** bezeichnet.  Alle Kernverweise werden zusammen mit der Azure CLI installiert. Es ist nicht möglich, nur eine Teilmenge der Verweise auszuwählen.  Wenn Sie die CLI über Azure Cloud Shell ausführen, sind die Kernverweise immer auf dem neuesten Stand.  Eine umfassende Liste der Kernverweisbefehle finden Sie in der [Kernverweisliste für die Azure CLI](/cli/azure/reference-index).

### <a name="extension"></a>Durchwahl

Erweiterungen werden nicht zusammen mit der CLI bereitgestellt, können aber als CLI-Befehle ausgeführt werden.  Zwar sind einige Erweiterungen ständiger Teil der Azure CLI, oftmals ermöglicht eine Erweiterung jedoch den Zugriff auf Befehle einer privaten Vorschau oder auf experimentelle Befehle.  Ein einzelner Verweis wie etwa **az iot hub** kann sowohl Kern- als auch Erweiterungsbefehle enthalten.  Im Anschluss folgen vier Beispiele:

| Vollständiger Verweisbefehl | Kern | Erweiterung
|-|-|-|
| az iot hub list | ja |
| az iot hub query | | ja
| az iot hub certificate create | ja |
| az iot hub device identify create | | ja

> [!IMPORTANT]
> Vor der Verwendung muss durch Ausführen des Befehls [az extension add](/cli/azure/extension#az-extension-add) eine Erweiterung installiert werden.

Weitere Informationen zu Erweiterungsverweisen (einschließlich Installation und Aktualisierung) finden Sie unter [Verwenden von Erweiterungen mit der Azure CLI](azure-cli-extensions-overview.md).  Sehen Sie sich die Erweiterung [wiki tips](https://github.com/Azure/azure-network-cli-extension/wiki/Tips) an, um die Nutzung zu maximieren.  Unter [Verfügbare Erweiterungen für die Azure CLI](azure-cli-extensions-list.md) finden Sie eine vollständige Liste der Erweiterungsverweisbefehle.

## <a name="reference-status"></a>Verweisstatus

Azure CLI-Verweise fallen unabhängig von ihrem Typ in drei Statuskategorien: **Allgemein verfügbar**, **Public Preview** und **Experimentell**.  Stabilität und Supportebene werden durch den Verweisbefehlstatus (nicht durch den Typ) bestimmt.

| | Allgemein verfügbar  | Public Preview | Experimentell
|-|-|-|-|
| **Stabilität** | Dauerhaft | Kann als Reaktion auf Kundenfeedback geändert werden.  Unterliegt den Bedingungen für [Microsoft Azure-Vorschauversionen](https://azure.microsoft.com/support/legal/preview-supplemental-terms/). | Kann als Reaktion auf Kundenfeedback geändert werden.  Wird häufig zur öffentlichen Vorschau migriert.  Kann entfernt werden.
| **Supportebene** | Vollständig | Partial | Keine

Die meisten Befehle und Parameter für einen Verweis haben zwar einen einzelnen Status, dies ist jedoch nicht immer der Fall.  Ein allgemein verfügbarer Verweis, der für weitere Befehle erweitert wird, kann über Verweisbefehle mit dem Status „Allgemein verfügbar“, „Vorschau“ und „Experimentell“ verfügen. Darüber hinaus kann ein einzelner Befehl über Parameter verfügen, die in unterschiedliche Statuskategorien fallen. Dies ist der Fall, wenn neue Parameter hinzugefügt werden, um den Funktionsumfang zu erweitern.  Die folgende Tabelle enthält Beispiele für Verweise mit verschiedenen Statuswerten:

| Vollständiger Verweisbefehl | Parameter | type | Allgemein verfügbar | Public Preview | Experimentell
|-|-|-|-|-|-|
| az network dns zone list | Alle | Core | ja |
| az network dns zone create | --name, --resource-group, --if-none-match, --parent-name | Core | ja |
|  | --newFutureParameter1 | Core | | ja
|  | --newFutureParameter2 | Core | | | ja
| az network vhub list | Alle |Durchwahl | ja
| az network vhub create | --address-prefix, --name, --resource-group, -vwan, --location, --sku |Durchwahl | ja
|  | --newFutureParameter1 |Durchwahl | | ja
|  | --newFutureParameter2|Durchwahl | | | ja
| az network firewall create | Alle | Durchwahl | | | ja

> [!NOTE]
> Warnungen mit einem Hinweis auf **Public Preview** oder **experimentell** sind Teil der Azure CLI-Befehlsausgabe und ganz normal.

## <a name="see-also"></a>Weitere Informationen

- [Kernverweisliste für die Azure CLI](/cli/azure/reference-index)
- [Verfügbare Erweiterungen für die Azure CLI](azure-cli-extensions-list.md)

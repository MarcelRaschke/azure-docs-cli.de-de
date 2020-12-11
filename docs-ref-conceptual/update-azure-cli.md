---
title: Aktualisieren der Azure-Befehlszeilenschnittstelle
description: Referenz zur Aktualisierung der Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 10/19/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 91ed79b9f59af4ad070983eb7d0744bc85d09216
ms.sourcegitcommit: 9beaf9abb794f1006a56acee4e1cfb8ea7fe2405
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/08/2020
ms.locfileid: "96850874"
---
# <a name="update-the-azure-cli"></a>Aktualisieren der Azure-Befehlszeilenschnittstelle

Sie können sich darauf verlassen, dass Paket-Manager eine lokale Installation der Azure CLI in Windows-, macOS- und Linux-Umgebungen aktualisieren (siehe Abschnitt `Update` in den jeweiligen plattformspezifischen Installationsanweisungen). Die CLI bietet außerdem Befehle im Tool zum manuellen oder automatischen Aktualisieren.

## <a name="manual-update"></a>Manuelle Aktualisierung
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

`az upgrade` wird unter Windows und macOS und in einigen Linux-Distributionen unterstützt, sofern auch die Installation unterstützt wird. Damit wird nur das Upgrade auf die neuste Version unterstützt. Wenn Sie die Azure CLI über Azure Cloud Shell ausführen, verwenden Sie wahrscheinlich bereits die aktuelle Azure CLI-Installation. Ist dies beispielsweise aufgrund eines Ad-hoc-Release einer Nebenversion zur Fehlerbehebung nicht der Fall, müssen Sie auf den nächsten Build von Azure Cloud Shell warten, da `az upgrade` in Azure Cloud Shell nicht unterstützt wird.

Ist `azure-cli` bereits die aktuelle Version, werden bei der Ausführung von `az upgrade` alle installierten [Erweiterungen](azure-cli-extensions-overview.md) überprüft und aktualisiert.

## <a name="automatic-update"></a>Automatische Aktualisierung

Automatische Upgrades sind für die Azure CLI standardmäßig deaktiviert. Wenn Sie stets die aktuelle Version verwenden möchten, können Sie automatische Upgrades über die [Konfiguration](/cli/azure/config) aktivieren.

```azurecli
az config set auto-upgrade.enable=yes
```

Die Azure CLI prüft regelmäßig auf neue Versionen und fordert Sie nach Abschluss der Befehlsausführung zur Aktualisierung auf, sobald das Update verfügbar ist.

Die Aufforderungsmeldung und die Ausgabemeldungen während des Upgrades unterbrechen unter Umständen das Befehlsergebnis, wenn es einer Variablen oder in einem automatisierten Flow zugewiesen ist. Zur Vermeidung von Unterbrechungen können Sie die folgende Konfiguration verwenden, um zuzulassen, dass das Update automatisch ohne Bestätigung ausgeführt wird und nur Warnungen und Fehler während des Upgrades angezeigt werden.

```azurecli
az config auto-upgrade.prompt=no
```

Standardmäßig werden alle installierten Erweiterungen ebenfalls aktualisiert. Sie können die Aktualisierung von Erweiterungen über die Konfiguration deaktivieren.

```azurecli
az config auto-upgrade.all=no
```

> [!NOTE]
> Warten Sie, bis `az upgrade` abgeschlossen ist, bevor Sie mit dem nächsten Befehlssatz fortfahren. Andernfalls weisen die neuen Versionen der CLI (und Erweiterungen) möglicherweise Breaking Changes auf.

Wenn Sie die Funktion für automatische Updates nicht mehr verwenden möchten, um beispielsweise die stabile Ausführung von Befehlsskripts zu gewährleisten, können Sie sie über die Konfiguration deaktivieren.
```azurecli
az config set auto-upgrade.enable=no
```

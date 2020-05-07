---
title: Azure CLI – Interaktiver Modus
description: Verwenden Sie die Azure CLI im interaktiven Modus.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 7b3ee1e284e7f771c661bb65bf8b8ab53dafd77f
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2020
ms.locfileid: "77779515"
---
# <a name="azure-cli-interactive-mode"></a>Azure CLI – Interaktiver Modus

Sie können die Azure CLI im interaktiven Modus verwenden, indem Sie den Befehl `az interactive` ausführen.
Bei diesem Modus arbeiten Sie in einer interaktiven Shell mit automatischer Vervollständigung, Befehlsbeschreibungen und Beispielen.

![Interaktiver Modus](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> Wir verwenden hier nicht das Standarddesign, da es auf einem schwarzen Hintergrund nicht so gut lesbar ist.

Wenn Sie noch nicht bei Ihrem Konto angemeldet sind, verwenden Sie dazu den `login`-Befehl.

## <a name="configure"></a>Konfigurieren

Im interaktiven Modus werden optional Beschreibungen zu Befehlen und Parametern sowie Befehlsbeispiele angezeigt.
Über `F1` können Sie Beschreibungen und Beispiele aktivieren oder deaktivieren.

![Beschreibungen und Beispiele](./media/interactive-azure-cli/descriptions-and-examples.png)

Sie können die Anzeige von Standardwerten für Parameter über `F2` aktivieren oder deaktivieren.

![Standardwerte](./media/interactive-azure-cli/defaults.png)

`F3` schaltet die Anzeige einiger Tastenkombinationen ein oder aus.

![Tastenkombinationen](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a>`Scope`

Sie können den Bereich Ihres interaktiven Modus auf eine bestimmte Befehlsgruppe wie `vm` oder `vm image` festlegen.
In diesem Fall werden alle Befehle für diesen Bereich interpretiert.
Dies ist eine hervorragende Kompakteigenschaft, wenn Sie Ihre gesamte Arbeit in dieser Befehlsgruppe ausführen.

Statt diese Befehle einzugeben:

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

können Sie den Bereich auf die Befehlsgruppe „vm“ festlegen und folgende Befehle eingeben:

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

Sie können den Bereich auch auf Befehlsgruppen einer niedrigeren Ebene beschränken.
Mit `vm image` können Sie den Bereich auf `%%vm image` festlegen.
Da der Bereich bereits auf `vm` festgelegt ist, verwenden wir in diesem Fall `%%image`.

```azurecli
az vm>> %%image
az vm image>>
```

An diesem Punkt können wir den Bereich mit `vm` wieder auf `%%..` erweitern oder einfach mit `%%` auf das Stammverzeichnis festlegen.

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a>Abfrage

Sie können eine JMESPath-Abfrage für die Ergebnisse des zuletzt ausgeführten Befehls ausführen, indem Sie `??` gefolgt von einer JMESPath-Abfrage verwenden.
Nach dem Erstellen einer Gruppe können Sie beispielsweise die ID der neuen Gruppe abrufen.

```azurecli
az>> group create -n myRG -l westEurope
az>> "?? id"
```

Mithilfe dieser Syntax können Sie auch das Ergebnis des vorherigen Befehls als Argument für den nächsten Befehl verwenden.* Nach dem Auflisten aller Gruppen können Sie z. B. alle Ressourcen des Typs `virtualMachine` in der ersten Gruppe mit dem Standort „Europa, Westen“ auflisten. 

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait -o json
az>> group list -o json
az>> resource list -g "?? [?location=='westeurope'].name | [0]" --query "[?type=='Microsoft.Compute/virtualMachines'].name
```

Weitere Informationen zum Abfragen der Ergebnisse Ihrer Befehle finden Sie unter [Abfragen von Befehlsergebnissen mit der Azure CLI](query-azure-cli.md).

## <a name="bash-commands"></a>Bash-Befehle

Mit `#[cmd]` können Sie Shellbefehle ausführen, ohne den interaktiven Modus zu verlassen.

```azurecli
az>> #dir
```

## <a name="examples"></a>Beispiele

Für einige Befehle gibt es zahlreiche Beispiele.
Mit `CTRL-N` können Sie zur nächsten und mit `CTRL-Y` zur vorherigen Seite mit Beispielen scrollen.

![Beispiele](./media/interactive-azure-cli/examples.png)

Über `::#` können Sie sich auch ein bestimmtes Beispiel ansehen.

```azurecli
az>> vm create ::8
```

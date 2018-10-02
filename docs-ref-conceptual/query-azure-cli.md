---
title: Abfragen von Befehlsergebnissen mit der Azure CLI
description: Es wird beschrieben, wie Sie JMESPath-Abfragen für die Ausgabe von Azure CLI-Befehlen ausführen.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 4522242952e5d257449c9c593885c62de2f56d0f
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/25/2018
ms.locfileid: "47178030"
---
# <a name="use-jmespath-queries-with-azure-cli"></a>Verwenden von JMESPath-Abfragen mit der Azure CLI 

Die Azure CLI verwendet das Argument `--query`, um eine [JMESPath-Abfrage](http://jmespath.org) für die Ergebnisse von Befehlen auszuführen. JMESPath ist eine Abfragesprache für JSON, die es ermöglicht, Daten aus der CLI-Ausgabe auszuwählen und zu präsentieren. Diese Abfragen werden für die JSON-Ausgabe ausgeführt, bevor irgendeine Anzeigeformatierung stattfindet.

Das Argument `--query` wird von allen Befehlen der Azure-Befehlszeilenschnittstelle unterstützt. Die Beispiele in diesem Artikel decken allgemeine Anwendungsfälle ab und veranschaulichen die Verwendung der Features von JMESPath.

## <a name="work-with-dictionary-output"></a>Verwenden einer Wörterbuchausgabe

Befehle, die ein JSON-Wörterbuch zurückgeben, können allein anhand ihrer Schlüsselnamen durchsucht werden. Bei Schlüsselpfaden wird als Trennzeichen das `.`-Zeichen verwendet. Im folgenden Beispiel wird mithilfe von Pull eine Liste mit den öffentlichen SSH-Schlüsseln abgerufen, die beim Herstellen einer Verbindung mit einem virtuellen Linux-Computer zulässig sind:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

Mehrere Werte können in einem sortierten Array platziert werden. Das folgende Beispiel zeigt das Abrufen des Azure-Imageangebotsnamens und der Größe des Betriebssystemdatenträgers:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

Wenn die Ausgabe Schlüssel enthalten soll, können Sie eine alternative Wörterbuchsyntax verwenden.  Bei der Auswahl von Elementen in einem Wörterbuch wird das Format `{displayKey:keyPath, ...}` verwendet, um nach dem `keyPath`-JMESPath-Ausdruck zu filtern. In den Ausgabewerten werden die Schlüssel-Wert-Paare in `{displayKey: value}` geändert. Das nächste Beispiel baut auf der Abfrage des letzten Beispiels auf und weist der Ausgabe Schlüssel zu, um sie deutlicher zu machen:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

Beim Anzeigen von Informationen im Ausgabeformat `table` ermöglicht die Wörterbuchanzeige das Festlegen eigener Spaltenüberschriften. Weitere Informationen zu Ausgabeformaten finden Sie unter [Ausgabeformate für Azure CLI-Befehle](/cli/azure/format-output-azure-cli).

> [!NOTE]
> Bestimmte Schlüssel werden herausgefiltert und nicht in der Tabellenansicht gedruckt. Diese Schlüssel sind `id`, `type` und `etag`. Wenn Sie diese Informationen benötigen, können Sie den Schlüsselnamen ändern und so die Filterung umgehen.
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a>Verwenden von Listenausgaben

CLI-Befehle, die mehrere Werte zurückgeben können, geben ein Array zurück. Auf Arrayelemente wird über einen Index zugegriffen, und sie werden unter Umständen nicht jedes Mal in der gleichen Reihenfolge zurückgegeben. Sie können alle Arrayelemente gleichzeitig abfragen, indem Sie sie mit dem Operator `[]` vereinfachen. Der Operator wird nach dem Array oder als erstes Element in einen Ausdruck eingefügt. Bei einem vereinfachten Array wird die darauffolgende Abfrage für jedes Arrayelement ausgeführt.

Im folgenden Beispiel werden jeweils der Name und das Betriebssystem der virtuellen Computer in einer Ressourcengruppe ausgegeben.

```azurecli-interactive
az vm list -g QueryDemo --query '[].{name:name, image:storageProfile.imageReference.offer}'
```

```json
[
  {
    "image": "CentOS",
    "name": "CentBox"
  },
  {
    "image": "openSUSE-Leap",
    "name": "SUSEBox"
  },
  {
    "image": "UbuntuServer",
    "name": "TestVM"
  },
  {
    "image": "UbuntuServer",
    "name": "Test2"
  },
  {
    "image": "WindowsServer",
    "name": "WinServ"
  }
]
```

Auch Arrays, die einem Schlüsselpfad angehören, können vereinfacht werden. Die folgende Abfrage ruft die Azure-Objekt-IDs für die NICs ab, mit denen ein virtueller Computer verbunden ist.

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a>Filtern der Arrayausgabe mit Prädikaten

JMESPath bietet [Filterausdrücke](http://jmespath.org/specification.html#filterexpressions) zum Herausfiltern der angezeigten Daten. Diese Ausdrücke sind besonders hilfreich, wenn sie mit [integrierten JMESPath-Funktionen](http://jmespath.org/specification.html#built-in-functions) kombiniert werden, um teilweise Übereinstimmungen zu ermitteln oder Daten in ein Standardformat zu konvertieren. Filterausdrücke können nur für Arraydaten verwendet werden. In allen anderen Fällen geben Sie den Wert `null` zurück. Sie können beispielsweise die Ausgabe von Befehlen wie `vm list` filtern, um nach bestimmten Arten von virtuellen Computern zu suchen. Das folgende Beispiel baut auf dem vorherigen Beispiel auf und filtert den VM-Typ heraus, um nur virtuelle Windows-Computer zu erfassen und deren Namen auszugeben.

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a>Interaktives Experimentieren mit Abfragen

Wenn Sie sich mit JMESPath vertraut machen möchten, können Sie in der interaktiven Umgebung des Python-Pakets [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) mit Abfragen experimentieren. Daten werden als Eingabe übergeben. Anschließend werden programminterne Abfragen geschrieben und bearbeitet, um die Daten zu extrahieren.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```

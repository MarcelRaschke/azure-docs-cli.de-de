---
title: Abfragen von Befehlsergebnissen mit Azure CLI 2.0
description: Erfahren Sie, wie Sie JMESPath-Abfragen für die Ausgabe von Azure CLI 2.0-Befehlen ausführen.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: ed8f8ac160dd8225170ffcfff9619d94b92e456a
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/18/2018
ms.locfileid: "34306164"
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a>Verwenden von JMESPath-Abfragen mit der Azure CLI 2.0

Die Azure CLI 2.0 verwendet das Argument `--query`, um eine [JMESPath-Abfrage](http://jmespath.org) für die Ergebnisse von Befehlen auszuführen. JMESPath ist eine Abfragesprache für JSON, die es ermöglicht, Daten aus der CLI-Ausgabe auszuwählen und zu präsentieren. Diese Abfragen werden für die JSON-Ausgabe ausgeführt, bevor irgendeine andere Anzeigeformatierung stattfindet.

Das Argument `--query` wird von allen Befehlen der Azure-Befehlszeilenschnittstelle unterstützt. Die Beispiele in diesem Artikel decken allgemeine Anwendungsfälle ab und veranschaulichen die Verwendung der Features von JMESPath.

## <a name="work-with-dictionary-output"></a>Verwenden einer Wörterbuchausgabe

Befehle, die ein JSON-Wörterbuch zurückgeben, können allein anhand ihrer Schlüsselnamen durchsucht werden. Bei Schlüsselpfaden wird als Trennzeichen das `.`-Zeichen verwendet. Im folgenden Beispiel wird mithilfe von Pull eine Liste mit den öffentlichen SSH-Schlüsseln abgerufen, die beim Herstellen einer Verbindung mit einem virtuellen Linux-Computer zulässig sind:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

Sie können auch mehrere Werte abrufen und in einem sortierten Array platzieren. Das Array verfügt zwar über keinerlei Schlüsselinformationen, die Reihenfolge der Arrayelemente entspricht jedoch der Reihenfolge der abgefragten Schlüssel. Das folgende Beispiel zeigt das Abrufen des Azure-Imageangebotsnamens und der Größe des Betriebssystemdatenträgers:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

Wenn die Ausgabe Schlüssel enthalten soll, können Sie eine alternative Wörterbuchsyntax verwenden. Bei der Auswahl mehrerer Elemente in einem Wörterbuch wird das Format `{displayKey:keyPath, ...}` verwendet, um nach dem `keyPath`-JMESPath-Ausdruck zu filtern. Dies wird in der Ausgabe als `{displayKey: value}` angezeigt. Das nächste Beispiel baut auf der Abfrage des letzten Beispiels auf und weist der Ausgabe Schlüssel zu, um sie deutlicher zu machen:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

Beim Anzeigen von Informationen im Ausgabeformat `table` ist die Wörterbuchanzeige besonders hilfreich. Hierbei können eigene Spaltenüberschriften festgelegt werden, um die Lesbarkeit der Ausgabe weiter zu verbessern. Weitere Informationen zu Ausgabeformaten finden Sie unter [Ausgabeformate für Azure CLI 2.0-Befehle](/cli/azure/format-output-azure-cli).

> [!NOTE]
> Bestimmte Schlüssel werden herausgefiltert und nicht in der Tabellenansicht gedruckt. Diese Schlüssel sind `id`, `type` und `etag`. Wenn Sie diese Informationen benötigen, können Sie den Schlüsselnamen ändern und so die Filterung umgehen.
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a>Verwenden von Listenausgaben

CLI-Befehle, die mehrere Werte zurückgeben können, geben immer ein Array zurück. Auf die Elemente eines Arrays kann über einen Index zugegriffen werden, es gibt jedoch niemals eine Reihenfolgengarantie von der Befehlszeilenschnittstelle. Beim Abfragen eines Arrays von Werten empfiehlt es sich, die Werte mit dem Operator `[]` zu vereinfachen. Der Operator wird nach dem Schlüssel für das Array oder als erstes Element im Ausdruck geschrieben. Durch die Vereinfachung wird die darauf folgende Abfrage für jedes einzelne Element im Array ausgeführt, und die resultierenden Werte werden in einem neuen Array platziert. Im folgenden Beispiel werden jeweils der Name und das Betriebssystem der virtuellen Computer in einer Ressourcengruppe ausgegeben. 

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

Auch Arrays, die einem Schlüsselpfad angehören, können vereinfacht werden. Dieses Beispiel zeigt eine Abfrage, die die Azure-Objekt-IDs für die NICs abruft, mit denen ein virtueller Computer verbunden ist.

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

Beim Experimentieren mit JMESPath-Ausdrücken empfiehlt sich eine Arbeitsweise, bei der Sie Abfragen schnell bearbeiten und die Ausgabe untersuchen können. Das Python-Paket [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) bietet eine interaktive Umgebung, in der Sie Daten mittels Piping als Eingabe verwenden und programminterne Abfragen schreiben können, um die Daten zu extrahieren.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```

---
title: Abfragen von Befehlsergebnissen mit der Azure CLI
description: Es wird beschrieben, wie Sie JMESPath-Abfragen für die Ausgabe von Azure CLI-Befehlen ausführen.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/12/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 1605b072a68d9aa781290fd862f1d67a847f571e
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593301"
---
# <a name="query-azure-cli-command-output"></a>Abfragen der Azure CLI-Befehlsausgabe

Die Azure CLI verwendet das Argument `--query`, um eine [JMESPath-Abfrage](http://jmespath.org) für die Ergebnisse von Befehlen auszuführen. JMESPath ist eine Abfragesprache für JSON, die es ermöglicht, Daten aus der CLI-Ausgabe auszuwählen und zu ändern. Abfragen werden für die JSON-Ausgabe ausgeführt, bevor irgendeine Anzeigeformatierung stattfindet.

Das Argument `--query` wird von allen Befehlen der Azure-Befehlszeilenschnittstelle unterstützt. In diesem Artikel wird anhand einer Reihe von kleinen, einfachen Beispielen beschrieben, wie die Features von JMESPath verwendet werden.

## <a name="dictionary-and-list-cli-results"></a>CLI-Ergebnisse im Wörterbuch- und Listenformat

Selbst wenn Sie ein anderes Ausgabeformat als JSON verwenden, werden die Ergebnisse von CLI-Befehlen für Abfragen zunächst als JSON-Ausgabe behandelt. CLI-Ergebnisse werden in Form eines JSON-Arrays oder -Wörterbuchs zurückgegeben. Arrays sind Sequenzen von Objekten, die indiziert werden können, und Wörterbücher sind unsortierte Objekte, auf die mit Schlüsseln zugegriffen wird. Befehle, die mehr als ein Objekt zurückgeben _können_, geben ein Array zurück, und Befehle, die _immer_ _nur_ ein einzelnes Objekt zurückgeben, geben ein Wörterbuch zurück.

## <a name="get-properties-in-a-dictionary"></a>Abrufen von Eigenschaften in einem Wörterbuch

Bei der Arbeit mit Ergebnissen im Wörterbuchformat können Sie auf Eigenschaften der obersten Ebene nur mit dem Schlüssel zugreifen. Das Zeichen `.` (__Teilausdruck__) wird verwendet, um auf Eigenschaften von geschachtelten Wörterbüchern zuzugreifen. Bevor wir uns mit Abfragen befassen, werfen wir einen Blick auf die unveränderte Ausgabe des Befehls `az vm show`:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM -o json
```

Der Befehl gibt ein Wörterbuch aus. Teile des Inhalts wurden hier weggelassen.

```json
{
  "additionalCapabilities": null,
  "availabilitySet": null,
  "diagnosticsProfile": {
    "bootDiagnostics": {
      "enabled": true,
      "storageUri": "https://xxxxxx.blob.core.windows.net/"
    }
  },
  ...
  "osProfile": {
    "adminPassword": null,
    "adminUsername": "azureuser",
    "allowExtensionOperations": true,
    "computerName": "TestVM",
    "customData": null,
    "linuxConfiguration": {
      "disablePasswordAuthentication": true,
      "provisionVmAgent": true,
      "ssh": {
        "publicKeys": [
          {
            "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
            "path": "/home/azureuser/.ssh/authorized_keys"
          }
        ]
      }
    },
    "secrets": [],
    "windowsConfiguration": null
  },
  ....
}
```

Der folgende Befehl ruft durch Hinzufügen einer Abfrage die öffentlichen SSH-Schlüssel ab, die zum Herstellen einer Verbindung mit der VM autorisiert sind:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys -o json
```

```json
[
  {
    "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
    "path": "/home/azureuser/.ssh/authorized_keys"
  }
]
```

Um mehrere Eigenschaften abzurufen, schließen Sie Ausdrücke als durch Trennzeichen getrennte Liste in eckige Klammern `[ ]` (eine __Mehrfachauswahlliste__) ein. Mit dem folgenden Befehl können Sie den Namen der VM, den Administrator und den SSH-Schlüssel gleichzeitig abrufen:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '[name, osProfile.adminUsername, osProfile.linuxConfiguration.ssh.publicKeys[0].keyData]' -o json
```

```json
[
  "TestVM",
  "azureuser",
  "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
]
```

Diese Werte werden im Ergebnisarray in der Reihenfolge aufgeführt, in der sie in der Abfrage übergeben wurden. Da das Ergebnis ein Array ist, sind keine Schlüssel mit den Ergebnissen verknüpft.

## <a name="rename-properties-in-a-query"></a>Umbenennen von Eigenschaften in einer Abfrage

Um beim Abfragen mehrerer Werte ein Wörterbuch anstelle eines Arrays abzurufen, verwenden Sie den Operator `{ }` (__Mehrfachauswahl-Hash__).
Das Format für einen Mehrfachauswahl-Hash ist `{displayName:JMESPathExpression, ...}`.
`displayName` ist die in der Ausgabe angezeigte Zeichenfolge, und `JMESPathExpression` ist der JMESPath-Ausdruck, der ausgewertet werden soll. Im Folgenden wird wieder das Beispiel aus dem letzten Abschnitt verwendet, aber die Mehrfachauswahlliste in einen Hash geändert:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKey:osProfile.linuxConfiguration.ssh.publicKeys[0].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "ssh-key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
}
```

## <a name="get-properties-in-an-array"></a>Abrufen von Eigenschaften in einem Array

Ein Array verfügt nicht über eigene Eigenschaften, kann aber indiziert werden. Dieses Feature wird im letzten Beispiel mit dem Ausdruck `publicKeys[0]` veranschaulicht, der das erste Element des `publicKeys`-Arrays abruft. Es gibt keine Garantie, dass die CLI-Ausgabe sortiert ist. Sie sollten daher die Indizierung nur dann verwenden, wenn Sie die Reihenfolge kennen oder das zurückgegebene Element für Sie nicht von Bedeutung ist. Um auf die Eigenschaften von Elementen in einem Array zuzugreifen, führen Sie einen von zwei Vorgängen aus: _Vereinfachen_ und _Filtern_. In diesem Abschnitt wird beschrieben, wie ein Array vereinfacht wird.

Zum Vereinfachen eines Arrays wird der JMESPath-Operator `[]` verwendet. Alle Ausdrücke nach dem `[]`-Operator werden auf jedes Element im aktuellen Array angewendet.
Wenn `[]` am Anfang der Abfrage steht, wird das Ergebnis des CLI-Befehls vereinfacht. Die Ergebnisse von `az vm list` können mit diesem Feature überprüft werden.
Mit der folgenden Abfrage werden der Name, das Betriebssystem und der Administratorname für jede VM in einer Ressourcengruppe abgerufen:

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, admin:osProfile.adminUsername}' -o json
```

```json
[
  {
    "Name": "Test-2",
    "OS": "Linux",
    "admin": "sttramer"
  },
  {
    "Name": "TestVM",
    "OS": "Linux",
    "admin": "azureuser"
  },
  {
    "Name": "WinTest",
    "OS": "Windows",
    "admin": "winadmin"
  }
]
```

Wird diese Abfrage mit dem Ausgabeformat `--output table` kombiniert, entsprechen die Spaltennamen dem `displayKey`-Wert des Mehrfachauswahl-Hashes:

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, Admin:osProfile.adminUsername}' --output table
```

```output
Name     OS       Admin
-------  -------  ---------
Test-2   Linux    sttramer
TestVM   Linux    azureuser
WinTest  Windows  winadmin
```

> [!NOTE]
>
> Bestimmte Schlüssel werden herausgefiltert und nicht in der Tabellenansicht gedruckt. Diese Schlüssel sind `id`, `type` und `etag`. Um diese Werte anzuzeigen, können Sie den Schlüsselnamen in einem Mehrfachauswahl-Hash ändern.
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

Jedes Array kann vereinfacht werden, nicht nur das vom Befehl zurückgegebene Ergebnis der obersten Ebene. Im letzten Abschnitt wurde der Ausdruck `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` verwendet, um den öffentlichen SSH-Schlüssel für die Anmeldung abzurufen. Zum Abrufen _aller_ öffentlichen SSH-Schlüssel könnte der Ausdruck stattdessen als `osProfile.linuxConfiguration.ssh.publicKeys[].keyData` geschrieben werden.
Dieser Abfrageausdruck vereinfacht das Array `osProfile.linuxConfiguration.ssh.publicKeys` und führt dann den Ausdruck `keyData` für jedes Element aus:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKeys:osProfile.linuxConfiguration.ssh.publicKeys[].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "sshKeys": [
    "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso\n"
  ]
}
```

## <a name="filter-arrays"></a>Filtern von Arrays

Der zweite Vorgang zum Abrufen von Daten aus einem Array ist das _Filtern_. Zum Filtern wird der JMESPath-Operator `[?...]` verwendet.
Dieser Operator akzeptiert ein Prädikat als Inhalt. Ein Prädikat ist eine beliebige Anweisung, die zu `true` oder `false` ausgewertet werden kann. Ausdrücke, bei denen das Prädikat zu `true` ausgewertet wird, sind in der Ausgabe enthalten.

JMESPath bietet die standardmäßigen Vergleichsoperatoren und logischen Operatoren. Dazu zählen `<`, `<=`, `>`, `>=`, `==` und `!=`. JMESPath unterstützt auch logisches AND (`&&`), OR (`||`) und NOT (`!`). Ausdrücke können zum Erstellen komplexerer Prädikatausdrücke in Klammern gruppiert werden. Ausführliche Informationen zu Prädikaten und logischen Vorgängen finden Sie in der [JMESPath-Spezifikation](http://jmespath.org/specification.html).

Im letzten Abschnitt haben wir ein Array vereinfacht, um die vollständige Liste aller VMs in einer Ressourcengruppe abzurufen. Mithilfe von Filtern kann diese Ausgabe auf Linux-VMs beschränkt werden:

```azurecli-interactive
az vm list -g QueryDemo --query "[?storageProfile.osDisk.osType=='Linux'].{Name:name,  admin:osProfile.adminUsername}" --output table
```

```output
Name    Admin
------  ---------
Test-2  sttramer
TestVM  azureuser
```

> [!IMPORTANT]
>
> In JMESPath werden Zeichenfolgen immer in einfache Anführungszeichen (`'`) gesetzt. Wenn Sie in einem Filterprädikat doppelte Anführungszeichen innerhalb einer Zeichenfolge verwenden, ist die Ausgabe leer.

JMESPath verfügt auch über integrierte Funktionen, die das Filtern erleichtern. Eine dieser Funktionen ist `contains(string, substring)`. Diese Funktion überprüft, ob eine Zeichenfolge eine Teilzeichenfolge enthält. Ausdrücke werden vor dem Aufrufen der Funktion ausgewertet. Das erste Argument kann daher ein vollständiger JMESPath-Ausdruck sein. Im nächsten Beispiel werden alle VMs mit SSD-Speicher für den Betriebssystemdatenträger abgerufen:

```azurecli-interactive
az vm list -g QueryDemo --query "[?contains(storageProfile.osDisk.managedDisk.storageAccountType,'SSD')].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

Diese Abfrage ist relativ lang. Der Schlüssel `storageProfile.osDisk.managedDisk.storageAccountType` wird zweimal erwähnt und in der Ausgabe neu erstellt. Eine Möglichkeit zum Kürzen der Abfrage besteht darin, den Filter nach dem Vereinfachen und Auswählen von Daten anzuwenden.

```azurecli-interactive
az vm list -g QueryDemo --query "[].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}[?contains(Storage,'SSD')]" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

Bei großen Arrays lässt sich der Vorgang möglicherweise beschleunigen, indem der Filter vor der Auswahl von Daten angewendet wird.

Die vollständige Liste der Funktionen finden Sie in der JMESPath-Spezifikation unter [Built-in Functions](http://jmespath.org/specification.html#built-in-functions) (Integrierte Funktionen).

## <a name="change-output"></a>Änder der Ausgabe

JMESPath-Funktionen haben zudem einen weiteren Zweck: das Bearbeiten bzw. Ändern der Ergebnisse einer Abfrage. Jede Funktion, die einen nicht booleschen Wert zurückgibt, ändert das Ergebnis eines Ausdrucks.
Mit `sort_by(array, &sort_expression)` können Sie Daten beispielsweise nach einem Eigenschaftswert sortieren. JMESPath verwendet einen speziellen Operator (`&`) für Ausdrücke, die später im Rahmen einer Funktion ausgewertet werden sollen. Das nächste Beispiel zeigt, wie Sie eine VM-Liste nach der Größe des Betriebssystemdatenträgers sortieren:

```azurecli-interactive
az vm list -g QueryDemo --query "sort_by([].{Name:name, Size:storageProfile.osDisk.diskSizeGb}, &Size)" --output table
```

```output
Name     Size
-------  ------
TestVM   30
Test-2   32
WinTest  127
```

Die vollständige Liste der Funktionen finden Sie in der JMESPath-Spezifikation unter [Built-in Functions](http://jmespath.org/specification.html#built-in-functions) (Integrierte Funktionen).

## <a name="experiment-with-queries-interactively"></a>Interaktives Experimentieren mit Abfragen

Für Ihre ersten Experimente mit JMESPath bietet das Python-Paket [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) eine interaktive Umgebung zur Verwendung von Abfragen. Daten werden als Eingabe übergeben, und anschließend werden Abfragen geschrieben und im Editor ausgeführt.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```

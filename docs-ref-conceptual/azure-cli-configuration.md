---
title: Konfigurationsoptionen für die Azure-Befehlszeilenschnittstelle
description: Informationen zum Konfigurieren der Azure CLI 2.0
keywords: Azure CLI, Azure-Befehlszeilenschnittstelle, Konfiguration, Einstellungen, Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: b0d26beac83a7ce3bba44d5e64d129a211c82836
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/18/2018
ms.locfileid: "34305875"
---
# <a name="azure-cli-20-configuration"></a>Konfiguration der Azure CLI 2.0

Die Azure CLI 2.0 ermöglicht die Überschreibung interner Einstellungen (etwa für die Protokollierung und die Datensammlung) durch eine Benutzerkonfiguration sowie die Bereitstellung von Standardoptionen für einige erforderliche Parameter. Die CLI bietet einen praktischen Befehl für die Verwaltung einiger dieser Werte (`az configure`). Andere können in einer Konfigurationsdatei oder mithilfe von Umgebungsvariablen festgelegt werden.

Von der CLI verwendete Konfigurationswerte werden in der folgenden Reihenfolge ausgewertet. Die Liste ist nach absteigender Priorität sortiert.

1. Befehlszeilenparameter
2. Umgebungsvariablen
3. In der Konfigurationsdatei enthaltene oder mit `az configure` festgelegte Werte

## <a name="cli-configuration-with-az-configure"></a>CLI-Konfiguration mit „az configure“

Standardwerte für die CLI werden mit dem Befehl [az configure](/cli/azure/reference-index#az-configure) festgelegt.
Dieser Befehl akzeptiert ein einzelnes Argument: `--defaults` (eine durch Leerzeichen getrennte Liste mit `key=value`-Paaren). Die angegebenen Werte werden von der CLI anstelle von erforderlichen Argumenten verwendet.

Folgende Schlüssel können verwendet werden:

| NAME | BESCHREIBUNG |
|------|-------------|
| group | Die Standardressourcengruppe für alle Befehle. |
| location | Der Standardstandort für alle Befehle. |
| Web- | Der Standard-App-Name für `az webapp`-Befehle. |
| vm | Der Standard-VM-Name für `az vm`-Befehle. |
| vmss | Der Standard-VMSS-Name für `az vmss`-Befehle. |
| acr | Der standardmäßige Containerregistrierungsname für `az acr`-Befehle. |
| acs | Der standardmäßige Containerdienstname für `az acs`-Befehle. |

Das folgende Beispiel zeigt, wie Sie die Standardressourcengruppe und den Standardstandort für alle Befehle festlegen.

```azurecli-interactive
az configure --defaults location=westus2 group=MyResourceGroup
```

## <a name="cli-configuration-file"></a>CLI-Konfigurationsdatei

Die CLI-Konfigurationsdatei enthält weitere Einstellungen für die Verwaltung des CLI-Verhaltens. Sie befindet sich unter `$AZURE_CONFIG_DIR/config`. `AZURE_CONFIG_DIR` hat standardmäßig den Wert `$HOME/.azure` (Linux und macOS) bzw. `%USERPROFILE%\.azure` (Windows).

Konfigurationsdateien sind im INI-Dateiformat geschrieben. Die einzelnen Abschnitte in den Dateien beginnen jeweils mit einem `[section-name]`-Header, gefolgt von einer Liste mit Einträgen vom Typ `key=value`. Bei Abschnittsnamen wird die Groß-/Kleinschreibung beachtet, bei Schlüsselnamen nicht.
Zeilen, die mit `#` oder `;` beginnen, sind Kommentare. Inlinekommentare sind nicht zulässig. Bei booleschen Werten wird die Groß-/Kleinschreibung nicht beachtet, und sie werden durch folgende Werte dargestellt:

* __True:__ 1, yes, true, on
* __False:__ 0, no, false, off

Das folgende Beispiel zeigt eine CLI-Konfigurationsdatei, die sämtliche Bestätigungsaufforderungen deaktiviert und eine Protokollierung im Verzeichnis `/var/log/azure` einrichtet.

```ini
[core]
disable_confirm_prompt=Yes

[logging]
enable_log_file=yes
log_dir=/var/log/azure
```

Ausführliche Informationen zu allen verfügbaren Konfigurationswerten und zu deren Bedeutung finden Sie im nächsten Abschnitt. Umfassende Details zum INI-Dateiformat finden Sie in der [Python-Dokumentation zu INI](https://docs.python.org/3/library/configparser.html#supported-ini-file-structure).

## <a name="cli-configuration-values-and-environment-variables"></a>CLI-Konfigurationswerte und Umgebungsvariablen

Die folgende Tabelle enthält sämtliche Abschnitte und Optionsnamen, die in einer Konfigurationsdatei verwendet werden können. Die entsprechenden Umgebungsvariablen können als `AZURE_{section}_{name}` (in Großbuchstaben) festgelegt werden. So können Sie beispielsweise den Standardwert für `storage_account` des Abschnitts `batchai` in der Variablen `AZURE_BATCHAI_STORAGE_ACCOUNT` festlegen.

Werte mit einem Standardwert müssen in Befehlszeilenargumenten nicht vorhanden sein, auch wenn sie erforderlich sind.

| Abschnitt | NAME      | Typ | BESCHREIBUNG|
|---------|-----------|------|------------|
| __core__ | output | Zeichenfolge | Das Standardausgabeformat. Mögliche Optionen: `json`, `jsonc`, `tsv` oder `table`. |
| | disable\_confirm\_prompt | boolean | Dient zum Aktivieren/Deaktivieren von Bestätigungsaufforderungen. |
| | collect\_telemetry | boolean | Erlaubt Microsoft das Sammeln anonymer Daten zur Verwendung der CLI. Informationen zum Datenschutz finden Sie in den [Nutzungsbedingungen für die Azure CLI 2.0](http://aka.ms/AzureCliLegal). |
| __logging__ | enable\_log\_file | boolean | Dient zum Aktivieren/Deaktivieren der Protokollierung. |
| | log\_dir | Zeichenfolge | Das Verzeichnis, in das Protokolle geschrieben werden sollen. Standardwert: `${AZURE_CONFIG_DIR}/logs` |
| __storage__ | connection\_string | Zeichenfolge | Die Standardverbindungszeichenfolge für `az storage`-Befehle. |
| | Konto | Zeichenfolge | Der Standardkontoname für `az storage`-Befehle. |
| | key | Zeichenfolge | Der Standardkontoschlüssel für `az storage`-Befehle. |
| | sas\_token | Zeichenfolge | Das Standard-SAS-Token für `az storage`-Befehle. |
| __batchai__ | storage\_account | Zeichenfolge | Das Standardspeicherkonto für `az batchai`-Befehle. |
| | storage\_key | Zeichenfolge | Der Standardspeicherschlüssel für `az batchai`-Befehle. |
| __batch__ | Konto | Zeichenfolge | Der Azure Batch-Standardkontoname für `az batch`-Befehle. |
| | access\_key | Zeichenfolge | Der Standardzugriffsschlüssel für `az batch`-Befehle. Wird nur für die `aad`-Autorisierung verwendet. |
| | endpoint | Zeichenfolge | Der Standardendpunkt für `az batch`-Befehle, mit dem eine Verbindung hergestellt werden soll. |
| | auth\_mode | Zeichenfolge | Der Autorisierungsmodus für `az batch`-Befehle. Kann `shared_key` oder `aad` sein. |

> [!NOTE]
> In Ihrer Konfigurationsdatei begegnen Ihnen möglicherweise noch andere Werte, diese werden jedoch direkt über CLI-Befehle verwaltet (einschließlich `az configure`). Abgesehen von den in der obigen Tabelle aufgeführten Werten sollten Sie keine anderen Werte selbst ändern.
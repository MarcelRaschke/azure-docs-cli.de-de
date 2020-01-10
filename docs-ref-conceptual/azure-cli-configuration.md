---
title: Konfigurationsoptionen für die Azure-Befehlszeilenschnittstelle
description: Konfigurieren der Azure CLI
keywords: Azure CLI, Azure-Befehlszeilenschnittstelle, Konfiguration, Einstellungen, Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/11/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 792a4bde1876bda620d31bccb7abcfc8e880332f
ms.sourcegitcommit: 503cf343422ab8d2a587d2ccb795953b8ad66376
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/31/2019
ms.locfileid: "75559993"
---
# <a name="azure-cli-configuration"></a>Azure CLI-Konfiguration

Die Azure CLI ermöglicht die Benutzerkonfiguration von Einstellungen, z.B. Protokollierung, Datensammlung und Standardargumentwerte.
Die CLI bietet einen praktischen Befehl für die Verwaltung einiger Standardwerte: `az configure`. Andere Werte können in einer Konfigurationsdatei oder mit Umgebungsvariablen festgelegt werden.

Von der CLI verwendete Konfigurationswerte werden in der folgenden Reihenfolge ausgewertet. Die Liste ist nach absteigender Priorität sortiert.

1. Befehlszeilenparameter
2. Umgebungsvariablen
3. In der Konfigurationsdatei enthaltene oder mit `az configure` festgelegte Werte

## <a name="cli-configuration-with-az-configure"></a>CLI-Konfiguration mit „az configure“

Standardwerte für die CLI werden mit dem Befehl [az configure](/cli/azure/reference-index#az-configure) festgelegt.
Dieser Befehl akzeptiert ein einzelnes Argument: `--defaults` (eine durch Leerzeichen getrennte Liste mit `key=value`-Paaren). Die angegebenen Werte werden von der CLI anstelle von erforderlichen Argumenten verwendet.

Die folgende Tabelle enthält eine Liste der verfügbaren Konfigurationsschlüssel.

| Name | BESCHREIBUNG |
|------|-------------|
| group | Die Standardressourcengruppe für alle Befehle. |
| location | Der Standardstandort für alle Befehle. |
| Web- | Der Standard-App-Name für `az webapp`-Befehle. |
| vm | Der Standard-VM-Name für `az vm`-Befehle. |
| vmss | Der Standardname einer VM-Skalierungsgruppe (VMSS), der für `az vmss`-Befehle verwendet wird |
| acr | Der standardmäßige Containerregistrierungsname für `az acr`-Befehle. |

Das folgende Beispiel zeigt, wie Sie die Standardressourcengruppe und den Standardstandort für alle Befehle festlegen.

```azurecli-interactive
az configure --defaults location=westus2 group=MyResourceGroup
```

## <a name="cli-configuration-file"></a>CLI-Konfigurationsdatei

Die CLI-Konfigurationsdatei enthält weitere Einstellungen für die Verwaltung des CLI-Verhaltens. Sie befindet sich unter `$AZURE_CONFIG_DIR/config`. `AZURE_CONFIG_DIR` hat standardmäßig den Wert `$HOME/.azure` (Linux und macOS) bzw. `%USERPROFILE%\.azure` (Windows).

Konfigurationsdateien sind im INI-Dateiformat geschrieben. Dieses Dateiformat wird durch Abschnittsheader gefolgt von einer Liste von Schlüssel-Wert-Einträgen definiert.

* Abschnittsheader werden als `[section-name]` geschrieben. Bei Abschnittsnamen wird zwischen Groß- und Kleinschreibung unterschieden.
* Einträge werden als `key=value` geschrieben. Bei Schlüsselnamen wird nicht zwischen Groß- und Kleinschreibung unterschieden.
* Zeilen, die mit `#` oder `;` beginnen, sind Kommentare. Inlinekommentare sind nicht zulässig.

Bei booleschen Werten wird die Groß-/Kleinschreibung nicht beachtet, und sie werden durch folgende Werte dargestellt:

* __True__: 1, yes, true, on
* __False__: 0, no, false, off

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

Die folgende Tabelle enthält sämtliche Abschnitte und Optionsnamen, die in einer Konfigurationsdatei verwendet werden können. Die entsprechenden Umgebungsvariablen werden als `AZURE_{section}_{name}` (in Großbuchstaben) festgelegt. Der `storage_account`-Standardwert für `batchai` wird beispielsweise in der Variablen `AZURE_BATCHAI_STORAGE_ACCOUNT` festgelegt.

Wenn Sie einen Standardwert angeben, wird dieses Argument von keinem Befehl mehr benötigt. Stattdessen wird der Standardwert verwendet.

| `Section` | Name      | type | BESCHREIBUNG|
|---------|-----------|------|------------|
| __core__ | output | string | Das Standardausgabeformat. Mögliche Optionen: `json`, `jsonc`, `tsv` oder `table`. |
| | disable\_confirm\_prompt | boolean | Dient zum Aktivieren/Deaktivieren von Bestätigungsaufforderungen. |
| | collect\_telemetry | boolean | Erlaubt Microsoft das Sammeln anonymer Daten zur Verwendung der CLI. Informationen zum Datenschutz finden Sie in den [Nutzungsbedingungen für die Azure CLI](http://aka.ms/AzureCliLegal). |
| __logging__ | enable\_log\_file | boolean | Dient zum Aktivieren/Deaktivieren der Protokollierung. |
| | log\_dir | string | Das Verzeichnis, in das Protokolle geschrieben werden sollen. Standardmäßig ist dieser Wert auf `${AZURE_CONFIG_DIR}/logs` festgelegt. |
| __storage__ | connection\_string | string | Die Standardverbindungszeichenfolge für `az storage`-Befehle. |
| | account | string | Der Standardkontoname für `az storage`-Befehle. |
| | Schlüssel | string | Der Standardkontoschlüssel für `az storage`-Befehle. |
| | sas\_token | string | Das Standard-SAS-Token für `az storage`-Befehle. |
| __batchai__ | storage\_account | string | Das Standardspeicherkonto für `az batchai`-Befehle. |
| | storage\_key | string | Der Standardspeicherschlüssel für `az batchai`-Befehle. |
| __batch__ | account | string | Der Azure Batch-Standardkontoname für `az batch`-Befehle. |
| | access\_key | string | Der Standardzugriffsschlüssel für `az batch`-Befehle. Wird nur für die `aad`-Autorisierung verwendet. |
| | endpoint | string | Der Standardendpunkt für `az batch`-Befehle, mit dem eine Verbindung hergestellt werden soll. |
| | auth\_mode | string | Der Autorisierungsmodus für `az batch`-Befehle. Kann `shared_key` oder `aad` sein. |
| __cloud__ | name | string | Die Standardcloud für alle `az`-Befehle.  Die möglichen Werte sind `AzureCloud` (Standard) oder `AzureChinaCloud`, `AzureUSGovernment`, `AzureGermanCloud`. Zum Ändern von Clouds können Sie den Befehl `az cloud set –name` verwenden.  Ein Beispiel finden Sie unter [Verwalten von Clouds mit der Azure CLI](manage-clouds-azure-cli.md). |

> [!NOTE]
> In Ihrer Konfigurationsdatei begegnen Ihnen möglicherweise noch andere Werte, diese werden jedoch direkt über CLI-Befehle verwaltet (einschließlich `az configure`). Abgesehen von den in der obigen Tabelle aufgeführten Werten sollten Sie keine anderen Werte selbst ändern.

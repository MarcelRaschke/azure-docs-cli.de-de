---
title: Azure CLI 2.0-Erweiterungen
description: Verwenden von Erweiterungen mit Azure CLI 2.0
keywords: Azure CLI, Erweiterungen
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: b503c51ffc55ceda30738e34171c7da92532f328
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967723"
---
# <a name="using-extensions-with-the-azure-cli-20"></a>Verwenden von Erweiterungen mit Azure CLI 2.0

Erweiterungen sind einzelne Module, die nicht mit der Azure CLI bereitgestellt werden und Funktionen über neue Befehle hinzufügen. Dies können experimentelle Angebote oder Vorabangebote, spezielle Tools von Microsoft oder von Ihnen selbst geschriebene benutzerdefinierte Features sein. Erweiterungen ermöglichen das flexible Anpassen der CLI an Ihre eigenen Anforderungen, ohne dass Sie viele zusätzliche Pakete mitliefern müssen, die nicht als Teil des Kernfeaturesatzes angesehen werden.

In diesem Artikel wird beschrieben, wie Sie Erweiterungen für die CLI installieren, aktualisieren und entfernen. Außerdem werden häufige Fragen zum Verhalten von Erweiterungen beantwortet.

## <a name="find-extensions"></a>Suchen von Erweiterungen

Um zu ermitteln, welche Erweiterungen verfügbar sind, können Sie [az extension list-available](/cli/azure/extension#az-extension-list-available) verwenden. Mit diesem Befehl werden die offiziellen Erweiterungen aufgeführt, die von Microsoft bereitgestellt und verwaltet werden.

```azurecli-interactive
az extension list-available --output table
```

Auf der Dokumentationswebsite wird darüber hinaus eine [Liste der Microsoft-Erweiterungen](azure-cli-extensions-list.md) bereitgestellt.

## <a name="install-extensions"></a>Installieren von Erweiterungen

Nachdem Sie eine zu installierende Erweiterung gefunden haben, können Sie [az extension add](https://docs.microsoft.com/cli/azure/extension#az-extension-add) verwenden, um sie abzurufen. Wenn die Erweiterung in `az extension list-available` aufgeführt wird, können Sie die Erweiterung anhand des Namens installieren.

```azurecli-interactive
az extension add --name <extension-name>
```

Wenn die Erweiterung von einer externen Ressource stammt oder Sie über einen direkten Link dafür verfügen, können Sie die Quell-URL oder den lokalen Pfad angeben. Dies _muss_ eine kompilierte Python-Wheeldatei sein.

```azurecli-interactive
az extension add --source <URL-or-path>
```

Nach der Installation einer Erweiterung befindet sich diese unter dem Wert der Shellvariablen `$AZURE_EXTENSION_DIR`. Wenn diese Variable nicht festgelegt ist, befindet sich der Wert standardmäßig unter `$HOME/.azure/cliextensions` (Linux und macOS) bzw. `%USERPROFILE%\.azure\cliextensions` (Windows).

## <a name="update-extensions"></a>Aktualisieren von Erweiterungen

Wenn eine Erweiterung anhand des Namens installiert wurde, kann sie mithilfe von [az extension update](https://docs.microsoft.com/cli/azure/extension#az-extension-update) aktualisiert werden.

```azurecli-interactive
az extension update --name <extension-name>
```

Andernfalls kann eine Erweiterung anhand der Quelle gemäß den Anweisungen unter [Installieren von Erweiterungen](#install-extensions) aktualisiert werden.

Falls der Name einer Erweiterung von der CLI nicht aufgelöst werden kann, deinstallieren Sie die Erweiterung, und installieren Sie sie anschließend erneut. Außerdem ist es möglich, dass die Erweiterung nicht mehr als Vorschauversion verfügbar und zu einem integrierten Befehl für die CLI geworden ist. Versuchen Sie, die CLI wie unter [Installieren von Azure CLI 2.0](install-azure-cli.md) beschrieben zu installieren, und überprüfen Sie, ob die Befehle der Erweiterung hinzugefügt wurden.

## <a name="uninstall-extensions"></a>Deinstallieren von Erweiterungen

Wenn Sie eine Erweiterung nicht mehr benötigen, können Sie sie mit [az extension remove](https://docs.microsoft.com/cli/azure/extension#az-extension-remove) entfernen.

```azurecli-interactive
az extension remove --name <extension-name>
```

Sie können eine Erweiterung auch manuell entfernen, indem Sie sie am Installationsspeicherort löschen. Dies ist der Wert der Shellvariablen `$AZURE_EXTENSION_DIR`.
Wenn diese Variable nicht festgelegt ist, befindet sich der Wert standardmäßig unter `$HOME/.azure/cliextensions` (Linux und macOS) bzw. `%USERPROFILE%\.azure\cliextensions` (Windows).

```bash
rm -rf $AZURE_EXTENSION_DIR/<extension-name>
```

Es wird empfohlen, die Deinstallation mit `az extension remove` durchzuführen.

## <a name="faq"></a>Häufig gestellte Fragen

Hier sind einige Antworten auf andere häufig gestellte Fragen zu CLI-Erweiterungen aufgeführt.

### <a name="what-file-formats-are-allowed-for-installation"></a>Welche Dateiformate sind für die Installation zulässig?

Derzeit können nur kompilierte Python-Wheels als Erweiterungen installiert werden.

### <a name="can-extensions-replace-existing-commands"></a>Können Erweiterungen vorhandene Befehle ersetzen?

Ja. Erweiterungen können vorhandene Befehle ersetzen, aber vor dem Ausführen eines ersetzten Befehls wird von der CLI eine Warnung ausgegeben.

### <a name="how-can-i-tell-if-an-extension-is-in-pre-release"></a>Woran erkenne ich, dass es sich bei einer Erweiterung um eine Vorabversion handelt?

Für eine Erweiterung sollte in der dazugehörigen Dokumentation und in den Versionsinformationen angegeben sein, wenn es sich um eine Vorabversion handelt. Es kommt auch häufiger vor, dass Microsoft Vorschauversionen von Befehlen für die CLI als Erweiterungen veröffentlicht, die nach der Vorschauphase des Produkts in die Hauptoberfläche der CLI integriert werden sollen.

### <a name="can-extensions-depend-upon-each-other"></a>Können Erweiterungen voneinander abhängig sein?

Nein. Erweiterungen müssen einzelne Pakete sein, die nicht voneinander abhängig sind. Dies liegt daran, dass für die CLI nicht garantiert ist, wann Erweiterungen geladen werden. Es kann also nicht sichergestellt werden, dass die Anforderungen von Abhängigkeiten erfüllt werden. Bei der Installation einer Erweiterung wird nur die jeweilige Erweiterung installiert, und sie sollte auch dann funktionieren, wenn Sie andere Erweiterungen entfernen.

### <a name="are-extensions-updated-along-with-the-cli"></a>Werden Erweiterungen zusammen mit der CLI aktualisiert?

Nein. Erweiterungen müssen separat aktualisiert werden, wie unter [Aktualisieren von Erweiterungen](#update-extensions) beschrieben.

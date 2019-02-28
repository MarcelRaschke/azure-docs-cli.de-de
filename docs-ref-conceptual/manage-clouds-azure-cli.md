---
title: Auswählen von Clouds mit der Azure CLI
description: Die Azure CLI ermöglicht die Erstellung, Anmeldung und Verwaltung von bzw. bei mehreren Clouds.
author: sptramer
manager: carmonm
ms.author: sttramer
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 14f51e068c4d2b332b0de93406822e148d734701
ms.sourcegitcommit: 032f35d553754fbac78b218259a8d6a697ac220e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "56458687"
---
# <a name="select-clouds-with-the-azure-cli"></a>Auswählen von Clouds mit der Azure CLI

Wenn Sie regionsübergreifend arbeiten oder [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/) verwenden, müssen Sie möglicherweise mehrere Clouds verwenden. Hierzu stellt Ihnen Microsoft Clouds zur Verfügung, die mit regionalen Gesetzen in Einklang stehen. In diesem Artikel erfahren Sie, wie Sie Informationen zu Clouds abrufen, wie Sie die aktuelle Cloud ändern und wie Sie neue Clouds registrieren bzw. ihre Registrierung aufheben.

## <a name="list-available-clouds"></a>Auflisten verfügbarer Clouds

Die verfügbaren Clouds können mit dem Befehl [az cloud list](/cli/azure/cloud#az-cloud-list) aufgelistet werden. Mit diesem Befehl erfahren Sie, welche Cloud derzeit aktiv ist, und erhalten Informationen zum aktuellen Profil, zu regionalen Suffixen und zu Hostnamen.

Gehen Sie wie folgt vor, um die aktive Cloud und eine Liste mit allen verfügbaren Clouds abzurufen:

```azurecli-interactive
az cloud list --output table
```

```output
IsActive    Name               Profile
----------  -----------------  ---------
True        AzureCloud         latest
            AzureChinaCloud    latest
            AzureUSGovernment  latest
            AzureGermanCloud   latest
```

Für die derzeit aktive Cloud ist in der Spalte `IsActive` der Wert `True` angegeben. Es kann immer nur eine Cloud aktiv sein. Ausführlichere Informationen zu einer Cloud (einschließlich der Endpunkte, die sie für Azure-Dienste verwendet) erhalten Sie mit dem Befehl `cloud show`:

```azurecli-interactive
az cloud show --name AzureChinaCloud --output json
```

```json
{
  "endpoints": {
    "activeDirectory": "https://login.chinacloudapi.cn",
    "activeDirectoryDataLakeResourceId": null,
    "activeDirectoryGraphResourceId": "https://graph.chinacloudapi.cn/",
    "activeDirectoryResourceId": "https://management.core.chinacloudapi.cn/",
    "batchResourceId": "https://batch.chinacloudapi.cn/",
    "gallery": "https://gallery.chinacloudapi.cn/",
    "management": "https://management.core.chinacloudapi.cn/",
    "resourceManager": "https://management.chinacloudapi.cn",
    "sqlManagement": "https://management.core.chinacloudapi.cn:8443/",
    "vmImageAliasDoc": "https://raw.githubusercontent.com/Azure/azure-rest-api-specs/master/arm-compute/quickstart-templates/aliases.json"
  },
  "isActive": false,
  "name": "AzureChinaCloud",
  "profile": "latest",
  "suffixes": {
    "azureDatalakeAnalyticsCatalogAndJobEndpoint": null,
    "azureDatalakeStoreFileSystemEndpoint": null,
    "keyvaultDns": ".vault.azure.cn",
    "sqlServerHostname": ".database.chinacloudapi.cn",
    "storageEndpoint": "core.chinacloudapi.cn"
  }
}
```

## <a name="switch-the-active-cloud"></a>Wechseln der aktiven Cloud

Führen Sie zum Wechseln der aktiven Cloud den Befehl [az cloud set](/cli/azure/cloud#az-cloud-set) aus. Dieser Befehl erfordert ein Argument: den Namen der Cloud.

```azurecli-interactive
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> Sollte die Authentifizierung für die aktivierte Cloud abgelaufen sein, müssen Sie sich erneut authentifizieren, bevor Sie weitere CLI-Aufgaben ausführen. Beim erstmaligen Wechsel zu der neuen Cloud muss auch das aktive Abonnement festgelegt werden.
> Eine Anleitung zur Authentifizierung finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md). Weitere Informationen zur Abonnementverwaltung finden Sie unter [Verwalten von Azure-Abonnements mit der Azure CLI](manage-azure-subscriptions-azure-cli.md).

## <a name="register-a-new-cloud"></a>Registrieren einer neuen Cloud

Registrieren Sie eine neue Cloud, wenn Sie über eigene Endpunkte für Azure Stack verfügen. Eine Cloud wird mit dem Befehl [az cloud register](/cli/azure/cloud#az-cloud-register) erstellt. Dieser Befehl erfordert einen Namen und eine Reihe von Dienstendpunkten. Informationen zum Registrieren einer Cloud für die Verwendung mit Azure Stack finden Sie unter [Verwenden von API-Versionsprofilen mit der Azure CLI in Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).

Für China, US Government oder deutsche Regionen müssen Sie keine Informationen registrieren. Diese Clouds werden von Microsoft verwaltet und sind standardmäßig verfügbar.  Weitere Informationen zu allen verfügbaren Endpunkteinstellungen finden Sie in der [Dokumentation für `az cloud register`](/cli/azure/cloud#az-cloud-register).

Durch Registrieren einer Cloud wird nicht automatisch zu dieser Cloud gewechselt. Wählen Sie die neu erstellte Cloud mithilfe des Befehls `az cloud set` aus.

## <a name="update-an-existing-cloud"></a>Aktualisieren einer vorhandenen Cloud

Sie können auch eine vorhandene Cloud aktualisieren, sofern Sie über die erforderlichen Berechtigungen verfügen. Bei der Aktualisierung einer Cloud wird zu einem anderen Azure-Dienstprofil gewechselt, oder die Verbindungsendpunkte werden geändert.
Aktualisieren Sie eine Cloud mit dem Befehl [az cloud update](/cli/azure/cloud#az-cloud-update). Dieser akzeptiert die gleichen Argumente wie `az cloud register`.

## <a name="unregister-a-cloud"></a>Aufheben der Registrierung einer Cloud

Wenn Sie eine erstellte Cloud nicht mehr benötigen, kann ihre Registrierung mit dem Befehl [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) aufgehoben werden:

```azurecli-interactive
az cloud unregister --name MyCloud
```

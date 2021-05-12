---
title: Breaking Change in der Azure CLI-Betaversion
description: Migrieren von „accessTokens.json“ zur Azure Identity und MSAL
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 04/19/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: d8836f6532e37602e8663b0125451deaef994fee
ms.sourcegitcommit: ced987fe078a63b4bbc8dba1295381e9d0a0ce91
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/20/2021
ms.locfileid: "107795217"
---
# <a name="migrate-to-azure-identity"></a>Migrieren zur Azure-Identität

Bei der Azure CLI-Betaversion wird [ADAL](https://github.com/AzureAD/azure-activedirectory-library-for-python) intern durch [Azure Identity](https://github.com/Azure/azure-sdk-for-python/tree/master/sdk/identity/azure-identity) und [MSAL](https://github.com/AzureAD/microsoft-authentication-library-for-python) ersetzt. Vorhandener ADAL-Tokencache (`~/.azure/accessToken.json`) wird automatisch zu MSAL-verschlüsseltem Tokencache migriert, wenn ein Befehl ausgeführt wird, der Anmeldeinformationen erfordert.

Dieser Artikel enthält Details zu diesem Breaking Change und Beispiele zum Abrufen eines Zugriffstokens in der Azure CLI-Betaversion.

## <a name="beta-release-breaking-change"></a>Breaking Change im Betarelease

Die aktuelle Azure CLI speichert die ADAL-Aktualisierungstoken und -Zugriffstoken in `~/.azure/accessToken.json`. Die Betaversion der Azure CLI verwendet MSAL und generiert `accessTokens.json` nach der erfolgreichen Anmeldung nicht mehr.  Die Token werden im freigegebenen Tokencache von MSAL namens `msal.cache` gespeichert.  Verwenden Sie stattdessen`az account get-access-token`, um ein Zugriffstoken abzurufen. 

Der MSAL-Tokencache wird unter Windows, macOS und Linux mit einer Desktopumgebung verschlüsselt. Daher gibt es keinen direkten Zugriff auf den MSAL-Tokencache. Jeder vorhandene Workflow, der von `accessTokens.json` abhängt, funktioniert nicht mehr.

## <a name="alternatives-to-consider"></a>Zu berücksichtigende Alternativen

##### <a name="call-az-account-get-access-token"></a>Rufen Sie `az account get-access-token` auf.

Sie können [az account get-access-token](/cli/azure/account#az_account_get_access_token) in einem Terminal manuell aufrufen oder einen Teilprozess nutzen, um den Befehl über eine anderen Programmiersprache aufzurufen. Standardmäßig gilt das zurückgegebene Token für das Standardabonnement bzw. den Standardmandanten, das bzw. der mit [az account show](/cli/azure/account#az_account_show) angezeigt wird.

```azurecli
# get the active subscription
az account show --output table

# get access token for the default subscription
az account get-access-token

# get access toekn for a specific subscription
az account get-access-token --subscription "mySubscriptionName"
```

##### <a name="use-azureclicredential"></a>Verwenden Sie `AzureCliCredential`

Bei `AzureCliCredential` handelt es sich um einen Anmeldeinformationstyp in allen vorhandenen Programmiersprachen-SDKs. Intern wird ein Teilprozess zum Aufrufen von `az account get-access-token` verwendet, um ein Zugriffstoken von den aktuell angemeldeten CLI-Konten abzurufen. 

##### <a name="access-shared-msal-cache"></a>Zugreifen auf den freigegebenen MSAL-Cache

Erstanbieter-Apps können mit `SharedTokenCacheCredential` aus dem Azure Identity-SDK direkt auf den freigegebenen MSAL-Cache zugreifen.

## <a name="see-also"></a>Siehe auch
* Versionshinweise für die [Azure CLI-Betaversion](/cli/azure/release-notes-azure-cli?toc=%2Fcli%2Fazure%2Ftoc.json&bc=%2Fcli%2Fazure%2Fbreadcrumb%2Ftoc.json&tabs=azure-cli-beta)
* [Installieren der Azure CLI-Betaversion](/cli/azure/install-azure-cli-beta)
* [AzureCliCredential-Klasse](/dotnet/api/azure.identity.azureclicredential?view=azure-dotnet&preserve-view=true) in .NET
* [AzureCliCredential-Klasse](/python/api/azure-identity/azure.identity.azureclicredential?view=azure-python&preserve-view=true) in Java
* [AzureCliCredential-Klasse](/python/api/azure-identity/azure.identity.azureclicredential?view=azure-python&preserve-view=true) in Python
* [SharedTokenCacheCredential-Klasse](/dotnet/api/azure.identity.sharedtokencachecredential?view=azure-dotnet&preserve-view=true) in .NET
* [SharedTokenCacheCredential-Klasse](/java/api/com.azure.identity.sharedtokencachecredential?view=azure-java-stable&preserve-view=true) in Java
* [SharedTokenCacheCredential-Klasse](/python/api/azure-identity/azure.identity.sharedtokencachecredential?view=azure-python&preserve-view=true) in Python

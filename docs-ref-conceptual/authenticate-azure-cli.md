---
title: Anmelden mit Azure CLI 2.0
description: Melden Sie sich mit der Azure CLI 2.0 interaktiv oder mit lokalen Anmeldeinformationen an.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.service: active-directory
ms.component: authentication
ms.openlocfilehash: f6f3e8bc015420795dda48da093bc92bbf246529
ms.sourcegitcommit: 8e6e3129f8f4824a8acfa12edb5dae52466d4be8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2018
ms.locfileid: "45626923"
---
# <a name="sign-in-with-azure-cli-20"></a>Anmelden mit Azure CLI 2.0

Es gibt mehrere Authentifizierungstypen für die Azure CLI. Den einfachsten Einstieg ermöglicht der [Azure Cloud Shell](/azure/cloud-shell/overview)-Dienst, der Sie automatisch anmeldet. Lokal können Sie sich interaktiv über Ihren Browser mit dem Befehl `az login` anmelden. Beim Schreiben von Skripts wird die Verwendung von Dienstprinzipalen empfohlen. Indem Sie einem Dienstprinzipal nur die erforderlichen Mindestberechtigungen erteilen, können Sie Ihre Automatisierung schützen.

Ihre Anmeldeinformationen werden nicht von der CLI gespeichert. Stattdessen wird von Azure ein [Authentifizierungsaktualisierungstoken](https://docs.microsoft.com/en-us/azure/active-directory/develop/v1-id-and-access-tokens#refresh-tokens) generiert und gespeichert. Ab August 2018 wird dieses Token nach 90-tägiger Inaktivität widerrufen. Dieser Wert kann jedoch von Microsoft oder von Ihrem Mandantenadministrator geändert werden. Wenn das Token widerrufen wurde, werden Sie von der Befehlszeilenschnittstelle aufgefordert, sich erneut anzumelden.

Nach der Anmeldung werden CLI-Befehle für Ihr Standardabonnement ausgeführt. Sollten Sie über mehrere Abonnements verfügen, können Sie das [Standardabonnement ändern](manage-azure-subscriptions-azure-cli.md).

## <a name="sign-in-interactively"></a>Interaktives Anmelden

Die Standardauthentifizierungsmethode der Azure CLI ist die Anmeldung über einen Webbrowser mit Zugriffstoken.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="sign-in-with-credentials-on-the-command-line"></a>Anmelden mit Anmeldeinformationen über die Befehlszeile

Geben Sie Ihre Azure-Benutzeranmeldeinformationen in der Befehlszeile an.

> [!Note]
> Dieser Ansatz funktioniert nicht für Microsoft-Konten oder Konten, für die die Authentifizierung in zwei Schritten aktiviert ist.

```azurecli
az login -u <username> -p <password>
```

> [!IMPORTANT]
> Wenn Sie die Anzeige Ihres Kennworts in der Konsole vermeiden möchten und `az login` interaktiv verwenden, können Sie den Befehl `read -s` unter `bash` nutzen.
>
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login -u <username> -p $AZ_PASS
> ```
>
> Verwenden Sie unter PowerShell das `Read-Host -AsSecureString`-Cmdlet und die Konvertierung in sichere Zeichenfolgen.
>
> ```powershell
> $securePass =  Read-Host "Azure password: " -AsSecureString;
> $AzPass = [Runtime.InteropServices.Marshal]::PtrToStringAuto([Runtime.InteropServices.Marshal]::SecureStringToBSTR($securePass));
> az login -u <username> -p $AzPass;
> $AzPass = ""
> ```

## <a name="sign-in-with-a-specific-tenant"></a>Anmelden mit einem bestimmten Mandanten

Sie können mit dem Argument `--tenant` einen Mandanten auswählen, unter dem Sie sich anmelden möchten. Der Wert dieses Arguments kann eine Domäne vom Typ `.onmicrosoft.com` oder die Azure-Objekt-ID für den Mandanten sein. Mit `--tenant` können sowohl interaktive Methoden als auch die Befehlszeile für die Anmeldung verwendet werden.

```azurecli
az login --tenant <tenant>
```

## <a name="sign-in-with-a-service-principal"></a>Anmelden mit einem Dienstprinzipal

Dienstprinzipale sind Konten, die nicht an einen bestimmten Benutzer gebunden sind und über Berechtigungen verfügen können, die ihnen über vordefinierte Rollen zugewiesen werden. Die Authentifizierung mit einem Dienstprinzipal ist die beste Methode zum Schreiben sicherer Skripts oder Programme und ermöglicht das Anwenden von Berechtigungseinschränkungen und lokal gespeicherten statischen Anmeldeinformationen. Weitere Informationen zu Dienstprinzipalen finden Sie unter [Erstellen eines Azure-Dienstprinzipals mit Azure CLI 2.0](create-an-azure-service-principal-azure-cli.md).

Für die Anmeldung mit einem Dienstprinzipal benötigen Sie Folgendes:

* Die dem Dienstprinzipal zugeordnete URL bzw. den zugeordneten Namen
* Das Dienstprinzipalkennwort oder das X509-Zertifikat (im PEM-Format), das zum Erstellen des Dienstprinzipals verwendet wurde
* Den dem Dienstprinzipal zugeordneten Mandanten, als `.onmicrosoft.com`-Domäne oder Azure-Objekt-ID

```azurecli
az login --service-principal -u <app-url> -p <password-or-cert> --tenant <tenant>
```

> [!IMPORTANT]
> Wenn Sie die Anzeige Ihres Kennworts in der Konsole vermeiden möchten und `az login` interaktiv verwenden, können Sie den Befehl `read -s` unter `bash` nutzen.
>
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login --service-principal -u <app-url> -p $AZ_PASS --tenant <tenant>
> ```
>
> Verwenden Sie unter PowerShell das `Read-Host -AsSecureString`-Cmdlet und die Konvertierung in sichere Zeichenfolgen.
>
> ```powershell
> $securePass =  Read-Host "Azure password: " -AsSecureString;
> $AzPass = [Runtime.InteropServices.Marshal]::PtrToStringAuto([Runtime.InteropServices.Marshal]::SecureStringToBSTR($securePass));
> az login --service-principal -u <app-url> -p $AzPass --tenant <tenant>;
> $AzPass = ""
> ```

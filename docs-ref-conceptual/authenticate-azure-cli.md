---
title: Anmelden mit Azure CLI 2.0
description: Melden Sie sich mit der Azure CLI 2.0 interaktiv oder mit lokalen Anmeldeinformationen an.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/09/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.service: active-directory
ms.component: authentication
ms.openlocfilehash: a0e05b3306cc273486b1b5fc887ceedbf78cb779
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967757"
---
# <a name="sign-in-with-azure-cli-20"></a>Anmelden mit Azure CLI 2.0

Es gibt mehrere Möglichkeiten, sich bei der Azure-CLI zu authentifizieren. Melden Sie sich am besten interaktiv per Browser über Azure Cloud Shell oder den Befehl `az login` an.
Es wird empfohlen, Dienstprinzipale zu verwenden. Dabei handelt es sich um Konten mit eingeschränkten Berechtigungen. Indem Sie einem Dienstprinzipal nur die erforderlichen Mindestberechtigungen erteilen, können Sie Ihre Automatisierungsskripts noch sicherer machen.

Die privaten Anmeldeinformationen werden nicht lokal gespeichert. Stattdessen wird von Azure ein Authentifizierungstoken generiert und gespeichert. Nach der Anmeldung ist das Authentifizierungstoken gültig, bis es 14 Tage lang nicht verwendet wird. Dann müssen Sie sich erneut authentifizieren.

Nach der Anmeldung werden CLI-Befehle für Ihr Standardabonnement ausgeführt. Sollten Sie über mehrere Abonnements verfügen, können Sie das [Standardabonnement ändern](manage-azure-subscriptions-azure-cli.md).

## <a name="interactive-sign-in"></a>Interaktive Anmeldung

Die Standardauthentifizierungsmethode der Azure CLI ist die Anmeldung über einen Webbrowser mit Zugriffstoken.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>Befehlszeile

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

Wenn Sie mehrere Mandanten verwenden, können Sie mit dem Argument `--tenant` den Mandanten auswählen, unter dem Sie sich anmelden. Der Wert dieses Arguments kann eine Domäne vom Typ `.onmicrosoft.com` oder die Azure-Objekt-ID für den Mandanten sein. Sie können sich interaktiv anmelden oder Ihre Anmeldeinformationen mit den Argumenten `--user` und `--password` angeben.

```azurecli
az login --tenant <tenant>
```

## <a name="sign-in-with-a-service-principal"></a>Anmelden mit einem Dienstprinzipal

Dienstprinzipale sind Konten, die nicht an einen bestimmten Benutzer gebunden sind und über Berechtigungen verfügen können, die ihnen über vordefinierte Rollen zugewiesen werden. Die Authentifizierung mit einem Dienstprinzipal ist die beste Methode zum Schreiben sicherer Skripts oder Programme und ermöglicht das Anwenden von Berechtigungseinschränkungen und lokal gespeicherten statischen Anmeldeinformationen. Weitere Informationen zu Dienstprinzipalen finden Sie unter [Erstellen eines Azure-Dienstprinzipals mit Azure CLI 2.0](create-an-azure-service-principal-azure-cli.md).

Für die Anmeldung mit einem Dienstprinzipal geben Sie den Benutzernamen, das Kennwort oder die PEM-Zertifikatdatei und den Mandanten an, der dem Dienstprinzipal zugeordnet ist:

```azurecli
az login --service-principal -u <app-url> -p <password-or-cert> --tenant <tenant>
```

Der Mandantenwert ist der dem Dienstprinzipal zugeordnete Azure Active Directory-Mandant. Hierbei kann es sich um eine Domäne vom Typ `.onmicrosoft.com` oder um die Azure-Objekt-ID für den Mandanten handeln.
Die Mandantenobjekt-ID für Ihr derzeit aktives Konto können Sie mithilfe des folgenden Befehls abrufen:

```azurecli-interactive
az account show --query 'tenantId' -o tsv
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

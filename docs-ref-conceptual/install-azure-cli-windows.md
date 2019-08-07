---
title: Installieren der Azure-Befehlszeilenschnittstelle für Windows
description: Installieren der Azure CLI unter Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/01/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 6c972ba69344f9e8bcd14a96a90e9dadb6cd8132
ms.sourcegitcommit: 61965f5d95d0dae3752ad6a0e5a93db27a623c28
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/06/2019
ms.locfileid: "68830972"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="d8523-103">Installieren der Azure CLI unter Windows</span><span class="sxs-lookup"><span data-stu-id="d8523-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="d8523-104">Unter Windows wird die Azure CLI über eine MSI-Datei installiert. Dadurch können Sie über die Windows-Eingabeaufforderung (CMD) oder über PowerShell auf die CLI zugreifen.</span><span class="sxs-lookup"><span data-stu-id="d8523-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="d8523-105">Bei der Installation für ein Windows-Subsystem für Linux (WSL) sind Pakete für Ihre Linux-Distribution verfügbar.</span><span class="sxs-lookup"><span data-stu-id="d8523-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="d8523-106">Die Liste der unterstützten Paket-Manager bzw. Informationen zur manuellen Installation unter WSL finden Sie auf der [Hauptseite für die Installation](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d8523-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="d8523-107">Installieren oder Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d8523-107">Install or update</span></span>

<span data-ttu-id="d8523-108">Das verteilbare MSI-Installationsprogramm wird zum Installieren oder Aktualisieren der Azure-Befehlszeilenschnittstelle (Azure Command Line Interface, Azure CLI) unter Windows verwendet.</span><span class="sxs-lookup"><span data-stu-id="d8523-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="d8523-109">Sie müssen keine aktuellen Versionen deinstallieren, bevor Sie das MSI-Installationsprogramm ausführen.</span><span class="sxs-lookup"><span data-stu-id="d8523-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="d8523-110">MSI-Installationsprogramm herunterladen</span><span class="sxs-lookup"><span data-stu-id="d8523-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="d8523-111">Wenn das Installationsprogramm fragt, ob Änderungen am Computer vorgenommen werden dürfen, klicken Sie auf „Ja“.</span><span class="sxs-lookup"><span data-stu-id="d8523-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="d8523-112">Sie können die Azure-Befehlszeilenschnittstelle auch mithilfe von PowerShell installieren.</span><span class="sxs-lookup"><span data-stu-id="d8523-112">You can also install the Azure CLI using PowerShell.</span></span> <span data-ttu-id="d8523-113">Starten Sie PowerShell als Administrator, und führen Sie den folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="d8523-113">Start PowerShell as administrator and run the following command:</span></span>

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'
   ```
<span data-ttu-id="d8523-114">Dadurch wird die aktuelle Version der Azure-Befehlszeilenschnittstelle für Windows heruntergeladen und installiert.</span><span class="sxs-lookup"><span data-stu-id="d8523-114">This will download and install the latest version of the Azure CLI for Windows.</span></span> <span data-ttu-id="d8523-115">Haben Sie bereits eine Version installiert, wird diese aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="d8523-115">If you already have a version installed, it will update the existing version.</span></span> <span data-ttu-id="d8523-116">Nach Abschluss der Installation müssen Sie PowerShell erneut öffnen, damit die Azure-Befehlszeilenschnittstelle verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="d8523-116">After the installation is complete, you will need to reopen PowerShell to use the Azure CLI.</span></span>

<span data-ttu-id="d8523-117">Sie können nun mit dem Befehl `az` über die Windows-Eingabeaufforderung oder PowerShell die Azure CLI ausführen.</span><span class="sxs-lookup"><span data-stu-id="d8523-117">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="d8523-118">In PowerShell stehen einige Features zur Vervollständigung mit der TAB-TASTE zur Verfügung, die an der Windows-Eingabeaufforderung nicht verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="d8523-118">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="d8523-119">Führen Sie den Befehl [az login](/cli/azure/reference-index#az-login) aus, um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="d8523-119">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="d8523-120">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d8523-120">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="d8523-121">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="d8523-121">Troubleshooting</span></span>

<span data-ttu-id="d8523-122">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation unter Windows auftreten können.</span><span class="sxs-lookup"><span data-stu-id="d8523-122">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="d8523-123">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="d8523-123">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="d8523-124">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="d8523-124">Proxy blocks connection</span></span>

<span data-ttu-id="d8523-125">Wenn Sie das MSI-Installationsprogramm nicht herunterladen können, da Ihr Proxy die Verbindung blockiert, stellen Sie sicher, dass Sie den Proxy richtig konfiguriert haben.</span><span class="sxs-lookup"><span data-stu-id="d8523-125">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="d8523-126">Für Windows 10 werden diese Einstellungen im Bereich `Settings > Network & Internet > Proxy` verwaltet.</span><span class="sxs-lookup"><span data-stu-id="d8523-126">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="d8523-127">Wenden Sie sich an Ihren Systemadministrator, um Informationen zu den erforderlichen Einstellungen zu erhalten oder wenn Ihr Computer ggf. konfigurationsverwaltet ist oder ein erweitertes Setup erfordert.</span><span class="sxs-lookup"><span data-stu-id="d8523-127">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d8523-128">Diese Einstellungen sind auch erforderlich, damit Sie mit der CLI sowohl über PowerShell als auch über die Eingabeaufforderung auf Azure-Dienste zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="d8523-128">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="d8523-129">Führen Sie dazu in PowerShell den folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="d8523-129">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="d8523-130">Zum Abrufen der MSI muss Ihr Proxy HTTPS-Verbindungen mit den folgenden Adressen zulassen:</span><span class="sxs-lookup"><span data-stu-id="d8523-130">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="d8523-131">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="d8523-131">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="d8523-132">Sie deinstallieren die Azure-Befehlszeilenschnittstelle über die Liste „Apps und Features“ in Windows.</span><span class="sxs-lookup"><span data-stu-id="d8523-132">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="d8523-133">Gehen Sie zum Deinstallieren wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="d8523-133">To uninstall:</span></span>

| <span data-ttu-id="d8523-134">Plattform</span><span class="sxs-lookup"><span data-stu-id="d8523-134">Platform</span></span> | <span data-ttu-id="d8523-135">Anleitung</span><span class="sxs-lookup"><span data-stu-id="d8523-135">Instructions</span></span> |
|---|---|
| <span data-ttu-id="d8523-136">Windows 10</span><span class="sxs-lookup"><span data-stu-id="d8523-136">Windows 10</span></span> | <span data-ttu-id="d8523-137">Start > Einstellungen > Apps</span><span class="sxs-lookup"><span data-stu-id="d8523-137">Start > Settings > Apps</span></span> |
| <span data-ttu-id="d8523-138">Windows 8</span><span class="sxs-lookup"><span data-stu-id="d8523-138">Windows 8</span></span><br/><span data-ttu-id="d8523-139">Windows 7</span><span class="sxs-lookup"><span data-stu-id="d8523-139">Windows 7</span></span> | <span data-ttu-id="d8523-140">Start > Systemsteuerung > Programme > Programm deinstallieren</span><span class="sxs-lookup"><span data-stu-id="d8523-140">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="d8523-141">Geben Sie auf diesem Bildschirm __Azure CLI__ in die Suchleiste des Programms ein.</span><span class="sxs-lookup"><span data-stu-id="d8523-141">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="d8523-142">Das Programm zum Deinstallieren wird als __Microsoft CLI 2.0 for Azure__ angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d8523-142">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="d8523-143">Wählen Sie diese Anwendung aus, und klicken Sie dann auf die Schaltfläche `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="d8523-143">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d8523-144">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="d8523-144">Next Steps</span></span>

<span data-ttu-id="d8523-145">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="d8523-145">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="d8523-146">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="d8523-146">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

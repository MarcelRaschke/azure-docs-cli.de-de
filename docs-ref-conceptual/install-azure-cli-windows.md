---
title: Installieren der Azure-Befehlszeilenschnittstelle für Windows
description: Installieren der Azure CLI unter Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 06/16/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devx-track-azurecli
ms.openlocfilehash: dc6386e8bc1dfc4d11dafcdb947e9ff0b336ed25
ms.sourcegitcommit: bf84dfb62e910ea246586481863bb43d09d07795
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/04/2020
ms.locfileid: "87551505"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="661ee-103">Installieren der Azure CLI unter Windows</span><span class="sxs-lookup"><span data-stu-id="661ee-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="661ee-104">Unter Windows wird die Azure CLI über eine MSI-Datei installiert. Dadurch können Sie über die Windows-Eingabeaufforderung (CMD) oder über PowerShell auf die CLI zugreifen.</span><span class="sxs-lookup"><span data-stu-id="661ee-104">For Windows, the Azure CLI is installed via a MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="661ee-105">Bei der Installation für ein Windows-Subsystem für Linux (WSL) sind Pakete für Ihre Linux-Distribution verfügbar.</span><span class="sxs-lookup"><span data-stu-id="661ee-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="661ee-106">Die Liste der unterstützten Paket-Manager bzw. Informationen zur manuellen Installation unter WSL finden Sie auf der [Hauptseite für die Installation](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="661ee-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="661ee-107">Installieren oder Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="661ee-107">Install or update</span></span>

<span data-ttu-id="661ee-108">Das verteilbare MSI-Installationsprogramm wird zum Installieren oder Aktualisieren der Azure-Befehlszeilenschnittstelle (Azure Command Line Interface, Azure CLI) unter Windows verwendet.</span><span class="sxs-lookup"><span data-stu-id="661ee-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="661ee-109">Sie müssen aktuelle Versionen nicht deinstallieren, bevor Sie das MSI-Installationsprogramm verwenden, da mit der MSI-Datei vorhandene Versionen aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="661ee-109">You don't need to uninstall current versions before using the MSI installer because the MSI will update any existing version.</span></span>

# <a name="microsoft-installer-msi"></a>[<span data-ttu-id="661ee-110">Microsoft Installer (MSI)</span><span class="sxs-lookup"><span data-stu-id="661ee-110">Microsoft Installer (MSI)</span></span>](#tab/azure-cli)

<span data-ttu-id="661ee-111">Wenn das Installationsprogramm fragt, ob Änderungen am Computer vorgenommen werden dürfen, klicken Sie auf „Ja“.</span><span class="sxs-lookup"><span data-stu-id="661ee-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

### <a name="azure-cli-current-version"></a><span data-ttu-id="661ee-112">Aktuelle Version der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="661ee-112">Azure CLI current version</span></span>

<span data-ttu-id="661ee-113">Laden Sie die aktuelle Version der Azure CLI herunter, und installieren Sie sie.</span><span class="sxs-lookup"><span data-stu-id="661ee-113">Download and install the current release of the Azure CLI.</span></span>  

> [!div class="nextstepaction"]
> [<span data-ttu-id="661ee-114">Aktuelle Version der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="661ee-114">Current release of the Azure CLI</span></span>](https://aka.ms/installazurecliwindows)

### <a name="azure-cli-beta-version"></a><span data-ttu-id="661ee-115">Azure CLI-Betaversion</span><span class="sxs-lookup"><span data-stu-id="661ee-115">Azure CLI beta version</span></span>

<span data-ttu-id="661ee-116">Die Betaversion der Azure CLI unterstützt alle CLI-Befehle, die in der aktuellen veröffentlichten Version verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="661ee-116">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span> <span data-ttu-id="661ee-117">Die Betaversion ist eine Migration der veröffentlichten Azure CLI, da die AAD-Authentifizierungsplattform (v1.0) nicht mehr unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="661ee-117">The beta version is a migration from the released Azure CLI as the AAD authentication platform (v1.0) is being deprecated.</span></span>  <span data-ttu-id="661ee-118">[Microsoft Identity Platform (v2.0)](/azure/active-directory/develop/v2-overview) ist die neue Authentifizierungsmethode und wird von der Betaversion der Azure CLI verwendet.</span><span class="sxs-lookup"><span data-stu-id="661ee-118">[Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview) is the new authentication method and is used by Azure CLI beta.</span></span>  <span data-ttu-id="661ee-119">Es wird empfohlen, die Betaversion vorab zu testen.</span><span class="sxs-lookup"><span data-stu-id="661ee-119">We recommend that you try the beta version in advance.</span></span>  

<span data-ttu-id="661ee-120">Weitere Informationen zur Azure CLI-Betaversion finden Sie in den [Versionshinweisen](release-notes-azure-cli?tabs=azure-cli-beta).</span><span class="sxs-lookup"><span data-stu-id="661ee-120">For more information about Azure CLI beta, please see [release notes](release-notes-azure-cli?tabs=azure-cli-beta).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="661ee-121">Die Betaversion garantiert keine Qualität auf Produktebene, daher sollte sie nicht in der Produktionsumgebung verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="661ee-121">The beta version does not guarantee product level quality so it should not be used in your production environment.</span></span>

<span data-ttu-id="661ee-122">Laden Sie die Betaversion der Azure CLI herunter, und installieren Sie sie.</span><span class="sxs-lookup"><span data-stu-id="661ee-122">Download and install the beta version of the Azure CLI.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="661ee-123">Betaversion der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="661ee-123">Beta release of the Azure CLI</span></span>](https://aka.ms/installazurecliwindowsbeta)

# <a name="microsoft-installer-msi-with-powershell"></a>[<span data-ttu-id="661ee-124">Microsoft Installer (MSI) mit PowerShell</span><span class="sxs-lookup"><span data-stu-id="661ee-124">Microsoft Installer (MSI) with PowerShell</span></span>](#tab/azure-powershell)

<span data-ttu-id="661ee-125">Sie können die Azure-Befehlszeilenschnittstelle auch mithilfe von PowerShell installieren.</span><span class="sxs-lookup"><span data-stu-id="661ee-125">You can also install the Azure CLI using PowerShell.</span></span> <span data-ttu-id="661ee-126">Starten Sie PowerShell als Administrator, und führen Sie den folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="661ee-126">Start PowerShell as administrator and run the following command:</span></span>

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```

<span data-ttu-id="661ee-127">Dadurch wird die aktuelle Version der Azure-Befehlszeilenschnittstelle für Windows heruntergeladen und installiert.</span><span class="sxs-lookup"><span data-stu-id="661ee-127">This will download and install the latest version of the Azure CLI for Windows.</span></span> <span data-ttu-id="661ee-128">Haben Sie bereits eine Version installiert, wird die vorhandene Version vom Installationsprogramm aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="661ee-128">If you already have a version installed, the installer will update the existing version.</span></span> <span data-ttu-id="661ee-129">Nach Abschluss der Installation müssen Sie PowerShell erneut öffnen, damit die Azure-Befehlszeilenschnittstelle verwendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="661ee-129">After the installation is complete, you will need to reopen PowerShell to use the Azure CLI.</span></span>

---

## <a name="run-the-azure-cli"></a><span data-ttu-id="661ee-130">Ausführen der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="661ee-130">Run the Azure CLI</span></span>

<span data-ttu-id="661ee-131">Sie können nun mit dem Befehl `az` über die Windows-Eingabeaufforderung oder PowerShell die Azure CLI ausführen.</span><span class="sxs-lookup"><span data-stu-id="661ee-131">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="661ee-132">In PowerShell stehen einige Features zur Vervollständigung mit der TAB-TASTE zur Verfügung, die an der Windows-Eingabeaufforderung nicht verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="661ee-132">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="661ee-133">Führen Sie den Befehl [az login](/cli/azure/reference-index#az-login) aus, um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="661ee-133">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="661ee-134">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="661ee-134">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="661ee-135">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="661ee-135">Troubleshooting</span></span>

<span data-ttu-id="661ee-136">In diesem Abschnitt finden Sie einige allgemeine Probleme, die bei der Installation unter Windows auftreten können.</span><span class="sxs-lookup"><span data-stu-id="661ee-136">Here are some common problems seen when installing on Windows.</span></span> <span data-ttu-id="661ee-137">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="661ee-137">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="661ee-138">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="661ee-138">Proxy blocks connection</span></span>

<span data-ttu-id="661ee-139">Wenn Sie das MSI-Installationsprogramm nicht herunterladen können, da Ihr Proxy die Verbindung blockiert, stellen Sie sicher, dass Sie den Proxy richtig konfiguriert haben.</span><span class="sxs-lookup"><span data-stu-id="661ee-139">If you can't download the MSI installer because your proxy is blocking the connection, make sure that you have your proxy properly configured.</span></span> <span data-ttu-id="661ee-140">Für Windows 10 werden diese Einstellungen im Bereich `Settings > Network & Internet > Proxy` verwaltet.</span><span class="sxs-lookup"><span data-stu-id="661ee-140">For Windows 10, these settings are managed in the `Settings > Network & Internet > Proxy` pane.</span></span> <span data-ttu-id="661ee-141">Wenden Sie sich an Ihren Systemadministrator, um Informationen zu den erforderlichen Einstellungen zu erhalten oder wenn Ihr Computer ggf. konfigurationsverwaltet ist oder ein erweitertes Setup erfordert.</span><span class="sxs-lookup"><span data-stu-id="661ee-141">Contact your system administrator for the required settings, or for situations where your machine may be configuration-managed or require advanced setup.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="661ee-142">Diese Einstellungen sind auch erforderlich, damit Sie mit der CLI sowohl über PowerShell als auch über die Eingabeaufforderung auf Azure-Dienste zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="661ee-142">These settings are also required to be able to access Azure services with the CLI, from both PowerShell or the Command Prompt.</span></span> <span data-ttu-id="661ee-143">Führen Sie dazu in PowerShell den folgenden Befehl aus:</span><span class="sxs-lookup"><span data-stu-id="661ee-143">In PowerShell, you do this with the following command:</span></span>
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

<span data-ttu-id="661ee-144">Zum Abrufen der MSI muss Ihr Proxy HTTPS-Verbindungen mit den folgenden Adressen zulassen:</span><span class="sxs-lookup"><span data-stu-id="661ee-144">In order to get the MSI, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a><span data-ttu-id="661ee-145">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="661ee-145">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="661ee-146">Sie deinstallieren die Azure-Befehlszeilenschnittstelle über die Liste „Apps und Features“ in Windows.</span><span class="sxs-lookup"><span data-stu-id="661ee-146">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="661ee-147">Gehen Sie zum Deinstallieren wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="661ee-147">To uninstall:</span></span>

| <span data-ttu-id="661ee-148">Plattform</span><span class="sxs-lookup"><span data-stu-id="661ee-148">Platform</span></span> | <span data-ttu-id="661ee-149">Instructions</span><span class="sxs-lookup"><span data-stu-id="661ee-149">Instructions</span></span> |
|---|---|
| <span data-ttu-id="661ee-150">Windows 10</span><span class="sxs-lookup"><span data-stu-id="661ee-150">Windows 10</span></span> | <span data-ttu-id="661ee-151">Start > Einstellungen > Apps</span><span class="sxs-lookup"><span data-stu-id="661ee-151">Start > Settings > Apps</span></span> |
| <span data-ttu-id="661ee-152">Windows 8 und Windows 7</span><span class="sxs-lookup"><span data-stu-id="661ee-152">Windows 8 and Windows 7</span></span> | <span data-ttu-id="661ee-153">Start > Systemsteuerung > Programme > Programm deinstallieren</span><span class="sxs-lookup"><span data-stu-id="661ee-153">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="661ee-154">Geben Sie auf diesem Bildschirm __Azure CLI__ in die Suchleiste des Programms ein.</span><span class="sxs-lookup"><span data-stu-id="661ee-154">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="661ee-155">Das Programm zum Deinstallieren wird als __Microsoft CLI 2.0 for Azure__ angezeigt.</span><span class="sxs-lookup"><span data-stu-id="661ee-155">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="661ee-156">Wählen Sie diese Anwendung aus, und klicken Sie dann auf die Schaltfläche `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="661ee-156">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="661ee-157">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="661ee-157">Next Steps</span></span>

<span data-ttu-id="661ee-158">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="661ee-158">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="661ee-159">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="661ee-159">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

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
ms.openlocfilehash: c5c499800e49dcdc536337e7655ec1ee280d48f2
ms.sourcegitcommit: 65bf8561a6e047e4eab52186e066a2e8c21f1d40
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/07/2019
ms.locfileid: "65240546"
---
# <a name="install-azure-cli-on-windows"></a><span data-ttu-id="0396a-103">Installieren der Azure CLI unter Windows</span><span class="sxs-lookup"><span data-stu-id="0396a-103">Install Azure CLI on Windows</span></span>

<span data-ttu-id="0396a-104">Unter Windows wird die Azure CLI über eine MSI-Datei installiert. Dadurch können Sie über die Windows-Eingabeaufforderung (CMD) oder über PowerShell auf die CLI zugreifen.</span><span class="sxs-lookup"><span data-stu-id="0396a-104">For Windows the Azure CLI is installed via an MSI, which gives you access to the CLI through the Windows Command Prompt (CMD) or PowerShell.</span></span>
<span data-ttu-id="0396a-105">Bei der Installation für ein Windows-Subsystem für Linux (WSL) sind Pakete für Ihre Linux-Distribution verfügbar.</span><span class="sxs-lookup"><span data-stu-id="0396a-105">When installing for Windows Subsystem for Linux (WSL), packages are available for your Linux distribution.</span></span> <span data-ttu-id="0396a-106">Die Liste der unterstützten Paket-Manager bzw. Informationen zur manuellen Installation unter WSL finden Sie auf der [Hauptseite für die Installation](install-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0396a-106">See the [main install page](install-azure-cli.md) for the list of supported package managers or how to install manually under WSL.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a><span data-ttu-id="0396a-107">Installieren oder Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0396a-107">Install or update</span></span>

<span data-ttu-id="0396a-108">Das verteilbare MSI-Installationsprogramm wird zum Installieren oder Aktualisieren der Azure-Befehlszeilenschnittstelle (Azure Command Line Interface, Azure CLI) unter Windows verwendet.</span><span class="sxs-lookup"><span data-stu-id="0396a-108">The MSI distributable is used for installing or updating the Azure CLI on Windows.</span></span> <span data-ttu-id="0396a-109">Sie müssen keine aktuellen Versionen deinstallieren, bevor Sie das MSI-Installationsprogramm ausführen.</span><span class="sxs-lookup"><span data-stu-id="0396a-109">You don't need to uninstall any current versions before using the MSI installer.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="0396a-110">MSI-Installationsprogramm herunterladen</span><span class="sxs-lookup"><span data-stu-id="0396a-110">Download the MSI installer</span></span>](https://aka.ms/installazurecliwindows)

<span data-ttu-id="0396a-111">Wenn das Installationsprogramm fragt, ob Änderungen am Computer vorgenommen werden dürfen, klicken Sie auf „Ja“.</span><span class="sxs-lookup"><span data-stu-id="0396a-111">When the installer asks if it can make changes to your computer, click the "Yes" box.</span></span>

<span data-ttu-id="0396a-112">Sie können nun mit dem Befehl `az` über die Windows-Eingabeaufforderung oder PowerShell die Azure CLI ausführen.</span><span class="sxs-lookup"><span data-stu-id="0396a-112">You can now run the Azure CLI with the `az` command from either Windows Command Prompt or PowerShell.</span></span> <span data-ttu-id="0396a-113">In PowerShell stehen einige Features zur Vervollständigung mit der TAB-TASTE zur Verfügung, die an der Windows-Eingabeaufforderung nicht verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="0396a-113">PowerShell offers some tab completion features not available from Windows Command Prompt.</span></span> <span data-ttu-id="0396a-114">Führen Sie den Befehl [az login](/cli/azure/reference-index#az-login) aus, um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="0396a-114">To sign in, run the [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="0396a-115">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0396a-115">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="uninstall"></a><span data-ttu-id="0396a-116">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="0396a-116">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="0396a-117">Sie deinstallieren die Azure-Befehlszeilenschnittstelle über die Liste „Apps und Features“ in Windows.</span><span class="sxs-lookup"><span data-stu-id="0396a-117">You uninstall the Azure CLI from the Windows "Apps and Features" list.</span></span> <span data-ttu-id="0396a-118">Gehen Sie zum Deinstallieren wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="0396a-118">To uninstall:</span></span>

| <span data-ttu-id="0396a-119">Plattform</span><span class="sxs-lookup"><span data-stu-id="0396a-119">Platform</span></span> | <span data-ttu-id="0396a-120">Anleitung</span><span class="sxs-lookup"><span data-stu-id="0396a-120">Instructions</span></span> |
|---|---|
| <span data-ttu-id="0396a-121">Windows 10</span><span class="sxs-lookup"><span data-stu-id="0396a-121">Windows 10</span></span> | <span data-ttu-id="0396a-122">Start > Einstellungen > Apps</span><span class="sxs-lookup"><span data-stu-id="0396a-122">Start > Settings > Apps</span></span> |
| <span data-ttu-id="0396a-123">Windows 8</span><span class="sxs-lookup"><span data-stu-id="0396a-123">Windows 8</span></span><br/><span data-ttu-id="0396a-124">Windows 7</span><span class="sxs-lookup"><span data-stu-id="0396a-124">Windows 7</span></span> | <span data-ttu-id="0396a-125">Start > Systemsteuerung > Programme > Programm deinstallieren</span><span class="sxs-lookup"><span data-stu-id="0396a-125">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="0396a-126">Geben Sie auf diesem Bildschirm __Azure CLI__ in die Suchleiste des Programms ein.</span><span class="sxs-lookup"><span data-stu-id="0396a-126">Once on this screen type __Azure CLI__ into the program search bar.</span></span> <span data-ttu-id="0396a-127">Das Programm zum Deinstallieren wird als __Microsoft CLI 2.0 for Azure__ angezeigt.</span><span class="sxs-lookup"><span data-stu-id="0396a-127">The program to uninstall is listed as __Microsoft CLI 2.0 for Azure__.</span></span> <span data-ttu-id="0396a-128">Wählen Sie diese Anwendung aus, und klicken Sie dann auf die Schaltfläche `Uninstall`.</span><span class="sxs-lookup"><span data-stu-id="0396a-128">Select this application, then click the `Uninstall` button.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0396a-129">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="0396a-129">Next Steps</span></span>

<span data-ttu-id="0396a-130">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="0396a-130">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="0396a-131">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="0396a-131">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

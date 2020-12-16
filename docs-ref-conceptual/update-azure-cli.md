---
title: Aktualisieren der Azure-Befehlszeilenschnittstelle
description: Referenz zur Aktualisierung der Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 10/19/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 475b58bca5ec9dca52a70416cb89860dcbd39278
ms.sourcegitcommit: e1faf297ba2cdf2ba7e821fbeedff9c9a724c975
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/16/2020
ms.locfileid: "97576784"
---
# <a name="update-the-azure-cli"></a><span data-ttu-id="7fcf6-103">Aktualisieren der Azure-Befehlszeilenschnittstelle</span><span class="sxs-lookup"><span data-stu-id="7fcf6-103">Update the Azure CLI</span></span>

<span data-ttu-id="7fcf6-104">Sie können sich darauf verlassen, dass Paket-Manager eine lokale Installation der Azure CLI in Windows-, macOS- und Linux-Umgebungen aktualisieren (siehe Abschnitt `Update` in den jeweiligen plattformspezifischen Installationsanweisungen).</span><span class="sxs-lookup"><span data-stu-id="7fcf6-104">You can rely on package managers to update a local install of the Azure CLI on Windows, macOS and Linux environments (see the `Update` section in each platform-specific install instruction).</span></span> <span data-ttu-id="7fcf6-105">Die CLI bietet außerdem Befehle im Tool zum manuellen oder automatischen Aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-105">The CLI also provides in-tool commands to upgrade manually or automatically.</span></span>

## <a name="manual-update"></a><span data-ttu-id="7fcf6-106">Manuelle Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="7fcf6-106">Manual Update</span></span>
[!INCLUDE [az-upgrade](includes/az-upgrade.md)]

<span data-ttu-id="7fcf6-107">`az upgrade` wird unter Windows und macOS und in einigen Linux-Distributionen unterstützt, sofern auch die Installation unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-107">`az upgrade` is supported on Windows, macOS and some Linux distros as long as installation is supported.</span></span> <span data-ttu-id="7fcf6-108">Damit wird nur das Upgrade auf die neuste Version unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-108">It only supports upgrading to the latest version.</span></span> <span data-ttu-id="7fcf6-109">Wenn Sie die Azure CLI über Azure Cloud Shell ausführen, verwenden Sie wahrscheinlich bereits die aktuelle Azure CLI-Installation.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-109">If you are running the Azure CLI through Azure Cloud Shell, you are most likely already using the most recent Azure CLI install.</span></span> <span data-ttu-id="7fcf6-110">Ist dies beispielsweise aufgrund eines Ad-hoc-Release einer Nebenversion zur Fehlerbehebung nicht der Fall, müssen Sie auf den nächsten Build von Azure Cloud Shell warten, da `az upgrade` in Azure Cloud Shell nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-110">If not due to cases like ad-hoc release of a minor bug fix version, you need to wait for the next build of Azure Cloud Shell as `az upgrade` is not supported in Azure Cloud Shell.</span></span>

<span data-ttu-id="7fcf6-111">Ist `azure-cli` bereits die aktuelle Version, werden bei der Ausführung von `az upgrade` alle installierten [Erweiterungen](azure-cli-extensions-overview.md) überprüft und aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-111">When `azure-cli` is already the latest version, running `az upgrade` will check and update all installed [extensions](azure-cli-extensions-overview.md).</span></span>

## <a name="automatic-update"></a><span data-ttu-id="7fcf6-112">Automatische Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="7fcf6-112">Automatic Update</span></span>

<span data-ttu-id="7fcf6-113">Automatische Upgrades sind für die Azure CLI standardmäßig deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-113">By default, auto-upgrade for Azure CLI is disabled.</span></span> <span data-ttu-id="7fcf6-114">Wenn Sie stets die aktuelle Version verwenden möchten, können Sie automatische Upgrades über die [Konfiguration](/cli/azure/config) aktivieren.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-114">If you would like to keep up with the latest version, you can enable auto-upgrade through [configuration](/cli/azure/config).</span></span>

```azurecli
az config set auto-upgrade.enable=yes
```

<span data-ttu-id="7fcf6-115">Die Azure CLI prüft regelmäßig auf neue Versionen und fordert Sie nach Abschluss der Befehlsausführung zur Aktualisierung auf, sobald das Update verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-115">The Azure CLI will check new versions regularly and prompt you to upgrade after any command finishes running once the update is available.</span></span>

<span data-ttu-id="7fcf6-116">Die Aufforderungsmeldung und die Ausgabemeldungen während des Upgrades unterbrechen unter Umständen das Befehlsergebnis, wenn es einer Variablen oder in einem automatisierten Flow zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-116">The prompt message and output messages during upgrade may interrupt your command result if it is assigned to some variable or in an automated flow.</span></span> <span data-ttu-id="7fcf6-117">Zur Vermeidung von Unterbrechungen können Sie die folgende Konfiguration verwenden, um zuzulassen, dass das Update automatisch ohne Bestätigung ausgeführt wird und nur Warnungen und Fehler während des Upgrades angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-117">To avoid interruption, you can use the following configuration to allow the update to happen automatically without confirmation and only show warnings and errors during the upgrade.</span></span>

```azurecli
az config set auto-upgrade.prompt=no
```

<span data-ttu-id="7fcf6-118">Standardmäßig werden alle installierten Erweiterungen ebenfalls aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-118">By default, all installed extensions will also be updated.</span></span> <span data-ttu-id="7fcf6-119">Sie können die Aktualisierung von Erweiterungen über die Konfiguration deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-119">You can disable extension update through configuration.</span></span>

```azurecli
az config set auto-upgrade.all=no
```

> [!NOTE]
> <span data-ttu-id="7fcf6-120">Warten Sie, bis `az upgrade` abgeschlossen ist, bevor Sie mit dem nächsten Befehlssatz fortfahren. Andernfalls weisen die neuen Versionen der CLI (und Erweiterungen) möglicherweise Breaking Changes auf.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-120">Please wait for `az upgrade` to complete before proceeding to the next set of commands, else the new versions of the CLI (+extensions) may have breaking changes.</span></span>

<span data-ttu-id="7fcf6-121">Wenn Sie die Funktion für automatische Updates nicht mehr verwenden möchten, um beispielsweise die stabile Ausführung von Befehlsskripts zu gewährleisten, können Sie sie über die Konfiguration deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="7fcf6-121">If you decide not to use the automatic update feature any more for cases like keeping command scripts running stably, you can turn it off through configuration.</span></span>
```azurecli
az config set auto-upgrade.enable=no
```

---
title: Unterschiede zwischen Azure CLI-Produkten
description: Es wird beschrieben, wie Azure CLI-Produkte benannt sind und mit einer Version versehen und aktualisiert werden.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 07/12/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 3cd61d2166d03f7b9d58db1ee1cee77d17b5b336
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2020
ms.locfileid: "77779974"
---
# <a name="differences-between-azure-cli-products"></a><span data-ttu-id="af226-103">Unterschiede zwischen Azure CLI-Produkten</span><span class="sxs-lookup"><span data-stu-id="af226-103">Differences between Azure CLI products</span></span>

<span data-ttu-id="af226-104">Ab Ende Juni 2018 wurden explizite Versionsnummern aus den Produktnamen der Azure CLI entfernt.</span><span class="sxs-lookup"><span data-stu-id="af226-104">As of the end of June 2018, explicit version numbers have been removed from Azure CLI product names.</span></span> <span data-ttu-id="af226-105">Diese Änderung trägt zur Vermeidung von verwirrenden Informationen bei, die in der Dokumentation an einigen Stellen enthalten waren. Benutzer wurden aufgefordert, „die Azure CLI“ zu verwenden, aber es war nicht klar, welche Version des Produkts gemeint war.</span><span class="sxs-lookup"><span data-stu-id="af226-105">This change helps eliminate confusion that sometimes showed up in documentation where users were told to use "the Azure CLI" but it was unclear what version of the product was being referenced.</span></span> <span data-ttu-id="af226-106">Wenn Sie mit den alten Produktnamen vertraut sind, helfen Ihnen diese Informationen zu den Änderungen weiter:</span><span class="sxs-lookup"><span data-stu-id="af226-106">If you're familiar with the old product names, here is how they have changed:</span></span>

* <span data-ttu-id="af226-107">Azure CLI-Version 2.0 und höher wird jetzt nur noch als „Azure CLI“ bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="af226-107">Azure CLI versions 2.0 and later are now referred to only as "Azure CLI."</span></span>
* <span data-ttu-id="af226-108">Frühere Versionen der Azure CLI (1.x und früher) werden jetzt als „klassische Azure CLI“ bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="af226-108">Earlier Azure CLI versions (1.x and lower) are now referred to as "Azure classic CLI."</span></span>

<span data-ttu-id="af226-109">Mit der Änderung in „klassische Azure CLI“ wird verdeutlicht, dass dieses Tool nur mit dem klassischen Bereitstellungsmodell verwendet werden sollte.</span><span class="sxs-lookup"><span data-stu-id="af226-109">The name change to Azure classic CLI makes it clear that this tool is meant to be used only with the classic deployment model.</span></span> <span data-ttu-id="af226-110">Die klassische CLI wird nicht mehr aktualisiert oder gewartet.</span><span class="sxs-lookup"><span data-stu-id="af226-110">The classic CLI is also no longer updated or maintained.</span></span> <span data-ttu-id="af226-111">Aus diesem und vielen anderen Gründen wird empfohlen, alle klassischen Bereitstellungen auf das Azure Resource Manager-Modell umzustellen und zur letzten verfügbaren Version der Azure CLI zu migrieren.</span><span class="sxs-lookup"><span data-stu-id="af226-111">For this reason, and many more, it's recommended that you move any classic deployments to use the Azure Resource Manager model and migrate to the latest available version of the Azure CLI.</span></span>

<span data-ttu-id="af226-112">Falls Sie noch die klassische CLI nutzen, helfen Ihnen die Informationen zum Migrationsprozess in den folgenden Artikeln weiter:</span><span class="sxs-lookup"><span data-stu-id="af226-112">If you are still using the classic CLI, you can learn about the process of migrating in the following articles:</span></span>

* [<span data-ttu-id="af226-113">Migrieren von der klassischen Bereitstellung zum Azure Resource Manager</span><span class="sxs-lookup"><span data-stu-id="af226-113">Migrate from Classic to Azure Resource Manager</span></span>](/azure/virtual-machines/linux/migration-classic-resource-manager-overview)
* [<span data-ttu-id="af226-114">Installieren der Azure-Befehlszeilenschnittstelle</span><span class="sxs-lookup"><span data-stu-id="af226-114">Install the Azure CLI</span></span>](install-azure-cli.md)
* <span data-ttu-id="af226-115">[Migrating from Azure classic CLI to Azure CLI](https://github.com/Azure/azure-cli/blob/dev/doc/classic_cli_migration.md) (Migrieren von der klassischen Azure CLI zur Azure CLI)</span><span class="sxs-lookup"><span data-stu-id="af226-115">[Migrating from Azure classic CLI to Azure CLI](https://github.com/Azure/azure-cli/blob/dev/doc/classic_cli_migration.md)</span></span>

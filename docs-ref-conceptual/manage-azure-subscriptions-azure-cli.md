---
title: Verwalten von Azure-Abonnements mit der Azure CLI
description: Hier erfahren Sie mehr über Azure-Mandanten, -Benutzer und -Abonnements. Verwenden Sie die Azure CLI, um Ihre Abonnements zu verwalten, Verwaltungsgruppen zu erstellen und Abonnements zu sperren.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/29/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 6a980c45627c79c9e3f8c6c920944cc3dc62281f
ms.sourcegitcommit: 3e79897e0aeca4d74bc8ff0410121b011b5884ec
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/03/2021
ms.locfileid: "99495226"
---
# <a name="use-azure-subscriptions-with-azure-cli"></a><span data-ttu-id="ff630-104">Verwenden von Azure-Abonnements mit der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="ff630-104">Use Azure subscriptions with Azure CLI</span></span>

<span data-ttu-id="ff630-105">Sie verfügen möglicherweise über mehrere Abonnements in Azure.</span><span class="sxs-lookup"><span data-stu-id="ff630-105">You might have multiple subscriptions within Azure.</span></span> <span data-ttu-id="ff630-106">Sie können mehreren Organisationen angehören, oder Ihre Organisation teilt unter Umständen den Zugriff auf bestimmte Ressourcen gruppierungsübergreifend auf.</span><span class="sxs-lookup"><span data-stu-id="ff630-106">You can be part of more than one organization or your organization might divide access to certain resources across groupings.</span></span> <span data-ttu-id="ff630-107">Die Azure CLI unterstützt sowohl die globale Auswahl eines Abonnements als auch die Auswahl per Befehl.</span><span class="sxs-lookup"><span data-stu-id="ff630-107">The Azure CLI supports selecting a subscription both globally and per command.</span></span>

<span data-ttu-id="ff630-108">Ausführliche Informationen zu Abonnements, der Abrechnung und der Kostenverwaltung finden Sie in der [Dokumentation zur Abrechnungs- und Kostenverwaltung in Azure](/azure/billing/).</span><span class="sxs-lookup"><span data-stu-id="ff630-108">For detailed information on subscriptions, billing, and cost management, see the [billing and cost management documentation](/azure/billing/).</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="ff630-109">Mandanten, Benutzer und Abonnements</span><span class="sxs-lookup"><span data-stu-id="ff630-109">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="ff630-110">Ein _Mandant_ ist die Azure Active Directory-Entität, die eine gesamte Organisation umfasst.</span><span class="sxs-lookup"><span data-stu-id="ff630-110">A _tenant_ is the Azure Active Directory entity that encompasses a whole organization.</span></span> <span data-ttu-id="ff630-111">Ein Mandant verfügt über mindestens ein _Abonnement_ und mindestens einen _Benutzer_.</span><span class="sxs-lookup"><span data-stu-id="ff630-111">A tenant has one or more _subscription_ and _user_.</span></span> <span data-ttu-id="ff630-112">Ein Benutzer ist eine Person und nur einem einzelnen Mandanten zugeordnet: der Organisation, der er angehört.</span><span class="sxs-lookup"><span data-stu-id="ff630-112">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="ff630-113">Benutzer sind Konten, die sich bei Azure anmelden, um Ressourcen zu erstellen, zu verwalten und zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="ff630-113">Users are those accounts that sign in to Azure to create, manage, and use resources.</span></span> <span data-ttu-id="ff630-114">Ein Benutzer hat möglicherweise Zugriff auf mehrere _Abonnements_. Hierbei handelt es sich um die Vereinbarungen mit Microsoft, die die Verwendung von Clouddiensten wie Azure regeln.</span><span class="sxs-lookup"><span data-stu-id="ff630-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="ff630-115">Jede Ressource ist einem Abonnement zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="ff630-115">Every resource is associated with a subscription.</span></span>

* <span data-ttu-id="ff630-116">Weitere Informationen zu den Unterschieden zwischen Mandanten, Benutzern und Abonnements finden Sie im [Microsoft Azure-Glossar](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="ff630-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>
* <span data-ttu-id="ff630-117">Informationen zum Hinzufügen eines neuen Abonnements zu Ihrem Azure Active Directory-Mandanten finden Sie unter [Zuordnen oder Hinzufügen eines Azure-Abonnements zu Ihrem Azure Active Directory-Mandanten](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="ff630-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [Associate or add an Azure subscription to your Azure Active Directory tenant](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
* <span data-ttu-id="ff630-118">Informationen zum Anmelden bei einem bestimmten Mandanten finden Sie unter [Anmelden mit der Azure CLI](./authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="ff630-118">To learn how to sign in to a specific tenant, see [Sign in with the Azure CLI](./authenticate-azure-cli.md).</span></span>

## <a name="commands-in-a-subscription"></a><span data-ttu-id="ff630-119">Befehle in einem Abonnement</span><span class="sxs-lookup"><span data-stu-id="ff630-119">Commands in a subscription</span></span>

<span data-ttu-id="ff630-120">Viele Azure CLI Befehle werden im Kontext eines Abonnements ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="ff630-120">Many Azure CLI commands act within a subscription.</span></span> <span data-ttu-id="ff630-121">Sie können jederzeit angeben, in welchem Abonnement Sie arbeiten möchten. Verwenden Sie dazu den Parameter **subscription** in Ihrem Befehl.</span><span class="sxs-lookup"><span data-stu-id="ff630-121">You can always specify which subscription to work in by using the **subscription** parameter in your command.</span></span> <span data-ttu-id="ff630-122">Dieser Parameter ist optional.</span><span class="sxs-lookup"><span data-stu-id="ff630-122">That parameter is optional.</span></span> <span data-ttu-id="ff630-123">Wenn Sie kein Abonnement angeben, verwendet der Befehl das aktuelle, aktive Abonnement.</span><span class="sxs-lookup"><span data-stu-id="ff630-123">If you don't specify a subscription, the command uses your current, active subscription.</span></span>

<span data-ttu-id="ff630-124">Führen Sie zum Anzeigen des derzeit verwendeten Abonnements den Befehl [az account show](/cli/azure/account#az_account_show) aus:</span><span class="sxs-lookup"><span data-stu-id="ff630-124">To see the subscription you're currently using, run the [az account show](/cli/azure/account#az_account_show) command:</span></span>

```azurecli
az account show --output table
```

> [!TIP]
> <span data-ttu-id="ff630-125">Der Parameter `--output` ist ein globaler Parameter und für alle Befehle verfügbar.</span><span class="sxs-lookup"><span data-stu-id="ff630-125">The `--output` parameter is a global parameter, available for all commands.</span></span> <span data-ttu-id="ff630-126">Mit dem Wert **table** wird die Ausgabe in einem benutzerfreundlichen Format angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ff630-126">The **table** value presents output in a friendly format.</span></span> <span data-ttu-id="ff630-127">Weitere Informationen finden Sie unter [Ausgabeformate für Azure CLI-Befehle](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="ff630-127">For more information, see [Output formats for Azure CLI commands](/cli/azure/format-output-azure-cli).</span></span>

<span data-ttu-id="ff630-128">Abonnements enthalten Ressourcengruppen.</span><span class="sxs-lookup"><span data-stu-id="ff630-128">Subscriptions contain resource groups.</span></span> <span data-ttu-id="ff630-129">Eine Azure-Ressourcengruppe ist ein Container, der verwandte Ressourcen für eine Azure-Lösung enthält.</span><span class="sxs-lookup"><span data-stu-id="ff630-129">An Azure resource group is a container that holds related resources for an Azure solution.</span></span> <span data-ttu-id="ff630-130">Wenn Ihr Befehl mit Ressourcen im aktiven Abonnement funktioniert, muss `--subscription` nicht angegeben werden.</span><span class="sxs-lookup"><span data-stu-id="ff630-130">If your command works with resources in your active subscription, you don't need to specify `--subscription`.</span></span>

<span data-ttu-id="ff630-131">Mit dem folgenden Befehl wird ein Speicherkonto in der angegebenen Ressourcengruppe erstellt:</span><span class="sxs-lookup"><span data-stu-id="ff630-131">This command creates a storage account in the specified resource group:</span></span>

```azurecli
az storage account create --resource-group StorageGroups --name storage136 \
    --location eastus --sku Standard_LRS
```

<span data-ttu-id="ff630-132">Ist die Speichergruppe nicht Teil Ihres aktuellen aktiven Abonnements, tritt bei diesem Befehl ein Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="ff630-132">If the storage group isn't part of your current active subscription, this command fails.</span></span>

<span data-ttu-id="ff630-133">Ändern Sie ggf. das aktive Abonnement wie im nächsten Abschnitt beschrieben, oder geben Sie das Abonnement im Befehl an:</span><span class="sxs-lookup"><span data-stu-id="ff630-133">If necessary, change the active subscription, as described in the next section, or specify the subscription in the command:</span></span>

```azurecli
az storage account create --resource-group StorageGroups --subscription "My Demos" \
    --name storage136 --location eastus --sku Standard_LRS
```

## <a name="change-the-active-subscription"></a><span data-ttu-id="ff630-134">Ändern des aktiven Abonnements</span><span class="sxs-lookup"><span data-stu-id="ff630-134">Change the active subscription</span></span>

<span data-ttu-id="ff630-135">Sie können das aktive Abonnement mithilfe des Befehls [az account set](/cli/azure/account#az-account-set) ändern.</span><span class="sxs-lookup"><span data-stu-id="ff630-135">You can change your active subscription by using the [az account set](/cli/azure/account#az-account-set) command.</span></span>

<span data-ttu-id="ff630-136">Rufen Sie eine Liste Ihrer Abonnements mithilfe des Befehls [az account list](/cli/azure/account#az-account-list) ab.</span><span class="sxs-lookup"><span data-stu-id="ff630-136">Get a list of your subscriptions with the [az account list](/cli/azure/account#az-account-list) command:</span></span>

```azurecli
az account list --output table
```

<span data-ttu-id="ff630-137">Mit diesem Befehl werden alle Abonnements aufgelistet, auf die Sie zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="ff630-137">This command lists all the subscriptions you can access.</span></span> <span data-ttu-id="ff630-138">Ihr aktives Abonnement ist in der Spalte `IsDefault` durch `True` gekennzeichnet.</span><span class="sxs-lookup"><span data-stu-id="ff630-138">Your active subscription is marked as `True` in the `IsDefault` column.</span></span> <span data-ttu-id="ff630-139">Wenn ein erwartetes Abonnement nicht angezeigt wird, fügen Sie den Parameter `--refresh` hinzu, um die aktuelle Liste der Abonnements zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="ff630-139">If you don't see a subscription you expect, add the `--refresh` parameter to get the most current list of subscriptions.</span></span>

<span data-ttu-id="ff630-140">Um zu einem anderen Abonnement zu wechseln, verwenden Sie [az account set](/cli/azure/account#az-account-set) mit der ID oder dem Namen des gewünschten Abonnements.</span><span class="sxs-lookup"><span data-stu-id="ff630-140">To switch to a different subscription, use [az account set](/cli/azure/account#az-account-set) with the subscription ID or name you want to switch to.</span></span>

```azurecli
az account set --subscription "My Demos"
```

<span data-ttu-id="ff630-141">Ihre Abonnements verfügen sowohl über einen Namen als auch über eine ID (GUID).</span><span class="sxs-lookup"><span data-stu-id="ff630-141">Your subscriptions have both a name and an ID, which is a GUID.</span></span> <span data-ttu-id="ff630-142">Beides kann für diese Befehle verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="ff630-142">You can use either for these commands.</span></span> <span data-ttu-id="ff630-143">Verwenden Sie Anführungszeichen für einen Namen mit Leerzeichen.</span><span class="sxs-lookup"><span data-stu-id="ff630-143">If you use a name that includes spaces, use quotation marks.</span></span>

<span data-ttu-id="ff630-144">Wenn Sie den Befehl [az account list](/cli/azure/account#az-account-list) erneut ausführen, wird in der Spalte `IsDefault` ihr aktuelles aktives Abonnement angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ff630-144">If you run the [az account list](/cli/azure/account#az-account-list) command again, the `IsDefault` column shows your current active subscription.</span></span>

## <a name="create-management-groups"></a><span data-ttu-id="ff630-145">Erstellen von Verwaltungsgruppen</span><span class="sxs-lookup"><span data-stu-id="ff630-145">Create management groups</span></span>

<span data-ttu-id="ff630-146">Azure-Verwaltungsgruppen enthalten Abonnements.</span><span class="sxs-lookup"><span data-stu-id="ff630-146">Azure management groups contain subscriptions.</span></span> <span data-ttu-id="ff630-147">Verwaltungsgruppen ermöglichen die Verwaltung des Zugriffs, der Richtlinien und der Compliance für diese Abonnements.</span><span class="sxs-lookup"><span data-stu-id="ff630-147">Management groups provide a way to manage access, policies, and compliance for those subscriptions.</span></span> <span data-ttu-id="ff630-148">Weitere Informationen finden Sie unter [Was sind Azure-Verwaltungsgruppen?](/azure/governance/management-groups/overview).</span><span class="sxs-lookup"><span data-stu-id="ff630-148">For more information, see [What are Azure management groups](/azure/governance/management-groups/overview).</span></span>

<span data-ttu-id="ff630-149">Verwenden Sie die Befehle vom Typ [az account management-group](/cli/azure/account/management-group) zum Erstellen und Verwalten von Verwaltungsgruppen.</span><span class="sxs-lookup"><span data-stu-id="ff630-149">Use the [az account management-group](/cli/azure/account/management-group) commands to create and manage Azure Management Groups.</span></span>

<span data-ttu-id="ff630-150">Mithilfe des Befehls [az account management-group create](/cli/azure/account/management-group#az_account_management_group_create) können Sie eine Verwaltungsgruppe für mehrere Abonnements erstellen:</span><span class="sxs-lookup"><span data-stu-id="ff630-150">You can create a management group for several of your subscriptions by using the [az account management-group create](/cli/azure/account/management-group#az_account_management_group_create) command:</span></span>

```azurecli
az account management-group create --name Contoso01
```

<span data-ttu-id="ff630-151">Verwenden Sie zum Anzeigen aller Verwaltungsgruppen den Befehl [az account management-group list](/cli/azure/account/management-group#az_account_management_group_list):</span><span class="sxs-lookup"><span data-stu-id="ff630-151">To see all your management groups, use the [az account management-group list](/cli/azure/account/management-group#az_account_management_group_list) command:</span></span>

```azurecli
az account management-group list
```

<span data-ttu-id="ff630-152">Fügen Sie mithilfe des Befehls [az account management-group subscription add](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_add) Abonnements zur neuen Gruppe hinzu:</span><span class="sxs-lookup"><span data-stu-id="ff630-152">Add subscriptions to your new group by using the [az account management-group subscription add](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_add) command:</span></span>

```azurecli
az account management-group subscription add --name Contoso01 --subscription "My Demos"
az account management-group subscription add --name Contoso01 --subscription "My Second Demos"
```

<span data-ttu-id="ff630-153">Verwenden Sie zum Entfernen eines Abonnements den Befehl [az account management-group subscription remove](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_remove):</span><span class="sxs-lookup"><span data-stu-id="ff630-153">To remove a subscription, use the [az account management-group subscription remove](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_remove) command:</span></span>

```azurecli
az account management-group subscription remove --name Contoso01 --subscription "My Demos"
```

<span data-ttu-id="ff630-154">Führen Sie zum Entfernen einer Verwaltungsgruppe den Befehl [az account management-group delete](/cli/azure/account/management-group#az_account_management_group_delete) aus:</span><span class="sxs-lookup"><span data-stu-id="ff630-154">To remove a management group, run the [az account management-group delete](/cli/azure/account/management-group#az_account_management_group_delete) command:</span></span>

```azurecli
az account management-group delete --name Contoso01
```

<span data-ttu-id="ff630-155">Durch das Entfernen eines Abonnements oder das Löschen einer Verwaltungsgruppe wird ein Abonnement nicht gelöscht oder deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="ff630-155">Removing a subscription or deleting a management group doesn't delete or deactivate a subscription.</span></span>

## <a name="set-a-subscription-lock"></a><span data-ttu-id="ff630-156">Festlegen einer Abonnementsperre</span><span class="sxs-lookup"><span data-stu-id="ff630-156">Set a subscription lock</span></span>

<span data-ttu-id="ff630-157">Als Administrator müssen Sie ein Abonnement möglicherweise sperren, um zu verhindern, dass Benutzer es löschen oder ändern.</span><span class="sxs-lookup"><span data-stu-id="ff630-157">As an administrator, you may need to lock a subscription to prevent users from deleting or modifying it.</span></span> <span data-ttu-id="ff630-158">Weitere Informationen finden Sie unter [Sperren von Ressourcen, um unerwartete Änderungen zu verhindern](/azure/azure-resource-manager/management/lock-resources).</span><span class="sxs-lookup"><span data-stu-id="ff630-158">For more information, see [Lock resources to prevent unexpected changes](/azure/azure-resource-manager/management/lock-resources).</span></span>

<span data-ttu-id="ff630-159">Verwenden Sie in Azure CLI die Befehle vom Typ [az account lock](/cli/azure/account/lock).</span><span class="sxs-lookup"><span data-stu-id="ff630-159">In Azure CLI, use the [az account lock](/cli/azure/account/lock) commands.</span></span> <span data-ttu-id="ff630-160">Beispielsweise kann der Befehl [az account lock create](/cli/azure/account/lock#az_account_lock_create) Benutzer am Löschen eines Abonnements hindern:</span><span class="sxs-lookup"><span data-stu-id="ff630-160">For instance, the [az account lock create](/cli/azure/account/lock#az_account_lock_create) command can prevent users from deleting a subscription:</span></span>

```azurecli
az account lock create --name "Cannot delete subscription" --lock-type CanNotDelete
```

> [!NOTE]
> <span data-ttu-id="ff630-161">Sie müssen über die entsprechenden Berechtigungen verfügen, um Sperren erstellen oder ändern zu können.</span><span class="sxs-lookup"><span data-stu-id="ff630-161">You need to have appropriate permissions to create or change locks.</span></span>

<span data-ttu-id="ff630-162">Verwenden Sie zum Anzeigen der aktuellen Sperren für Ihr Abonnement den Befehl [az account lock list](/cli/azure/account/lock#az_account_lock_list):</span><span class="sxs-lookup"><span data-stu-id="ff630-162">To see the current locks on your subscription, use the [az account lock list](/cli/azure/account/lock#az_account_lock_list) command:</span></span>

```azurecli
az account lock list --output table
```

<span data-ttu-id="ff630-163">Wenn Sie ein Konto als schreibgeschützt festlegen, ähnelt das Ergebnis dem Zuweisen von Berechtigungen der Rolle „Leser“ für alle Benutzer.</span><span class="sxs-lookup"><span data-stu-id="ff630-163">If you make an account read-only, the result resembles assigning permissions of the Reader role to all users.</span></span> <span data-ttu-id="ff630-164">Weitere Informationen zum Festlegen von Berechtigungen für einzelne Benutzer und Rollen finden Sie unter [Hinzufügen oder Entfernen von Azure-Rollenzuweisungen mithilfe der Azure-Befehlszeilenschnittstelle](/azure/role-based-access-control/role-assignments-cli).</span><span class="sxs-lookup"><span data-stu-id="ff630-164">To learn about setting permissions for individual users and roles, see [Add or remove Azure role assignments using Azure CLI](/azure/role-based-access-control/role-assignments-cli).</span></span>

<span data-ttu-id="ff630-165">Verwenden Sie zum Anzeigen der Details für eine Sperre den Befehl [az account lock show](/cli/azure/account/lock#az_account_lock_show):</span><span class="sxs-lookup"><span data-stu-id="ff630-165">To see details for a lock, use the [az account lock show](/cli/azure/account/lock#az_account_lock_show) command:</span></span>

```azurecli
az account lock show --name "Cannot delete subscription"
```

<span data-ttu-id="ff630-166">Sie können eine Sperre mithilfe des Befehls [az account lock delete](/cli/azure/account/lock#az_account_lock_delete) entfernen:</span><span class="sxs-lookup"><span data-stu-id="ff630-166">You can remove a lock by using the [az account lock delete](/cli/azure/account/lock#az_account_lock_delete) command:</span></span>

```azurecli
az account lock delete --name "Cannot delete subscription"
```

## <a name="see-also"></a><span data-ttu-id="ff630-167">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="ff630-167">See also</span></span>

* [<span data-ttu-id="ff630-168">Microsoft Azure-Glossar: Ein Wörterbuch der Cloudterminologie auf der Azure Platform</span><span class="sxs-lookup"><span data-stu-id="ff630-168">Azure cloud terminology dictionary</span></span>](/azure/azure-glossary-cloud-terminology)
* [<span data-ttu-id="ff630-169">Zuordnen oder Hinzufügen eines Azure-Abonnements zu Ihrem Azure Active Directory-Mandanten</span><span class="sxs-lookup"><span data-stu-id="ff630-169">Associate or add an Azure subscription to your Azure Active Directory tenant</span></span>](/azure/active-directory/active-directory-how-subscriptions-associated-directory)
* [<span data-ttu-id="ff630-170">Anmelden mit der Azure CLI</span><span class="sxs-lookup"><span data-stu-id="ff630-170">Sign in with Azure CLI</span></span>](./authenticate-azure-cli.md)

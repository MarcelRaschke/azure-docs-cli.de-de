---
title: Azure CLI – Interaktiver Modus
description: Verwenden Sie die Azure CLI im interaktiven Modus.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 3a1cb95ecd851aca6eb5d0caf5bb0d2bfb4bf210
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/09/2020
ms.locfileid: "89562973"
---
# <a name="azure-cli-interactive-mode"></a><span data-ttu-id="e5289-103">Azure CLI – Interaktiver Modus</span><span class="sxs-lookup"><span data-stu-id="e5289-103">Azure CLI interactive mode</span></span>

<span data-ttu-id="e5289-104">Sie können die Azure CLI im interaktiven Modus verwenden, indem Sie den Befehl `az interactive` ausführen.</span><span class="sxs-lookup"><span data-stu-id="e5289-104">You can use Azure CLI in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="e5289-105">Bei diesem Modus arbeiten Sie in einer interaktiven Shell mit automatischer Vervollständigung, Befehlsbeschreibungen und Beispielen.</span><span class="sxs-lookup"><span data-stu-id="e5289-105">This mode places you in an interactive shell with auto-completion, command descriptions, and examples.</span></span>

![Interaktiver Modus](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="e5289-107">Wir verwenden hier nicht das Standarddesign, da es auf einem schwarzen Hintergrund nicht so gut lesbar ist.</span><span class="sxs-lookup"><span data-stu-id="e5289-107">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="e5289-108">Wenn Sie noch nicht bei Ihrem Konto angemeldet sind, verwenden Sie dazu den `login`-Befehl.</span><span class="sxs-lookup"><span data-stu-id="e5289-108">If you're not already signed in to your account, use the `login` command.</span></span>

## <a name="configure"></a><span data-ttu-id="e5289-109">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="e5289-109">Configure</span></span>

<span data-ttu-id="e5289-110">Im interaktiven Modus werden optional Beschreibungen zu Befehlen und Parametern sowie Befehlsbeispiele angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e5289-110">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="e5289-111">Über `F1` können Sie Beschreibungen und Beispiele aktivieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="e5289-111">Turn descriptions and examples on or off using `F1`.</span></span>

![Beschreibungen und Beispiele](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="e5289-113">Sie können die Anzeige von Standardwerten für Parameter über `F2` aktivieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="e5289-113">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![Standardwerte](./media/interactive-azure-cli/defaults.png)

<span data-ttu-id="e5289-115">`F3` schaltet die Anzeige einiger Tastenkombinationen ein oder aus.</span><span class="sxs-lookup"><span data-stu-id="e5289-115">`F3` toggles the display of some key gestures.</span></span>

![Tastenkombinationen](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="e5289-117">`Scope`</span><span class="sxs-lookup"><span data-stu-id="e5289-117">Scope</span></span>

<span data-ttu-id="e5289-118">Sie können den Bereich Ihres interaktiven Modus auf eine bestimmte Befehlsgruppe wie `vm` oder `vm image` festlegen.</span><span class="sxs-lookup"><span data-stu-id="e5289-118">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="e5289-119">In diesem Fall werden alle Befehle für diesen Bereich interpretiert.</span><span class="sxs-lookup"><span data-stu-id="e5289-119">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="e5289-120">Dies ist eine hervorragende Kompakteigenschaft, wenn Sie Ihre gesamte Arbeit in dieser Befehlsgruppe ausführen.</span><span class="sxs-lookup"><span data-stu-id="e5289-120">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="e5289-121">Statt diese Befehle einzugeben:</span><span class="sxs-lookup"><span data-stu-id="e5289-121">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="e5289-122">können Sie den Bereich auf die Befehlsgruppe „vm“ festlegen und folgende Befehle eingeben:</span><span class="sxs-lookup"><span data-stu-id="e5289-122">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="e5289-123">Sie können den Bereich auch auf Befehlsgruppen einer niedrigeren Ebene beschränken.</span><span class="sxs-lookup"><span data-stu-id="e5289-123">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="e5289-124">Mit `%%vm image` können Sie den Bereich auf `vm image` festlegen.</span><span class="sxs-lookup"><span data-stu-id="e5289-124">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="e5289-125">Da der Bereich bereits auf `vm` festgelegt ist, verwenden wir in diesem Fall `%%image`.</span><span class="sxs-lookup"><span data-stu-id="e5289-125">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="e5289-126">An diesem Punkt können wir den Bereich mit `%%..` wieder auf `vm` erweitern oder einfach mit `%%` auf das Stammverzeichnis festlegen.</span><span class="sxs-lookup"><span data-stu-id="e5289-126">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="e5289-127">Abfrage</span><span class="sxs-lookup"><span data-stu-id="e5289-127">Query</span></span>

<span data-ttu-id="e5289-128">Sie können eine JMESPath-Abfrage für die Ergebnisse des zuletzt ausgeführten Befehls ausführen, indem Sie `??` gefolgt von einer JMESPath-Abfrage verwenden.</span><span class="sxs-lookup"><span data-stu-id="e5289-128">You can execute a JMESPath query on the results of the last command that you executed by using `??`followed by a JMESPath query.</span></span>
<span data-ttu-id="e5289-129">Nach dem Erstellen einer Gruppe können Sie beispielsweise die ID der neuen Gruppe abrufen.</span><span class="sxs-lookup"><span data-stu-id="e5289-129">For example, after you created a group, you can retrieve the id of the new group.</span></span>

```azurecli
az>> group create -n myRG -l westEurope
az>> "?? id"
```

<span data-ttu-id="e5289-130">Mithilfe dieser Syntax können Sie auch das Ergebnis des vorherigen Befehls als Argument für den nächsten Befehl verwenden.\* Nach dem Auflisten aller Gruppen können Sie z. B. alle Ressourcen des Typs `virtualMachine` in der ersten Gruppe mit dem Standort „Europa, Westen“ auflisten.</span><span class="sxs-lookup"><span data-stu-id="e5289-130">You can also use this syntax to use the result of the previous command as an argument for your next command.\* For instance after having listed all groups, list all the resources of type `virtualMachine`on the first group whose location is westeurope.</span></span> 

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait -o json
az>> group list -o json
az>> resource list -g "?? [?location=='westeurope'].name | [0]" --query "[?type=='Microsoft.Compute/virtualMachines'].name
```

<span data-ttu-id="e5289-131">Weitere Informationen zum Abfragen der Ergebnisse Ihrer Befehle finden Sie unter [Abfragen von Befehlsergebnissen mit der Azure CLI](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e5289-131">To learn more about querying the results of your commands, see [Query command results with the Azure CLI](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="e5289-132">Bash-Befehle</span><span class="sxs-lookup"><span data-stu-id="e5289-132">Bash commands</span></span>

<span data-ttu-id="e5289-133">Mit `#[cmd]` können Sie Shellbefehle ausführen, ohne den interaktiven Modus zu verlassen.</span><span class="sxs-lookup"><span data-stu-id="e5289-133">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="e5289-134">Beispiele</span><span class="sxs-lookup"><span data-stu-id="e5289-134">Examples</span></span>

<span data-ttu-id="e5289-135">Für einige Befehle gibt es zahlreiche Beispiele.</span><span class="sxs-lookup"><span data-stu-id="e5289-135">Some commands have lots of examples.</span></span>
<span data-ttu-id="e5289-136">Mit `CTRL-N` können Sie zur nächsten und mit `CTRL-Y` zur vorherigen Seite mit Beispielen scrollen.</span><span class="sxs-lookup"><span data-stu-id="e5289-136">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![Beispiele](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="e5289-138">Über `::#` können Sie sich auch ein bestimmtes Beispiel ansehen.</span><span class="sxs-lookup"><span data-stu-id="e5289-138">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```

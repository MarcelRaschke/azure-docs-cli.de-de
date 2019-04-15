---
title: Azure CLI – Interaktiver Modus
description: Verwenden Sie die Azure CLI im interaktiven Modus.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: a325b799c7384037ae336093aa5274c7cbf53cbc
ms.sourcegitcommit: cf47338210116437d7dc0f6037d2dabd5c5e6a4b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/09/2019
ms.locfileid: "59429012"
---
# <a name="azure-cli-interactive-mode"></a><span data-ttu-id="a27f9-103">Azure CLI – Interaktiver Modus</span><span class="sxs-lookup"><span data-stu-id="a27f9-103">Azure CLI interactive mode</span></span>

<span data-ttu-id="a27f9-104">Sie können die Azure CLI im interaktiven Modus verwenden, indem Sie den Befehl `az interactive` ausführen.</span><span class="sxs-lookup"><span data-stu-id="a27f9-104">You can use Azure CLI in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="a27f9-105">Bei diesem Modus arbeiten Sie in einer interaktiven Shell mit automatischer Vervollständigung, Befehlsbeschreibungen und Beispielen.</span><span class="sxs-lookup"><span data-stu-id="a27f9-105">This mode places you in an interactive shell with auto-completion, command descriptions, and examples.</span></span>

![Interaktiver Modus](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="a27f9-107">Wir verwenden hier nicht das Standarddesign, da es auf einem schwarzen Hintergrund nicht so gut lesbar ist.</span><span class="sxs-lookup"><span data-stu-id="a27f9-107">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="a27f9-108">Wenn Sie noch nicht bei Ihrem Konto angemeldet sind, verwenden Sie dazu den `login`-Befehl.</span><span class="sxs-lookup"><span data-stu-id="a27f9-108">If you're not already signed in to your account, use the `login` command.</span></span>

## <a name="configure"></a><span data-ttu-id="a27f9-109">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="a27f9-109">Configure</span></span>

<span data-ttu-id="a27f9-110">Im interaktiven Modus werden optional Beschreibungen zu Befehlen und Parametern sowie Befehlsbeispiele angezeigt.</span><span class="sxs-lookup"><span data-stu-id="a27f9-110">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="a27f9-111">Über `F1` können Sie Beschreibungen und Beispiele aktivieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="a27f9-111">Turn descriptions and examples on or off using `F1`.</span></span>

![Beschreibungen und Beispiele](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="a27f9-113">Sie können die Anzeige von Standardwerten für Parameter über `F2` aktivieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="a27f9-113">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![Standardwerte](./media/interactive-azure-cli/defaults.png)

`F3` <span data-ttu-id="a27f9-115">schaltet die Anzeige einiger Tastenkombinationen ein oder aus.</span><span class="sxs-lookup"><span data-stu-id="a27f9-115">toggles the display of some key gestures.</span></span>

![Tastenkombinationen](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="a27f9-117">Bereich</span><span class="sxs-lookup"><span data-stu-id="a27f9-117">Scope</span></span>

<span data-ttu-id="a27f9-118">Sie können den Bereich Ihres interaktiven Modus auf eine bestimmte Befehlsgruppe wie `vm` oder `vm image` festlegen.</span><span class="sxs-lookup"><span data-stu-id="a27f9-118">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="a27f9-119">In diesem Fall werden alle Befehle für diesen Bereich interpretiert.</span><span class="sxs-lookup"><span data-stu-id="a27f9-119">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="a27f9-120">Dies ist eine hervorragende Kompakteigenschaft, wenn Sie Ihre gesamte Arbeit in dieser Befehlsgruppe ausführen.</span><span class="sxs-lookup"><span data-stu-id="a27f9-120">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="a27f9-121">Statt diese Befehle einzugeben:</span><span class="sxs-lookup"><span data-stu-id="a27f9-121">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="a27f9-122">können Sie den Bereich auf die Befehlsgruppe „vm“ festlegen und folgende Befehle eingeben:</span><span class="sxs-lookup"><span data-stu-id="a27f9-122">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="a27f9-123">Sie können den Bereich auch auf Befehlsgruppen einer niedrigeren Ebene beschränken.</span><span class="sxs-lookup"><span data-stu-id="a27f9-123">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="a27f9-124">Mit `%%vm image` können Sie den Bereich auf `vm image` festlegen.</span><span class="sxs-lookup"><span data-stu-id="a27f9-124">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="a27f9-125">Da der Bereich bereits auf `vm` festgelegt ist, verwenden wir in diesem Fall `%%image`.</span><span class="sxs-lookup"><span data-stu-id="a27f9-125">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="a27f9-126">An diesem Punkt können wir den Bereich mit `%%..` wieder auf `vm` erweitern oder einfach mit `%%` auf das Stammverzeichnis festlegen.</span><span class="sxs-lookup"><span data-stu-id="a27f9-126">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="a27f9-127">Abfragen</span><span class="sxs-lookup"><span data-stu-id="a27f9-127">Query</span></span>

<span data-ttu-id="a27f9-128">Sie können eine JMESPath-Abfrage für die Ergebnisse des zuletzt ausgeführten Befehls ausführen, indem Sie `??` gefolgt von einer JMESPath-Abfrage verwenden.</span><span class="sxs-lookup"><span data-stu-id="a27f9-128">You can execute a JMESPath query on the results of the last command that you executed by using `??`followed by a JMESPath query.</span></span>
<span data-ttu-id="a27f9-129">Nach dem Erstellen einer Gruppe können Sie beispielsweise die ID der neuen Gruppe abrufen.</span><span class="sxs-lookup"><span data-stu-id="a27f9-129">For example, after you created a group, you can retrieve the id of the new group.</span></span>

```azurecli
az>> group create -n myRG -l westEurope
az>> "?? id"
```

<span data-ttu-id="a27f9-130">Mithilfe dieser Syntax können Sie auch das Ergebnis des vorherigen Befehls als Argument für den nächsten Befehl verwenden.\* Nach dem Auflisten aller Gruppen können Sie z. B. alle Ressourcen des Typs `virtualMachine` in der ersten Gruppe mit dem Standort „Europa, Westen“ auflisten.</span><span class="sxs-lookup"><span data-stu-id="a27f9-130">You can also use this syntax to use the result of the previous command as an argument for your next command.\* For instance after having listed all groups, list all the resources of type `virtualMachine`on the first group whose location is westeurope.</span></span> 

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait -o json
az>> group list -o json
az>> resource list -g "?? [?location=='westeurope'].name | [0]" --query "[?type=='Microsoft.Compute/virtualMachines'].name
```

<span data-ttu-id="a27f9-131">Weitere Informationen zum Abfragen der Ergebnisse Ihrer Befehle finden Sie unter [Abfragen von Befehlsergebnissen mit der Azure CLI](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="a27f9-131">To learn more about querying the results of your commands, see [Query command results with the Azure CLI](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="a27f9-132">Bash-Befehle</span><span class="sxs-lookup"><span data-stu-id="a27f9-132">Bash commands</span></span>

<span data-ttu-id="a27f9-133">Mit `#[cmd]` können Sie Shellbefehle ausführen, ohne den interaktiven Modus zu verlassen.</span><span class="sxs-lookup"><span data-stu-id="a27f9-133">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="a27f9-134">Beispiele</span><span class="sxs-lookup"><span data-stu-id="a27f9-134">Examples</span></span>

<span data-ttu-id="a27f9-135">Für einige Befehle gibt es zahlreiche Beispiele.</span><span class="sxs-lookup"><span data-stu-id="a27f9-135">Some commands have lots of examples.</span></span>
<span data-ttu-id="a27f9-136">Mit `CTRL-N` können Sie zur nächsten und mit `CTRL-Y` zur vorherigen Seite mit Beispielen scrollen.</span><span class="sxs-lookup"><span data-stu-id="a27f9-136">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![Beispiele](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="a27f9-138">Über `::#` können Sie sich auch ein bestimmtes Beispiel ansehen.</span><span class="sxs-lookup"><span data-stu-id="a27f9-138">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```

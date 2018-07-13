---
title: Azure CLI 2.0 – Interaktiver Modus
description: Verwenden Sie die Azure CLI 2.0 im interaktiven Modus.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/06/2017
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 1ee7da8dfdde402d4d536f7ab4bb0599a8f3fa1d
ms.sourcegitcommit: fb3fed8701aff6c46af856e8fdc3e56ff9a678bc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/11/2018
ms.locfileid: "38229191"
---
# <a name="interactive-azure-cli-20"></a><span data-ttu-id="e040b-103">Interaktive Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="e040b-103">Interactive Azure CLI 2.0</span></span>

<span data-ttu-id="e040b-104">Sie können die Azure CLI 2.0 im interaktiven Modus verwenden, indem Sie den Befehl `az interactive` ausführen.</span><span class="sxs-lookup"><span data-stu-id="e040b-104">You can use Azure CLI 2.0 in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="e040b-105">So gelangen Sie zu einer interaktiven Shell, in der Ihre Befehle automatisch vervollständigt werden und in der Sie auf Beschreibungen von Befehlen und ihren Parametern sowie auf Befehlsbeispiele zugreifen können.</span><span class="sxs-lookup"><span data-stu-id="e040b-105">That places you in an interactive shell where your commands are auto-completed and you have access to descriptions of commands and their parameters and command examples.</span></span>

![Interaktiver Modus](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="e040b-107">Wir verwenden hier nicht das Standarddesign, da es auf einem schwarzen Hintergrund nicht so gut lesbar ist.</span><span class="sxs-lookup"><span data-stu-id="e040b-107">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="e040b-108">Wenn Sie noch nicht bei Ihrem Konto angemeldet sind, verwenden Sie dazu den `login`-Befehl.</span><span class="sxs-lookup"><span data-stu-id="e040b-108">If you're not already signed in to your account, use the `login` command.</span></span>

## <a name="configure"></a><span data-ttu-id="e040b-109">Konfigurieren</span><span class="sxs-lookup"><span data-stu-id="e040b-109">Configure</span></span>

<span data-ttu-id="e040b-110">Im interaktiven Modus werden optional Beschreibungen zu Befehlen und Parametern sowie Befehlsbeispiele angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e040b-110">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="e040b-111">Über `F1` können Sie Beschreibungen und Beispiele aktivieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="e040b-111">You can turn descriptions and examples on or off using `F1`.</span></span>

![Beschreibungen und Beispiele](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="e040b-113">Sie können die Anzeige von Standardwerten für Parameter über `F2` aktivieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="e040b-113">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![Standardwerte](./media/interactive-azure-cli/defaults.png)

<span data-ttu-id="e040b-115">`F3` schaltet die Anzeige einiger Tastenkombinationen ein oder aus.</span><span class="sxs-lookup"><span data-stu-id="e040b-115">`F3` toggles the display of some key gestures.</span></span>

![Tastenkombinationen](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="e040b-117">Umfang</span><span class="sxs-lookup"><span data-stu-id="e040b-117">Scope</span></span>

<span data-ttu-id="e040b-118">Sie können den Bereich Ihres interaktiven Modus auf eine bestimmte Befehlsgruppe wie `vm` oder `vm image` festlegen.</span><span class="sxs-lookup"><span data-stu-id="e040b-118">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="e040b-119">In diesem Fall werden alle Befehle für diesen Bereich interpretiert.</span><span class="sxs-lookup"><span data-stu-id="e040b-119">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="e040b-120">Dies ist eine hervorragende Kompakteigenschaft, wenn Sie Ihre gesamte Arbeit in dieser Befehlsgruppe ausführen.</span><span class="sxs-lookup"><span data-stu-id="e040b-120">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="e040b-121">Statt diese Befehle einzugeben:</span><span class="sxs-lookup"><span data-stu-id="e040b-121">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="e040b-122">können Sie den Bereich auf die Befehlsgruppe „vm“ festlegen und folgende Befehle eingeben:</span><span class="sxs-lookup"><span data-stu-id="e040b-122">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="e040b-123">Sie können den Bereich auch auf Befehlsgruppen einer niedrigeren Ebene beschränken.</span><span class="sxs-lookup"><span data-stu-id="e040b-123">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="e040b-124">Mit `%%vm image` können Sie den Bereich auf `vm image` festlegen.</span><span class="sxs-lookup"><span data-stu-id="e040b-124">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="e040b-125">Da der Bereich bereits auf `vm` festgelegt ist, verwenden wir in diesem Fall `%%image`.</span><span class="sxs-lookup"><span data-stu-id="e040b-125">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="e040b-126">An diesem Punkt können wir den Bereich mit `%%..` wieder auf `vm` erweitern oder einfach mit `%%` auf das Stammverzeichnis festlegen.</span><span class="sxs-lookup"><span data-stu-id="e040b-126">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="e040b-127">Abfragen</span><span class="sxs-lookup"><span data-stu-id="e040b-127">Query</span></span>

<span data-ttu-id="e040b-128">Sie können eine JMESPath-Abfrage für die Ergebnisse des zuletzt ausgeführten Befehls ausführen.</span><span class="sxs-lookup"><span data-stu-id="e040b-128">You can execute a JMESPath query on the results of the last command that you executed.</span></span>
<span data-ttu-id="e040b-129">Beispielsweise können Sie nach der Erstellung eines virtuellen Computers sicherstellen, dass er vollständig bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="e040b-129">For example, after you create a VM, you can make sure it has fully provisioned.</span></span>

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait
az>> ? [*].provisioningState
```

```output
[
  "Creating"
]
```

<span data-ttu-id="e040b-130">Weitere Informationen zum Abfragen der Ergebnisse Ihrer Befehle finden Sie unter [Verwenden von JMESPath-Abfragen mit Azure CLI 2.0](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e040b-130">To learn more about querying the results of your commands, see [Query command results with Azure 2.0](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="e040b-131">Bash-Befehle</span><span class="sxs-lookup"><span data-stu-id="e040b-131">Bash commands</span></span>

<span data-ttu-id="e040b-132">Mit `#[cmd]` können Sie Shellbefehle ausführen, ohne den interaktiven Modus zu verlassen.</span><span class="sxs-lookup"><span data-stu-id="e040b-132">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="e040b-133">Beispiele</span><span class="sxs-lookup"><span data-stu-id="e040b-133">Examples</span></span>

<span data-ttu-id="e040b-134">Für einige Befehle gibt es zahlreiche Beispiele.</span><span class="sxs-lookup"><span data-stu-id="e040b-134">Some commands have lots of examples.</span></span>
<span data-ttu-id="e040b-135">Mit `CTRL-N` können Sie zur nächsten und mit `CTRL-Y` zur vorherigen Seite mit Beispielen scrollen.</span><span class="sxs-lookup"><span data-stu-id="e040b-135">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![Beispiele](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="e040b-137">Über `::#` können Sie sich auch ein bestimmtes Beispiel ansehen.</span><span class="sxs-lookup"><span data-stu-id="e040b-137">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```

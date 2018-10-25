---
title: Manuelles Installieren der Azure CLI für Linux
description: Manuelles Installieren der Azure CLI unter Linux
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 38d32f62cbaff7d5f1bdf7fd52bf00d47e9e14b1
ms.sourcegitcommit: 6d9169ed547df151f99e5a3ac86578634486419a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/23/2018
ms.locfileid: "49652497"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="799ed-103">Manuelles Installieren der Azure CLI unter Linux</span><span class="sxs-lookup"><span data-stu-id="799ed-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="799ed-104">Ist kein Paket für die Azure CLI für Ihre Distribution vorhanden, installieren Sie die CLI manuell durch Ausführung eines Skripts.</span><span class="sxs-lookup"><span data-stu-id="799ed-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

> [!NOTE]
> <span data-ttu-id="799ed-105">Es wird dringend empfohlen, die CLI mit einem Paket-Manager zu installieren.</span><span class="sxs-lookup"><span data-stu-id="799ed-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="799ed-106">Ein Paket-Manager stellt sicher, dass Sie immer die neuesten Updates erhalten, und gewährleistet die Stabilität der CLI-Komponenten.</span><span class="sxs-lookup"><span data-stu-id="799ed-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="799ed-107">Überprüfen Sie vor der manuellen Installation, ob ein Paket für Ihre Distribution verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="799ed-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="799ed-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="799ed-108">Prerequisites</span></span>

<span data-ttu-id="799ed-109">Die CLI benötigt die folgende Software:</span><span class="sxs-lookup"><span data-stu-id="799ed-109">The CLI requires the following software:</span></span>

* [<span data-ttu-id="799ed-110">Python 2.7 oder Python 3.x</span><span class="sxs-lookup"><span data-stu-id="799ed-110">Python 2.7 or Python 3.x</span></span>](https://www.python.org/downloads/)
* [<span data-ttu-id="799ed-111">libffi</span><span class="sxs-lookup"><span data-stu-id="799ed-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="799ed-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="799ed-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

## <a name="install-or-update"></a><span data-ttu-id="799ed-113">Installieren oder Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="799ed-113">Install or update</span></span>

<span data-ttu-id="799ed-114">Sowohl für die Installation als auch die Aktualisierung der CLI muss das Installationsskript erneut ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="799ed-114">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="799ed-115">Installieren Sie die CLI durch Ausführen von `curl`.</span><span class="sxs-lookup"><span data-stu-id="799ed-115">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="799ed-116">Das Skript kann auch heruntergeladen und lokal ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="799ed-116">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="799ed-117">Unter Umständen müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="799ed-117">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="799ed-118">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="799ed-118">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="799ed-119">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="799ed-119">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="799ed-120">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="799ed-120">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="799ed-121">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="799ed-121">Troubleshooting</span></span>

<span data-ttu-id="799ed-122">In diesem Abschnitt werden einige allgemeine Probleme beschrieben, die bei einer manuellen Installation auftreten können.</span><span class="sxs-lookup"><span data-stu-id="799ed-122">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="799ed-123">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="799ed-123">If you experience a problem not covered here, [file an issue on github](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="799ed-124">curl-Fehler „Objekt verschoben“</span><span class="sxs-lookup"><span data-stu-id="799ed-124">curl "Object Moved" error</span></span>

<span data-ttu-id="799ed-125">Wenn Sie einen Fehler von `curl` im Zusammenhang mit dem `-L`-Parameter oder eine Fehlermeldung mit dem Text „Objekt verschoben“ erhalten, versuchen Sie, die vollständige URL anstatt der `aka.ms`-Umleitung zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="799ed-125">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="799ed-126">Der Befehl `az` wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="799ed-126">`az` command not found</span></span>

<span data-ttu-id="799ed-127">Wenn Sie den Befehl nicht ausführen können, nachdem Sie die Installation durchgeführt und `bash` oder `zsh` verwendet haben, leeren Sie den Befehlshash-Cache Ihrer Shell.</span><span class="sxs-lookup"><span data-stu-id="799ed-127">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="799ed-128">Ausführen</span><span class="sxs-lookup"><span data-stu-id="799ed-128">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="799ed-129">Überprüfen Sie, ob das Problem behoben wurde.</span><span class="sxs-lookup"><span data-stu-id="799ed-129">and check if the problem is resolved.</span></span>

<span data-ttu-id="799ed-130">Dieses Problem kann auch auftreten, wenn Sie die Shell nach der Installation nicht neu gestartet haben.</span><span class="sxs-lookup"><span data-stu-id="799ed-130">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="799ed-131">Stellen Sie sicher, dass sich der Befehl `az` in `$PATH` befindet.</span><span class="sxs-lookup"><span data-stu-id="799ed-131">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="799ed-132">Den Befehl `az` finden Sie hier:</span><span class="sxs-lookup"><span data-stu-id="799ed-132">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

## <a name="uninstall"></a><span data-ttu-id="799ed-133">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="799ed-133">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="799ed-134">Sie können die CLI deinstallieren, indem Sie die Dateien direkt aus dem Verzeichnis löschen, das Sie bei der Installation ausgewählt haben.</span><span class="sxs-lookup"><span data-stu-id="799ed-134">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="799ed-135">Das Standardinstallationsverzeichnis ist `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="799ed-135">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="799ed-136">Entfernen Sie die installierten CLI-Dateien.</span><span class="sxs-lookup"><span data-stu-id="799ed-136">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="799ed-137">Ändern Sie die Datei `$HOME/.bash_profile`, indem Sie die folgende Zeile entfernen:</span><span class="sxs-lookup"><span data-stu-id="799ed-137">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="799ed-138">Laden Sie bei Verwendung von `bash` oder `zsh` den Befehlscache Ihrer Shell neu.</span><span class="sxs-lookup"><span data-stu-id="799ed-138">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```

## <a name="next-steps"></a><span data-ttu-id="799ed-139">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="799ed-139">Next Steps</span></span>

<span data-ttu-id="799ed-140">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="799ed-140">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="799ed-141">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="799ed-141">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

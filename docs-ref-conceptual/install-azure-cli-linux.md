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
ms.devlang: azurecli
ms.openlocfilehash: caca30ec186f302e47f2978b9bfe616d4b2a5c02
ms.sourcegitcommit: 443e14098d6643cdb2e178847d1c79b1b95146ce
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/26/2019
ms.locfileid: "74543638"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="ca3e7-103">Manuelles Installieren der Azure CLI unter Linux</span><span class="sxs-lookup"><span data-stu-id="ca3e7-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="ca3e7-104">Ist kein Paket für die Azure CLI für Ihre Distribution vorhanden, installieren Sie die CLI manuell durch Ausführung eines Skripts.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> <span data-ttu-id="ca3e7-105">Es wird dringend empfohlen, die CLI mit einem Paket-Manager zu installieren.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="ca3e7-106">Ein Paket-Manager stellt sicher, dass Sie immer die neuesten Updates erhalten, und gewährleistet die Stabilität der CLI-Komponenten.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="ca3e7-107">Überprüfen Sie vor der manuellen Installation, ob ein Paket für Ihre Distribution verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca3e7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ca3e7-108">Prerequisites</span></span>

<span data-ttu-id="ca3e7-109">Die CLI benötigt die folgende Software:</span><span class="sxs-lookup"><span data-stu-id="ca3e7-109">The CLI requires the following software:</span></span>

* <span data-ttu-id="ca3e7-110">[Python 3.6.x oder 3.7.x](https://www.python.org/downloads/)</span><span class="sxs-lookup"><span data-stu-id="ca3e7-110">[Python 3.6.x or 3.7.x](https://www.python.org/downloads/).</span></span> 
* [<span data-ttu-id="ca3e7-111">libffi</span><span class="sxs-lookup"><span data-stu-id="ca3e7-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="ca3e7-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="ca3e7-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="ca3e7-113">Die CLI ist mit Python 2.7.x kompatibel, diese Version läuft am 1. Januar 2020 aus.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-113">The CLI is also compatible with Python 2.7.x, which is being end-of-lifed on January 1, 2020.</span></span> <span data-ttu-id="ca3e7-114">In zukünftigen Versionen der Azure CLI wird Python 2.7 nicht mehr unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-114">A future version of Azure CLI will drop support for Python 2.7.</span></span> <span data-ttu-id="ca3e7-115">Daher wird empfohlen, Python 3 zum Ausführen der CLI zu installieren.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-115">For this reason we recommend that you install Python 3 to run the CLI.</span></span> 

## <a name="install-or-update"></a><span data-ttu-id="ca3e7-116">Installieren oder Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ca3e7-116">Install or update</span></span>

<span data-ttu-id="ca3e7-117">Sowohl für die Installation als auch die Aktualisierung der CLI muss das Installationsskript erneut ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-117">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="ca3e7-118">Installieren Sie die CLI durch Ausführen von `curl`.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-118">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="ca3e7-119">Das Skript kann auch heruntergeladen und lokal ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-119">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="ca3e7-120">Unter Umständen müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-120">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="ca3e7-121">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-121">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="ca3e7-122">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-122">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="ca3e7-123">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="ca3e7-123">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="ca3e7-124">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="ca3e7-124">Troubleshooting</span></span>

<span data-ttu-id="ca3e7-125">In diesem Abschnitt werden einige allgemeine Probleme beschrieben, die bei einer manuellen Installation auftreten können.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-125">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="ca3e7-126">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="ca3e7-126">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="ca3e7-127">curl-Fehler „Objekt verschoben“</span><span class="sxs-lookup"><span data-stu-id="ca3e7-127">curl "Object Moved" error</span></span>

<span data-ttu-id="ca3e7-128">Wenn Sie einen Fehler von `curl` im Zusammenhang mit dem `-L`-Parameter oder eine Fehlermeldung mit dem Text „Objekt verschoben“ erhalten, versuchen Sie, die vollständige URL anstatt der `aka.ms`-Umleitung zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="ca3e7-128">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="ca3e7-129">Der Befehl `az` wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-129">`az` command not found</span></span>

<span data-ttu-id="ca3e7-130">Wenn Sie den Befehl nicht ausführen können, nachdem Sie die Installation durchgeführt und `bash` oder `zsh` verwendet haben, leeren Sie den Befehlshash-Cache Ihrer Shell.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-130">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="ca3e7-131">Ausführen</span><span class="sxs-lookup"><span data-stu-id="ca3e7-131">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="ca3e7-132">Überprüfen Sie, ob das Problem behoben wurde.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-132">and check if the problem is resolved.</span></span>

<span data-ttu-id="ca3e7-133">Dieses Problem kann auch auftreten, wenn Sie die Shell nach der Installation nicht neu gestartet haben.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-133">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="ca3e7-134">Stellen Sie sicher, dass sich der Befehl `az` in `$PATH` befindet.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-134">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="ca3e7-135">Den Befehl `az` finden Sie hier:</span><span class="sxs-lookup"><span data-stu-id="ca3e7-135">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="ca3e7-136">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-136">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="ca3e7-137">Zum Abrufen der Installationsskripts muss Ihr Proxy HTTPS-Verbindungen mit den folgenden Adressen zulassen:</span><span class="sxs-lookup"><span data-stu-id="ca3e7-137">In order to get the installation scripts, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* <span data-ttu-id="ca3e7-138">Endpunkte, die vom Paket-Manager Ihrer Distribution (sofern vorhanden) für Core-Pakete verwendet werden</span><span class="sxs-lookup"><span data-stu-id="ca3e7-138">Endpoints used by your distribution's package manager (if any) for core packages</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="ca3e7-139">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="ca3e7-139">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="ca3e7-140">Sie können die CLI deinstallieren, indem Sie die Dateien direkt aus dem Verzeichnis löschen, das Sie bei der Installation ausgewählt haben.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-140">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="ca3e7-141">Das Standardinstallationsverzeichnis ist `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-141">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="ca3e7-142">Entfernen Sie die installierten CLI-Dateien.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-142">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="ca3e7-143">Ändern Sie die Datei `$HOME/.bash_profile`, indem Sie die folgende Zeile entfernen:</span><span class="sxs-lookup"><span data-stu-id="ca3e7-143">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="ca3e7-144">Laden Sie bei Verwendung von `bash` oder `zsh` den Befehlscache Ihrer Shell neu.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-144">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```

## <a name="next-steps"></a><span data-ttu-id="ca3e7-145">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="ca3e7-145">Next Steps</span></span>

<span data-ttu-id="ca3e7-146">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="ca3e7-146">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="ca3e7-147">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="ca3e7-147">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

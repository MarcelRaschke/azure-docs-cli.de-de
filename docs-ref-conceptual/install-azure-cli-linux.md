---
title: Manuelles Installieren der Azure CLI für Linux
description: Manuelles Installieren der Azure CLI unter Linux
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 9a98da54f397c1fd03a7cc6b581a769afe84ef88
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2020
ms.locfileid: "77779583"
---
# <a name="install-azure-cli-on-linux-manually"></a><span data-ttu-id="75e40-103">Manuelles Installieren der Azure CLI unter Linux</span><span class="sxs-lookup"><span data-stu-id="75e40-103">Install Azure CLI on Linux manually</span></span>

<span data-ttu-id="75e40-104">Ist kein Paket für die Azure CLI für Ihre Distribution vorhanden, installieren Sie die CLI manuell durch Ausführung eines Skripts.</span><span class="sxs-lookup"><span data-stu-id="75e40-104">If there's no package for the Azure CLI for you your distribution, install the CLI manually by running a script.</span></span>

[!INCLUDE [current-version](includes/current-version.md)]

> [!NOTE]
> <span data-ttu-id="75e40-105">Es wird dringend empfohlen, die CLI mit einem Paket-Manager zu installieren.</span><span class="sxs-lookup"><span data-stu-id="75e40-105">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="75e40-106">Ein Paket-Manager stellt sicher, dass Sie immer die neuesten Updates erhalten, und gewährleistet die Stabilität der CLI-Komponenten.</span><span class="sxs-lookup"><span data-stu-id="75e40-106">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="75e40-107">Überprüfen Sie vor der manuellen Installation, ob ein Paket für Ihre Distribution verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="75e40-107">Check and see if there is a package for your distribution before installing manually.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75e40-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="75e40-108">Prerequisites</span></span>

<span data-ttu-id="75e40-109">Die CLI benötigt die folgende Software:</span><span class="sxs-lookup"><span data-stu-id="75e40-109">The CLI requires the following software:</span></span>

* <span data-ttu-id="75e40-110">[Python 3.6.x, 3.7.x oder 3.8.x](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="75e40-110">[Python 3.6.x, 3.7.x or 3.8.x](https://www.python.org/downloads/).</span></span> 
* [<span data-ttu-id="75e40-111">libffi</span><span class="sxs-lookup"><span data-stu-id="75e40-111">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="75e40-112">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="75e40-112">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="75e40-113">Die CLI unterstützt Python 2.7 seit Version `2.1.0` nicht mehr.</span><span class="sxs-lookup"><span data-stu-id="75e40-113">The CLI has dropped support for Python 2.7 since version `2.1.0`.</span></span> <span data-ttu-id="75e40-114">Bei neuen Versionen wird die ordnungsgemäße Ausführung mit Python 2.7 nicht mehr garantiert.</span><span class="sxs-lookup"><span data-stu-id="75e40-114">New versions no longer guarantee to run with Python 2.7 correctly.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="75e40-115">Installieren oder Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="75e40-115">Install or update</span></span>

<span data-ttu-id="75e40-116">Sowohl für die Installation als auch die Aktualisierung der CLI muss das Installationsskript erneut ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="75e40-116">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="75e40-117">Installieren Sie die CLI durch Ausführen von `curl`.</span><span class="sxs-lookup"><span data-stu-id="75e40-117">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="75e40-118">Das Skript kann auch heruntergeladen und lokal ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="75e40-118">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="75e40-119">Unter Umständen müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="75e40-119">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="75e40-120">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="75e40-120">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="75e40-121">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="75e40-121">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](includes/interactive-login.md)]

<span data-ttu-id="75e40-122">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="75e40-122">To learn more about different authentication methods, see [Sign in with Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="75e40-123">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="75e40-123">Troubleshooting</span></span>

<span data-ttu-id="75e40-124">In diesem Abschnitt werden einige allgemeine Probleme beschrieben, die bei einer manuellen Installation auftreten können.</span><span class="sxs-lookup"><span data-stu-id="75e40-124">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="75e40-125">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="75e40-125">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="75e40-126">curl-Fehler „Objekt verschoben“</span><span class="sxs-lookup"><span data-stu-id="75e40-126">curl "Object Moved" error</span></span>

<span data-ttu-id="75e40-127">Wenn Sie einen Fehler von `curl` im Zusammenhang mit dem `-L`-Parameter oder eine Fehlermeldung mit dem Text „Objekt verschoben“ erhalten, versuchen Sie, die vollständige URL anstatt der `aka.ms`-Umleitung zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="75e40-127">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="75e40-128">Der Befehl `az` wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="75e40-128">`az` command not found</span></span>

<span data-ttu-id="75e40-129">Wenn Sie den Befehl nicht ausführen können, nachdem Sie die Installation durchgeführt und `bash` oder `zsh` verwendet haben, leeren Sie den Befehlshash-Cache Ihrer Shell.</span><span class="sxs-lookup"><span data-stu-id="75e40-129">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="75e40-130">Ausführen</span><span class="sxs-lookup"><span data-stu-id="75e40-130">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="75e40-131">Überprüfen Sie, ob das Problem behoben wurde.</span><span class="sxs-lookup"><span data-stu-id="75e40-131">and check if the problem is resolved.</span></span>

<span data-ttu-id="75e40-132">Dieses Problem kann auch auftreten, wenn Sie die Shell nach der Installation nicht neu gestartet haben.</span><span class="sxs-lookup"><span data-stu-id="75e40-132">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="75e40-133">Stellen Sie sicher, dass sich der Befehl `az` in `$PATH` befindet.</span><span class="sxs-lookup"><span data-stu-id="75e40-133">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="75e40-134">Den Befehl `az` finden Sie hier:</span><span class="sxs-lookup"><span data-stu-id="75e40-134">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="75e40-135">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="75e40-135">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

<span data-ttu-id="75e40-136">Zum Abrufen der Installationsskripts muss Ihr Proxy HTTPS-Verbindungen mit den folgenden Adressen zulassen:</span><span class="sxs-lookup"><span data-stu-id="75e40-136">In order to get the installation scripts, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* <span data-ttu-id="75e40-137">Endpunkte, die vom Paket-Manager Ihrer Distribution (sofern vorhanden) für Core-Pakete verwendet werden</span><span class="sxs-lookup"><span data-stu-id="75e40-137">Endpoints used by your distribution's package manager (if any) for core packages</span></span>

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="75e40-138">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="75e40-138">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

<span data-ttu-id="75e40-139">Sie können die CLI deinstallieren, indem Sie die Dateien direkt aus dem Verzeichnis löschen, das Sie bei der Installation ausgewählt haben.</span><span class="sxs-lookup"><span data-stu-id="75e40-139">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="75e40-140">Das Standardinstallationsverzeichnis ist `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="75e40-140">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="75e40-141">Entfernen Sie die installierten CLI-Dateien.</span><span class="sxs-lookup"><span data-stu-id="75e40-141">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="75e40-142">Ändern Sie die Datei `$HOME/.bash_profile`, indem Sie die folgende Zeile entfernen:</span><span class="sxs-lookup"><span data-stu-id="75e40-142">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="75e40-143">Laden Sie bei Verwendung von `bash` oder `zsh` den Befehlscache Ihrer Shell neu.</span><span class="sxs-lookup"><span data-stu-id="75e40-143">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```

## <a name="next-steps"></a><span data-ttu-id="75e40-144">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="75e40-144">Next Steps</span></span>

<span data-ttu-id="75e40-145">Machen Sie sich nach der Installation der Azure-Befehlszeilenschnittstelle kurz mit den Features sowie mit häufig verwendeten Befehlen vertraut.</span><span class="sxs-lookup"><span data-stu-id="75e40-145">Now that you've installed the Azure CLI, take a short tour of its features and common commands.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="75e40-146">Erste Schritte mit Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="75e40-146">Get started with the Azure CLI</span></span>](get-started-with-azure-cli.md)

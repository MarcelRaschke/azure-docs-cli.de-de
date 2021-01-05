---
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 12/15/2020
ms.topic: include
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 2cba7031b3fe4c54edcb7c0dcef6f37b97d2f785
ms.sourcegitcommit: d5f026468ea20bbd7ef35bdbf9852bcb2b812d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/23/2020
ms.locfileid: "97744615"
---
## <a name="overview"></a><span data-ttu-id="a8a8b-101">Übersicht</span><span class="sxs-lookup"><span data-stu-id="a8a8b-101">Overview</span></span>

> [!NOTE]
> <span data-ttu-id="a8a8b-102">Es wird dringend empfohlen, die CLI mit einem Paket-Manager zu installieren.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-102">It's strongly recommend to install the CLI with a package manager.</span></span> <span data-ttu-id="a8a8b-103">Ein Paket-Manager stellt sicher, dass Sie immer die neuesten Updates erhalten, und gewährleistet die Stabilität der CLI-Komponenten.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-103">A package manager makes sure you always get the latest updates, and guarantees the stability of CLI components.</span></span> <span data-ttu-id="a8a8b-104">Überprüfen Sie vor der manuellen Installation, ob ein Paket für Ihre Distribution verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-104">Check and see if there is a package for your distribution before installing manually.</span></span>

<span data-ttu-id="a8a8b-105">Die CLI benötigt die folgende Software:</span><span class="sxs-lookup"><span data-stu-id="a8a8b-105">The CLI requires the following software:</span></span>

* <span data-ttu-id="a8a8b-106">[Python 3.6.x, 3.7.x oder 3.8.x](https://www.python.org/downloads/).</span><span class="sxs-lookup"><span data-stu-id="a8a8b-106">[Python 3.6.x, 3.7.x or 3.8.x](https://www.python.org/downloads/).</span></span>
* [<span data-ttu-id="a8a8b-107">libffi</span><span class="sxs-lookup"><span data-stu-id="a8a8b-107">libffi</span></span>](https://sourceware.org/libffi/)
* [<span data-ttu-id="a8a8b-108">OpenSSL 1.0.2</span><span class="sxs-lookup"><span data-stu-id="a8a8b-108">OpenSSL 1.0.2</span></span>](https://www.openssl.org/source/)

> [!IMPORTANT]
>
> <span data-ttu-id="a8a8b-109">Die CLI unterstützt Python 2.7 seit Version `2.1.0` nicht mehr.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-109">The CLI has dropped support for Python 2.7 since version `2.1.0`.</span></span> <span data-ttu-id="a8a8b-110">Bei neuen Versionen wird die ordnungsgemäße Ausführung mit Python 2.7 nicht mehr garantiert.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-110">New versions no longer guarantee to run with Python 2.7 correctly.</span></span>

## <a name="install-or-update"></a><span data-ttu-id="a8a8b-111">Installieren oder Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a8a8b-111">Install or update</span></span>

<span data-ttu-id="a8a8b-112">Sowohl für die Installation als auch die Aktualisierung der CLI muss das Installationsskript erneut ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-112">Both installing and updating the CLI requires re-running the install script.</span></span> <span data-ttu-id="a8a8b-113">Installieren Sie die CLI durch Ausführen von `curl`.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-113">Install the CLI by running `curl`.</span></span>

```bash
curl -L https://aka.ms/InstallAzureCli | bash
```

<span data-ttu-id="a8a8b-114">Das Skript kann auch heruntergeladen und lokal ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-114">The script can also be downloaded and run locally.</span></span> <span data-ttu-id="a8a8b-115">Unter Umständen müssen Sie Ihre Shell neu starten, damit einige Änderungen wirksam werden.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-115">You may have to restart your shell in order for changes to take effect.</span></span>

<span data-ttu-id="a8a8b-116">Sie können dann die Azure CLI mit dem Befehl `az` ausführen.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-116">You can then run the Azure CLI with the `az` command.</span></span> <span data-ttu-id="a8a8b-117">Verwenden Sie den Befehl [az login](/cli/azure/reference-index#az-login), um sich anzumelden.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-117">To sign in, use [az login](/cli/azure/reference-index#az-login) command.</span></span>

[!INCLUDE [interactive-login](interactive-login.md)]

<span data-ttu-id="a8a8b-118">Weitere Informationen zu verschiedenen Authentifizierungsmethoden finden Sie unter [Anmelden mit der Azure CLI](../authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="a8a8b-118">To learn more about different authentication methods, see [Sign in with Azure CLI](../authenticate-azure-cli.md).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="a8a8b-119">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="a8a8b-119">Troubleshooting</span></span>

<span data-ttu-id="a8a8b-120">In diesem Abschnitt werden einige allgemeine Probleme beschrieben, die bei einer manuellen Installation auftreten können.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-120">Here are some common problems seen during a manual installation.</span></span> <span data-ttu-id="a8a8b-121">Falls ein Problem auftritt, das hier nicht behandelt wird, [melden Sie es auf GitHub](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="a8a8b-121">If you experience a problem not covered here, [file an issue on GitHub](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="a8a8b-122">curl-Fehler „Objekt verschoben“</span><span class="sxs-lookup"><span data-stu-id="a8a8b-122">curl "Object Moved" error</span></span>

<span data-ttu-id="a8a8b-123">Wenn Sie einen Fehler von `curl` im Zusammenhang mit dem `-L`-Parameter oder eine Fehlermeldung mit dem Text „Objekt verschoben“ erhalten, versuchen Sie, die vollständige URL anstatt der `aka.ms`-Umleitung zu verwenden:</span><span class="sxs-lookup"><span data-stu-id="a8a8b-123">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="a8a8b-124">Der Befehl `az` wurde nicht gefunden.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-124">`az` command not found</span></span>

<span data-ttu-id="a8a8b-125">Wenn Sie den Befehl nicht ausführen können, nachdem Sie die Installation durchgeführt und `bash` oder `zsh` verwendet haben, leeren Sie den Befehlshash-Cache Ihrer Shell.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-125">If you can't run the command after installation and using `bash` or `zsh`, clear your shell's command hash cache.</span></span> <span data-ttu-id="a8a8b-126">Ausführen</span><span class="sxs-lookup"><span data-stu-id="a8a8b-126">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="a8a8b-127">Überprüfen Sie, ob das Problem behoben wurde.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-127">and check if the problem is resolved.</span></span>

<span data-ttu-id="a8a8b-128">Dieses Problem kann auch auftreten, wenn Sie die Shell nach der Installation nicht neu gestartet haben.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-128">The issue can also occur if you didn't restart your shell after installation.</span></span> <span data-ttu-id="a8a8b-129">Stellen Sie sicher, dass sich der Befehl `az` in `$PATH` befindet.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-129">Make sure that the location of the `az` command is in your `$PATH`.</span></span> <span data-ttu-id="a8a8b-130">Den Befehl `az` finden Sie hier:</span><span class="sxs-lookup"><span data-stu-id="a8a8b-130">The location of the `az` command is</span></span>

```bash
<install path>/bin
```

### <a name="proxy-blocks-connection"></a><span data-ttu-id="a8a8b-131">Der Proxy blockiert die Verbindung.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-131">Proxy blocks connection</span></span>

[!INCLUDE[configure-proxy](configure-proxy.md)]

<span data-ttu-id="a8a8b-132">Zum Abrufen der Installationsskripts muss Ihr Proxy HTTPS-Verbindungen mit den folgenden Adressen zulassen:</span><span class="sxs-lookup"><span data-stu-id="a8a8b-132">In order to get the installation scripts, your proxy needs to allow HTTPS connections to the following addresses:</span></span>

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`
* `https://pypi.python.org`
* <span data-ttu-id="a8a8b-133">Endpunkte, die vom Paket-Manager Ihrer Distribution (sofern vorhanden) für Core-Pakete verwendet werden</span><span class="sxs-lookup"><span data-stu-id="a8a8b-133">Endpoints used by your distribution's package manager (if any) for core packages</span></span>

[!INCLUDE[troubleshoot-wsl.md](troubleshoot-wsl.md)]

## <a name="uninstall"></a><span data-ttu-id="a8a8b-134">Deinstallieren</span><span class="sxs-lookup"><span data-stu-id="a8a8b-134">Uninstall</span></span>

[!INCLUDE [uninstall-boilerplate.md](uninstall-boilerplate.md)]

<span data-ttu-id="a8a8b-135">Sie können die CLI deinstallieren, indem Sie die Dateien direkt aus dem Verzeichnis löschen, das Sie bei der Installation ausgewählt haben.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-135">Uninstall the CLI by directly deleting the files from the location chosen at the time of installation.</span></span> <span data-ttu-id="a8a8b-136">Das Standardinstallationsverzeichnis ist `$HOME`.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-136">The default install location is `$HOME`.</span></span>

1. <span data-ttu-id="a8a8b-137">Entfernen Sie die installierten CLI-Dateien.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-137">Remove the installed CLI files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="a8a8b-138">Ändern Sie die Datei `$HOME/.bash_profile`, indem Sie die folgende Zeile entfernen:</span><span class="sxs-lookup"><span data-stu-id="a8a8b-138">Modify your `$HOME/.bash_profile` file to remove the following line:</span></span>

   ```text
   <install location>/lib/azure-cli/az.completion
   ```

3. <span data-ttu-id="a8a8b-139">Laden Sie bei Verwendung von `bash` oder `zsh` den Befehlscache Ihrer Shell neu.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-139">If using `bash` or `zsh`, reload your shell's command cache.</span></span>

   ```bash
   hash -r
   ```
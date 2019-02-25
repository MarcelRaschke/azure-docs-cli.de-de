---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/26/2018
ms.topic: include
ms.openlocfilehash: ee0b2b0c8c557aa54255f28429bb3a174c0e21a9
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158410"
---
### <a name="cli-fails-to-install-or-run-on-windows-subsystem-for-linux"></a>Die CLI kann auf dem Windows-Subsystem für Linux nicht installiert oder ausgeführt werden.

Das [Windows-Subsystem für Linux (WSL)](/windows/wsl/about) ist eine Übersetzungsebene für Systemaufrufe, die auf der Windows-Plattform basiert. Daher tritt unter Umständen ein Fehler auf, wenn Sie die Azure CLI installieren oder ausführen. Die CLI nutzt einige Features, die in WSL unter Umständen einen Fehler enthalten. Falls unabhängig von der Art der CLI-Installation ein Fehler auftritt, ist die Wahrscheinlichkeit hoch, dass ein Problem mit dem WSL und nicht mit dem CLI-Installationsvorgang vorliegt.

So beheben Sie Probleme mit Ihrer WSL-Installation und ggf andere Probleme:

* Führen Sie möglichst den gleichen Installationsvorgang auf einem Linux-Computer oder einem virtuellen Computer aus, um zu sehen, ob er erfolgreich ist. Ist dies der Fall, hängt das Problem mit hoher Wahrscheinlichkeit mit WSL zusammen. Informationen zum Starten eines virtuellen Linux-Computers in Azure finden Sie in der Dokumentation zum [Erstellen eines virtuellen Linux-Computers im Azure-Portal](/azure/virtual-machines/linux/quick-create-portal).
* Stellen Sie sicher, dass die neueste Version von WSL ausgeführt wird. Um die aktuelle Version zu erhalten, [aktualisieren Sie Ihre Windows 10-Installation](https://support.microsoft.com/help/4027667/windows-10-update).
* Suchen Sie nach [offenen Problemen](https://github.com/Microsoft/WSL/issues) mit WSL. Mithilfe dieser Informationen kann Ihr Problem vielleicht behoben werden.
  Häufig finden Sie Vorschläge, wie Sie das Problem umgehen, bzw. Informationen zu einem Release, in dem das Problem behoben wird.
* Gibt es noch keinen Eintrag für Ihr Problem, [melden Sie ein neues Problem mit WSL](https://github.com/Microsoft/WSL/issues/new), und geben Sie dabei möglichst viele Details an.

Treten beim Installieren oder Ausführen auf dem WSL weiterhin Probleme auf, ziehen Sie die [Installation der CLI für Windows](../install-azure-cli-windows.md) in Betracht.

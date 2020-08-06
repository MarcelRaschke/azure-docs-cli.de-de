---
title: Azure CLI-Referenzen für das Azure-Netzwerk
description: Landing Page der Azure CLI-Referenzen für das Azure-Netzwerk
author: dbradish-microsoft
manager: barbkess
ms.devlang: azurecli
ms.topic: reference
ms.date: 06/30/2020
ms.author: dbradish
ms.service: azure-cli
ms.reviewer: mohnader
ms.openlocfilehash: b86d29d700437925390157af2f4379775de40350
ms.sourcegitcommit: 7668cbf8b9fab82c3a4506cbc70e70392f149d12
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/31/2020
ms.locfileid: "87455541"
---
# <a name="azure-cli-for-azure-network"></a>Azure CLI für das Azure-Netzwerk

Die Azure-Befehlszeilenschnittstelle ([Azure CLI](/cli/azure/what-is-azure-cli)) setzt sich aus Befehlen zum Erstellen und Verwalten von Azure-Ressourcen zusammen.  Die CLI steht in vielen Azure-Diensten zur Verfügung – unter anderem auch im Azure-Netzwerk, um die Verwaltung von Netzwerkdiensten über die Befehlszeile zu ermöglichen.

## <a name="references-for-azure-network"></a>Referenzen für das Azure-Netzwerk

Die Azure-Netzwerk-CLI umfasst zwei Komponenten: **Kern** und **Erweiterung**.  Die Befehle der Azure CLI-Kernkomponente sind standardmäßig in der CLI enthalten und werden vollständig unterstützt.  Eine Erweiterung ermöglicht den Zugriff auf experimentelle und vorab veröffentlichte Befehle und muss vor der Verwendung installiert werden.  Beispielinstallationsskripts finden Sie unter [Installieren von Erweiterungspaketen](#installing-extension-references).

Unter [az network](/cli/azure/network) finden Sie eine vollständige Liste der Azure CLI-Kernreferenzen für das Azure-Netzwerk.  Über die weiter unten bereitgestellten Links gelangen Sie zu Erweiterungsreferenzen.

### <a name="virtual-network"></a>Virtuelles Netzwerk

| Untergruppe | Verweis | Zweck | Ist Erweiterung
|-|-|-|-|
| Appliance | [az network virtual-appliance](/cli/azure/network/virtual-appliance) | Verwalten eines virtuellen Netzwerkgeräts
| DNS | [az network private-dns](/cli/azure/network/private-dns) | Verwalten von Domänen vom Typ „Privates DNS“ in Azure |
| Endpunkt | [az network service-endpoint](/cli/azure/network/service-endpoint) | Verwalten von Richtlinien im Zusammenhang mit Dienstendpunkten |
| NAT | [az network nat](/cli/azure/network/nat) | Verwalten von NAT-Ressourcen (Network Address Translation, Netzwerkadressenübersetzung) |
| NIC | [az network nic](/cli/azure/network/nic) | Verwalten von Netzwerkschnittstellen |
| Peering | [az peering](/cli/azure/ext/peering/peering) | Verwalten des Peerings | ja
| Profil | [az network profile](/cli/azure/network/profile) | Verwalten von Netzwerkprofilen |
| Route | [az network route-filter](/cli/azure/network/route-filter) | Verwalten von Routenfiltern |
| Route | [az network route-table](/cli/azure/network/route-table) | Verwalten von Routingtabellen |
| VMware | [az network vmware](/cli/azure/ext/vmware/vmware) | Befehle zum Verwalten von Azure VMware Solution-Instanzen | ja
| vNet | [az network vnet](/cli/azure/network/vnet) | Verwalten virtueller Azure-Netzwerke |
| vNet | [az network vnet-tap](/cli/azure/ext/virtual-network-tap/network/vnet/tap) | Verwalten von TAPs für virtuelle Netzwerke | ja
| vNet | [az network vnet-gateway](/cli/azure/network/vnet-gateway) | Verwenden eines Azure-Gateways für virtuelle Netzwerke für sichere, standortübergreifende Konnektivität |

### <a name="wan-and-on-premise-connectivity"></a>WAN und lokale Konnektivität

| Untergruppe | Verweis | Zweck | Ist Erweiterung
|-|-|-|-|
| Querverbindung | [az network cross-connection](/cli/azure/ext/express-route-cross-connection/network/cross-connection) | Verwalten von Azure-Netzwerkressourcen | ja
| ExpressRoute | [az network express-route](/cli/azure/network/express-route) | Verwalten von Azure-IoT-Hubs |
| vHub | [az network vhub](/cli/azure/ext/virtual-wan/network/vhub) | Verwalten virtueller Hubs | ja
| VPN | [az network vpn-connection](/cli/azure/network/vpn-connection) | Verwalten von VPN-Verbindungen |
| VPN | [az network vpn-gateway](/cli/azure/ext/virtual-wan/network/vpn-gateway) | Verwalten von VPN-Gateways | ja
| VPN | [az network vpn-site](/cli/azure/ext/virtual-wan/network/vpn-site) | Verwalten von VPN-Standortkonfigurationen | ja
| vRouter | [az network vrouter](/cli/azure/network/vrouter) | Verwalten des virtuellen Routers |
| vWAN | [az network vwan](/cli/azure/ext/virtual-wan/network/vwan) | Verwalten virtueller WANs | ja

### <a name="load-balancing-and-ip"></a>Lastenausgleich und IP

| Untergruppe | Verweis | Zweck | Ist Erweiterung
|-|-|-|-|
| Application Gateway | [az network application-gateway](/cli/azure/network/application-gateway) | Verwalten von Routing- und Lastenausgleichsdienste auf der Anwendungsebene |
| Lastenausgleich | [az network lb](/cli/azure/network/lb) | Verwalten und Konfigurieren von Lastenausgleichsmodulen |
| IP | [az network ip-group](/cli/azure/ext/ip-group/network/ip-group) | Verwalten von IP-Adressgruppen | ja
| IP | [az network public-ip](/cli/azure/network/public-ip) | Verwalten öffentlicher IP-Adressen |
| Front Door | [az network front-door](/cli/azure/ext/front-door/network/front-door) | Verwalten von Front Door-Netzwerkressourcen | ja
| Lokales Gateway | [az network local-gateway](/cli/azure/network/local-gateway) | Verwalten lokaler Gateways |
| Traffic Manager | [az network traffic-manager](/cli/azure/network/traffic-manager) | Verwalten des Routings von eingehendem Datenverkehr |

### <a name="security"></a>Sicherheit

| Untergruppe | Verweis | Zweck | Ist Erweiterung
|-|-|-|-|
| ASG | [az asg](/cli/azure/network/asg) | Verwalten von Anwendungssicherheitsgruppen |
| Bastion | [az network bastion](/cli/azure/network/bastion) | Verwalten des Azure Bastion-Hosts |
| DDoS | [az network ddos-protection](/cli/azure/network/ddos-protection) | Verwalten von DDoS Protection-Plänen |
| Firewall | [az network firewall](/cli/azure/ext/azure-firewall/network/firewall) | Verwalten und Konfigurieren von Azure Firewall-Instanzen | ja
| Firewall | [az network security-partner-provider](/cli/azure/network/security-partner-provider) | Verwalten des Azure-Sicherheitspartneranbieters |
| NSG | [az network nsg](/cli/azure/network/nsg)| Verwalten von Azure-Netzwerksicherheitsgruppen |
| Privater Endpunkt | [az network private-endpoint](/cli/azure/network/private-endpoint) | Verwalten privater Endpunkte |
| Privater Endpunkt | [az network private-endpoint-connection](/cli/azure/network/private-endpoint-connection) | Verwalten von Verbindungen mit privaten Endpunkten |
| Private Link | [az network private-link-resource](/cli/azure/network/private-link-resource) | Verwalten von Private Link-Ressourcen |
| Private Link | [az network private-link-service](/cli/azure/network/private-link-service) | Verwalten von Private Link-Diensten |

### <a name="monitoring"></a>Überwachung

| Untergruppe | Verweis | Zweck | Ist Erweiterung
|-|-|-|-|
| Watcher | [az network watcher](/cli/azure/network/watcher) | Verwalten von Azure Network Watcher |

### <a name="list"></a>List

| Untergruppe | Verweis | Zweck | Ist Erweiterung
|-|-|-|-|
| Dienst | [az network list-service-aliases](/cli/azure/network#az-network-list-service-aliases) | Auflisten verfügbarer Dienstaliase in der Region, die für Dienstendpunkt-Richtlinien verwendet werden können |
| Dienst | [az network list-service-tags](/cli/azure/network#az-network-list-service-tags) | Auflisten aller Diensttags, die zu unterschiedlichen Ressourcen gehören |
| Verwendung | [az network list-usages](/cli/azure/network#az-network-list-usages) | Auflisten der Anzahl von Netzwerkressourcen in einer Region, die im Rahmen eines Abonnementkontingents verwendet werden |

## <a name="installing-extension-references"></a>Installieren von Erweiterungspaketen

Azure CLI-Erweiterungsreferenzen müssen vor der Verwendung installiert werden.  Mit dem Befehl [az extension add](/cli/azure/azure-cli-extensions-overview) wird eine Erweiterungsreferenz anhand des Namens installiert.  Weitere Informationen zu Erweiterungen finden Sie unter [Verwenden von Erweiterungen mit der Azure CLI](/cli/azure/azure-cli-extensions-overview).

```azurecli
## get a list of available Azure CLI extensions
az extension list-available --output table

# install the extension for az network express-route-cross-connection
az extension add --name express-route-cross-connection

# install the extension for az network front-door
az extension add --name front-door

# install the extension for az network virtual-wan
az extension add --name virtual-wan

# install the extension for az network vm-repair
az extension add --name virtual-network-tap

# install the extension for az network vmware
az extension add --name vmware

# install the extension for az peering
az extension add --name peering
```

## <a name="popular-network-articles-using-the-azure-cli"></a>Beliebte Netzwerkartikel mit der Azure CLI

- [Erstellen von virtuellen Computern](/cli/azure/azure-cli-vm-tutorial)
- [Erstellen eines virtuellen Netzwerks](/azure/virtual-network/quick-create-cli)
- [Azure CLI-Beispiele für Windows-VMs](/azure/virtual-machines/windows/cli-samples?toc=%2Fcli%2Fazure%2Ftoc.json&bc=%2Fcli%2Fazure%2Fbreadcrumb%2Ftoc.json)
- [Erstellen einer VM-Skalierungsgruppe](/azure/virtual-machine-scale-sets/quick-create-cli)
- [Ausführen von virtuellen Computern vom Typ „Azure IoT Edge unter Ubuntu“](/azure/iot-edge/how-to-install-iot-edge-ubuntuvm#deploy-from-azure-cli)
- [Durchführen eines Lastenausgleichs für virtuelle Linux-Computer in Azure](/azure/virtual-machines/linux/tutorial-load-balancer)
- [Erstellen und Verwalten virtueller Azure-Netzwerke für virtuelle Linux-Computer](/azure/virtual-machines/linux/tutorial-virtual-network)
- [Konfigurieren eines Dienstendpunkts für Cosmos DB](/azure/cosmos-db/how-to-configure-vnet-service-endpoint#configure-using-cli)

## <a name="see-also"></a>Weitere Informationen

- Unter [Erste Schritte mit der Azure CLI](/cli/azure/get-started-with-azure-cli) erhalten Sie Informationen zur Installation und Anmeldung.

- Entdecken Sie weitere [Befehle](/cli/azure/reference-index) und [Erweiterungen](/cli/azure/azure-cli-extensions-list) in der Azure CLI-Dokumentation.

- Verwalten Sie virtuelle Linux- oder Windows-Computer mit [az vm](/cli/azure/vm).

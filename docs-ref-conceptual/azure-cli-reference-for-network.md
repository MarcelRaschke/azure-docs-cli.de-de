---
title: Azure CLI-Referenzen für das Azure-Netzwerk
description: Landing Page der Azure CLI-Referenzen für das Azure-Netzwerk
author: dbradish-microsoft
manager: barbkess
ms.topic: reference
ms.date: 04/09/2021
ms.author: dbradish
ms.service: azure-cli
ms.devlang: azurecli
ms.reviewer: mohnader
ms.custom: devx-track-azurecli
ms.openlocfilehash: 59a8fcbe6f6a6eb2972ec5ba0c90799da3e94e85
ms.sourcegitcommit: f11f08a8b571d9909044693a8dc52c0cf2e9b2bc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/19/2021
ms.locfileid: "107707744"
---
# <a name="azure-cli-for-azure-network"></a>Azure CLI für das Azure-Netzwerk

Die Azure-Befehlszeilenschnittstelle ([Azure CLI](./what-is-azure-cli.md)) setzt sich aus Befehlen zum Erstellen und Verwalten von Azure-Ressourcen zusammen. Sie steht in vielen Azure-Diensten zur Verfügung – unter anderem auch im Azure-Netzwerk – und ermöglicht die Verwaltung von Netzwerkdiensten über die Befehlszeile.

## <a name="references-for-azure-network"></a>Referenzen für das Azure-Netzwerk

Die [Azure-Netzwerk](/azure/networking/)-CLI setzt sich aus zwei Teilen zusammen: **Kern** und **Erweiterung**. Die Befehle der Azure CLI-Kernkomponente sind standardmäßig in der CLI enthalten und werden vollständig unterstützt. Eine Erweiterung ermöglicht Ihnen den Zugriff auf experimentelle und vorab veröffentlichte Befehle und wird automatisch installiert, wenn Sie zum ersten Mal einen Erweiterungsverweis ausführen. Weitere Informationen zu Erweiterungsverweisen finden Sie unter [Verwenden von Erweiterungen mit der Azure CLI](./azure-cli-extensions-overview.md).

Unter [az network](/cli/azure/network) finden Sie eine vollständige Liste der Azure CLI-Kernreferenzen für das Azure-Netzwerk.  Über die weiter unten bereitgestellten Links gelangen Sie zu Erweiterungsreferenzen.

> [!NOTE]
> Sie werden bei der ersten Verwendung aufgefordert, einen Erweiterungsverweis zu installieren. Alternativ können Sie den Befehl `az extension add` verwenden, um eine Erweiterung manuell zu installieren.

### <a name="virtual-network"></a>Virtuelles Netzwerk

| Untergruppe | Verweis | Zweck | Ist Erweiterung
|-|-|-|-|
| Appliance | [az network virtual-appliance](/cli/azure/network/virtual-appliance) | Verwalten eines virtuellen Netzwerkgeräts
| DNS | [az network private-dns](/cli/azure/network/private-dns) | Verwalten von Domänen vom Typ „Privates DNS“ in Azure |
| Endpunkt | [az network service-endpoint](/cli/azure/network/service-endpoint) | Verwalten von Richtlinien im Zusammenhang mit Dienstendpunkten |
| NAT | [az network nat](/cli/azure/network/nat) | Verwalten von NAT-Ressourcen (Network Address Translation, Netzwerkadressenübersetzung) |
| NIC | [az network nic](/cli/azure/network/nic) | Verwalten von Netzwerkschnittstellen |
| NIC | [az network nic vtap-config](/cli/azure/network/nic/vtap-config) | Verwalten von TAP-Konfigurationen für virtuelle Netzwerke | ja
| Peering | [az peering](/cli/azure/peering) | Verwalten des Peerings | ja
| Profil | [az network profile](/cli/azure/network/profile) | Verwalten von Netzwerkprofilen |
| Route | [az network route-filter](/cli/azure/network/route-filter) | Verwalten von Routenfiltern |
| Route | [az network routeserver](/cli/azure/network/routeserver) | Verwalten von Routenservern |
| Route | [az network route-table](/cli/azure/network/route-table) | Verwalten von Routingtabellen |
| VMware | [az network vmware](/cli/azure/vmware) | Befehle zum Verwalten von Azure VMware Solution-Instanzen | ja
| vNet | [az network vnet](/cli/azure/network/vnet) | Verwalten virtueller Azure-Netzwerke |
| vNet | [az network vnet-tap](/cli/azure/network/vnet/tap) | Verwalten von TAPs für virtuelle Netzwerke | ja
| vNet | [az network vnet-gateway](/cli/azure/network/vnet-gateway) | Verwenden eines Azure-Gateways für virtuelle Netzwerke für sichere, standortübergreifende Konnektivität |

### <a name="wan-and-on-premise-connectivity"></a>WAN und lokale Konnektivität

| Untergruppe | Verweis | Zweck | Ist Erweiterung
|-|-|-|-|
| Querverbindung | [az network cross-connection](/cli/azure/network/cross-connection) | Verwalten von Azure-Netzwerkressourcen | ja
| ExpressRoute | [az network express-route](/cli/azure/network/express-route) | Verwalten dedizierter privater Glasfasernetzverbindungen mit Azure |
| vHub | [az network vhub](/cli/azure/network/vhub) | Verwalten virtueller Hubs | ja
| VPN | [az network p2s-vpn-gateway](/cli/azure/network/p2s-vpn-gateway) | Verwalten von Point-to-Site-VPN-Gateways | ja
| VPN | [az network vpn-connection](/cli/azure/network/vpn-connection) | Verwalten von VPN-Verbindungen |
| VPN | [az network vpn-gateway](/cli/azure/network/vpn-gateway) | Verwalten von VPN-Gateways | ja
| VPN | [az network vpn-server-config](/cli/azure/network/vpn-server-config) | Verwalten von VPN-Serverkonfigurationen | ja
| VPN | [az network vpn-site](/cli/azure/network/vpn-site) | Verwalten von VPN-Standortkonfigurationen | ja
| vRouter | [az network vrouter](/cli/azure/network/vrouter) | Verwalten von virtuellen Routern |
| vWAN | [az network vwan](/cli/azure/network/vwan) | Verwalten virtueller WANs | ja

### <a name="load-balancing-and-ip"></a>Lastenausgleich und IP

| Untergruppe | Verweis | Zweck | Ist Erweiterung
|-|-|-|-|
| Anwendungsgateway | [az network application-gateway](/cli/azure/network/application-gateway) | Verwalten von Routing- und Lastenausgleichsdiensten auf der Anwendungsebene |
| Front Door | [az network front-door](/cli/azure/network/front-door) | Verwalten von Front Door-Netzwerkressourcen | ja
| IP | [az network ip-group](/cli/azure/network/ip-group) | Verwalten von IP-Adressgruppen | ja
| IP | [az network public-ip](/cli/azure/network/public-ip) | Verwalten öffentlicher IP-Adressen |
| Lastenausgleich | [az network cross-region-lb](/cli/azure/network/cross-region-lb) | Verwalten und Konfigurieren von regionsübergreifenden Lastenausgleichsmodulen |
| Lastenausgleich | [az network lb](/cli/azure/network/lb) | Verwalten und Konfigurieren von Lastenausgleichsmodulen |
| Lokales Gateway | [az network local-gateway](/cli/azure/network/local-gateway) | Verwalten lokaler Gateways |
| Traffic Manager | [az network traffic-manager](/cli/azure/network/traffic-manager) | Verwalten des Routings von eingehendem Datenverkehr |

### <a name="security"></a>Sicherheit

| Untergruppe | Verweis | Zweck | Ist Erweiterung
|-|-|-|-|
| ASG | [az asg](/cli/azure/network/asg) | Verwalten von Anwendungssicherheitsgruppen |
| Bastion | [az network bastion](/cli/azure/network/bastion) | Verwalten von Azure-Bastionhosts |
| DDoS | [az network ddos-protection](/cli/azure/network/ddos-protection) | Verwalten von DDoS Protection-Plänen |
| Firewall | [az network firewall](/cli/azure/network/firewall) | Verwalten und Konfigurieren von Azure Firewall-Instanzen | ja
| Firewall | [az network security-partner-provider](/cli/azure/network/security-partner-provider) | Verwalten von Azure-Sicherheitspartneranbietern |
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
| Dienst | [az network list-service-aliases](/cli/azure/network#az_network_list_service_aliases) | Auflisten verfügbarer Dienstaliase in der Region, die für Dienstendpunkt-Richtlinien verwendet werden können |
| Dienst | [az network list-service-tags](/cli/azure/network#az_network_list_service_tags) | Auflisten aller Diensttags, die zu unterschiedlichen Ressourcen gehören |
| Verwendung | [az network list-usages](/cli/azure/network#az_network_list_usages) | Auflisten der Anzahl von Netzwerkressourcen in einer Region, die im Rahmen eines Abonnementkontingents verwendet werden |

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

- Unter [Erste Schritte mit der Azure CLI](./get-started-with-azure-cli.md) erhalten Sie Informationen zur Installation und Anmeldung.

- Entdecken Sie weitere [Befehle](/cli/azure/reference-index) und [Erweiterungen](./azure-cli-extensions-list.md) in der Azure CLI-Dokumentation.

- Verwalten Sie virtuelle Linux- oder Windows-Computer mit [az vm](/cli/azure/vm).
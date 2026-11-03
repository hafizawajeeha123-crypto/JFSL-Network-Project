JFSL Network Design and Implementation
Design and implementation of a secure, redundant network for **Jubilee Financial
Services Ltd (JFSL)**, Nairobi, Kenya, built in **Cisco Packet Tracer**.

Features
- Hierarchical design (Core / Distribution / Access) with redundancy
- 5 departments in separate VLANs: HR, CS, MK, LM, IT (Voice VLAN 120)
- Subnetting: Data 192.168.20.0/24, Voice 10.10.10.0/24, Public 190.200.100.0
- Inter-VLAN routing on multilayer switches
- Dual ISP (Safaricom + JTL) for redundancy and load balancing
- OSPF on routers and L3 switches
- DHCP, DNS, WEB and EMAIL servers at an external server site
- VoIP on Cisco 2811 (telephony-service, 4-digit extensions)
- Wi-Fi AP in each department
- Port security (sticky, violation shutdown)
- SSH + standard ACL on VTY (IT department only)
- PAT/NAT with ACL
- Site-to-site IPsec VPN (HQ <-> Server site)

 Devices
| Device | Model | Qty |
|---|---|---|
| Routers | Cisco 2911 | 2 |
| Voice gateway | Cisco 2811 | 1 |
| Multilayer switches | (model) | 2 |
| Access switches | (model) | 6 |

 IP Addressing
(Table of VLAN IDs, subnets, gateways)

## How to run
1. Install Cisco Packet Tracer
2. Open `JFSL_Network.pkt`
3. Test using ping between departments, phone calls, and VPN

## Testing
(ping, OSPF neighbors, VPN status)

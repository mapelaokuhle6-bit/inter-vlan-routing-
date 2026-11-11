# inter-vlan-routing-
Cisco Packet Tracer project demonstrating VLAN configuration and Router-on-a-Stick inter-VLAN routing.
# Inter-VLAN Routing using Cisco Packet Tracer

## 1. Project Overview

This project demonstrates the configuration of Virtual Local Area Networks (VLANs) and inter-VLAN routing using Cisco Packet Tracer.

The network represents a company with two departments:

- Human Resources (HR) – VLAN 10
- Information Technology (IT) – VLAN 20

Router-on-a-Stick was used to enable communication between the two VLANs.

## 2. Project Objectives

- Create and configure VLAN 10 and VLAN 20.
- Assign switch ports to the correct VLANs.
- Configure a trunk link between the switch and router.
- Configure router subinterfaces.
- Configure IP addresses and default gateways.
- Test communication between different VLANs.

## 3. Tools and Equipment

- Cisco Packet Tracer
- Cisco 2960 Switch
- Cisco 1941 Router
- Four PCs
- Copper Straight-Through Ethernet cables

## 4. Network Addressing

| Device | IP Address | VLAN | Default Gateway |
|---|---|---|---|
| PC0 | 192.168.10.10 | 10 | 192.168.10.1 |
| PC1 | 192.168.10.11 | 10 | 192.168.10.1 |
| PC2 | 192.168.20.10 | 20 | 192.168.20.1 |
| PC3 | 192.168.20.11 | 20 | 192.168.20.1 |

Subnet mask: 255.255.255.0

## 5. VLAN Configuration

- VLAN 10: Human Resources
- VLAN 20: Information Technology
- Switch ports Fa0/1–Fa0/2 assigned to VLAN 10.
- Switch ports Fa0/3–Fa0/4 assigned to VLAN 20.
- Switch port Fa0/5 configured as a trunk.

## 6. Inter-VLAN Routing

Router-on-a-Stick was implemented using two router subinterfaces:

- G0/0.10 – VLAN 10 – 192.168.10.1
- G0/0.20 – VLAN 20 – 192.168.20.1

IEEE 802.1Q encapsulation was used to identify VLAN traffic.

## 7. Testing and Verification

The network was tested using:

- `show vlan brief`
- `show interfaces trunk`
- `show ip interface brief`
- `show ip route`
- `ping`

Testing results [100%  , 0 loss ]

## 8. Skills Demonstrated

- VLAN configuration
- Switch port configuration
- Trunking
- Router subinterface configuration
- Inter-VLAN routing
- IP addressing and subnetting
- Network troubleshooting
- Cisco IOS command-line interface (CLI)

## 9. What I Learned

Through this project, I gained practical experience in separating departments into different VLANs and enabling communication between them using Router-on-a-Stick.

This project improved my understanding of switching, routing and network connectivity.

## 10. Project Files

- `inter-vlan-routing.pkt` – Cisco Packet Tracer project file.
- `screenshots/` – Network topology and configuration evidence.

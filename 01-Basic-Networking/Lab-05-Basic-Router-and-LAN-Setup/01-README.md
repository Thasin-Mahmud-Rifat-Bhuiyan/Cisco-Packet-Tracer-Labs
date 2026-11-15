# Basic Router and LAN Setup

## 1. Objective
To create a basic Local Area Network (LAN) using one router, two switches, and six PCs, and understand how network devices communicate through interconnected switches and a router.

## 2. Tools Used
- Cisco Packet Tracer
- 1 Router
- 2 Cisco Switches
- 6 PCs
- Ethernet Cables

## 3. Network Topology
In this lab, one router is connected to the first switch. The two switches are interconnected, and six PCs are connected to the switches.

**Topology Type:** Basic Router and LAN Setup

## 4. IP Address Configuration

| Device | IP Address | Subnet Mask |
|---|---|---|
| Router (LAN Interface) | 192.168.1.1 | 255.255.255.0 |
| PC0 | 192.168.1.2 | 255.255.255.0 |
| PC1 | 192.168.1.3 | 255.255.255.0 |
| PC2 | 192.168.1.4 | 255.255.255.0 |
| PC3 | 192.168.1.5 | 255.255.255.0 |
| PC4 | 192.168.1.6 | 255.255.255.0 |
| PC5 | 192.168.1.7 | 255.255.255.0 |

**Default Gateway for all PCs:** `192.168.1.1`

*Note: These are example IP addresses. Replace them with the actual addresses used in your Packet Tracer project.*

## 5. Configuration Steps
1. Place one router, two switches, and six PCs in Cisco Packet Tracer.
2. Connect the router to the first switch.
3. Connect the first switch to the second switch.
4. Connect three PCs to each switch.
5. Configure unique IP addresses and subnet masks on all PCs.
6. Configure the router's LAN interface.
7. Set the default gateway on each PC to the router's LAN IP address.
8. Check all cable connections and link status.

## 6. Router Configuration Commands

Example Cisco IOS commands:

```bash
enable
configure terminal
interface gigabitEthernet 0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
exit
end
```

*Note: The interface name may differ depending on the router model.*

## 7. Verification
Use the `ping` command to test connectivity between PCs connected to different switches and the router.

Example:

```bash
ping 192.168.1.1
ping 192.168.1.5
ping 192.168.1.7
```

## 8. Expected Output
All six PCs should be able to communicate with each other and reach the router if the connections and IP configurations are correct.

## 9. Learning Outcomes
- Understanding basic router configuration.
- Learning how to connect multiple switches.
- Understanding LAN communication.
- Understanding the role of a default gateway.
- Configuring IPv4 addresses.
- Testing network connectivity using the ping command.

## 10. Files Included
- `basic-router-lan.pkt` – Cisco Packet Tracer project file.
- `topology.png` – Network topology screenshot.
- `connectivity-test.png` – Ping test screenshot.

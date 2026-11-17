# RIP Routing with 3 Routers, 3 Switches and 6 PCs

## 1. Objective
To configure RIP (Routing Information Protocol) on three routers and establish communication between three different LAN networks using Cisco Packet Tracer.

## 2. Tools Used
- Cisco Packet Tracer
- 3 Routers
- 3 Cisco Switches
- 6 PCs
- Ethernet Cables
- Serial Cables (if required by the router model)

## 3. Network Topology
In this lab, three routers are connected in a linear topology. Each router is connected to one switch, and each switch connects two PCs.

**Topology Type:** Dynamic Routing (RIP)

## 4. IP Address Configuration

### LAN Addressing

| Device | IP Address | Subnet Mask | Default Gateway |
|---|---|---|---|
| PC0 | 192.168.1.2 | 255.255.255.0 | 192.168.1.1 |
| PC1 | 192.168.1.3 | 255.255.255.0 | 192.168.1.1 |
| PC2 | 192.168.2.2 | 255.255.255.0 | 192.168.2.1 |
| PC3 | 192.168.2.3 | 255.255.255.0 | 192.168.2.1 |
| PC4 | 192.168.3.2 | 255.255.255.0 | 192.168.3.1 |
| PC5 | 192.168.3.3 | 255.255.255.0 | 192.168.3.1 |

### Router LAN Interfaces

| Router | LAN Interface IP |
|---|---|
| Router0 | 192.168.1.1 |
| Router1 | 192.168.2.1 |
| Router2 | 192.168.3.1 |

### Router-to-Router Connections

| Connection | Network | Router IPs |
|---|---|---|
| Router0 - Router1 | 10.0.12.0/30 | 10.0.12.1, 10.0.12.2 |
| Router1 - Router2 | 10.0.23.0/30 | 10.0.23.1, 10.0.23.2 |

*Note: These are example IP addresses. Interface names and IP assignments should match your actual Packet Tracer topology.*

## 5. Configuration Steps
1. Place three routers, three switches, and six PCs in Cisco Packet Tracer.
2. Connect each router to its respective switch.
3. Connect two PCs to each switch.
4. Connect Router0 to Router1.
5. Connect Router1 to Router2.
6. Configure IP addresses on all PCs and router interfaces.
7. Configure the default gateway on each PC.
8. Enable the router interfaces.
9. Configure RIP routing on all three routers.

## 6. RIP Configuration Commands

### Router0

```bash
enable
configure terminal
router rip
version 2
no auto-summary
network 192.168.1.0
network 10.0.12.0
end
```

### Router1

```bash
enable
configure terminal
router rip
version 2
no auto-summary
network 192.168.2.0
network 10.0.12.0
network 10.0.23.0
end
```

### Router2

```bash
enable
configure terminal
router rip
version 2
no auto-summary
network 192.168.3.0
network 10.0.23.0
end
```

*Note: These RIP network commands assume the example addressing scheme above and Cisco IOS RIP configuration.*

## 7. Verification

Use the following commands to verify RIP configuration and routing information:

```bash
show ip protocols
show ip route
```

Use the `ping` command to test communication between PCs on different LANs.

Example:

```bash
ping 192.168.2.2
ping 192.168.3.2
ping 192.168.3.3
```

## 8. Expected Output
All six PCs should be able to communicate across the three LAN networks after successful RIP configuration and routing convergence.

## 9. Learning Outcomes
- Understanding Dynamic Routing.
- Learning how RIP works.
- Configuring RIP Version 2.
- Connecting multiple routers.
- Understanding routing tables.
- Enabling communication between different LAN networks.
- Verifying network connectivity using ping.

## 10. Files Included
- `rip-routing.pkt` – Cisco Packet Tracer project file.
- `topology.png` – Network topology screenshot.
- `rip-configuration.png` – RIP configuration screenshot.
- `routing-table.png` – Router routing table screenshot.
- `connectivity-test.png` – Ping test screenshot.

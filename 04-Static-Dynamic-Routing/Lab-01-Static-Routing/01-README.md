# Lab 01: Static Routing

## Objective
To configure static routing between two different LANs using two routers in Cisco Packet Tracer.

## Tools Used
- Cisco Packet Tracer
- 2 Routers
- 2 Switches
- 4 PCs
- Ethernet cables

## Network Topology
The network consists of two routers connected to each other. Each router connects to a local switch, and each switch connects to two PCs.

## IP Addressing

| Device | IP Address |
|---|---|
| Router0 - Inter-router link | 192.168.1.2 |
| Router1 - Inter-router link | 192.168.1.4 |
| Router0 - LAN interface | 192.168.2.3 |
| Router1 - LAN interface | 192.168.3.3 |
| PC0 | 192.168.2.7 |
| PC1 | 192.168.2.9 |
| PC2 | 192.168.3.5 |
| PC3 | 192.168.3.7 |

## Configuration Tasks
1. Create the network topology.
2. Assign IP addresses to router interfaces and PCs.
3. Configure the default gateways on all PCs.
4. Configure static routes on both routers.
5. Verify connectivity between the two LANs using ping.

## Static Routing
- Router0: Add a route to network 192.168.3.0/24 through 192.168.1.4.
- Router1: Add a route to network 192.168.2.0/24 through 192.168.1.2.

## Verification
- Check router interfaces using `show ip interface brief`.
- Check routing tables using `show ip route`.
- Test connectivity between PCs on different LANs using `ping`.

## Result
Static routes allow devices in the two LANs to communicate with each other, provided that the IP configuration and routing are correct.

## Files
- `static-routing.pkt` — Packet Tracer project
- `topology.png` — Network topology
- `commands.txt` — Router configuration commands
- `connectivity-test.png` — Connectivity test results

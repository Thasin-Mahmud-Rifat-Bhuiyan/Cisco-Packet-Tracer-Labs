# Lab 02: Implementation of LAN (Local Area Network)

## Objective
To implement a Local Area Network (LAN) using a network switch and multiple PCs in Cisco Packet Tracer and establish communication between the connected devices.

## Tools Used
- Cisco Packet Tracer
- 1 Cisco 2960 Switch
- 4 PCs
- Ethernet Straight-Through Cables

## Network Topology
A star topology is implemented using one central Cisco 2960 switch connected to four PCs. All PCs belong to the same local network.

## IP Addressing

| Device | IP Address | Subnet Mask |
|---|---|---|
| PC0 | 10.1.1.1 | 255.255.255.0 |
| PC1 | 10.1.1.2 | 255.255.255.0 |
| PC2 | 10.1.1.3 | 255.255.255.0 |
| PC3 | 10.1.1.4 | 255.255.255.0 |

## Configuration Tasks
1. Create a LAN topology using a Cisco 2960 switch.
2. Connect four PCs to the switch using Ethernet cables.
3. Assign unique IP addresses to all PCs.
4. Configure the same subnet mask on all PCs.
5. Ensure all PCs belong to the same network.
6. Test communication between the PCs using the ping command.

## Verification
- Check the IP configuration of each PC.
- Verify that all PCs are connected to the switch.
- Use the ping command to test communication between different PCs.
- Confirm successful connectivity within the LAN.

## Expected Result
All four PCs should be able to communicate with each other through the central switch within the same LAN.

## Files
- `lan-implementation.pkt` — Cisco Packet Tracer project file.
- `topology.png` — Network topology screenshot.
- `connectivity-test.png` — Ping test results.

## Learning Outcomes
- Understand the concept of Local Area Network (LAN).
- Learn how to implement a LAN using a Cisco 2960 switch.
- Understand star topology.
- Learn manual IPv4 address configuration.
- Practice communication between multiple PCs.
- Understand basic LAN connectivity testing.

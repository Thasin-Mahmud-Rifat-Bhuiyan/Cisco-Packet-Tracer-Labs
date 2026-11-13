# Lab 03: Star Topology (6 PCs)

## Objective
To implement a Star Topology using six PCs connected to a central Cisco 2960 switch and establish communication between all connected devices.

## Tools Used
- Cisco Packet Tracer
- 1 Cisco 2960 Switch
- 6 PCs
- 6 Ethernet Straight-Through Cables

## Network Topology
In Star Topology, all devices are connected to a central device, usually a switch or hub.

In this lab, six PCs are connected to a central Cisco 2960 switch using Ethernet cables.

## Configuration Tasks
1. Create a network topology using one central switch.
2. Connect six PCs to the switch.
3. Assign unique IP addresses to all PCs.
4. Configure the same subnet mask for all PCs.
5. Ensure all PCs belong to the same network.
6. Test communication between PCs using the `ping` command.

## IP Addressing

| Device | IP Address | Subnet Mask |
|---|---|---|
| PC0 | 192.168.1.1 | 255.255.255.0 |
| PC1 | 192.168.1.2 | 255.255.255.0 |
| PC2 | 192.168.1.3 | 255.255.255.0 |
| PC3 | 192.168.1.4 | 255.255.255.0 |
| PC4 | 192.168.1.5 | 255.255.255.0 |
| PC5 | 192.168.1.6 | 255.255.255.0 |

*Note: These are example IP addresses. Replace them with the actual addresses used in your Packet Tracer project.*

## Verification
- Check the IP configuration of all six PCs.
- Verify that all PCs are connected to the central switch.
- Use the `ping` command to test communication between PCs.
- Confirm successful connectivity within the LAN.

## Advantages
- Easy to install and manage.
- Easy to identify network problems.
- Failure of one PC's cable does not normally affect other PCs.
- Easy to add or remove devices.

## Disadvantages
- Failure of the central switch affects the entire network.
- Requires more cables than Bus Topology.
- Installation cost can be higher.

## Expected Result
All six PCs should be able to communicate with each other through the central switch within the same LAN.

## Files
- `star-topology.pkt` — Cisco Packet Tracer project file.
- `topology.png` — Network topology screenshot.
- `connectivity-test.png` — Ping test results.

## Learning Outcomes
- Understand Star Topology.
- Learn to connect multiple PCs to a central switch.
- Understand IPv4 address configuration.
- Practice communication between six PCs.
- Learn network connectivity testing using the ping command.

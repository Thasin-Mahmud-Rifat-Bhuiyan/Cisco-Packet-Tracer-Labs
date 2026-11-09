# Lab 01: PC-to-PC Communication

## Objective
To establish direct communication between two PCs in Cisco Packet Tracer by configuring IP addresses and testing network connectivity.

## Tools Used
- Cisco Packet Tracer
- 2 PCs
- Ethernet Crossover Cable (or a suitable cable supported by the devices)

## Network Topology
Two PCs are connected directly to each other using an Ethernet cable to establish a simple peer-to-peer network.

## Configuration Tasks
1. Create a network topology with two PCs.
2. Connect both PCs using an Ethernet cable.
3. Assign a unique IP address to each PC.
4. Configure the same subnet mask for both PCs.
5. Ensure both PCs belong to the same network.
6. Open the Command Prompt on each PC.
7. Test connectivity using the `ping` command.

## IP Addressing

| Device | IP Address | Subnet Mask |
|---|---|---|
| PC0 | 192.168.1.1 | 255.255.255.0 |
| PC1 | 192.168.1.2 | 255.255.255.0 |

*Note: These are example IP addresses. Replace them with the actual addresses used in your Packet Tracer project.*

## Verification
- Check the IP configuration of both PCs.
- Open Command Prompt on PC0.
- Execute `ping 192.168.1.2`.
- Verify whether PC1 responds successfully.
- Test communication in the opposite direction as well.

## Expected Result
Both PCs should be able to communicate directly with each other through their assigned IP addresses without using a router or switch.

## Files
- `pc-to-pc.pkt` — Cisco Packet Tracer project file.
- `topology.png` — Network topology screenshot.

## Learning Outcomes
- Understand basic peer-to-peer communication.
- Learn how to assign IPv4 addresses manually.
- Understand subnet masks.
- Learn direct PC-to-PC connectivity.
- Practice network testing using the `ping` command.

# Bus-Like Network Topology (5 PCs and 5 Switches)

## 1. Objective
To create a linear network using 5 PCs and 5 switches and understand how devices communicate within a network.

## 2. Tools Used
- Cisco Packet Tracer
- 5 PCs
- 5 Cisco Switches
- Copper Straight-Through Cables

## 3. Network Topology
The network consists of 5 PCs and 5 switches. Each PC is connected to a separate switch, and the switches are connected in a linear chain.

**Topology Type:** Linear (Daisy Chain / Bus-Like Arrangement)

## 4. IP Address Configuration

| Device | IP Address | Subnet Mask |
|---|---|---|
| PC0 | 192.168.1.1 | 255.255.255.0 |
| PC1 | 192.168.1.2 | 255.255.255.0 |
| PC2 | 192.168.1.3 | 255.255.255.0 |
| PC3 | 192.168.1.4 | 255.255.255.0 |
| PC4 | 192.168.1.5 | 255.255.255.0 |

*Note: These are example IP addresses. Replace them if your lab uses different addresses.*

## 5. Configuration Steps
1. Place 5 PCs and 5 switches in Cisco Packet Tracer.
2. Connect each PC to a separate switch.
3. Connect the switches in a linear chain.
4. Configure the IP addresses and subnet masks on all PCs.
5. Check the physical connections and link status.

## 6. Verification
Use the `ping` command to test communication between PCs.

Example:

```bash
ping 192.168.1.2
ping 192.168.1.3
ping 192.168.1.4
ping 192.168.1.5
```

## 7. Expected Output
All PCs should be able to communicate with each other if the connections and IP configurations are correct.

## 8. Learning Outcomes
- Understanding linear network arrangements.
- Learning how switches connect multiple network devices.
- Configuring IPv4 addresses.
- Testing network connectivity using the ping command.

## 9. Files Included
- `bus-topology.pkt` – Cisco Packet Tracer project file.
- `topology.png` – Network topology screenshot.
- `connectivity-test.png` – Ping test screenshot.

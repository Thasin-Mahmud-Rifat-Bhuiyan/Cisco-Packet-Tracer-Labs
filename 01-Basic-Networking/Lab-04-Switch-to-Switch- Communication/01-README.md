# Switch-to-Switch Communication (6 PCs)

## 1. Objective
To establish communication between two switches and understand how data is transferred between PCs connected to different switches.

## 2. Tools Used
- Cisco Packet Tracer
- 2 Cisco Switches
- 6 PCs
- Ethernet Cables

## 3. Network Topology
In this lab, two switches are connected to each other. Three PCs are connected to each switch to create a small Local Area Network (LAN).

**Topology Type:** Switch-to-Switch Connection

## 4. IP Address Configuration

| Device | IP Address | Subnet Mask |
|---|---|---|
| PC0 | 192.168.1.1 | 255.255.255.0 |
| PC1 | 192.168.1.2 | 255.255.255.0 |
| PC2 | 192.168.1.3 | 255.255.255.0 |
| PC3 | 192.168.1.4 | 255.255.255.0 |
| PC4 | 192.168.1.5 | 255.255.255.0 |
| PC5 | 192.168.1.6 | 255.255.255.0 |

*Note: These are example IP addresses. Replace them if your lab uses different addresses.*

## 5. Configuration Steps
1. Place 2 switches and 6 PCs in Cisco Packet Tracer.
2. Connect 3 PCs to the first switch.
3. Connect the remaining 3 PCs to the second switch.
4. Connect both switches using an Ethernet cable.
5. Configure unique IP addresses on all 6 PCs within the same network.
6. Check all cable connections and link status.

## 6. Verification
Use the `ping` command to test communication between PCs connected to different switches.

Example:

```bash
ping 192.168.1.4
ping 192.168.1.5
ping 192.168.1.6
```

## 7. Expected Output
All 6 PCs should be able to communicate with each other if the switch connections and IP configurations are correct.

## 8. Learning Outcomes
- Understanding switch-to-switch communication.
- Learning how to connect multiple switches.
- Understanding LAN communication.
- Configuring IPv4 addresses.
- Testing connectivity using the ping command.

## 9. Files Included
- `switch-to-switch.pkt` – Cisco Packet Tracer project file.
- `topology.png` – Network topology screenshot.
- `connectivity-test.png` – Ping test screenshot.

# Lab 01: DNS Configuration

## Objective
To configure a DNS server in Cisco Packet Tracer and resolve domain names into IP addresses.

## Tools Used
- Cisco Packet Tracer
- Server-PT
- Switch
- PCs
- Ethernet cables

## Network Topology
A DNS server and client PCs are connected through a network switch.

## Configuration Tasks
1. Create the network topology.
2. Assign IP addresses to the server and client PCs.
3. Enable the DNS service on Server-PT.
4. Add a DNS A record that maps a domain name to an IP address.
5. Configure the client PCs to use the DNS server.
6. Test domain name resolution.

## Verification
- Check the DNS server IP address.
- Verify the DNS A record.
- Use `nslookup` if supported, or test the domain using `ping`.

## Expected Result
The client PC resolves the configured domain name to the correct IP address.

## Files
- `dns-configuration.pkt` — Packet Tracer project
- `topology.png` — Network topology
- `dns-records.txt` — DNS record details
- `dns-test.png` — DNS verification result

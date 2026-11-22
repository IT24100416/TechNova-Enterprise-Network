# TechNova Solutions — Enterprise Network Design and Implementation

A student group project completed for **IE3140 — Advanced Network Engineering** at **Sri Lanka Institute of Information Technology (SLIIT)**. The team designed and implemented a simulated enterprise network for TechNova Solutions in Cisco Packet Tracer, serving departmental LANs, a server network, and a remote branch.

> This repository documents an academic simulation. Results describe the tested Packet Tracer project and should not be read as production deployment claims.

## Project files

- Cisco Packet Tracer simulation: [`packet-tracer/TechNova.pkt`](packet-tracer/TechNova.pkt)
- Final assignment report: [`report/IE3140_Final_Report(1).pdf`](report/IE3140_Final_Report(1).pdf)
- Evidence screenshots: [`screenshots/`](screenshots/)

Open the `.pkt` file with Cisco Packet Tracer. The PDF report contains the detailed design, addressing plan, configuration evidence, and verification record.

## Network overview

The topology connects HR, Engineering, Sales, and Server VLANs at the main site with a remote branch through a routed WAN. The design also includes an ISP and simulated external server. The report documents IPv4 VLSM and IPv6 addressing, VLAN segmentation, inter-VLAN routing, single-area and multi-area OSPF, NAT/PAT, and Layer 2 protections.

### Technologies and topics

- IPv4 subnetting with VLSM and IPv6 addressing
- VLANs and inter-VLAN routing
- Single-area and multi-area OSPF, including MD5 authentication
- NAT/PAT for simulated external access
- Port security, BPDU Guard, and DHCP Snooping
- WAN connectivity and fault diagnosis
- ICMP and HTTP connectivity checks

## Verification highlights

The included evidence shows four OSPF neighbors in `FULL` state on R2-CORE, learned inter-area OSPF routes, and a PC-to-server ping that succeeds on repeat with 0% packet loss. The full report records broader endpoint and service checks, along with the conditions and limitations for each test.

### Multicast limitation

The report describes a multicast design, but **successful multicast streaming was not demonstrated**. In the tested Packet Tracer 9.0.0 Cisco 2911 simulation, the multicast configuration command was rejected. The design is documented as a feasibility attempt; there is no claim that multicast delivery worked, and the result does not establish a limitation of real Cisco IOS.

## Screenshots

### Enterprise topology

![TechNova enterprise network topology](screenshots/network-topology.png)

### OSPF neighbor and route verification

![R2-CORE OSPF neighbors and learned routes](screenshots/ospf-neighbors-and-routes.png)

### Connectivity test

![Repeated ping test from PC1 to the server](screenshots/connectivity-test.png)

## Team

- **J.A.D.S. Jayakodi**
- **R.M.S.S. Rathnayaka**
- **K.N. Munasinghe**
- **J.P.C.A. Jayasinghe**

This was a collaborative group assignment. The report’s teamwork and presentation section describes the team’s work ownership.

## Academic context

Prepared for IE3140 — Advanced Network Engineering, SLIIT. This repository is shared for learning and portfolio reference. Cisco Packet Tracer is required to inspect or run the simulation.

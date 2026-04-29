# Corporate-Network-Prototype

Multi-Site Corporate Network Prototype for **KI Software Entwicklung GmbH**
## Project Overview
This project involves the design and implementation of a secure, multi-site enterprise network for KI Software Entwicklung GmbH. The goal is to provide a functional prototype connecting a new headquarters in Vienna with two branch offices (Linz and Graz) using Cisco Packet Tracer.
## Key Requirements
Multi-Site Connectivity: Linking HQ, Linz, and Graz via GRE IP-Tunnels over an IPv4 transit network (VPN) (p. 1).
Logical Segmentation (VLANs): Organizing company departments into logical units for security and management (p. 1).
Abt. Produktion (
): Dedicated Production VLAN.
Abt. Verwaltung (
): Office/Admin VLAN.
Dynamic Addressing: Implementation of DHCP for all internal workstations to receive IP addresses automatically (p. 1).
Advanced IP Management: Utilizing VLSM (Variable Length Subnet Masking) to maximize IP efficiency across different site sizes (p. 1).
## Security & Infrastructure
Border Security: Implementing NAT/PAT at the Vienna HQ border router for internet access (p. 1).
Internal Access Control: Restricting the File Server to internal intranet access only, ensuring no external visibility (p. 1).
LAN Security: Application of Layer 2 security protocols (e.g., Port Security) on switches to protect the local departments (p. 1).
Public Services: Hosting a WEB-Server with a fixed public IP address for external availability (p. 1).
## Repository Structure
/prototype: Contains the .pkt (Cisco Packet Tracer) simulation file.
/configs: Text-based exports of router and switch configurations for review.
/docs: Network diagrams, IP schema, and VLAN allocation tables.

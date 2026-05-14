# Corporate-Network-Prototype
> **Client:** KI Software Entwicklung GmbH  
> **Project Scope:** Multi-Site Enterprise Networking (VPN over IP-Transit)

## Project Overview
This project involves the design and implementation of a secure, multi-site enterprise network prototype. The goal is to connect a new headquarters in **Vienna** with two branch offices (**Linz** and **Graz**) using Cisco Packet Tracer, simulating a real-world corporate environment.

---

## Key Requirements

### 1. Connectivity & Routing
* **Multi-Site Connectivity:** Linking HQ, Linz, and Graz via **GRE IP-Tunnels** (Generic Routing Encapsulation - *a protocol used to wrap data packets inside another protocol for transport*) over an IPv4 transit network.
* **Advanced IP Management:** Utilizing **VLSM** (Variable Length Subnet Masking - *a way of dividing an IP network into subnets of different sizes to save addresses*) to maximize efficiency.
* **Dynamic Addressing:** Full implementation of **DHCP** (Dynamic Host Configuration Protocol - *automatically assigns IP addresses to devices*) for all workstations.

### 2. Logical Segmentation (VLANs)
* **Abt. Produktion (VLAN 10):** Dedicated production network.
* **Abt. Verwaltung (VLAN 20):** Office and administration network.
* **Management (VLAN 30):** Network for administrative device access.

### 3. Security & Infrastructure
* **Border Security:** Implementing **NAT/PAT** (Network Address Translation / Port Address Translation - *allows multiple devices on a private network to share a single public IP*) at the Vienna HQ.
* **Access Control:** **ACLs** (Access Control Lists - *rules that filter network traffic*) configured to restrict the File Server to internal intranet access only.
* **LAN Security:** Layer 2 protection via **Port Security** (restricting switch ports to specific MAC addresses) to prevent unauthorized hardware access.
* **Public Services:** Dedicated **WEB-Server** with a fixed public IP for external availability.

---

## 🏗 Repository Structure

| Directory | Content Description |
| :--- | :--- |
| `prototype` | Contains the `.pkt` (Cisco Packet Tracer) simulation files. |
| `configs` | Text-based exports of router and switch configurations. |
| `docs` | Network diagrams, IP schemas, and VLAN allocation tables. |

---

## Implementation Progress

### Week 1: Foundation (Vienna & ISP)
- [x] Topology defined and devices placed
- [x] VLSM calculation completed
- [x] HQ Vienna: Router-on-a-Stick and VLANs
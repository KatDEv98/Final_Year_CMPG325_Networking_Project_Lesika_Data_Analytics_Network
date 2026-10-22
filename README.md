# Lesika Data Analytics - Network Infrastructure Project

## Project Overview
This repository contains the complete design, configuration, testing, and documentation for the Lesika Data Analytics enterprise network. The project was developed in phases (milestones) to build a secure, highly available, and scalable network infrastructure using Cisco technologies in Cisco Packet Tracer.

## Repository Structure
This repository houses all Packet Tracer files (`.pkt`), device configurations, testing evidence, and design documentation (`.pdf`) for the project.

### 🟢 Milestone 1: Core Network Design & IP Addressing (Completed)
The first phase established the core routing infrastructure and IP addressing scheme using Variable Length Subnet Masking (VLSM).
*   **Dual-WAN Redundancy:** Configured a primary and backup ISP connection to meet the CR15 resilience standard.
*   **IP Addressing:** Designed and implemented a VLSM plan dividing the `192.168.60.0/24` block into specific point-to-point (`/30`) and LAN (`/27` and `/28`) segments.
*   **Future Expansion:** Successfully reserved the `192.168.60.192/26` block for an 18-month branch office expansion.
*   **Hardware:** Deployed and physically cabled Cisco 2911 ISR routers alongside Catalyst 2960 access and distribution switches.

### 🟢 Milestone 2: Routing Protocols, Security & Implementation (Completed)
The second phase focused on bringing the network to life with full inter-VLAN routing, core services, and security.
*   **Router-on-a-Stick:** Configured 802.1Q trunking and sub-interfaces on the edge router (R1) for inter-VLAN routing.
*   **Core Services:** Deployed a central DHCP server with `ip helper-address` relay across all VLANs, alongside an internal DNS server.
*   **Wireless & Security:** Implemented Staff and Guest Wi-Fi networks. Secured guest traffic using ACL 100 to isolate guests from internal servers.
*   **NAT Overload:** Configured Network Address Translation (PAT) to allow internal private IPs to access the Internet.

### 🟢 Milestone 3: Final Network Optimization & Fault Isolation (Completed)
The final phase focused on testing, network resilience, and the assigned troubleshooting challenge.
*   **Fault Isolation Scenarios:** Documented and tested 5 distinct network faults (Layer 1 through Layer 7), including disabled trunk ports, missing VLANs, wrong IP addresses, missing DHCP relays, and missing DNS records.
*   **Failover Testing:** Verified the CR15 requirement by simulating a primary ISP failure and confirming the floating static route seamlessly rerouted traffic to the backup ISP.
*   **Evidence & Reporting:** Compiled full testing evidence, screenshots, and the final technical report.

## Technologies & Tools
*   **Design & Simulation:** Cisco Packet Tracer
*   **Network Hardware:** Cisco ISR Routers (2911), Cisco Catalyst Switches (2960)
*   **Core Concepts:** IPv4, VLSM, Routing, VLANs (802.1Q), DHCP, DNS, NAT, ACLs, High Availability

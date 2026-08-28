# Lesika Data Analytics - Network Infrastructure Project

## Project Overview
This repository contains the design, configuration, and documentation for the Lesika Data Analytics enterprise network. The project is being developed in phases (milestones) to build a secure, highly available, and scalable network infrastructure using Cisco technologies.

## Repository Structure
This repository will house all Packet Tracer files (`.pkt`) and design documentation (`.pdf`) for the duration of the project.

### Milestone 1: Core Network Design & IP Addressing (Completed)
The first phase establishes the core routing infrastructure and IP addressing scheme using Variable Length Subnet Masking (VLSM).
* **Dual-WAN Redundancy:** Configured a primary and backup ISP connection to meet the CR15 resilience standard.
* **IP Addressing:** Designed and implemented a VLSM plan dividing a `/24` block into specific point-to-point (`/30`) and LAN (`/25`) segments.
* **Future Expansion:** Successfully reserved the `192.168.60.128/26` block for an 18-month branch office expansion.
* **Hardware:** Deployed and physically cabled Cisco 2911 and 4331 ISR routers alongside a Catalyst 2960 distribution switch.

### ⚪ Milestone 2: Routing Protocols & Security (Upcoming)
* *(Details to be added in the next phase of the project)*

### ⚪ Milestone 3: Final Network Optimization (Upcoming)
* *(Details to be added in the final phase of the project)*

## Technologies & Tools
* **Design & Simulation:** Cisco Packet Tracer
* **Network Hardware:** Cisco ISR Routers (2911, 4331), Cisco Catalyst Switches
* **Core Concepts:** IPv4, VLSM, Routing, Network Hardware Modules, High Availability

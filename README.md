# Enterprise WAN Architecture & Distributed Big Data Infrastructure

## Overview
An enterprise-grade Wide Area Network (WAN) design and multi-tier server architecture simulation engineered to support high-throughput, low-latency Big Data analytics and distributed database storage[cite: 7, 146, 157]. Developed for the Architecture and Operating Systems module (CMP4011 / CIS4011) under the Cardiff Metropolitan University curriculum[cite: 7, 8, 143, 163]. Grade Achieved: 76% (First-Class Honours / Distinction)[cite: 7, 8].

## Infrastructure Architecture & Technical Highlights

### 1. WAN Topology & Core Routing
- **Perimeter Routing:** Edge connectivity managed via MikroTik HEX S RB760iGS (Qualcomm IPQ4018 ARM dual-core processor @ 880 MHz) and Cisco 819HGW routers, configured with hardware-accelerated IPsec encryption[cite: 145, 151, 157].
- **Switching Matrix:** Managed multi-layer switching infrastructure incorporating TP-Link TL-SG1024DE and Cisco 3560 distribution switches providing 72+ Gigabit ports with Layer 2/3 traffic segmentation, QoS, and dedicated backbone uplinks[cite: 146, 157, 160].
- **Physical Media & Cabling:** Comprehensive deployment of straight-through Ethernet links for end-node and server connectivity paired with crossover cabling for inter-switch trunk distribution[cite: 151, 152, 158].

### 2. Enterprise Computing & Storage Capacity
- **Analytics & Database Nodes:** High-density server array powered by eight HP ProLiant ML30 Gen9 rack servers (Intel Xeon E3-1220 v5 quad-core @ 3.0 GHz, 32 GB RAM, 3.2 TB SSD storage) handling real-time query loads[cite: 145, 146, 147].
- **Endpoint Workstations:** Staff client terminals utilizing ASUS VivoBook 15 (Intel Core i5-9500T, 16 GB DDR4 RAM, 512 GB SSD) and Dell OptiPlex 5070 Micro administrative units[cite: 145, 147, 157].
- **Cloud Disaster Recovery:** Off-site encrypted cloud backup integrated via Sync.com supporting HIPAA-, GDPR-, and PIPEDA-compliant storage[cite: 147, 169].

### 3. Dual Operating System Architecture
- **Infrastructure Services (Windows Server 2019):** Hosts core network operations including Active Directory Domain Services (AD DS), DNS, and automated DHCP addressing[cite: 165, 167].
- **Application & Monitoring Services (Ubuntu Server 22.04 LTS):** Dedicated host for Apache HTTP web services, Postfix/Dovecot mail transfer agents, MySQL 8.0/PostgreSQL database instances, and automated system health monitoring[cite: 165, 167, 168].
- **Client Platforms:** Standardized on Windows 10/11 Pro with BitLocker drive encryption and centralized Group Policy management[cite: 165, 167].

### 4. Layered Security & Threat Mitigation
- **Hardware Firewalls:** Fortinet FortiGate 30E (FortiSoC2 ARM Cortex-A9 @ 1.2 GHz with hardware DPU) and Cisco ASA 5508-X appliances delivering Deep Packet Inspection (DPI), wire-speed IPS, and perimeter filtering[cite: 145, 146, 151, 160].
- **Endpoint Protection:** Multi-layered defense incorporating Microsoft Defender for Endpoint across server nodes, paired with client-level anti-malware safeguards[cite: 166, 169].
- **Structured Subnetting:** Organized Class C IPv4 allocation (`192.168.1.0/24`) isolating structured, unstructured, configuration, and backup servers across dedicated gateway interfaces[cite: 151, 152, 158].

## Repository Contents
- `Hardware Description.pdf` - In-depth hardware specifications, processor architectures, and hardware inventory[cite: 143, 145, 146, 147]
- `Software Techninal Design.pdf` - Operating system rationale, server roles, DBMS configurations, and security stack[cite: 163, 165, 167, 168, 169]
- `Network Configurations description.pdf` - Physical port tables, media types, and subnet allocation matrix[cite: 150, 151, 152]
- `Portfolio Map.pdf` - Complete architectural evolution and Cisco Packet Tracer network simulation topology[cite: 154, 155, 160]

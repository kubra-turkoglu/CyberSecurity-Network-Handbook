# CyberSecurity-Network-Handbook
# 🛡️ Network Fundamentals for Blue Teaming & Cyber Security

This repository is a comprehensive guide for those aiming to specialize in cybersecurity, covering critical network fundamentals, protocol analysis, and network architectures from a cybersecurity perspective.

> "If you don't understand the network, you cannot defend it."

```mermaid
graph LR
    %% Main Node
    Main[Network Fundamentals for Cybersecurity] --> Types[Network Types]
    Main --> Arch[Network Architecture]
    Main --> Proto[Addressing & Protocols]
    Main --> Hardware[Network Hardware]
    Main --> Security[Security & Monitoring]

    %% Network Types
    Types --> SOHO[SOHO: Small Office Home Office]
    Types --> Enterprise[Enterprise / Campus]
    Types --> WAN[WAN & Cloud Connectivity]

    %% Architecture
    Arch --> Layers[Hierarchical Layers]
    Layers --> L1[Access / Distribution / Core]
    Arch --> Seg[Segmentation]
    Seg --> L2[VLANs / DMZ / Guest Net]

    %% Protocols
    Proto --> L3[IP Addressing & Subnetting]
    Proto --> Services[Gateway Services: NAT / PAT]
    Proto --> Discovery[Discovery: ARP / DHCP / DNS]

    %% Hardware
    Hardware --> Inter[Intermediate: Switches / Routers / Firewalls]
    Hardware --> End[End Devices: Laptops / IoT / Servers]

    %% Security
    Security --> Analysis[Protocol Analysis: Wireshark / PCAP]
    Security --> Defense[Defense: IDS / IPS / ACLs]

    %% Styling
    style Main fill:#2d333b,stroke:#58a6ff,color:#fff
    style Security fill:#442d2d,stroke:#f85149,color:#fff
```

## 📌 Content Guide

I am detailing the impact of networking on cybersecurity under the following headings:

### 1. [OSI Model & Protocol Analysis](./Cheat-Sheets/networking-protocols.md)
- **Layered Security:** Attacks occurring at specific layers (L2 - MAC Spoofing, L3 - IP Spoofing, L4 - SYN Flood).
- **Critical Ports:** Vulnerability analysis of commonly used services (SSH, HTTP, SMB, FTP).

### 2. [DHCP Deep Dive (DORA Process)](./DHCP-Analysis/dhcp-process.md)
- **DORA Process:** Technical breakdown of Discover, Offer, Request, and Acknowledge steps.
- **Cybersecurity Note:** Rogue DHCP Server attacks and protection methods with DHCP Snooping.

### 3. [NAT & PAT Analysis](./NAT-PAT-DeepDive/nat-vs-pat.md)
- **IP Saving vs. Security:** Internet access scenarios for Private IP blocks.
- **Static NAT:** Securely exposing servers to the outside world.
- **PAT (NAT Overload):** Logic of port-based address translation.

### 4. [Network Architectures & Topologies](./Lab-Topologies/enterprise-arch.md)
- **SOHO vs. Enterprise:** Transition from small office networks to campus networks.
- **Hierarchical Design:** Roles of Access, Distribution, and Core layers.
- **Vulnerability Analysis:** Single Point of Failure and Redundancy.

---

## 🛠️ Key Information Table


| Protocol | Port | Layer | Security Status |
| :--- | :--- | :--- | :--- |
| **FTP** | 21 | L7 (App) | Unencrypted / vsftpd backdoor risk |
| **SSH** | 22 | L7 (App) | Encrypted / Secure Management |
| **DNS** | 53 | L7 (App) | DNS Poisoning / Tunneling risk |
| **HTTP** | 80 | L7 (App) | Unencrypted / Sniffing risk |
| **TCP** | - | L4 (Trans) | 3-Way Handshake / Connection-oriented |

---

## 🚀 Project Objectives
This study aims to demonstrate not only theoretical networking knowledge but also how this knowledge is used in **SOC Analysis**, **Penetration Testing**, and **Network Security** processes.

---
*Prepared by: Kubra Bozdogan*



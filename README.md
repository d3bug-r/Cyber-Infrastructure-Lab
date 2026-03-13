# 🛡️ Cyber Lab Infrastructure (Virtualization & Hardening)

**Project Owner:** D3bug

**Status:** In Progress (Month 2/7)

**Goal:** Master Cybersecurity Preparation & Network Engineering Level

---

## 🏗 Project Overview
This repository documents the deployment of a fully isolated and secured virtual infrastructure. The goal is to simulate a corporate network environment to practice routing, service configuration, and security hardening.

## 💻 Architecture
**Host:** Windows 11 (Hypervisor: VirtualBox)

### 1. The Gateway (Server)
* **OS:** Ubuntu Desktop 22.04 LTS
* **Role:** Router, Firewall, DNS, DHCP
* **Interfaces:**
    * `WAN` (NAT): Access to Internet
    * `LAN` (Internal Network): `192.168.1.20`

### 2. The Client (Target)
* **OS:** Windows 10 Pro
* **Role:** End-user machine
* **Network:** Isolated (No direct internet access), dependent on the Gateway.
* **IP:** Dynamic (via DHCP)

---

## 🔧 Skills & Technologies
* **Networking:** IPv4 Subnetting, NAT/Masquerade, Static Routing.
* **Services:**
    * **DNS:** BIND9 (Zones configuration, Forwarding).
    * **DHCP:** ISC-DHCP-SERVER (DORA process analysis).
* **Security:**
    * **Firewall:** Iptables (Stateful inspection).
    * **Analysis:** Wireshark (Packet capture & troubleshooting).

---

## 📂 Repository Structure
* `/Configs`: Raw configuration files (named.conf, dhcpd.conf, netplan).
* `/Docs`: Network diagrams and theoretical notes.
* `/Scripts`: Bash/Python automation scripts.

# Business-Network-Design-CiscoPacketTracer
Design and Implementation of a Company/Business System Network Design


# Business System Network Design | Cisco Packet Tracer

This project is a complete logical network design and implementation for a Trading Floor Support Centre using **Cisco Packet Tracer**. It supports over 600 users across 3 floors and is built with scalability, security, and redundancy in mind.

---

## 📡 Project Overview

- **Organization:** Trading Floor Support Centre  
- **Users:** 600+  
- **Floors:** 3 (2 departments per floor + Server Room)  
- **Goal:** Design a secure, scalable, and redundant network topology using Cisco technologies.

---

## 🏢 Department Layout

### 🥇 First Floor
- **Sales & Marketing**: 120 users (VLAN 10, 172.16.1.0/25)
- **HR & Logistics**: 120 users (VLAN 20, 172.16.1.128/25)

### 🥈 Second Floor
- **Finance & Accounts**: 120 users (VLAN 30, 172.16.2.0/25)
- **Admin & Public Relations**: 120 users (VLAN 40, 172.16.2.128/25)

### 🥉 Third Floor
- **ICT**: 120 users (VLAN 50, 172.16.3.0/25)
- **Server Room**: 12 devices (Static IPs)

---

## 🛠️ Technologies Implemented

- ✅ Cisco Packet Tracer Simulation
- ✅ Hierarchical Redundant Network Design
- ✅ VLAN Segmentation per Department
- ✅ Inter-VLAN Routing via Multilayer Switches
- ✅ OSPF Dynamic Routing Protocol
- ✅ DHCP Configuration (Central Server Room)
- ✅ SSH Access for Secure Remote Configuration
- ✅ Port-Security for Finance Dept. (Sticky MAC, Shutdown Mode)
- ✅ Wireless Network Setup (Access Points for each department)
- ✅ NAT Overload (PAT) for Internet Access
- ✅ Access Control Lists (ACLs)
- ✅ Redundant ISP Configuration using 2 routers

---

## 🌐 Public IP Configuration

| Subnet        | Description     | Purpose          |
|---------------|-----------------|------------------|
| 195.136.17.0/30 | ISP1 - MAIN     | Internet Access  |
| 195.136.17.4/30 | Backup ISP Link | Redundancy       |
| 195.136.17.8/30 | CORE-R2 Link    | Secondary Route  |
| 195.136.17.12/30| ISP2 - BACKUP   | Failover Access  |

---

## 🔐 Security Features

- SSH Enabled on all Routers and Multilayer Switches
- Sticky MAC-based Port Security for Finance VLAN
- ACL for PAT (NAT Overload)
- DHCP for dynamic address allocation
- Static IPs for critical servers

---

## 🧪 Testing & Validation

- ✅ VLAN-to-VLAN communication via Inter-VLAN routing
- ✅ DHCP functionality verified for all clients
- ✅ Server Room devices statically addressed and reachable
- ✅ Remote access via SSH tested
- ✅ ISP redundancy tested with failover scenario
- ✅ Port Security violation tested in Finance Department

---

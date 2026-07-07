# Hotel Management Network (Cisco Packet Tracer)

## Project Overview

This project demonstrates a Hotel Management Network designed using Cisco Packet Tracer. The network is divided into three floors, each containing multiple departments connected through VLANs. The design provides logical segmentation, better security, efficient traffic management, and inter-VLAN communication using routers.

---

## Objectives

- Design a scalable hotel network.
- Separate departments using VLANs.
- Enable communication between VLANs.
- Reduce broadcast traffic.
- Improve network security.
- Connect multiple floors using routers.

---

# Network Topology

The hotel consists of three floors:

## 1st Floor
Departments:
- Reception
- Store
- Logistics

Router:
- F1 Router

Switch:
- F1 Switch (Cisco 2960)

---

## 2nd Floor
Departments:
- Sales
- HR
- Finance

Router:
- F2 Router

Switch:
- F2 Switch (Cisco 2960)

DNS Server:
- 172.16.1.66

---

## 3rd Floor
Departments:
- IT
- Admin

Router:
- F3 Router

Switch:
- F3 Switch (Cisco 2960)

---

# VLAN Configuration

| VLAN | Department | Network | Subnet Mask |
|------|------------|----------------|----------------|
| VLAN 10 | IT | 10.0.0.0/26 | 255.255.255.192 |
| VLAN 20 | Admin | 10.0.0.64/27 | 255.255.255.224 |
| VLAN 30 | Sales | 172.16.1.0/27 | 255.255.255.224 |
| VLAN 40 | HR | 172.16.1.32/28 | 255.255.255.240 |
| VLAN 50 | Finance | 172.16.1.48/28 | 255.255.255.240 |
| VLAN 60 | Store | 192.168.1.16/29 | 255.255.255.248 |
| VLAN 70 | Reception | 192.168.1.0/28 | 255.255.255.240 |
| VLAN 80 | Logistics | 192.168.1.32/28 | 255.255.255.240 |

---

# Devices Used

### Routers
- Cisco 2911 Router ×3

### Switches
- Cisco 2960-24TT Switch ×3

### End Devices
- PCs
- Printers
- DNS Server

---

# IP Addressing

## Third Floor

### VLAN 10 (IT)
Network: 10.0.0.0/26

Devices:
- PC: 10.0.0.2
- Printer: 10.0.0.3

---

### VLAN 20 (Admin)
Network: 10.0.0.64/27

Devices:
- PC: 10.0.0.66
- Printer: 10.0.0.67

---

## Second Floor

### VLAN 30 (Sales)
Network: 172.16.1.0/27

Devices:
- PC: 172.16.1.2
- Printer: 172.16.1.3

---

### VLAN 40 (HR)
Network: 172.16.1.32/28

Devices:
- PC: 172.16.1.34
- Printer: 172.16.1.35

---

### VLAN 50 (Finance)
Network: 172.16.1.48/28

Devices:
- PC: 172.16.1.50
- Printer: 172.16.1.51

---

### DNS Server

IP Address:
172.16.1.66

---

## First Floor

### VLAN 60 (Store)
Network: 192.168.1.16/29

Devices:
- PC: 192.168.1.66
- Printer: 192.168.1.67

---

### VLAN 70 (Reception)
Network: 192.168.1.0/28

Devices:
- PC1: 192.168.1.2
- PC2: 192.168.1.3
- Printer: 192.168.1.5

---

### VLAN 80 (Logistics)
Network: 192.168.1.32/28

Devices:
- PC: 192.168.1.34
- Printer: 192.168.1.35

---

# Inter-Router Connections

The three routers are connected using separate point-to-point links.

Router Links:
- F1 ↔ F2
- F2 ↔ F3
- F1 ↔ F3

Inter-router network:
192.168.100.0

---

# Features Implemented

- VLAN Segmentation
- Router-on-a-Stick Configuration
- Inter-VLAN Routing
- Trunk Ports
- DNS Server Connectivity
- Multi-floor Network Design
- Department-wise Network Isolation
- Efficient IP Addressing using VLSM

---

# Advantages

- Improved security through VLAN isolation.
- Reduced broadcast domains.
- Easier network management.
- Better scalability for future expansion.
- Faster communication within departments.
- Centralized routing between floors.

---

# Software Used

- Cisco Packet Tracer

---

# Future Improvements

- DHCP Server implementation
- ACLs for access control
- Dynamic routing (OSPF/EIGRP)
- Wireless Access Points
- Web and Mail Servers
- Network monitoring using SNMP
- Redundant links using STP

---

# Author

**Sahar Ayub**

Academic Course Project

Hotel Management Network using Cisco Packet Tracer

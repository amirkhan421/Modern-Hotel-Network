
# 🏨 Vic Modern Hotel Network Design

## 📌 Overview

This project presents the design and implementation of a **complete network infrastructure** for *Vic Modern Hotel*, a three-floor enterprise environment.

The goal is to build a **secure, scalable, and efficient network** using Cisco networking concepts such as VLANs, OSPF, DHCP, and network security.

## 🏢 Hotel Structure

The hotel consists of **three floors**, each containing multiple departments:

### 1st Floor

* Reception
* Store
* Logistics

### 2nd Floor

* Finance
* HR
* Sales/Marketing

### 3rd Floor

* IT
* Admin


## 🧠 Network Design Highlights

* **3 Routers** (one per floor, placed in server room)
* **Serial DCE connections** between routers
* **/30 subnetting** for router-to-router links
* **1 Switch per floor**
* **Wireless connectivity (WiFi)** for each floor
* **1 Printer per department**
* **VLAN segmentation for all departments**


## 🌐 IP Addressing & VLANs

### 1st Floor

| Department | VLAN | Network         |
| ---------- | ---- | --------------- |
| Reception  | 80   | 192.168.80.0/24 |
| Store      | 70   | 192.168.70.0/24 |
| Logistics  | 60   | 192.168.60.0/24 |



### 2nd Floor

| Department | VLAN | Network        |
| ---------- | ---- | -------------- |
| Finance    | 50   | 192.168.5.0/24 |
| HR         | 40   | 192.168.4.0/24 |
| Sales      | 30   | 192.168.3.0/24 |



### 3rd Floor

| Department | VLAN | Network        |
| ---------- | ---- | -------------- |
| Admin      | 20   | 192.168.2.0/24 |
| IT         | 10   | 192.168.1.0/24 |



## 🔗 Router Interconnections

| Link    | Network       |
| ------- | ------------- |
| R1 – R2 | 10.10.10.0/30 |
| R2 – R3 | 10.10.10.4/30 |
| R1 – R3 | 10.10.10.8/30 |



## ⚙️ Technologies Used

* VLAN (Virtual LAN)
* Inter-VLAN Routing (Router-on-a-Stick)
* OSPF (Dynamic Routing Protocol)
* DHCP (Dynamic IP Allocation)
* SSH (Secure Remote Access)
* Port Security (Sticky MAC)
* Wireless Networking (WiFi)



## 🔐 Security Features

* SSH configured on all routers for secure remote login
* Port Security implemented on IT switch

  * Only **Test PC** allowed
  * Sticky MAC address
  * Violation mode: Shutdown



## 🖥️ Special Configuration

* **Test PC** connected to IT switch (Fa0/1)
* Used for:

  * SSH testing
  * Network verification


## 📡 Network Services

* DHCP configured on routers
* All devices obtain IP addresses dynamically
* Full communication enabled across all VLANs



## ✅ Testing & Verification

The network was tested for:

* Inter-VLAN communication
* Router connectivity (OSPF)
* DHCP functionality
* SSH remote login
* End-to-end communication across all floors



## 🎯 Project Outcome

* Successfully designed a **multi-floor enterprise network**
* Implemented **secure and scalable architecture**
* Achieved **full connectivity across departments**
* Applied real-world networking concepts


## 🚀 Skills Demonstrated

* Network Design & Topology Planning
* VLAN Configuration
* Routing (OSPF)
* Network Security
* Troubleshooting
* Cisco Packet Tracer Simulation



## 📷 Screenshots

<img width="1745" height="1396" alt="network" src="https://github.com/user-attachments/assets/2b6b16a4-d718-418d-97b3-4007a3d2beb3" />


* Network topology
* VLAN configuration
* OSPF routing table
* Successful ping results



## 👨‍💻 Author

**Amir Khan**
BS Computer Science Student
| Aspiring Network Engineer | Cybersecurity Enthusiast


## 📌 Note

This project is created for **academic and learning purposes** to simulate a real-world hotel network environment.

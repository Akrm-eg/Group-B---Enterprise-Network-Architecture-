# 🌐 Enterprise Network Architecture (Huawei Datacom)

![Status](https://img.shields.io/badge/Status-Finished-green?style=for-the-badge)
![Huawei](https://img.shields.io/badge/Platform-Huawei%20Datacom-red?style=for-the-badge&logo=huawei)
![Simulation](https://img.shields.io/badge/Simulator-eNSP-blue?style=for-the-badge)
![Security](https://img.shields.io/badge/Security-Enabled-success?style=for-the-badge&logo=shield)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

---

## 📖 Overview
This project implements a **secure and resilient enterprise network architecture** using **Huawei Datacom technologies** in a simulated **eNSP environment**.  
It connects a **Headquarters (HQ)** and **Other Branch Offices** over a simulated ISP, ensuring **secure connectivity, centralized services, and high availability**.

---

## 👥 Team Members
- Akrm Usama  
- Husein Mohamed  
- Hanaa Elhamamy  
- Mohamed Ramadan  


---

## 🚀 Features & Objectives
- 🔒 **Secure WAN Connectivity** with IPSec VPN tunnels  
- 🖥️ **Centralized Services** at HQ (DHCP, FTP, AAA, VoIP, CCTV NVR)  
- 🖨️ **Site-local services** (printing, local NVR)  
- 📶 **Wireless & Wired Access** for employees and guests  
- 🛡️ **Traffic Segmentation with VLANs** (Employees, Guest, Servers, CCTV, Printers, Management,.......)  
- 🔄 **Redundant DHCP** for reliability  
- ⚙️ **Centralized Management & Security**  

---

## 🏗️ Network Design
- **Central Services at HQ:** DHCP, FTP, AAA, VoIP PBX, Core NVR  
- **ISP Connectivity:** RIP protocol simulating ISP routers  
- **Local Access:** Switches + Wireless APs  
- **CCTV:** Distributed NVRs with central HQ access
- **VOIP:** Separated Server for every branch 

---

## 🌐 HQ VLAN  Architecture
| VLAN ID | Subnet Example   | Purpose             |
|---------|------------------|---------------------|
| 10      | 10.0.x.0/24      | Employees           |
| 20      | 10.0.x.0/24      | Voice / VoIP        |
| 30      | 10.0.x.0/24      | Servers (FTP, AAA)  |
| 40      | 10.0.x.0/24      | CCTV + NVR          |
| 50      | 10.0.x.0/24      | Guest Internet      |
| 60      | 10.0.x.0/24      | Printers            |
| 200     | 10.0.x.0/24      | Management          |

## 🌐 Branch VLAN  Architecture
| VLAN ID | Subnet Example   | Purpose             |
|---------|------------------|---------------------|
| 10      | 10.2.x.0/24      | Employees           |
| 20      | 10.2.x.0/24      | Voice / VoIP        |
| 30      | 10.2.x.0/24      | Servers (FTP, AAA)  |
| 40      | 10.2.x.0/24      | CCTV + NVR          |
| 50      | 10.2.x.0/24      | Guest Internet      |
| 60      | 10.2.x.0/24      | Printers            |
| 200     | 10.2.x.0/24      | Management          |
---

## 🔐 Security Features
- **ACLs** for sensitive resources (FTP, CCTV)  
- **WPA2/3 wireless security**  
- **DHCP snooping & ARP inspection**  

---

## ✅ Acceptance Criteria
- ✅ 100% DHCP functionality across all sites  
- ✅ 24/7 CCTV availability from HQ  
- ✅ Guest VLAN Internet-only access  
- ✅ Printers only accessible within local VLAN  

---

## 📊 Project Progress
- [x] Network architecture design  
- [x] VLAN planning & segmentation  
- [x] Device configuration (routers, switches, firewalls)  
- [x] Service deployment (DHCP, AAA, FTP, VoIP, CCTV)  
- [x] Testing & validation against acceptance criteria  
- [x] Final documentation & optimization  

---

## 🛠️ Tools & Technologies
- Huawei eNSP  
- VLANs & ACLs  
- DHCP, AAA , VRRP , GRE , RIP 
- FTP & CCTV (NVR)
- VOIP 

---

## 📌 Conclusion
This design provides a **scalable, secure, and future-ready enterprise network**, supporting business-critical services while ensuring **performance, reliability, and security**.


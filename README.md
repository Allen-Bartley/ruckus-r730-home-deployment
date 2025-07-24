# 🚀 Enterprise Wi-Fi Deployment: Ruckus R730 Setup in a Legacy Home

---

## 🎯 Project Overview

This project documents the configuration and deployment of a Ruckus R730 Wi-Fi 6 access point in a legacy residential home where standard consumer-grade equipment failed to provide adequate coverage. By repurposing an enterprise-grade AP and adapting it to standalone use, the goal was twofold:

✅ **Solve a real-world technical challenge:** Restore strong, stable wireless coverage across a structurally complex house.
🚀 **Build professional credibility:** Learn hands-on with enterprise gear to improve practical skills and support IT career growth.

---

## 📜 Background & Motivation

Following the passing of my aunt and uncle, my brother and I received modest inheritances, and I inherited their home in Foster, West Virginia. While cleaning and renovating to make it livable, I began envisioning a space where I could grow professionally through IT and home lab projects. However, Wi-Fi coverage was poor—likely due to the home’s construction, which included sheetrock walls backed by hardwood paneling. This severely limited wireless signal range.

With job prospects in mind, I searched for used enterprise gear on eBay and found a Ruckus R730 access point. I hoped this would not only solve the wireless issue but also give me a valuable, hands-on learning experience with enterprise networking equipment.

This deployment became a home lab milestone and a symbolic turning point as I settled into a new chapter.

---

## 🛠️ Equipment List

| Item                         | Details                                                   |
| ---------------------------- | --------------------------------------------------------- |
| **Ruckus R730 Access Point** | Wi-Fi 6 enterprise AP, early chipset revision             |
| **PoE Injector**             | High-wattage (802.3at), matched to AP power needs         |
| **Ethernet Cables**          | Cat5e+ for stable throughput                              |
| **Windows 11 Laptop**        | Used for configuration, firmware upload, and IP discovery |

---

## 🔧 Technical Walkthrough: From Brick to Broadcast

### ✉️ Step 1: Gaining Initial Access

The device arrived password-locked. I performed a factory reset using the physical reset pinhole, restoring it to factory defaults and allowing access via the default IP address through a direct Ethernet connection.

### 🔄 Step 2: Firmware Discovery & Troubleshooting

Research revealed that due to the early Wi-Fi 6 chipset, this model was **incompatible with Ruckus's Unleashed firmware**, which is commonly used for controller-less setups. The chipset didn’t support newer firmware builds, so a different route was necessary.

### 🔎 Step 3: Sourcing and Flashing Solo Firmware

I located the appropriate Solo firmware on Ruckus's support site and verified its compatibility with my hardware revision. After downloading the correct firmware and logging into the web interface, I successfully flashed the device. The AP rebooted into the Solo interface with a streamlined configuration dashboard.

### 📶 Step 4: Final Network Configuration

Following reboot:

* Created separate SSIDs for **2.4 GHz** and **5 GHz** bands
* Enabled **WPA2/WPA3 encryption** and changed default credentials
* Manually selected wireless channels to reduce interference from neighboring access points
* Verified signal strength in previously unreachable zones

---

## 🧠 Challenges & Solutions Summary

| Challenge                        | Solution                                                      |
| -------------------------------- | ------------------------------------------------------------- |
| **Proprietary Firmware Lockout** | Factory reset and Solo firmware flash                         |
| **Unleashed Incompatibility**    | Adapted to chipset limitations using Solo AP firmware         |
| **Power & Cabling Requirements** | Installed high-wattage PoE injector for single cable solution |
| **Signal Loss in Dense Walls**   | Used enterprise-grade hardware and optimal placement          |

---

## 📡 Deployment Outcome

* ✅ **Operational Success:** Stable, high-performance Wi-Fi now reaches all corners of the home—including rooms that previously had no signal.
* 🎓 **Career Impact:** Experience gained in working with enterprise APs, firmware flashing, and PoE setups.
* 📚 **Personal Milestone:** This setup marked both a technical win and a personal moment of reclaiming and reimagining a meaningful space.

---

## 🔍 Skills Showcased

* Enterprise Hardware Integration
* Standalone Firmware Deployment
* PoE Implementation
* Wireless Security Configuration
* Environmental Troubleshooting
* Technical Documentation

---

## 🤝 Contributing or Learning From This Project?

This project is part of my personal IT portfolio to document hands-on experience with enterprise networking hardware. If you’re working on similar setups or studying for certifications like **CompTIA Network+**, **ISC2 CC**, or **Cisco CCNA**, feel free to fork this repo or ask questions!

🔗 [Portfolio](https://github.com/Allen-Bartley/personal-portfolio)

---

## 📉 Project Metadata

* 📌 **Status:** In Production
* 🗓️ **Deployment Date:** July 2025
* 🏡 **Location:** Legacy Home, Foster, West Virginia
* 👨‍💻 **Maintainer:** Allen Bartley

---

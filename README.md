# Ruckus R730 Wi-Fi 6 Access Point Setup

![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)
![Hardware](https://img.shields.io/badge/Hardware-Enterprise_WiFi-orange?style=flat-square)
![Skill](https://img.shields.io/badge/Skill-Firmware_Flash-blue?style=flat-square)
![Difficulty](https://img.shields.io/badge/Difficulty-Intermediate-yellow?style=flat-square)

## 🎯 Project Overview

This project documents setting up a used Ruckus R730 enterprise access point to solve Wi-Fi coverage issues in a house with dense walls. The R730 is an end-of-life enterprise AP that was Ruckus's first Wi-Fi 6 model, but it used early Wi-Fi 6 chips that weren't fully compliant with the final standard.

The main challenge was getting it working in standalone mode since Ruckus never released their standard "Unleashed" controller-free firmware for this particular model, likely due to the early chipset limitations.

---

## 🏠 Background & Problem

**The Issue:**
- Inherited a house with very poor Wi-Fi coverage
- Thick walls with hardwood paneling backing interfered with wireless signals
- Consumer routers couldn't provide adequate coverage throughout the house

**The Solution:**
- Purchased a used Ruckus R730 enterprise access point from eBay
- Goal was to solve the coverage problem while gaining hands-on experience with enterprise networking gear

---

## 🛠️ Hardware & Equipment

**Main Components:**
- **Ruckus R730 Access Point** (used, end-of-life enterprise model)
- **High-wattage PoE injector** (802.3at compatible)
- **Ethernet cables** (Cat5e)
- **Windows 11 laptop** for configuration

**Key Hardware Notes:**
- R730 was Ruckus's first Wi-Fi 6 access point
- Used early/prototype Wi-Fi 6 chips before the standard was finalized
- Required more power than standard consumer equipment

---

## 🔧 Setup Process

### Initial Access
1. **Factory Reset**: Device came password-protected from previous use
2. **Physical Reset**: Used pinhole reset button to restore factory defaults
3. **Direct Connection**: Connected laptop directly via Ethernet to access web interface

### Firmware Challenge
4. **Research**: Discovered this model lacks Unleashed firmware support
   - Unleashed = Ruckus's controller-free firmware for small deployments
   - Early Wi-Fi 6 chipset wasn't compatible with newer firmware builds
5. **Alternative Solution**: Located "Solo" firmware on Ruckus support site
   - Solo firmware designed for standalone operation without controller

### Firmware Installation
6. **Downloaded** correct Solo firmware version for hardware revision
7. **Flashed firmware** through web interface
8. **Verified** successful installation and reboot to Solo interface

### Network Configuration
9. **Created separate SSIDs** for 2.4GHz and 5GHz bands
10. **Configured security** with WPA2/WPA3 encryption
11. **Set custom channels** to avoid interference from neighbors
12. **Changed default credentials** and tested coverage

---

## ⚠️ Challenges Encountered

### Firmware Compatibility Issue
**Problem**: Standard Unleashed firmware wasn't available for this model
**Root Cause**: Early Wi-Fi 6 chipset predated final Wi-Fi 6 standard
**Solution**: Used Solo firmware instead, which provided standalone functionality

### Power Requirements
**Problem**: Higher power needs than consumer equipment
**Solution**: Purchased appropriate high-wattage PoE injector

### Coverage Planning
**Problem**: Dense wall construction interfering with signal
**Solution**: Strategic placement and enterprise-grade hardware provided needed coverage

---

## ✅ Results

**Successful Outcomes:**
- ✅ Full Wi-Fi coverage throughout the house, including previously dead zones
- ✅ Stable, high-performance wireless connectivity
- ✅ Hands-on experience with enterprise networking equipment
- ✅ Working knowledge of PoE implementation and enterprise AP configuration

**Performance Improvements:**
- Eliminated Wi-Fi dead zones in bedrooms and back rooms
- Consistent signal strength throughout the property
- Better performance than consumer routers in challenging environment

---

## 📚 Learning Outcomes

**Technical Skills Gained:**
- Enterprise access point configuration and setup
- Firmware research and installation procedures
- PoE power planning and implementation
- RF planning considerations for challenging environments

**Enterprise Equipment Experience:**
- Working with end-of-life enterprise gear
- Understanding firmware compatibility issues
- Adapting when standard solutions aren't available
- Enterprise vs. consumer equipment capabilities

**Problem-Solving Process:**
- Researching hardware limitations and workarounds
- Finding alternative firmware when standard options unavailable
- Balancing cost vs. performance for home lab use

---

## 💡 Key Takeaways

**Why This Approach Worked:**
- Enterprise hardware handled RF challenges better than consumer equipment
- Early research prevented compatibility surprises
- Solo firmware provided needed standalone functionality

**Lessons Learned:**
- End-of-life enterprise gear can be cost-effective for learning
- Always verify firmware availability before purchasing used enterprise equipment
- Early adoption hardware (like first-gen Wi-Fi 6) may have limited support

**Value for Career Development:**
- Practical experience with enterprise networking hardware
- Understanding of RF planning and deployment challenges
- Firmware management and troubleshooting skills

---

## 🔗 Related Projects

- [`residential-network-architecture`](https://github.com/Allen-Bartley/residential-network-architecture) - Overall network design
- [`personal-tech-inventory`](https://github.com/Allen-Bartley/personal-tech-inventory) - Lab equipment documentation

---

> **Project Status:** Complete and operational  
> **Deployment Date:** July 2025  
> **Current Status:** Providing reliable Wi-Fi coverage throughout property  
> **Skills Focus:** Enterprise networking hardware, firmware management, RF planning
# Homelab Network Architecture

This document describes the physical and logical network layout used in my personal homelab.

The goal is to keep the infrastructure simple, reliable, and expandable while separating critical services from experimental systems.

---

## Network Hardware

Router  
TP-Link Archer MR500

Switch  
Unmanaged Ethernet switch

ISP Device  
ISP modem

These components form the base network infrastructure.

---

## 🗺️ Planned Network Architecture

Internet
   │
ISP Modem
   │
Router (TP-Link Archer MR500)
   │
Switch
   ├── 🥧 Raspberry Pi (DNS / Pi-hole)
   ├── 🧠 Mini PC (Server / NAS)
   ├── 🎮 Main PC
   └── 🧑‍💻 Secondary PC (Guest Workstation)

---

## Design Principles

The network follows several design principles:

Simplicity  
The setup uses minimal hardware while remaining reliable.

Service Separation  
Critical network services are isolated from experimental workloads.

Low Power Infrastructure  
Always-on services run on low-power devices.

Scalability  
The architecture allows additional systems to be added easily.

---

## 🧠 Device Roles

### 🥧 Raspberry Pi
- DNS filtering (Pi-hole)
- Network services
- Optional VPN access

### 🧠 Mini PC
- Docker host
- Media server
- File storage (NAS)
- Game servers

### 🎮 Secondary PC
- Guest gaming system
- Workstation use
- Testing environment

### 🎮 Main PC
- Personal use
- Gaming

---

## Future Improvements

## 🛒 Hardware Acquisition Plan

### Priority 1
- Raspberry Pi 4 (4GB or 8GB)
- Power supply
- MicroSD card

### Priority 2
- Mini PC (Intel i5 or similar)
- RAM upgrade (if needed)
- SSD storage

### Priority 3
- UPS (optional)
- Network upgrades (future)

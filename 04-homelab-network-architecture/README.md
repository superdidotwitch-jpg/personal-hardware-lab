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

## Network Topology

Internet
   │
Modem
   │
Router (TP-Link Archer MR500)
   │
Unmanaged Switch
   ├── Raspberry Pi (Pi-hole DNS)
   ├── Mini PC (Server)
   └── Gaming PC

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

## Role of Each Device

Router  
Handles internet connectivity, NAT, and wireless networking.

Switch  
Provides simple wired connectivity between systems.

Raspberry Pi  
Runs network infrastructure services such as DNS filtering.

Mini PC Server  
Runs heavier workloads including containers, game servers, and media services.

Gaming PC  
Used for personal computing and gaming workloads.

---

## Future Improvements

Possible upgrades include:

- Managed switch with VLAN support
- Network monitoring
- Reverse proxy for external services
- Dedicated NAS storage

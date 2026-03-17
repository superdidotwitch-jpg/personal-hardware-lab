# Mini Homelab Project

This project explores building a compact, Raspberry Pi-driven homelab using a minimal hardware footprint.

The goal is to simulate advanced networking concepts using simple and affordable hardware.

---

## Core Idea

A Raspberry Pi acts as the central controller for network services while a small unmanaged switch provides physical connectivity.

The system focuses on software-defined networking concepts without requiring expensive managed hardware.

---

## Hardware Design

Raspberry Pi (external)

- Handles all network services
- Runs Docker and monitoring tools

Unmanaged Switch

- Provides basic connectivity
- No VLAN support at hardware level

Custom 3D-Printed Case

- Houses switch PCB
- Includes airflow and cable routing
- Designed to resemble a mini PC

---

## Software Stack

Pi-hole  
DNS filtering and ad blocking

Dnsmasq  
DHCP and VLAN tagging

iptables / nftables  
Firewall and segmentation

WireGuard / OpenVPN  
Secure remote access

Docker  
Service isolation

Grafana + Prometheus  
Monitoring and metrics

---

## Networking Concepts

- VLAN segmentation (software-defined)
- DHCP per VLAN
- Firewall rules per network segment
- Traffic monitoring

---

## Learning Outcomes

- Linux system administration
- Networking fundamentals
- Docker containerization
- VPN configuration
- Monitoring and observability

---

## Future Improvements

- OLED display for system stats
- Multi-Pi clustering
- IoT integration
- PoE-powered setup

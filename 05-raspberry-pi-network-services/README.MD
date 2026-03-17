# Raspberry Pi Network Services

This project documents the Raspberry Pi used to run critical network services within the homelab.

The Raspberry Pi is dedicated to lightweight infrastructure tasks that must remain available even if other systems are offline.

---

## Hardware

Device  
Raspberry Pi 4

Memory  
4GB RAM

Storage  
MicroSD card (32–128GB recommended)

Power  
USB-C power supply

Optional upgrades include:

- SSD via USB 3.0
- UPS HAT for power protection
- Passive cooling case

---

## Primary Service

Pi-hole DNS Filtering

Pi-hole acts as the network DNS server and blocks advertising and tracking domains.

Benefits include:

- Network-wide ad blocking
- Reduced tracking
- Faster browsing
- Centralized DNS control

---

## Why Use a Raspberry Pi

Low power consumption (~5W)

Silent operation

Always-on reliability

Separation from experimental servers

---

## Possible Additional Services

The Raspberry Pi may also run:

WireGuard VPN  
Network monitoring tools  
DHCP services  
DNS caching

---

## Integration with the Homelab

The Raspberry Pi is connected directly to the network switch and serves all devices on the network.

This keeps core infrastructure separate from experimental systems running on the server.

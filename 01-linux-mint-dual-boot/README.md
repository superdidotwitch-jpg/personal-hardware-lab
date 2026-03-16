# Linux Mint Dual Boot Journey

This document records my experience installing Linux Mint alongside Windows as part of my homelab learning process.

---

## Goal

Install Linux Mint Cinnamon alongside Windows while keeping both operating systems usable.

This setup allows experimentation with Linux without losing access to Windows.

---

## Initial Plan

- Install Linux Mint Cinnamon 22.2
- Allocate 100GB partition for Linux
- Keep Windows installation intact
- Use Linux for homelab experiments and server learning

---

## Problems Encountered

### Partition Size Issue

The original plan was to allocate 100GB, but only 50GB was available during installation.

Possible causes:

- Existing disk layout
- Previous partitions
- SSD configuration

---

### Bootloader Issue

After installation the system booted directly into Windows.

GRUB (Linux bootloader) was not appearing.

---

### USB Boot Issue

Initially the Linux Mint USB did not boot correctly and the system went straight into Windows.

Possible causes:

- USB not detected
- Secure Boot enabled
- Boot order configuration

---

## USB Creation

A bootable Linux USB was created using Rufus.

Recommended settings:

Partition scheme: GPT  
Target system: UEFI  
File system: FAT32  

---

## Boot Menu

Once the USB boot worked, the following options appeared:

- Start Linux Mint 22.2 Cinnamon 64-bit
- OEM Install
- Compatibility Mode
- Boot from next volume
- UEFI Firmware Settings
- Memory Test

---

## Installation Choice

The recommended option was:

Install Linux Mint alongside Windows Boot Manager

This automatically manages partitions and installs GRUB.

Other options:

Erase disk and install Linux Mint (not used)

Manual partitioning (advanced option)

---

## GRUB Repair Method

If GRUB does not appear after installation, it can be repaired using the Live USB.

Steps:

Boot into the Linux Mint live environment.

Open a terminal and run:

lsblk

Mount the Linux partition and reinstall GRUB if necessary.

Another option is to use the Boot Repair tool.

---

## Outcome

Linux Mint was successfully installed alongside Windows.

This project served as the first step in learning Linux and building a personal homelab environment.

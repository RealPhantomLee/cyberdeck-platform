# 🔌 Wiring & Connections  
Brick 2 — Cyberdeck

This document describes how hardware components are connected at a system level.

It is **not a step-by-step wiring guide**.

---

## Core Signal Paths

### Power
- Battery / power bank → Raspberry Pi
- Power must be stable at 5V
- Undervoltage causes instability and data corruption

---

### Storage
- microSD → Primary boot device
- Optional SSD → Secondary storage via USB or NVMe (Pi 5)

---

### Input
- Keyboard / controller → USB or Bluetooth
- Mouse is optional; system is keyboard-first

---

### Display
- HDMI → Primary display (if used)
- OLED → GPIO / I2C (optional, non-essential)

---

## Optional Peripheral Connections

### Networking
- External Wi-Fi adapter → USB
- Ethernet → Onboard or USB adapter

---

### Camera
- Pi Camera → CSI ribbon connector
- Used only if camera functionality is enabled

---

### Audio
- Speaker / mic → USB or GPIO
- Audio not required for baseline operation

---

## Design Notes

- Avoid unnecessary GPIO complexity early
- Prefer USB peripherals for modularity
- All optional components must be removable without breaking core functionality

---

## Diagrams

Visual diagrams and photos (if created) should be stored in:


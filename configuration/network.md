# 🌐 Network Configuration  
Brick 2 — Cyberdeck

This document describes the baseline networking configuration and expectations for the cyberdeck.

It focuses on **connectivity, safety, and predictability**.

---

## Network Philosophy

The cyberdeck should:
- Connect reliably when needed
- Remain silent when not in use
- Avoid unnecessary services
- Be predictable in unfamiliar environments

Networking is treated as **intentional**, not passive.

---

## Supported Network Interfaces

### Wired
- Ethernet (onboard or USB)
- Preferred for stability and labs

### Wireless
- Internal Wi-Fi (basic connectivity)
- External Wi-Fi adapters may be added later

Bluetooth is optional and disabled by default unless required.

---

## Default Behavior

- No automatic connection to unknown networks
- No broadcast services enabled by default
- No exposed services without intent
- SSH access only when explicitly enabled

---

## Headless Networking

The cyberdeck must support:
- SSH over Ethernet or Wi-Fi
- Operation without display or input peripherals

Network access should not depend on a GUI.

---

## Public vs Private Environments

Extra caution is required when:
- Using public Wi-Fi
- Operating in shared spaces
- Connecting to unknown infrastructure

These environments increase risk and should be treated accordingly.

---

## Notes

- Network configuration decisions should be logged in `notes.txt`
- Offensive or monitoring configurations belong in later bricks
- Simplicity is preferred over flexibili

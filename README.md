# Brick 2 — Cyberdeck Platform

**A portable, modular Raspberry Pi cyberdeck for field cybersecurity work — hardware selection, OS hardening, power, and reproducible build docs.**

This is **Brick #2** of a portable Kali Live USB security platform. See [Related projects](#related-projects).

---

## Overview

Brick 2 turns the persistent operating system from [Brick 1](https://github.com/RealPhantomLee/live-usb-encrypted-persistence) into a **physical, deployable system** that can be operated at a desk, in a lab, or in the field. The emphasis here is **hardware integration, mobility, power management, and documentation** — not offensive techniques (those belong to later bricks).

> Brick 1 is the brain. Brick 2 is the body.

---

## Brick Stack relationship

- **Depends on Brick 1** — Live USB or installed OS with encrypted persistence and hardened Linux baseline
- **Enables Bricks 3+** — operator HUD, security toolchain, SIEM, vulnerability management, and field workflows

---

## Goals

- Build a **portable, modular cyberdeck**
- Maintain **legal and ethical boundaries**
- Produce **repeatable documentation** so anyone can rebuild it
- Support **headless or local operation**
- Enable future expansion without redesign

---

## Design principles

- **Portable** — usable without fixed infrastructure
- **Modular** — components can be swapped or upgraded
- **Documented** — every decision is recorded
- **Repeatable** — rebuildable by following the docs alone
- **Field-ready** — stable power and networking

---

## Scope

### Included
- Hardware selection and layout
- Power solutions and optimization
- OS installation or cloning from Brick 1
- User hardening and basic configuration
- Networking setup (non-offensive)
- Optional display / headless workflows
- Build documentation and photos

### Explicitly excluded
- Wireless attacks
- Exploitation frameworks
- Payload delivery
- Red-team techniques

These belong in later bricks (toolchain layer, vulnerability management lab).

---

## Hardware baseline

### Minimum viable cyberdeck

| Component | Choice |
|-----------|--------|
| Compute | Raspberry Pi 4 (4–8 GB) or Pi 5 |
| Case | Protective or cyberdeck-style enclosure |
| Power | Battery bank or internal battery (5V/3A min for Pi 5) |
| Storage | microSD card (32 GB+) — optional SSD via USB 3.0 |
| Input | Compact USB keyboard or wireless controller |
| Display | Built-in screen, HDMI portable monitor, or headless SSH |

### Optional enhancements

- External Wi-Fi adapter with monitor-mode support (e.g., Alfa AWUS036ACS)
- OLED status display (I²C, 128×64) for power / network at-a-glance
- Camera module for photo / OSINT workflows
- Speaker and microphone for offline notes / TTS
- NVMe or USB-SSD upgrade path
- Touchscreen or e-ink display
- GPS receiver (NMEA over USB) for wardriving studies

---

## Repository layout

| Path | Purpose |
|------|---------|
| `hardware/` | BOM, wiring, power-budget notes |
| `os/` | OS install + clone procedures from Brick 1 |
| `configuration/` | Hardening configs, dotfiles, systemd unit overrides |
| `scripts/` | Setup automation (network, power-saving, headless) |
| `assets/` | Photos, diagrams, sticker-mockups |
| `CHANGELOG.md` | Build revisions and lessons learned |

---

## Build status

| Phase | Status |
|-------|--------|
| Hardware selection | ✅ Documented |
| OS clone from Brick 1 | ✅ Working |
| Hardening baseline | ✅ Applied |
| Networking (non-offensive) | ✅ Configured |
| Optional OLED layer | 🔄 In progress (see [Brick #3 HUD](https://github.com/RealPhantomLee/interface-hud-operator-controls)) |
| Field-ready power profile | ✅ Tested |

---

## Legal & ethical use

This platform is designed for **authorized testing only** — your own systems, deliberately vulnerable labs (HackTheBox, VulnHub), or systems you have written permission to test. The cyberdeck is not a weapon; it is a portable workstation.

---

## Related projects

This repo is part of a portable Kali Live USB security platform:

- [live-usb-encrypted-persistence](https://github.com/RealPhantomLee/live-usb-encrypted-persistence) — Brick #1: encrypted persistent USB
- **cyberdeck-platform** (this repo) — Brick #2: hardware platform
- [interface-hud-operator-controls](https://github.com/RealPhantomLee/interface-hud-operator-controls) — Brick #3: operator HUD
- [toolchain-layer](https://github.com/RealPhantomLee/toolchain-layer) — Brick #4: security tool inventory
- [logging-siem-wazuh](https://github.com/RealPhantomLee/logging-siem-wazuh) — Brick #5: SIEM
- [vulnerability-management-lab](https://github.com/RealPhantomLee/vulnerability-management-lab) — Brick #6: end-to-end VM lifecycle lab

---

## Author

**RealPhantomLee Tucker** — [github.com/RealPhantomLee](https://github.com/RealPhantomLee)

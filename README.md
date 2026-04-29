# 🧱 Brick 2 — Cyberdeck  
**Portable Cybersecurity Platform**


::contentReference[oaicite:0]{index=0}


---

## 📌 Overview

Brick 2 focuses on designing and building a **portable cyberdeck**—a self-contained, mobile computing platform used for cybersecurity labs, diagnostics, education, and portfolio demonstrations.

This brick transforms the **persistent operating system created in Brick 1** into a **physical, deployable system** that can be operated in the field, at a desk, or in a lab environment.

The emphasis of Brick 2 is **hardware integration, mobility, power management, and documentation**, not offensive techniques.

---

## 🔗 Brick Stack Relationship

- **Depends on Brick 1**  
  - Live USB or installed OS with encrypted persistence  
  - Hardened Linux environment  

- **Enables Brick 3+**  
  - Wireless testing  
  - Automation  
  - Advanced tooling  
  - Field-ready workflows  

> Brick 1 is the brain.  
> Brick 2 is the body.

---

## 🎯 Goals

- Build a **portable, modular cyberdeck**
- Maintain **legal and ethical boundaries**
- Create **repeatable documentation**
- Support **headless or local operation**
- Enable future expansion without redesign

---

## 🧠 Design Principles

- **Portable** – usable without fixed infrastructure  
- **Modular** – components can be swapped or upgraded  
- **Documented** – every decision is recorded  
- **Repeatable** – rebuildable by others  
- **Field-Ready** – stable power and networking  

---

## 🧩 Scope of This Brick

### Included
- Hardware selection and layout
- Power solutions and optimization
- OS installation or cloning from Brick 1
- User hardening and basic configuration
- Networking setup (non-offensive)
- Optional display / headless workflows
- Build documentation and photos

### Explicitly Excluded
- Wireless attacks
- Exploitation frameworks
- Payload delivery
- Red-team techniques

(Those belong in later bricks.)

---

## 🛠 Hardware Baseline

**Minimum Viable Cyberdeck**
- Raspberry Pi 4 or 5  
- Protective or cyberdeck-style case  
- Power source (battery bank or internal battery)  
- Storage (microSD ± SSD)  
- Input device (keyboard / controller)  
- Display or headless SSH  

**Optional Enhancements**
- External Wi-Fi adapter (monitor mode capable)
- OLED status display
- Camera module
- Speaker / microphone
- NVMe or USB SSD
- To

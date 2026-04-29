# 🔐 Encryption  
Brick 2 — Cyberdeck

This document explains the encryption strategy used for the cyberdeck.

Encryption is considered **mandatory**, not optional.

---

## Why Encryption Is Required

The cyberdeck is:
- Portable
- Removable
- Intended for field use

Without encryption:
- Loss = data exposure
- Theft = credential compromise
- Physical access = full system access

Encryption mitigates these risks.

---

## Encryption Scope

At minimum, encryption should cover:
- User home directories
- Tooling and logs
- Configuration files
- Credentials and keys

Preferred approach:
- Full disk encryption

Acceptable alternative:
- Encrypted partitions for sensitive data

---

## Threat Model (High-Level)

Encryption protects against:
- Device loss
- Unauthorized physical access
- Casual inspection of storage media

It does **not** protect against:
- Compromised running system
- Weak passwords
- Poor operational security

---

## Passphrase Considerations

- Must be strong but memorable
- Must be usable in field conditions
- Should not be written on the device

---

## Operational Notes

- Encryption adds boot-time friction (intentional)
- Boot requires physical presence
- Headless unlock must be considered during setup

---

## Notes

- Encryption method should be recorded in `notes.txt`
- Weak encryption defeats the purpose
- Encryption decisions affect usability—tradeoffs are acceptable

---

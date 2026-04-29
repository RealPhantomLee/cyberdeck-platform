# 👤 Users & Hardening  
Brick 2 — Cyberdeck

This document outlines basic user and system hardening expectations for the cyberdeck.

The goal is **reasonable security without unnecessary complexity**.

---

## User Model

- Single primary user is expected
- Root access is restricted
- Elevated privileges are intentional and limited

The cyberdeck is not a multi-user server.

---

## Account Principles

- Strong passwords are mandatory
- Default credentials are not acceptable
- User permissions should follow least privilege

Convenience should not override basic security.

---

## Service Exposure

- Unused services should be disabled
- No services should start automatically without reason
- Local-only services are preferred

---

## Physical Access Assumptions

- Physical access equals high risk
- Encryption is the primary mitigation
- Device should not be left unattended while unlocked

---

## Update Philosophy

- Updates are intentional, not automatic
- Stability is prioritized over cutting-edge versions
- Changes should be understood before applied

---

## Notes

- Hardening decisions should be logged in `notes.txt`
- Advanced security tooling belongs in later bricks
- Over-hardening at this stage is discouraged

---

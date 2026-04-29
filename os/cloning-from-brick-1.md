# 🧬 Cloning from Brick 1  
Brick 2 — Cyberdeck

This document explains how the Brick 1 environment is reused for Brick 2.

Cloning is a **design choice**, not a requirement.

---

## Conceptual Overview

Brick 1 establishes a:
- Hardened OS
- Encrypted environment
- Known-good baseline

Brick 2 reuses that environment by cloning it onto new hardware.

This creates **continuity across the stack**.

---

## What Is Being Cloned

Typically included:
- Operating system
- User configuration
- Encryption layout
- Base tooling
- Shell environment

Not guaranteed:
- Hardware-specific drivers
- Power profiles
- Interface settings

---

## Why Cloning Is Useful

- Reduces configuration drift
- Preserves security posture
- Saves time
- Makes rebuilds predictable

Brick 1 becomes the **reference implementation**.

---

## Hardware Differences

When cloning to new hardware:
- Drivers may need adjustment
- Display settings may differ
- Power behavior may change

These changes do **not** invalidate the clone.

They are expected.

---

## When NOT to Clone

Cloning may be avoided if:
- Architecture differs significantly
- Clean rebuild is desired
- Brick 1 environment is outdated

A fresh install is acceptable in these cases.

---

## Notes

- Cloning method details are intentionally omitted
- Chosen approach should be logged in `notes.txt`
- Major divergence from Brick 1 should be documented

---

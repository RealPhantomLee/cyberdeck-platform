# ⚠️ Sudo Usage Notes — Brick 2 Cyberdeck

Some setup scripts require elevated privileges (`sudo`) to perform system-level tasks.

This file explains **why sudo is needed**, **which scripts require it**, and **how to use them safely**.

---

## Why Sudo Is Used

Sudo is required only when a script needs to:
- Modify system configuration files (`/etc`)
- Manage system services (SSH, NetworkManager)
- Install or update system packages
- Read system-level information

Scripts that do not require these actions are designed to run without sudo.

---

## Scripts That Require Sudo

| Script | Why |
|------|-----|
| `00_first_boot.sh` | Sets hostname, installs packages, manages services |
| `update_safe.sh` | Updates system packages and backs up system configs |
| `net_mode.sh` | Enables/disables Wi-Fi, Bluetooth, and SSH |
| `backup_configs.sh` | **Optional** — required only to back up `/etc` and package lists |

---

## Scripts That Do NOT Require Sudo

| Script | Notes |
|------|------|
| `status.sh` | Read-only system information |
| `backup_configs.sh` | Can run without sudo for user-level backups |

---

## Safe Usage Guidelines

- Always read the script before running with sudo
- Run scripts from a local terminal, not over unknown networks
- Avoid running sudo scripts on untrusted systems
- Do not modify scripts unless you understand the change

---

## Philosophy

Sudo is used **intentionally and sparingly** in Brick 2.

If a task can be done without elevated privileges, it should be.

Advanced privilege management belongs in later bricks.

---

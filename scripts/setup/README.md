# scripts/setup — Brick 2 Operational Scripts

These scripts exist to make the Cyberdeck **repeatable, stable, and less frustrating** to set up.

They are intentionally **Brick 2-safe**:
- device health
- backups
- conservative updates
- network hygiene

They do **not** include recon, monitoring, or offensive workflows (those belong in Brick 3+).

---

## Files

### `00_first_boot.sh`
First-boot baseline setup helper.
- Creates standard folders (`captures/`, `logs/`, `backups/`, etc.)
- Optionally sets hostname
- Optionally enables SSH (OFF by default)
- Installs basic comfort tools (git, tmux, htop, rsync, etc.)

Run:
```bash
sudo ./00_first_boot.sh

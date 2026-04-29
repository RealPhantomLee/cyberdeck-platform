# 🔋 Power Management  
Brick 2 — Cyberdeck

This document describes power expectations and management principles for the cyberdeck.

Power stability is critical to reliability and data integrity.

---

## Power Goals

- Prevent unexpected shutdowns
- Avoid undervoltage conditions
- Preserve battery health
- Maintain predictable runtime

---

## Power Sources

Supported options:
- External battery bank
- Internal battery system
- Wall power (development / lab use)

All power sources must provide **stable 5V output**.

---

## Runtime Expectations

- Battery runtime will vary by configuration
- Displays, fans, and peripherals increase draw
- Headless operation significantly extends runtime

Exact runtime is less important than **consistency**.

---

## Shutdown Behavior

- The system should be shut down cleanly
- Sudden power loss risks filesystem corruption
- Battery depletion should not be routine

---

## Thermal Considerations

- Heat increases power draw
- Poor airflow reduces component lifespan
- Fans trade noise for stability

Thermal and power decisions are linked.

---

## Notes

- Power observations should be recorded in `notes.txt`
- Major power architecture changes belong in `CHANGELOG.md`
- Optimization comes later; stability comes first

---

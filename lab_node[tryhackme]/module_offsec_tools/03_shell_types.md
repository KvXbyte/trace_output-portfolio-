# 💻 Shells Overview

---

### Covered Topics:

- Bind vs Reverse Shells
- Shell spawning and command access
- Web shells and file upload risks
- Stabilizing shells with `python`, `bash`, and `nc`

---

### Key Notes:

- Reverse shells connect back to the attacker; bind shells wait for the attacker to connect.
- `nc -lvnp` is a staple listener setup for basic reverse shells.
- Upgrading shell access using `python -c` or `script /bin/bash` improves interaction.
- Shells are the pivot point—what comes next depends on privilege and access.

---

> The first shell is the foothold. The second is where the real story begins.

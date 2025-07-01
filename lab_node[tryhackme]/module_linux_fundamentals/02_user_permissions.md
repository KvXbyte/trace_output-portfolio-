# 🔐 User Permissions, Groups & Ownership

## Covered Topics:
- Understanding users vs groups
- File permissions: `rwx` for owner, group, others
- `chmod`, `chown`, and `usermod`
- Sticky bits, SUID, and SGID (intro-level)

## Key Notes:
- Use `ls -l` to check permission string (e.g., `drwxr-xr-x`)
- Modify permissions numerically (`chmod 755`) or symbolically (`chmod u+x`)
- `chown user:group file.txt` is essential in ownership transitions

---

> Access defines risk. Managing it cleanly is the first step in reducing attack surfaces.

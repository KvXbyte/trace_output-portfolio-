# ⚔️ AD Security Basics: Permissions & Weak Points

## Covered Topics:
- Share enumeration and misconfigurations
- Credential exposure via network shares or cached files
- Pass-the-Hash and Kerberoasting (intro-level)
- Defensive practices for AD environments

## Key Notes:
- Open shares are gold mines. `net view \\target` and `net share` help spot them.
- NTLM hashes should never be stored in plaintext—yet often are.
- Detection > Prevention: many AD attacks are stealthy, but traceable if logged well.

---

> If AD is the castle, then visibility is your moat—and logs are the drawbridge sensors.

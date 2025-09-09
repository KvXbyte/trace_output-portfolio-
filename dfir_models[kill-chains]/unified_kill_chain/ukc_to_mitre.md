# Unified Kill Chain ↔ MITRE ATT&CK Mapping

This document provides a crosswalk between **Unified Kill Chain (UKC) phases** and **MITRE ATT&CK tactics & techniques**.  
It connects the *big-picture progression* (UKC) to the *granular actions* (ATT&CK).

---

## 📌 Persistence (Maintain Presence)
- **T1547.001 — Boot or Logon Autostart Execution: Registry Run Keys / Startup Folder**  
  - Common persistence method via registry modification or startup folder entries.  
  - Detection: Sysmon Event ID 13 (Registry Set), autorun entries, suspicious `reg add` usage.  

- **T1547.009 — Shortcut Modification**  
  - Attackers create or modify `.lnk` files to maintain execution across logons.  

- **T1136 — Create Account**  
  - Persistence via creation of new local/domain accounts.  

---

## 📌 Defense Evasion (Obfuscate)
- **T1070.006 — Timestomping**  
  - Altering file MACB timestamps to evade forensic timelines.  
  - Detection: $MFT vs $SI/$FN timestamp mismatch, improbable sequences.  

- **T1070.004 — File Deletion**  
  - Removing artifacts to cover tracks.  

- **T1562.001 — Disable Security Tools**  
  - Stopping AV/EDR processes or tampering with defenses.  

---

## 📌 Command & Control
- **T1071.001 — Application Layer Protocol: Web Protocols**  
  - C2 over HTTP/HTTPS.  

- **T1071.004 — Application Layer Protocol: DNS**  
  - DNS tunneling for covert communications.  

- **T1095 — Non-Application Layer Protocol**  
  - Raw TCP/UDP used for C2 traffic.  

---

## 📌 Impact
- **T1486 — Data Encrypted for Impact**  
  - Ransomware-style encryption of victim files.  

- **T1499 — Endpoint Denial of Service**  
  - Resource exhaustion (CPU, memory, disk) to disrupt operations.  

---

## 📝 Notes
- This file is **iterative**: start with a few mapped techniques and expand as new detections are studied.  
- Not every ATT&CK technique is required — only those relevant to SOC/DFIR workflows.  
- Links can be added to full ATT&CK entries:  
  - [T1547.001 — Registry Run Keys / Startup Folder](https://attack.mitre.org/techniques/T1547/001/)  
  - [T1070.006 — Timestomping](https://attack.mitre.org/techniques/T1070/006/)  

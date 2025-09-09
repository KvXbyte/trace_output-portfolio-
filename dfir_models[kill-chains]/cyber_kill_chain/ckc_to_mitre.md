# Cyber Kill Chain ↔ MITRE ATT&CK Mapping

This document maps the classic **Cyber Kill Chain (CKC) 7 phases** to relevant **MITRE ATT&CK tactics & techniques**.  
It serves as a simplified bridge between Lockheed Martin’s storyboard model and MITRE’s granular catalog.

---

## 📌 Reconnaissance
- **T1595 — Active Scanning**  
- **T1592 — Gather Victim Host Information**  
- **T1598 — Phishing for Information**

---

## 📌 Weaponization
*(CKC concept, not directly mirrored in ATT&CK — focus on malware/tool prep)*  
- **T1587 — Develop Capabilities**  
- **T1588 — Obtain Capabilities**  
- **T1608 — Stage Capabilities**

---

## 📌 Delivery
- **T1566.001 — Phishing: Spearphishing Attachment**  
- **T1566.002 — Phishing: Spearphishing Link**  
- **T1192 — Spearphishing via Service**  
- **T1204.002 — User Execution: Malicious File**

---

## 📌 Exploitation
- **T1190 — Exploit Public-Facing Application**  
- **T1068 — Exploitation for Privilege Escalation**  
- **T1203 — Exploitation for Client Execution**

---

## 📌 Installation
- **T1547.001 — Boot or Logon Autostart Execution (Registry Run Keys/Startup Folder)**  
- **T1543 — Create or Modify System Process**  
- **T1053 — Scheduled Task/Job**

---

## 📌 Command & Control
- **T1071.001 — Application Layer Protocol: Web Protocols**  
- **T1071.004 — Application Layer Protocol: DNS**  
- **T1090 — Proxy**  
- **T1572 — Protocol Tunneling**

---

## 📌 Actions on Objectives
- **T1005 — Data from Local System**  
- **T1041 — Exfiltration Over C2 Channel**  
- **T1486 — Data Encrypted for Impact (Ransomware)**  
- **T1499 — Endpoint Denial of Service**

---

## 📝 Notes
- Cyber Kill Chain is high-level → best for **storytelling & reporting**.  
- ATT&CK brings the detail → specific techniques to watch for at each stage.  
- Together they make it easy to explain *“where in the chain this technique occurred.”*  

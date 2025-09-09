# Diamond Model — Pivot Examples

This file illustrates how to pivot between the four core nodes of the **Diamond Model of Intrusion Analysis**:  
**Adversary, Infrastructure, Capability, Victim.**

---

## 📌 Adversary → Infrastructure
- **Scenario:** Threat actor identified via phishing campaign.  
- **Pivot:** Track associated domains, IP addresses, and hosting providers.  
- **MITRE Tie-In:** 
  - **T1583 — Acquire Infrastructure** (domains, hosting, servers)  
  - **T1584 — Compromise Infrastructure**  

---

## 📌 Infrastructure → Capability
- **Scenario:** C2 server observed with unusual TLS certificates.  
- **Pivot:** Examine malware/toolkits communicating with that server.  
- **MITRE Tie-In:**  
  - **T1071 — Application Layer Protocol (C2 over HTTP/DNS)**  
  - **T1105 — Ingress Tool Transfer**

---

## 📌 Capability → Victim
- **Scenario:** Malware sample collected (keylogger).  
- **Pivot:** Identify victim endpoints infected with that sample.  
- **MITRE Tie-In:**  
  - **T1056.001 — Input Capture: Keylogging**  
  - **T1005 — Data from Local System**

---

## 📌 Victim → Adversary
- **Scenario:** Multiple finance department endpoints targeted.  
- **Pivot:** Compare targeting to known APT campaigns or threat actor profiles.  
- **MITRE Tie-In:**  
  - **T1591 — Gather Victim Identity Information**  
  - **T1036 — Masquerading** (used to blend into victim environment)

---

## 📝 Notes
- The **Diamond Model excels at relationship mapping** — how each piece connects to another.  
- In practice:  
  - Combine it with ATT&CK for techniques.  
  - Combine it with Kill Chains for sequence/timeline.  
- Especially powerful in **threat intelligence** and **case reporting** workflows.  

# 🚨 Incident Report — Eviction (Adversary Removal Simulation)

**Date:** 2025-09-08  
**Category:** SOC / DFIR (Hands-on Simulation)  
**Status:** Final  

---

## 1) Executive Summary
The *Eviction* simulation recreated a scenario where an adversary had established persistence inside a network.  
The SOC analyst’s role was to investigate logs, identify the adversary’s foothold, and execute **detection + eviction** actions.  

The exercise demonstrated incident response workflow: from detection and containment to eradication and post-incident validation.

---

## 2) Timeline of Events
| Time (UTC) | Event |
|------------|-------|
| 13:10 | Adversary persistence detected via suspicious scheduled task |
| 13:15 | SOC correlation rule triggered (process execution anomaly) |
| 13:25 | Analyst confirmed malicious task creation (T1053) |
| 13:40 | Containment action: disabled scheduled task, isolated host |
| 13:55 | Eradication: registry persistence removed, timestomped files analyzed |
| 14:15 | Post-action verification — system clear, monitoring rules tuned |

---

## 3) Technical Analysis
- **Persistence Mechanisms:**  
  - Malicious scheduled task (T1053)  
  - Registry Run Key entry (T1547.001)  

- **Defense Evasion:**  
  - Timestomping (T1070.006) attempted to obscure malicious file creation times.  

- **Detection Tools:**  
  - SIEM log queries (Windows Event IDs: 4698 – Scheduled Task Created, 7045 – Service Installed)  
  - File timestamp analysis vs. system logs  

---

## 4) Impact Assessment
- **Scope:** 1 endpoint host simulated  
- **Impact:** Adversary maintained limited persistence, potential lateral movement blocked  
- **Risk:** Minimal, due to rapid detection and eviction  

---

## 5) Mitigation & Response
- Disabled malicious scheduled tasks  
- Removed registry autorun entries  
- Enhanced SIEM rules to detect timestamp anomalies  
- Implemented validation checks on high-risk persistence techniques  

---

## 6) Lessons Learned
- **Eviction requires both removal + detection hardening.**  
- Scheduled tasks remain a common persistence vector (easily overlooked).  
- Defense evasion like timestomping is detectable when correlated against system logs.  
- Continuous monitoring of Event IDs + MITRE mappings provides strong defensive coverage.  

---

## 7) MITRE ATT&CK Mapping
- **Persistence:** T1053 — Scheduled Task/Job  
- **Persistence:** T1547.001 — Boot/Logon Autostart Execution: Registry Run Keys  
- **Defense Evasion:** T1070.006 — Indicator Removal on Host: Timestomping  

---

## 8) Notes
This report doubles as a **DFIR case study** — useful for referencing in `dfir_models[kill-chains]` and `forensic_toolset[analysis]`.  
The *Eviction* challenge directly reinforces Tier 1–2 SOC responsibilities and practical IR workflow.

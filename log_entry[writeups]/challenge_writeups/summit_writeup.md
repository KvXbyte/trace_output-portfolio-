# 🧩 Challenge Writeup — Summit (Pyramid of Pain)

**Platform:** TryHackMe  
**Date:** 2025-09-08  
**Difficulty:** Easy (Hands-on Scenario)  

---

## 1) Objective
The *Summit* challenge simulated a purple-team style engagement based on the **Pyramid of Pain**.  
The objective was to chase an adversary up the pyramid by detecting and disrupting their indicators, forcing them to increase operational cost until they eventually abandoned the attack.

---

## 2) Tools & Techniques Used
- **SIEM concepts:** log analysis, rule creation, and detection engineering  
- **MITRE ATT&CK alignment:** persistence, defense evasion, and C2 activity  
- **Purple Team Workflow:** collaborative detection and response against an active adversary  
- **Indicators of Attack (IOAs):** IPs, domains, hashes, TTPs  

---

## 3) Walkthrough
### Step 1 — Establish Pyramid Context  
- Reviewed **indicators by difficulty** (hashes at the bottom → TTPs at the top).  
- Mapped out which detections would provide the most lasting disruption.  

### Step 2 — Begin Adversary Tracking  
- Detected initial malware sample execution attempts.  
- Configured SIEM correlation rules to flag repeat hashes.  

### Step 3 — Escalate Detection  
- Identified domains and IP addresses tied to C2 callbacks.  
- Blocked network IOCs and monitored DNS logs.  

### Step 4 — Target TTPs  
- Mapped adversary behavior to **MITRE ATT&CK tactics**.  
- Noticed persistence via registry run keys (T1547.001) and timestomping attempts (T1070.006).  
- Built detection logic around process creation anomalies and timestamp inconsistencies.  

### Step 5 — Adversary Retreat  
- As detection rules hardened, the adversary’s cost rose.  
- Simulation concluded with successful adversary eviction.  

---

## 4) Lessons Learned
- The **higher up the pyramid** you disrupt, the more expensive it is for the attacker.  
- IOC-based blocking (hashes, IPs) is quick but easily bypassed.  
- Detecting **TTPs** provides long-term resilience and adaptability.  
- Purple Team methodology reinforces continuous tuning between attacker actions and defender responses.  

---

## 5) MITRE ATT&CK Mapping
- **Persistence:** T1547.001 — Boot/Logon Autostart Execution: Registry Run Keys  
- **Defense Evasion:** T1070.006 — Indicator Removal on Host: Timestomping  
- **Command & Control:** T1071 — Application Layer Protocol (HTTP/S traffic)  

---

## 6) Notes
- This challenge was one of the most engaging so far — hands-on, iterative, and aligned with real-world SOC workflows.  
- Strong candidate for linking into `dfir_models[kill-chains]` and `tactic_map[mitre-attack]` for future case studies.

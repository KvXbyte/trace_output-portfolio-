# 🌐 Networking Fundamentals — Module Export

**Source:** `module_networking_fundamentals`  
**Tags:** [Networking][SOC][Foundations]  
**Status:** Complete • Last Update: 2025-09  

---

### 1) Overview
This module established the **core networking and web fundamentals** needed for SOC and DFIR work.  
It covered basic LANs, the OSI model, packet structures, and extended into DNS, HTTP, and how websites function as an integrated system.

---

### 2) Skills Demonstrated
- Understanding nodes, IPs, and LAN components  
- Explaining layered communication via the OSI model  
- Analyzing packet and frame structure  
- Recognizing how routers, switches, and VLANs extend networks  
- Deep diving into DNS lookups and common abuse (poisoning/tunneling)  
- Exploring HTTP methods, headers, and request/response cycles  
- Connecting DNS + HTTP + OSI into end-to-end web flows  

---

### 3) Evidence / Artifacts
- THM completion (screenshots / notes)  
- Room-by-room `.md` exports under `module_networking_fundamentals/`  

---

### 4) SOC / DFIR Mappings
- **DNS logs** → critical data source for detecting C2, tunneling, exfiltration  
- **HTTP logs** → proxy analysis, phishing detection, web exploit trails  
- **OSI model** → framework for mapping attacks to specific layers  
- **Packets/Frames** → foundational for Wireshark/Tcpdump investigations  

---

### 5) Key Quick-Refs
- OSI layers mnemonic: **All People Seem To Need Data Processing**  
- DNS = domain ↔ IP translation; often exploited  
- HTTP verbs: GET (read), POST (submit), PUT (update), DELETE (remove)  
- Packets (L3) vs Frames (L2) distinction  

---

### 6) Reflection
This module reinforced the foundation all SOC and DFIR work rests on.  
DNS and HTTP stood out as especially critical — logs from these protocols will drive much of real-world detection and triage.  

---

### 7) Next Actions
- Begin practicing packet capture analysis with **Wireshark** and **Tcpdump**  
- Build a quick-reference “log decoder” for DNS/HTTP fields  
- Map networking artifacts into upcoming **MITRE ATT&CK** technique studies  

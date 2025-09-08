# 🛠️ tools_index[platforms]

A curated index of platforms and tools that support detection, forensics, and incident response.  
This folder acts as a quick reference for resources I’m learning, exploring, or saving for future use.  

---

## 🎯 Current Entries

### [SOC Prime – Threat Detection Marketplace (TDM)](./socprime_tdm.md)
- **Link:** [https://tdm.socprime.com/](https://tdm.socprime.com/)  
- **Focus:** Community-driven library of Sigma/YARA/Snort rules, mapped to MITRE ATT&CK.  
- **Why it matters:** Helps analysts deploy, share, and automate detections across SIEM/EDR platforms.  
- **Key Features:**  
  - Detection-as-Code library (mapped to MITRE ATT&CK)  
  - AI-enhanced search and rule customization  
  - Automated content delivery into SIEM/EDR  
  - Attack Detective integration for visibility gaps  

---

### [MITRE ATT&CK Navigator](./mitre_attack_navigator.md)
- **Link:** [https://mitre-attack.github.io/attack-navigator/](https://mitre-attack.github.io/attack-navigator/)  
- **Focus:** Interactive tool for mapping and visualizing ATT&CK coverage.  
- **Why it matters:** Helps analysts identify detection gaps and align SOC visibility with adversary behaviors.  
- **Key Features:**  
  - ATT&CK matrix visualization (Enterprise, ICS, Mobile)  
  - Custom layers and heatmaps  
  - JSON export/import for sharing coverage  
  - Collaboration for team analysis  

---

### [Sigma HQ](./sigma_hq.md)
- **Link:** [https://github.com/SigmaHQ/sigma](https://github.com/SigmaHQ/sigma)  
- **Focus:** Open detection-as-code format for SIEM queries.  
- **Why it matters:** Allows detections to be written once and reused across different platforms.  
- **Key Features:**  
  - Human-readable YAML rule format  
  - Conversion to SIEM queries via **sigmac**  
  - Community-driven ruleset  
  - ATT&CK mapping built into many rules  

---

### [Splunkbase](./splunkbase.md)
- **Link:** [https://splunkbase.splunk.com/](https://splunkbase.splunk.com/)  
- **Focus:** Marketplace for Splunk apps, add-ons, and dashboards.  
- **Why it matters:** Extends Splunk for threat detection, log parsing, and visualization.  
- **Key Features:**  
  - Prebuilt dashboards and parsers  
  - Integrations with security platforms (CrowdStrike, FireEye, etc.)  
  - Threat intel feeds and enrichment plugins  
  - Vendor and community contributions  

---

### [Autopsy](./autopsy.md)
- **Link:** [https://www.autopsy.com/](https://www.autopsy.com/)  
- **Focus:** Open-source forensic analysis platform for hard drives and smartphones.  
- **Why it matters:** Provides an accessible GUI for The Sleuth Kit, widely used in forensics labs.  
- **Key Features:**  
  - File system and artifact analysis  
  - Registry, browser, and email parsing  
  - Timeline and keyword search  
  - Reporting for investigations  

---

### [Volatility](./volatility.md)
- **Link:** [https://www.volatilityfoundation.org/](https://www.volatilityfoundation.org/)  
- **Focus:** Memory forensics framework for analyzing RAM dumps.  
- **Why it matters:** Crucial for investigating malware, rootkits, and active compromises.  
- **Key Features:**  
  - Process, DLL, and network connection analysis  
  - Detection of hidden/injected code  
  - File and registry extraction from memory  
  - Plugin ecosystem for advanced analysis  

---

### [Wireshark](./wireshark.md)
- **Link:** [https://www.wireshark.org/](https://www.wireshark.org/)  
- **Focus:** Packet capture and analysis tool for network traffic.  
- **Why it matters:** Essential for intrusion analysis, threat hunting, and validating alerts.  
- **Key Features:**  
  - Real-time packet capture and inspection  
  - Deep protocol analysis  
  - Filtering, coloring, and stream reconstruction  
  - Supports hundreds of protocols and plugins  

---

## 📌 Future Additions
- Other DFIR tools as I encounter them  
- Threat intel feeds and enrichment platforms  
- Cloud-specific detection services (Azure Sentinel, AWS GuardDuty, etc.)  

---

## 📝 Notes
This folder will expand as I build out my DFIR toolkit.  
Each entry can grow into its own `.md` file with deeper notes, commands, or workflows.

Each entry can grow into its own `.md` file with deeper notes, commands, or workflows.

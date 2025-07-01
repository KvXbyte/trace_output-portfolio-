# 🧊 Threat Report: IcedID Loader Behavior – July 1, 2025

## Summary

IcedID, historically known as a banking trojan, continues to evolve as a **loader** for second-stage malware including **Cobalt Strike**, **DarkVNC**, and custom backdoors.  
Recent campaigns have shown a pivot toward **business-themed phishing lures** and **living-off-the-land binaries (LOLBins)** for stealthy execution.

---

## TTP Breakdown

| Phase            | Technique                                | MITRE ID         |
|------------------|-------------------------------------------|------------------|
| Delivery         | Phishing with malicious attachments       | T1566.001        |
| Execution        | Use of `rundll32.exe`, `mshta.exe`        | T1218.011        |
| Persistence      | Registry Run key or Scheduled Task        | T1053.005        |
| Command & Control| HTTP/S beaconing to attacker domain       | T1071.001        |

---

## Behavioral Indicators

- Excel or OneNote launching LOLBins (e.g., `rundll32.exe`)
- Inbound phishing referencing invoices or payment changes
- Encrypted outbound HTTP requests to uncommon domains
- Registry writes to:
  - `HKCU\Software\Microsoft\Windows\CurrentVersion\Run`

---

## Detection Strategies

- Alert on Office > `rundll32` parent-child process chains
- Flag execution of LOLBins from temporary or user directories
- Monitor for anomalous scheduled task creation
- Use YARA rules for known IcedID loader stagers

---

## Sources

- [DFIR Report – IcedID Evolution](https://thedfirreport.com)
- [CISA Alert AA23-XXXA: IcedID Campaign Indicators](https://www.cisa.gov)
- [MITRE ATT&CK Navigator](https://attack.mitre.org)

---

> Loader behavior is quiet until it's not. The real payload is often waiting in the next beacon.

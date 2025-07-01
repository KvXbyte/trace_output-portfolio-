# Kawa4096 Ransomware Double‑Extortion Campaign (June 2025)

## Source  
– **Red Piranha Threat Intelligence Report** – June 2025  
  *(Crystal Eye, ThreatLabz) - Weekly summary on TransferLoader, KimJongRAT & Kawa4096*

## Summary  
New ransomware group **Kawa4096** emerged June 27, 2025, executing a **double‑extortion** attack: encrypting files & threatening to leak data.  
Initial access appears via **phishing or RDP**, with exfiltration over **Tor-enabled channels** prior to encryption.

## MITRE ATT&CK Mapping  
- **Initial Access**: Spearphishing Attachment (T1566.001), External Remote Services (T1133)  
- **Execution**: PowerShell (T1059.001)  
- **Persistence**: Scheduled Task/Job (T1053.005)  
- **Defense Evasion**: Signed Binary Proxy Execution (T1218), Event Log Clearing (T1070.001)  
- **Credential Access**: Credential Dumping (T1003)  
- **Discovery**: System Info Discovery (T1082)  
- **Impact**: Data Encrypted for Impact (T1486), Data Wiping (T1561)

## Indicators  
- Tor, Tox, or OnionMail traffic before encryption  
- Presence of files like `shield.msi` or specific ransom notes  
- Creation of new scheduled tasks, signed via LOLBins (e.g., mshta.exe)  
- Event log clearing activities  
- Abnormal PowerShell sessions following phishing

## Mitigation & Detection Suggestions  
- Block outbound Tor, Tox protocols & unusual port use  
- Alert on new scheduled task creation, especially from PowerShell  
- Monitor mshta.exe or other LOLBin executions  
- Detect presence of specific ransom note filenames or extensions  
- Track PowerShell running from unexpected locations

## KvXbyte Perspective  
This one hits differently—no need for exotic exploits when you’ve got phishing, decent defense evasion, and cloak-and-dagger exfil over Tor.  
What’s sneaky is how quietly they work: encrypted data, then extorted. RNA isn’t just ransomware—it’s a *psychological game*.  
Detection here means watching **before** encryption: trips into dark networks + LOLBin execution.  
If you miss that ? You’re already too late.

---

**Logged for those who care to look.**  
— KvXbyte

# Iranian State‑Sponsored Cyber Operations Fact Sheet (June 30, 2025)

## Source  
– **CISA / FBI / NSA / DOD** advisory – June 30, 2025 :contentReference[oaicite:2]{index=2}

## Summary  
A joint advisory warns U.S. critical infrastructure operators to remain vigilant against *Iranian state-sponsored or affiliated cyber activities*. These may include:
- Targeted ransomware and destructive attacks  
- Spearphishing campaigns and credential harvesting  
- Exploitation of VPN, ICS, and PLC systems in water/wastewater sectors

## MITRE ATT&CK Mapping  
- **Initial Access**: Spearphishing Attachment (T1566.001)  
- **Execution**: Command and Scripting Interpreter (T1059)  
- **Lateral Movement**: Exploitation for Defense Evasion (T1211)  
- **Impact**: Data Encrypted for Impact (T1486) or Data Destruction (T1485)  

## Indicators  
- Iranian-hosted VPN/proxy chains  
- Spearphishing emails referencing geopolitical themes  
- Unusual PLC traffic or ICS-level anomalies  
- Changes to physical-logic states tied to cyber activity

## Mitigation Recommendations  
- Enforce *phishing-resistant MFA* for all remote and VPN logons  
- Restrict network access to PLCs and ICS assets  
- Monitor ICS telemetry for unusual commands or patterns

## KvXbyte Perspective  
State-sponsored actors aren’t just painting targets—they’re probing infrastructure with quiet persistence. This advisory reminds us the strongest defense isn’t tech—it’s **context-driven vigilance**. Detection isn’t just logs—it’s understanding *what shouldn’t happen*.  
— keep your eyes on PLC logs as much as authentication logs.

---

**Logged for those who care to look.**  
— KvXbyte

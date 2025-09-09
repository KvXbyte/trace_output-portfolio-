# 🪟 Windows Event ID Cheat Sheet

Quick reference for key event IDs in SOC/DFIR triage.

---

## Logon Events
- **4624** → Successful Logon  
- **4625** → Failed Logon  
- **4648** → Logon with explicit credentials  

## Process Creation
- **4688** → Process Creation (critical for triage)  
- **4689** → Process Termination  

## Security Logs
- **1102** → Audit Log Cleared  
- **4720** → User Account Created  
- **4726** → User Account Deleted  

---

## Notes
Pair with Sysmon IDs (e.g., Sysmon Event ID 1 = Process Creation).

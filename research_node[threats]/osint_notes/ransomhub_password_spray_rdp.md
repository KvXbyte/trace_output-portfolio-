# RansomHub Ransomware via RDP Password Spray (June 2025)

## Source  
– **DFIR Report**: Hide Your RDP: Password Spray Leads to RansomHub Deployment (June 30, 2025) :contentReference[oaicite:3]{index=3}

## Summary  
- Attacker performed password spray against public RDP for ~4 hours  
- Gained access, used Mimikatz and CredentialsFileView to extract credentials  
- Discovery via living‑off‑the‑land binaries + Advanced IP Scanner, NetScan  
- Exfiltration with Rclone over SFTP  
- Lateral spread & ransomware execution (RansomHub) via SMB and remote services

## MITRE ATT&CK Mapping  
- **Initial Access**: Password Spray (T1110.002)  
- **Credential Access**: Credential Dumping (T1003), LSASS memory (Mimikatz)  
- **Discovery**: System Network Discovery (T1046), File/Directory Discovery (T1083)  
- **Lateral Movement**: Remote Desktop Protocol (T1021.001), SMB (T1021.002)  
- **Command and Control**: Rclone over SFTP (T1095)  
- **Impact**: Data Encrypted for Impact – Ransomware (T1486)

## Detection Opportunities  
- Monitor multiple failed RDP logons (4625/4624) from same source  
- Alert on execution of Mimikatz or CredentialsFileView; LSASS access  
- Flag use of Rclone during sessions, especially over unusual ports  
- Watch for SMB file creation events and scheduled service executions

## KvXbyte Perspective  
This case is a striking example of how simple tools and credentials can cut deeper than zero-days.  
RDP remains a pervasive weak point—especially when coupled with lateral tools like Atera or Splashtop.  
The carbon-copy of password-spray → credential dumping → ransomware execution signals how much detection value still lives in log analysis.

---  

**Logged for those who care to look.**  
— KvXbyte

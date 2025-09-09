# 🛡️ DFIR Persistence Notes

Common persistence mechanisms & detection tips.

---

## Windows
- **Registry Run Keys** (T1547.001) → Sysmon Event ID 13  
- **Scheduled Tasks** (T1053) → Windows Task Scheduler logs  
- **Service Creation** (T1543) → Event ID 7045  

## Linux
- **Cron Jobs** → `/etc/crontab`, `systemctl list-timers`  
- **Systemd Services** → `/etc/systemd/system/`  

---

## Anti-Forensic
- **Timestomping** (T1070.006) → Compare $MFT vs $SI timestamps  
- **Log Clearing** (T1070.001) → Windows Event ID 1102  

---

## Notes
These notes complement `dfir_models[kill-chains]` mapping files.

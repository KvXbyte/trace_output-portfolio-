# 📊 Splunk Query Cheat Sheet

Common SPL (Search Processing Language) commands for SOC/DFIR.

---

## Basic Searches
- `index=main` → Search default index  
- `sourcetype=wineventlog` → Filter Windows Event Logs  

## Fields & Extraction
- `stats count by src_ip` → Count events by source IP  
- `fields + user, src_ip, dest_ip` → Show specific fields  

## Filtering
- `search user=Administrator` → Limit results  
- `NOT src_ip=127.0.0.1` → Exclude localhost  

## Time
- `earliest=-24h latest=now` → Last 24 hours  
- `| timechart count by src_ip` → Graph over time  

---

## Notes
This sheet expands as Splunk labs are completed.

# 🪟 Windows & Active Directory — Module Export
**Source:** `module_windows_ad`  
**Tags:** [SOC][DFIR]  
**Status:** Complete • **Last Update:** 2025-09

## 1) Overview
Windows internals + Active Directory fundamentals: identities, policy, logging, and common admin tasks.

## 2) Skills Demonstrated
- AD structure: domains, OUs, users, groups, GPOs
- Event Viewer & Windows Logs (Security/System/Application)
- PowerShell basics for inventory & log collection
- Local security policy, services, Defender status

## 3) Evidence / Artifacts
- THM notes/screenshots

## 4) SOC / DFIR Mappings
- **[DFIR]** Event IDs used in timeline building
- **[SOC]** Authentication & process creation monitoring

## 5) Key Quick-Refs (Event IDs)
- 4624/4625 logon success/failure • 4672 special privs  
- 4688 process creation • 4648 explicit creds

## 6) Reflection
Understanding Windows auth and logging closed gaps between alerts and actual host evidence.

## 7) Next Actions
- Spin a tiny AD lab for hands-on GPO & auditing practice

# 🐧 Linux Fundamentals — Module Export
**Source:** `module_linux_fundamentals`  
**Tags:** [SOC][DFIR][NET]  
**Status:** Complete • **Last Update:** 2025-09

## 1) Overview
Core Linux skills for navigation, permissions, processes, services, and logs—bread-and-butter for blue team triage.

## 2) Skills Demonstrated
- Filesystem navigation, globbing, and search (`find`, `grep`, `cut`, `awk`)
- Users/groups & permissions (`chmod`, `chown`, `sudo`)
- Processes & services (`ps`, `top`, `systemctl`, `journalctl`)
- Networking (`ip`, `ss`, `netstat`, `curl`, `dig`)
- Log locations & rotation (`/var/log`, `rsyslog`, `logrotate`)

## 3) Evidence / Artifacts
- THM module notes & screenshots

## 4) SOC / DFIR Mappings
- **[DFIR]** Log triage and artifact collection paths
- **[SOC]** Service & process checks during escalation
- **[NET]** Quick verification of bindings and connections

## 5) Key Quick-Refs
- Logs: `/var/log/auth.log`, `/var/log/syslog`, `/var/log/secure`
- Permissions: `chmod u+rx file`, `chown user:group file`

## 6) Reflection
Comfortable on-box = faster investigations. This module tightened my CLI fluency under time pressure.

## 7) Next Actions
- Hardening checklist for baseline Linux hosts
- Small bash toolkit for repeatable triage

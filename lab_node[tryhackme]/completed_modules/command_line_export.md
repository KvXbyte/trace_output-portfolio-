# ⌨️ Command Line — Module Export
**Source:** `module_command_line`  
**Tags:** [SOC][DFIR]  
**Status:** Complete • **Last Update:** 2025-09

## 1) Overview
Cross-platform CLI (Bash, CMD, PowerShell) for visibility, collection, and quick automation.

## 2) Skills Demonstrated
- Pipes, redirection, and one-liners for data slicing
- System and process inspection across OSes
- File interrogation & hashing; quick inventory
- PowerShell objects, filtering, and export (`Export-Csv`, `ConvertTo-Json`)

## 3) Evidence / Artifacts
- THM notes and command sheets

## 4) SOC / DFIR Mappings
- Rapid host triage without GUI
- Repeatable collection steps that become runbooks

## 5) Key Quick-Refs
- PowerShell: `Get-Process | Sort CPU -desc | Select -First 10`
- Bash: `grep -R "keyword" /path 2>/dev/null`

## 6) Reflection
Command fluency = less context switching and faster case handling.

## 7) Next Actions
- Personal cross-OS “triage aliases” cheatsheet

# 🧰 Offensive Tooling (Defender’s Lens) — Module Export
**Source:** `module_offsec_tools`  
**Tags:** [SOC][DFIR]  
**Status:** Complete • **Last Update:** 2025-09

## 1) Overview
Awareness of common offensive utilities (e.g., discovery, password attacks, content enumeration) to improve **detection** and **response**.

> Note: Used strictly for defender education; no exploit instructions provided.

## 2) Skills Demonstrated
- Recognizing tool fingerprints in logs
- Understanding enumeration patterns and credential-attack signals
- Mapping typical attacker workflows to detections/hunts

## 3) Evidence / Artifacts
- THM notes

## 4) SOC / DFIR Mappings
- Alert triage patterns for brute-force/enumeration
- Post-event validation: scope, dwell time, and touched assets

## 5) Key Quick-Refs
- Defender cues: repeated 401/403s, directory bursts, abnormal method mix

## 6) Reflection
Knowing the tools from the other side makes my detections less noisy and my escalations sharper.

## 7) Next Actions
- Add log patterns to **edr_sim_logbook** with sample detections

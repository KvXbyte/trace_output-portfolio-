# 🌐 Networking — Module Export
**Source:** `module_networking`  
**Tags:** [NET][SOC][DFIR]  
**Status:** Complete • **Last Update:** 2025-09

## 1) Overview
OSI/TCP-IP models, common protocols/ports, packet capture & analysis, and scanning fundamentals.

## 2) Skills Demonstrated
- Subnetting, routing, DNS/HTTP/TLS fundamentals
- Packet capture & filtering (Wireshark/tcpdump)
- Basic host/service discovery & validation
- Reading flows for anomalies

## 3) Evidence / Artifacts
- THM captures & filters

## 4) SOC / DFIR Mappings
- **[DFIR]** PCAP/flow timeline reconstruction
- **[SOC]** Alert validation and scope determination

## 5) Key Quick-Refs
- Common ports: 22/80/443/3389/445/389/636
- tcpdump filter: `tcpdump -nnr file.pcap 'ip and (tcp or udp)'`

## 6) Reflection
From packets to story: this tightened how I translate network evidence into findings.

## 7) Next Actions
- Mini PCAP triage playbook + go-to display filters

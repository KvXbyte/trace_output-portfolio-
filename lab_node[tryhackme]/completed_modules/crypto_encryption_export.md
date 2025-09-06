# 🔐 Crypto & Encryption — Module Export
**Source:** `module_crypto_encryption`  
**Tags:** [SOC][DFIR]  
**Status:** Complete • **Last Update:** 2025-09

## 1) Overview
Hashing, symmetric/asymmetric encryption, keys, PKI/TLS—applied, not theoretical.

## 2) Skills Demonstrated
- Hash verification & integrity checking
- TLS/PKI basics and cert inspection
- Password storage concepts & cracking considerations (defender view)

## 3) Evidence / Artifacts
- THM notes

## 4) SOC / DFIR Mappings
- **[DFIR]** Verify artifact integrity during collection
- **[SOC]** Cert/cipher hygiene checks in exposure findings

## 5) Key Quick-Refs
- Linux: `sha256sum file`  
- Windows: `certutil -hashfile file SHA256`

## 6) Reflection
Understanding crypto primitives helps separate signal from “security theater.”

## 7) Next Actions
- Quick TLS checklist (protocols, ciphers, expiry, SANs)

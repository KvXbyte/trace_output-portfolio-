# 🔓 MITRE Tactic: Initial Access (TA0001)

## Overview

The **Initial Access** tactic consists of techniques adversaries use to gain an initial foothold within a network.  
This is often the first observable phase of an attack and can include phishing, drive-by compromises, exploitation of public-facing apps, and more.

---

## 📌 Common Techniques

| Technique ID | Name                          | Description                                     |
|--------------|-------------------------------|-------------------------------------------------|
| T1566.001    | Phishing: Spearphishing Attachment | Malicious files delivered via email             |
| T1190        | Exploit Public-Facing Application | Attacker leverages vulnerabilities in exposed apps |
| T1189        | Drive-by Compromise            | Target is compromised by visiting a malicious website |
| T1078        | Valid Accounts                 | Use of stolen or default credentials to gain access |
| T1133        | External Remote Services       | Exploiting remote access services (e.g., VPN, RDP) |

---

## 🔍 Detection Considerations

- Monitor email gateways for suspicious attachments and macro-enabled documents
- Inspect HTTP logs for suspicious referrers or browser behavior (drive-by indicators)
- Correlate VPN/RDP access with geolocation anomalies or logon time irregularities
- Use alerting for known exploit patterns or unusual user-agent strings

---

## 🛡️ Defensive Tips

- Enforce MFA wherever remote access or credential use is possible
- Disable macro execution by default in Microsoft Office products
- Patch exposed services regularly and use WAFs where applicable
- Use honeypots or sinkholes to catch opportunistic scans or drive-by traffic

---

## 📚 References

- [MITRE ATT&CK: Initial Access](https://attack.mitre.org/tactics/TA0001/)
- [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final)
- [Phishing Defense Guide – CISA](https://www.cisa.gov/news-events/resources/phishing-guidance)

---

> "The adversary doesn’t knock—they compromise the doormat. This is where you watch the threshold."  
> — KvXbyte

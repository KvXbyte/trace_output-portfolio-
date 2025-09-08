# 🧪 Experiment: Phishing Email Investigation

## 🔎 Objective
Analyze a suspicious email and identify potential indicators of compromise (IOCs).  
Practice basic forensic techniques on email artifacts.

---

## 🛠️ Tools Used
- Email client (to export `.eml`)  
- Online email header analyzer (e.g., MXToolbox)  
- WHOIS / VirusTotal (for domains or attachments)  

---

## 📂 Steps Taken
1. Exported a fake phishing email sample (`sample_email.eml`).  
2. Extracted and reviewed headers.  
3. Identified anomalies (spoofed sender, mismatched domains, etc.).  
4. Checked URLs/domains against threat intel sources.  

---

## 📊 Findings
- Suspicious domain: `login-verification[.]co`  
- Sender IP traced to unusual ASN  
- Links redirected to credential-harvesting site  

---

## 🎯 Takeaways
- Reinforced skill in reading email headers  
- Practiced using external validation tools  
- Identified practical workflow for quick SOC triage  

---

## 📒 References
- [MXToolbox Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)  
- [CISA Phishing Guidance](https://www.cisa.gov/topics/cyber-threats-and-advisories/phishing)  

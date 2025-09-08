# 🧪 Experiment: Phishing Email Investigation

## 🔎 Objective
Analyze a suspicious email and identify potential indicators of compromise (IOCs).  
Practice basic forensic techniques on email artifacts.

---

## 🛠️ Tools Used
- MXToolbox Header Analyzer  
- WHOIS Lookup  
- VirusTotal / URLScan.io  

---

## 📂 Steps Taken
1. Created a fake phishing email sample (`sample_email.eml`).  
2. Loaded headers into MXToolbox for analysis.  
3. Observed spoofed sender domain (`micros0ft-secure.com`) and suspicious link (`login-verification.co`).  
4. Ran WHOIS lookup on sender domain → flagged as abnormal.  
5. Checked suspicious URL on VirusTotal → multiple vendors flagged it as phishing.  

---

## 📊 Findings
- **Suspicious Domain:** `login-verification[.]co`  
- **Spoofed Sender:** `support@micros0ft-secure.com`  
- **Redirection:** URL would likely lead to credential-harvesting page  

---

## 🎯 Takeaways
- Reinforced workflow for analyzing email headers.  
- Learned to validate domains/links against external intel.  
- Demonstrated how simple artifacts (headers, links) reveal phishing intent.  

---

## 📒 References
- [MXToolbox Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)  
- [CISA Phishing Guidance](https://www.cisa.gov/topics/cyber-threats-and-advisories/phishing)  

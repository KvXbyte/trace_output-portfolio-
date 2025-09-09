# 🕵️ Cyber Kill Chain

**Purpose:**  
Developed by Lockheed Martin, the Cyber Kill Chain is a **7-step model** for describing and interrupting intrusions.  
It remains a baseline framework for visualizing attacker workflow.

---

## 📚 Phases
1. **Reconnaissance** → Gathering information about targets  
2. **Weaponization** → Coupling exploit with a payload  
3. **Delivery** → Transmitting the weapon to the target (phishing, USB, etc.)  
4. **Exploitation** → Triggering code execution on the victim  
5. **Installation** → Persistence mechanisms (malware, registry, services)  
6. **Command & Control (C2)** → Establishing communication with attacker infrastructure  
7. **Actions on Objectives** → Exfiltration, destruction, or other adversary goals  

---

## 🔗 SOC / DFIR Relevance
- A “storyboard” for incidents — where did we stop the adversary?  
- Helps analysts see intrusions as a chain of linked actions, not isolated alerts.  
- Breaking the chain at any stage can prevent mission success.

---

## 📝 Notes
- Simplified compared to MITRE ATT&CK, but very useful for executive-level reporting.  
- Often taught first before introducing Unified Kill Chain.  

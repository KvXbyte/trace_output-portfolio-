# 💎 Diamond Model of Intrusion Analysis

**Purpose:**  
A relational framework for structuring incidents.  
It emphasizes the relationships between four core features of any intrusion.

---

## 📚 The Four Nodes
- **Adversary** → The threat actor (who)  
- **Capability** → Tools, malware, exploits (what)  
- **Infrastructure** → Systems and channels used (how)  
- **Victim** → The targeted entity (whom/where)  

---

## 🔗 SOC / DFIR Relevance
- Encourages pivoting:  
  - Adversary ↔ Infrastructure (track their servers/domains)  
  - Capability ↔ Victim (see who else is hit by the same malware)  
- Provides a mental model for expanding investigations.  
- Supports structured reporting: “who, what, how, to whom.”

---

## 📝 Notes
- Complements Kill Chains (timeline) and MITRE ATT&CK (technique catalog).  
- Especially valuable in **threat intelligence** and **case study writeups**.  
- Will be extended with case examples inside GitHub (`cases/` planned).  

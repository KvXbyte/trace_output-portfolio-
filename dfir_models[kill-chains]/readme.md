# 🔎 DFIR Models — Kill Chains & Analysis Frameworks

This directory houses frameworks used to model adversary behavior and guide incident response.  
Unlike `tactic_map[mitre-attack]`, which catalogs techniques, these frameworks structure **attack progression** and **analysis narratives**.

---

## 📚 Included Frameworks

### [Cyber Kill Chain](./cyber_kill_chain)
- [README.md](./cyber_kill_chain/README.md) → Overview of the 7-step model  
- [ckc_to_mitre.md](./cyber_kill_chain/ckc_to_mitre.md) → Mapping Cyber Kill Chain phases to MITRE ATT&CK  

---

### [Unified Kill Chain](./unified_kill_chain)
- [README.md](./unified_kill_chain/README.md) → Extended lifecycle model  
- [ukc_to_mitre.md](./unified_kill_chain/ukc_to_mitre.md) → Mapping Unified Kill Chain phases to MITRE ATT&CK  

---

### [Diamond Model](./diamond_model)
- [README.md](./diamond_model/README.md) → Overview of the relational analysis model  
- [pivot_examples.md](./diamond_model/pivot_examples.md) → Practical pivots between Adversary, Infrastructure, Capability, and Victim  

---

## 🔗 Usage
- **Kill Chains** → Help analysts narrate *when* in the intrusion lifecycle events occur.  
- **Diamond Model** → Helps analysts map *relationships* between entities.  
- **MITRE ATT&CK** → Provides the *granular details* (tactics/techniques) that plug into these models.  

---

## 📎 Cross-References
- See [`../tactic_map[mitre-attack]`](../tactic_map[mitre-attack]) for ATT&CK mappings.  
- Related exports: [`completed_modules/module_cyber_defence_frameworks.md`](../completed_modules/module_cyber_defence_frameworks.md)  

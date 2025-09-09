# 🛡️ Cyber Defence Frameworks — Module Export

**Source:** `module_cyber_defence_frameworks`  
**Tags:** [SOC][DFIR][Frameworks]  
**Status:** Complete • Last Update: 2025-09  

---

### 1) Overview
This module focused on key defensive models: **Pyramid of Pain, Cyber Kill Chain, Unified Kill Chain, Diamond Model, and MITRE ATT&CK**.  
It also included hands-on scenarios (**Summit** and **Eviction**) to apply these frameworks in practice, bridging theory with adversary simulation.

---

### 2) Skills Demonstrated
- Prioritizing indicators by adversary cost (Pyramid of Pain)  
- Mapping adversary phases to detections (Cyber + Unified Kill Chain)  
- Structuring investigations with Adversary–Infrastructure–Capability–Victim (Diamond Model)  
- Using MITRE ATT&CK as a reference library for tactics & techniques  
- Applying frameworks in live adversary simulations (Summit & Eviction)  

---

### 3) Evidence / Artifacts
- THM completion (screenshots / notes)  
- Room-by-room `.md` exports under `module_cyber_defence_frameworks/`  

---

### 4) SOC / DFIR Mappings
- **Kill Chains** → Map to detection coverage and phase-based narratives  
- **Diamond Model** → Strong pivoting structure for adversary investigations  
- **MITRE ATT&CK** → Standardized reference for techniques, used alongside frameworks  
- **Scenarios** → Reinforced the need for purple-team alignment in detection strategy  

---

### 5) Key Quick-Refs
- Pyramid of Pain: IOC value ↑ = adversary pain ↑  
- Cyber Kill Chain (7 steps) → break chain early to prevent impact  
- Unified Kill Chain → extended lifecycle view beyond intrusion  
- Diamond Model nodes → Adversary, Infrastructure, Capability, Victim  

---

### 6) Reflection
This was a milestone module: not just theory but hands-on application.  
**Summit** in particular stood out as one of the best rooms so far — it captured the essence of detection engineering and purple-team workflows.  

---

### 7) Next Actions
- Expand Unified Kill Chain and Diamond Model into dedicated GitHub folders (`dfir_models[kill-chains]`)  
- Begin mapping selected MITRE techniques (e.g., T1547.001, Timestomping) into these frameworks  
- Draft DFIR-style case studies using Diamond Model structure  

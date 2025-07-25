# TryHackMe: Offensive Security Tooling (Export Summary)

**Track:** Offensive Tooling (Hydra, Gobuster, Shells, SQLMap)  
**Status:** ✅ Completed  
**Time Spent:** ~2.5 hours  
**Environment:** Simulated labs and manual exploitation workflows  
**Level:** Beginner → Intermediate

---

### 🧨 Core Takeaways

- **Brute Forcing:** Used Hydra for login cracking with thread control and wordlists.
- **Enumeration:** Identified hidden directories and pages via Gobuster.
- **Shell Access:** Distinguished between reverse, bind, and web shells.
- **Injection Attacks:** Performed SQL injection to extract database content using SQLMap.

---

### 🧠 Skills Practiced

| Tool       | Use Case & Technique                                       |
|------------|------------------------------------------------------------|
| Hydra      | Credential cracking on HTTP/SSH with flags like `-L -P`    |
| Gobuster   | Wordlist-based URL/path enumeration with HTTP response focus |
| Shells     | Reverse vs bind shell behavior, shell stabilization tips   |
| SQLMap     | SQLi testing, DB enumeration, and record dumping           |

---

### 💬 Reflections

Understanding how attacks work is essential to defense. This module made it clear how fast and quietly tools can extract data or gain access when misconfigurations are present.

---

> “Red team tools aren’t just weapons—they’re warning signs. Learn them, so you can see them coming.”  
> — KvXbyte

# phantom_alert

**Cast:** KvXbyte, Echo, Ph1sh3r

---

**[14:21] Echo:** *beep-beep* (New alert: “Suspicious PowerShell.”)

**[14:22] Ph1sh3r:** The most dangerous kind of shell is the one with poetry in it.

**[14:23] KvXbyte:** Pull command line, parent process, network calls. MITRE map?

**[14:24] Echo:** *bip* (T1059.001 candidate. Parent: `Teams.exe`. Child: `powershell.exe -enc ...`)

**[14:25] Ph1sh3r:** Ah yes, the classic “productivity app launches cyber spellbook.”

**[14:26] KvXbyte:** Decode the base64.

**[14:27] Echo:** *beep...* (Result: set wallpaper to a corgi in a spacesuit. No exfil, no creds.)

**[14:28] Ph1sh3r:** So… a corgi-ops deployment. Threat level: adorable.

**[14:29] KvXbyte:** Document as **FP – benign user customization**. Add detection note: exclude wallpaper scripts with no net IO.

**[14:30] Ph1sh3r:** Adding `Tactic: Aesthetic`. Technique: `T-00BARK`.

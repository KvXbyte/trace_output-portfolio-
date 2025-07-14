⚙️ **PowerShell Basics**

---

### Covered Topics:
- Cmdlets structure: `Verb-Noun` (e.g., `Get-Process`, `Set-Item`)
- Variables and object handling
- File and directory operations: `Get-ChildItem`, `Remove-Item`, `Out-File`
- Admin commands: `Get-Service`, `Start-Process`, `Get-EventLog`
- Scripting fundamentals and execution policies

---

### Key Notes:
- `Get-Command *net*` helps locate relevant cmdlets quickly.
- PowerShell returns **objects**, not text—use `Select-Object`, `Format-Table`, or `Where-Object` to manipulate output.
- Execution policy may block scripts: use `Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass` for temporary override.
- Use `| Export-Csv` to save output for logs or analysis.

---

> PowerShell isn’t just a shell—it’s automation with context.

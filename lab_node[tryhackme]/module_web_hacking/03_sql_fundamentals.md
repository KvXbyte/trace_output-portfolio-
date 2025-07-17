# 🗃️ SQL Fundamentals

**Focus:** Query logic, data manipulation, basic injection principles

---

## 📘 Key Concepts

- SQL basics: `SELECT`, `FROM`, `WHERE`, `AND/OR`
- Injection payloads: `' OR '1'='1`, `--`, `UNION SELECT`
- Vulnerable patterns: user-supplied input passed directly into query strings

---

## 🧠 Notes

SQL Injection (SQLi) remains one of the most common vulnerabilities. Even basic login forms can be bypassed when input is not properly filtered or escaped.

---

## 🧪 Observations

- Database errors can leak critical structure info
- Using `' OR 1=1--` still works more often than it should

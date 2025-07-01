# 🌐 Protocol Comparison Reference

A quick-reference sheet comparing common secure and insecure protocols, focusing on use cases and exam-relevant details.

---

## Secure vs Insecure Protocols

| Protocol     | Port | Purpose                    | Secure? | Notes                              |
|--------------|------|-----------------------------|--------|-------------------------------------|
| HTTP         | 80   | Web browsing                | ❌ No   | Use HTTPS instead                   |
| HTTPS        | 443  | Secure web traffic          | ✅ Yes  | Uses TLS/SSL                        |
| FTP          | 21   | File Transfer               | ❌ No   | Credentials sent in plaintext       |
| SFTP         | 22   | Secure file transfer        | ✅ Yes  | Runs over SSH                       |
| FTPS         | 990  | FTP over SSL/TLS            | ✅ Yes  | Common in enterprise environments   |
| SSH          | 22   | Secure remote shell         | ✅ Yes  | Replaces Telnet                     |
| Telnet       | 23   | Remote terminal access      | ❌ No   | Deprecated for security reasons     |
| SMTP         | 25   | Sending email               | ⚠️ Optional | Secure if paired with STARTTLS      |
| IMAP/POP3    | 143/110 | Retrieving email          | ⚠️ Optional | Use over SSL/TLS (993/995)          |
| RDP          | 3389 | Remote desktop              | ⚠️ With proper hardening            |
| DNS          | 53   | Domain resolution           | ⚠️ Limited | DNSSEC adds integrity               |

---

## Best Practices

- Disable insecure protocols where possible
- Use secure alternatives (SSH > Telnet, SFTP > FTP)
- Harden remote access tools like RDP with MFA and logging
- Monitor usage of legacy protocols in SIEM

---

> Protocols are trust channels—choose wisely.

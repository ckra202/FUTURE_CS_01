# OWASP Top 10 Checklist – Task 1: OWASP Juice Shop Assessment

**Intern:** Christian Dolce
**Date:** 07/02/2025
**Application:** OWASP Juice Shop  
**Tools Used:** Burp Suite, Firefox, Docker, Linux (Kali)

---

| OWASP Category (2021)           | Tested? | Vulnerability Found? | Description                                                                 |
|---------------------------------|---------|-----------------------|-----------------------------------------------------------------------------|
| A01:2021 – Broken Access Control | ❌      | ❌                    | Not tested in this phase.                                                  |
| A02:2021 – Cryptographic Failures | ❌      | ❌                    | Not applicable to current testing scope.                                   |
| A03:2021 – Injection             | ✅      | ✅                    | Reflected XSS, Stored XSS, and SQL Injection were confirmed.               |
| A04:2021 – Insecure Design       | ❌      | ❌                    | Not assessed in this phase.                                                |
| A05:2021 – Security Misconfiguration | ❌  | ❌                    | Not assessed during this round.                                            |
| A06:2021 – Vulnerable and Outdated Components | ❌ | ❌            | Not tested.                                                                |
| A07:2021 – Identification and Authentication Failures | ✅ | ✅    | SQL Injection led to login bypass (auth failure).                         |
| A08:2021 – Software and Data Integrity Failures | ❌ | ❌             | Not tested.                                                                |
| A09:2021 – Security Logging and Monitoring Failures | ❌ | ❌         | Not in scope.                                                              |
| A10:2021 – Server-Side Request Forgery (SSRF) | ❌ | ❌               | Not tested.
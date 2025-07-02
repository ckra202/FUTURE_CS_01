# Task 1 Vulnerability Analysis – OWASP Juice Shop

**Intern:** Christian Dolce
**Internship:** Future Interns – Cybersecurity Internship 2025  
**Project Duration:** June 28 – July 28, 2025  
**Folder:** `/Task_1_Vulnerability_Analysis

---

## 🔍 Objective

Conduct a hands-on vulnerability assessment of the OWASP Juice Shop application using Burp Suite, simulate real-world attack techniques (XSS, SQLi), and document findings mapped to the OWASP Top 10.

---

## 🛠️ Tools & Environment

- **Operating System:** Kali Linux  
- **Web Application:** OWASP Juice Shop (via Docker/Podman)  
- **Proxy Tool:** Burp Suite Community Edition  
- **Browser:** Firefox (manual proxy setup) & Burp Chromium  
- **Networking:** Custom hostname `juicebox.local` mapped to `127.0.0.1`

---

## 🧪 Vulnerabilities Identified

### 1. Reflected XSS in Search
- **OWASP:** A03 – Injection  
- **Severity:** Medium  
- **PoC:** `<img src=x onerror=alert(1)>` in search bar  
- **Status:** Alert triggered  
- **Screenshot:** `xss_search_alert.png`

### 2. SQL Injection – Login Bypass
- **OWASP:** A03 – Injection  
- **Severity:** High  
- **PoC:** `' OR 1=1--` in login email field  
- **Status:** Successful login without credentials  
- **Screenshot:** `sqli_login_success.png`

### 3. Stored XSS via Feedback
- **OWASP:** A03 – Injection  
- **Severity:** High  
- **PoC:** `<img src=x onerror=alert('Stored XSS')>` submitted in feedback form  
- **Status:** Payload stored and rendered in About Us  
- **Screenshot:** `stored_xss_about_us.png`

---

## 📎 Supporting Artifacts

- `Task_1_Report.pdf'-formal write-up of vulnerabilities
- `burp_http_history.xml` – Captured HTTP requests and responses
- Screenshots:
  - `xss_search_alert.png`
  - `sqli_login_success.png`
  - `stored_xss_about_us.png`

---

## ✅ Skills Demonstrated

- Proxy-based traffic interception
- Manual vulnerability discovery
- OWASP Top 10 mapping
- Burp Suite usage (Proxy, Repeater, HTTP Logs)
- Ethical hacking workflow and documentation

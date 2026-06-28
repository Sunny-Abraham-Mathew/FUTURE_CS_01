# FUTURE_CS_01
# 📋 Project Overview

This repository contains a vulnerability assessment conducted on **http://zero.webappsecurity.com/**  for Task 1 at Future Interns Cybersecurity Internship.

The assessment focused on identifying security weaknesses through passive and non-intrusive testing techniques using industry-standard security tools. No exploitation attempts, service disruption, or unauthorized access activities were performed during the assessment.

---

# 🎯 Objective

To analyze the security posture of the target web application, identify potential vulnerabilities, and document findings along with remediation recommendations.

---
## 📁 Repository Structure

```text
FUTURE_CS_01/
├── README.md
├── Vulnerability_Assessment_Report_Sunny.pdf
├── Zap.png
├── Burpsuite.png
└── nmap.png
```

# 🔍 Scope

**Target URL:** http://zero.webappsecurity.com/

**Assessment Type:** Vulnerability Assessment (Passive & Limited Safe Enumeration)

**Assessment Date:** 25 June 2026

**Pages Analyzed:** Publicly accessible pages and application components

### What Was Performed

* Passive vulnerability scanning
* HTTP response and security header analysis
* Web application reconnaissance
* Port and service enumeration

### What Was NOT Performed

* Authentication bypass attempts
* Brute-force attacks
* Denial-of-Service (DoS) testing
* Unauthorized exploitation of vulnerabilities
* Any activity that could negatively impact the target system

---


# 🛠️ Tools Used

| Tool                         | Purpose                                                |
| ---------------------------- | ------------------------------------------------------ |
| OWASP ZAP                    | Automated vulnerability scanning and passive analysis  |
| Burp Suite Community Edition | HTTP request/response inspection and manual validation |
| Nmap                         | Port scanning and service enumeration                  |

---

# 📊 Assessment Summary

The assessment identified multiple security issues of varying severity levels, including:

* Missing or misconfigured security headers
* Cookie security weaknesses
* Information disclosure findings
* Configuration-related issues
* Potential client-side security concerns

Detailed findings, evidence, risk ratings, and remediation recommendations are documented within this repository.

---
Severity    Count
CRITICAL    1
HIGH        3
MEDIUM      6
LOW         3

Total Findings: 13
| ID      | Finding                                                                  | Severity | Source     |
| ------- | ------------------------------------------------------------------------ | -------- | ---------- |
| VULN-01 | Content Security Policy (CSP) Header Not Set                             | Medium   | OWASP ZAP  |
| VULN-02 | Cross-Domain Misconfiguration                                            | Medium   | OWASP ZAP  |
| VULN-03 | Exposed Server Status Page                                               | Medium   | OWASP ZAP  |
| VULN-04 | Missing Anti-clickjacking Header                                         | Medium   | OWASP ZAP  |
| VULN-05 | Vulnerable JS Library                                                    | Medium   | OWASP ZAP  |
| VULN-06 | In-Page Banner Information Leak                                          | Low      | OWASP ZAP  |
| VULN-07 | Server Leaks Version Information via "Server" HTTP Response Header Field | Low      | OWASP ZAP  |
| VULN-08 | X-Content-Type-Options Header Missing                                    | Low      | OWASP ZAP  |
| VULN-09 | Expired SSL Certificate                                                  | High     | Nmap       |
| VULN-10 | SSLv2 Enabled                                                            | Critical | Nmap       |
| VULN-11 | Outdated, End-of-Life Software Stack                                     | High     | Nmap       |
| VULN-12 | Risky HTTP Methods (PUT/DELETE/TRACE/PATCH)                              | Medium   | Nmap       |
| VULN-13 | Weak Transport Security Due to Expired SSL/TLS Certificate               | High     | Burp Suite |


# ⚠️ Disclaimer

This assessment was conducted solely for educational and authorized security research purposes. All testing activities were performed responsibly and within the intended scope of the target application.

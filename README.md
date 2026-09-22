# OWASP Juice Shop VAPT

A Vulnerability Assessment and Penetration Testing (VAPT) project performed against the OWASP Juice Shop web application in a controlled local laboratory environment.

## Project Overview

This project demonstrates a structured web application security assessment covering:

- Planning and Scoping
- Reconnaissance
- Vulnerability Scanning and Assessment
- Manual Verification and Proof of Concept
- Post-Exploitation and Impact Analysis
- Risk Assessment
- Remediation Recommendations
- Retesting Methodology

The assessment was performed against a locally hosted OWASP Juice Shop instance for educational and cybersecurity training purposes.

## Target

| Item            | Details                     |
| --------------- | --------------------------- |
| Application     | OWASP Juice Shop            |
| Environment     | Controlled Local Laboratory |
| Target URL      | `http://127.0.0.1:3000`     |
| Assessment Type | Web Application VAPT        |

## Tools Used

- Burp Suite
- OWASP ZAP
- Nmap
- FFUF
- SQLMap
- Wappalyzer
- Browser Developer Tools

## Confirmed Vulnerabilities

| Finding ID | Vulnerability                                                 | Severity |
| ---------- | ------------------------------------------------------------- | -------- |
| BAC        | Broken Access Control – Privilege Escalation                  | Critical |
| IDOR       | Insecure Direct Object Reference – Unauthorized Basket Access | Medium   |
| AUTH       | Weak Password Recovery Mechanism via Security Question        | Critical |
| SQLI-01    | SQL Injection – Authentication Bypass                         | Critical |
| SQLI-02    | SQL Injection – Product Search/Data Extraction                | High     |
| XSS        | Reflected Cross-Site Scripting – Search Parameter             | Medium   |
| CSRF       | Cross-Site Request Forgery – Profile Update                   | Medium   |
| OR         | Open Redirect – Unvalidated Redirect Parameter                | Medium   |

### Severity Distribution

- Critical: 3
- High: 1
- Medium: 4
- Low: 0
- Total Confirmed Findings: 8

## Assessment Evidence

The repository contains supporting evidence collected during the assessment, including:

- Reconnaissance results
- OWASP ZAP scan evidence
- Burp Suite requests and responses
- FFUF reconnaissance evidence
- SQLMap results
- Proof-of-concept screenshots
- Successful validation evidence
- Remediation and retesting documentation

Evidence is organized under the `evidence/` directory.

## Final Report

The complete VAPT assessment report is available here:

`report/VAPT-Report-Final.pdf`

The report contains:

- Executive Summary
- Assessment Scope
- Methodology
- Reconnaissance
- Vulnerability Assessment
- Manual Verification and PoC
- Risk Assessment
- Technical Findings
- Impact Analysis
- CVSS Scoring
- Remediation Recommendations
- Retesting Methodology
- Conclusion

## Report Source

The LaTeX source used to prepare the report is available under:

`report/latex-source/`

## Repository Structure

```text
OWASP-Juice-Shop-VAPT/
│
├── README.md
├── .gitignore
│
├── report/
│   ├── VAPT-Report-Final.pdf
│   └── latex-source/
│       ├── main.tex
│       └── sections/
│
├── evidence/
│   ├── phase2/
│   ├── phase3/
│   └── phase4/
│
└── archive/
    ├── Phase-1-Planning-and-Scoping/
    ├── Phase-2-Reconnaissance/
    ├── Phase-3-Vulnerability-Scanning-and-Assessment/
    └── Phase-4-Manual-Verification-and-PoC/
```

## Retesting Status

The report documents the planned retesting methodology. At the time of the assessment, remediation had not yet been implemented and retesting had not been performed.

## Disclaimer

This assessment was conducted against an intentionally vulnerable OWASP Juice Shop instance hosted in a controlled local laboratory environment for educational and cybersecurity training purposes.

No unauthorized real-world systems were tested.

The findings and evidence in this repository are intended for educational, portfolio, and cybersecurity training purposes.

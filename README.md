# OWASP Juice Shop VAPT

A Vulnerability Assessment and Penetration Testing (VAPT) project performed against the OWASP Juice Shop web application in a controlled local laboratory environment.

## Project Overview

This project demonstrates a structured web application security assessment covering the complete VAPT lifecycle:

- Planning and Scoping
- Reconnaissance
- Vulnerability Scanning and Assessment
- Manual Verification and Proof of Concept
- Post-Exploitation and Impact Analysis
- Reporting and Risk Assessment
- Remediation Recommendations and Retesting Methodology

The assessment was performed against a locally hosted OWASP Juice Shop instance for educational and cybersecurity training purposes.

## Target

| Item | Details |
|---|---|
| Application | OWASP Juice Shop |
| Environment | Controlled Local Laboratory |
| Target URL | `http://127.0.0.1:3000` |
| Assessment Type | Web Application VAPT |

## Tools Used

- Burp Suite
- OWASP ZAP
- Nmap
- FFUF
- SQLMap
- Wappalyzer
- Browser Developer Tools

## Confirmed Vulnerabilities

| Finding ID | Vulnerability | Severity |
|---|---|---|
| BAC | Broken Access Control – Privilege Escalation via Registration | Critical |
| IDOR | Insecure Direct Object Reference – Unauthorized Basket Access | Medium |
| AUTH | Weak Password Recovery | Critical |
| SQLI-01 | SQL Injection – Authentication Bypass | Critical |
| SQLI-02 | SQL Injection – Product Search and Data Extraction | High |
| XSS | Reflected Cross-Site Scripting – Search Parameter | Medium |
| CSRF | Cross-Site Request Forgery – Profile Update | Medium |
| OR | Open Redirect – Unvalidated Redirect Parameter | Medium |

### Severity Distribution

- Critical: 3
- High: 1
- Medium: 4
- Low: 0
- Total Confirmed Findings: 8

## Assessment Evidence

The repository contains supporting evidence collected during the assessment, including:

- Reconnaissance results
- Nmap scanning results
- Wappalyzer technology identification
- FFUF directory discovery
- OWASP ZAP scanning evidence
- Burp Suite requests and responses
- SQLMap results
- Manual proof-of-concept evidence
- Successful vulnerability validation evidence
- Impact analysis documentation
- Remediation and retesting methodology

Evidence is organized under the `evidence/` directory.

## Final VAPT Report

The complete VAPT assessment report is available here:

[**VAPT-Report-Final.pdf**](report/VAPT-Report-Final.pdf)

The report contains:

- Executive Summary
- Assessment Scope
- Methodology
- Reconnaissance
- Vulnerability Assessment
- Manual Verification and PoC
- Post-Exploitation and Impact Analysis
- Risk Assessment
- Technical Findings
- CVSS Scoring
- Remediation Recommendations
- Retesting Methodology
- Conclusion

## Report Source

The LaTeX source used to prepare the report is available under:

[**report/latex-source/**](report/latex-source/)

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
│   │   └── images-proved/
│   ├── phase3/
│   │   └── zap/
│   └── phase4/
│       ├── authentication/
│       ├── bac/
│       ├── csrf/
│       ├── idor/
│       ├── openredirect/
│       ├── sqli-1/
│       ├── sqli-2/
│       └── xss-reflected/
│
└── archive/
    ├── Phase-1-Planning-and-Scoping/
    ├── Phase-2-Reconnaissance/
    ├── Phase-3-Vulnerability-Scanning-and-Assessment/
    ├── Phase-4-Manual-Verification-and-PoC/
    ├── Phase-5-Post-Exploitation-and-Impact-Analysis/
    ├── Phase-6-Reporting-and-Risk-Assessment/
    └── Phase-7-Remediation-and-Retesting/

# Phase 4 — Manual Verification and Proof of Concept

## Overview

Phase 4 focuses on the manual verification and proof-of-concept testing of security vulnerabilities identified during the assessment.

The objective of this phase was to determine whether potential security weaknesses were actually exploitable, verify their security impact, and collect supporting evidence.

The assessment used both findings identified during automated scanning and vulnerabilities identified directly through manual testing.

Only vulnerabilities that were successfully validated and supported by appropriate evidence were treated as confirmed findings.

---

## Objective

The main objectives of Phase 4 were:

- Manually verify potential vulnerabilities identified during Phase 3.
- Identify additional vulnerabilities through manual security testing.
- Validate the exploitability of identified weaknesses.
- Demonstrate the security impact of confirmed vulnerabilities.
- Collect proof-of-concept evidence.
- Document affected endpoints and parameters.
- Record the testing methodology and observed results.
- Provide evidence for the final VAPT findings.

---

## Testing Tools

The following tools and techniques were used during manual verification and proof-of-concept testing:

| Tool / Technique | Purpose |
|---|---|
| Burp Suite | HTTP request interception, modification, and manual testing |
| SQLMap | SQL Injection validation and database information extraction |
| Browser Developer Tools | Client-side request and response analysis |
| Manual Testing | Vulnerability identification and verification |
| Crafted HTTP Requests | Controlled proof-of-concept testing |

---

## Phase 3 to Phase 4 Validation

Phase 3 was primarily focused on automated vulnerability scanning and alert review.

OWASP ZAP identified potential security issues that required further investigation.

The following findings were carried forward from automated scanning for manual validation:

| Finding ID | Vulnerability | Source |
|---|---|---|
| SQLI-02 | SQL Injection – Product Search and Data Extraction | OWASP ZAP |
| OR | Open Redirect – Unvalidated Redirect Parameter | OWASP ZAP |

The remaining confirmed findings were identified through manual security testing during Phase 4.

The assessment followed the process:

## Confirmed Vulnerabilities

The manual verification and proof-of-concept phase confirmed the following eight vulnerabilities in the OWASP Juice Shop application.

| Finding ID | Vulnerability | Severity | Status |
|---|---|---|---|
| BAC | Broken Access Control – Privilege Escalation via Registration | Critical | Confirmed |
| IDOR | Insecure Direct Object Reference – Unauthorized Basket Access | Medium | Confirmed |
| AUTH | Weak Password Recovery | Critical | Confirmed |
| SQLI-01 | SQL Injection – Authentication Bypass | Critical | Confirmed |
| SQLI-02 | SQL Injection – Product Search and Data Extraction | High | Confirmed |
| XSS | Reflected Cross-Site Scripting – Search Parameter | Medium | Confirmed |
| CSRF | Cross-Site Request Forgery – Profile Update | Medium | Confirmed |
| OR | Open Redirect – Unvalidated Redirect Parameter | Medium | Confirmed |

These findings were manually verified and supported by proof-of-concept testing and evidence collected during the assessment.

```text
Automated Scanning / Manual Discovery
                ↓
           Alert Review
                ↓
       Manual Verification
                ↓
       Proof of Concept
                ↓
        Evidence Collection
                ↓
        Confirmed Finding

evidence/phase4/
├── authentication/
├── bac/
├── csrf/
├── idor/
├── openredirect/
├── sqli-1/
├── sqli-2/
└── xss-reflected/

# Phase 4 — Manual Verification and Proof of Concept

## Objective

This phase focuses on manually verifying potential and manually identified vulnerabilities in the OWASP Juice Shop application.

The purpose of this phase was to determine whether the identified security weaknesses were actually exploitable, confirm their security impact, and collect supporting proof-of-concept evidence.

Phase 4 includes both:

- Findings identified through automated scanning and subsequently validated manually.
- Vulnerabilities identified directly through manual security testing.

---

## Testing Approach

The following tools and techniques were used during manual verification:

- Burp Suite
- SQLMap
- Browser Developer Tools
- Manual HTTP request and response analysis
- Controlled proof-of-concept testing

Automated scanner alerts were treated as potential vulnerabilities until manual testing confirmed their actual behavior and impact.

---

## Confirmed Vulnerabilities

The following eight vulnerabilities were manually verified and confirmed during the assessment:

| Finding ID | Vulnerability | Severity | Status |
|---|---|---|---|
| BAC | Broken Access Control – Privilege Escalation | Critical | Confirmed |
| IDOR | Insecure Direct Object Reference – Unauthorized Basket Access | Medium | Confirmed |
| AUTH | Weak Password Recovery Mechanism via Security Question | Critical | Confirmed |
| SQLI-01 | SQL Injection – Authentication Bypass | Critical | Confirmed |
| SQLI-02 | SQL Injection – Product Search/Data Extraction | High | Confirmed |
| XSS | Reflected Cross-Site Scripting – Search Parameter | Medium | Confirmed |
| CSRF | Cross-Site Request Forgery – Profile Update | Medium | Confirmed |
| OR | Open Redirect – Unvalidated Redirect Parameter | Medium | Confirmed |

---

## Manual Verification Summary

### 1. Broken Access Control — Privilege Escalation

**Finding ID:** `BAC`

The registration functionality was manually tested to determine whether client-controlled role information could be modified.

Burp Suite was used to intercept and modify the registration request. The modified request was then used to verify whether an administrator-level account could be created.

The vulnerability was successfully confirmed.

**Evidence:**

```text
evidence/
└── phase4/
    └── bac/
        ├── bac01-burp-registration-request.jpg
        ├── bac02-burp-role-admin-modification.jpg
        ├── bac03-admin-page-access.jpg
        └── bac04-admin-registration-challenge-success.jpg

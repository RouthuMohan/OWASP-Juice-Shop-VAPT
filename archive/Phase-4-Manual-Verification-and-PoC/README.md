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

# Phase 6 — Reporting and Risk Assessment

## Overview

Phase 6 focused on consolidating the results of the VAPT assessment into a structured security assessment report and evaluating the risk associated with the confirmed vulnerabilities.

The findings confirmed during the assessment were documented with their severity, CVSS scores, affected functionality, security impact, evidence, and remediation recommendations.

The final report was prepared using the evidence collected throughout the assessment and the findings confirmed during the manual verification and proof-of-concept phase.

## Objectives

The main objectives of Phase 6 were:

- Consolidate the results of the VAPT assessment.
- Document all confirmed security findings.
- Assign severity levels based on the assessed risk.
- Document CVSS 3.1 scores and vectors.
- Analyze the potential impact of each finding.
- Reference supporting proof-of-concept evidence.
- Provide remediation recommendations.
- Prepare the final VAPT security assessment report.
- Present the overall security posture of the assessed application.

## Confirmed Vulnerabilities

The final assessment identified **8 confirmed vulnerabilities**.

| Finding ID | Vulnerability | Severity | CVSS 3.1 |
|---|---|---|---:|
| BAC | Broken Access Control – Privilege Escalation via Registration | Critical | 9.8 |
| IDOR | Insecure Direct Object Reference – Unauthorized Basket Access | Medium | 6.5 |
| AUTH | Weak Password Recovery | Critical | 9.1 |
| SQLI-01 | SQL Injection – Authentication Bypass | Critical | 9.8 |
| SQLI-02 | SQL Injection – Product Search and Data Extraction | High | 7.5 |
| XSS | Reflected Cross-Site Scripting – Search Parameter | Medium | 6.1 |
| CSRF | Cross-Site Request Forgery – Profile Update | Medium | 4.3 |
| OR | Open Redirect – Unvalidated Redirect Parameter | Medium | 4.3 |

## Risk Distribution

The final severity distribution was:

| Severity | Number of Findings |
|---|---:|
| Critical | 3 |
| High | 1 |
| Medium | 4 |
| Low | 0 |
| **Total** | **8** |

## CVSS Assessment

CVSS 3.1 scoring was used to communicate the technical severity of the confirmed vulnerabilities.

The final scores were:

- BAC — 9.8 (Critical)
- IDOR — 6.5 (Medium)
- AUTH — 9.1 (Critical)
- SQLI-01 — 9.8 (Critical)
- SQLI-02 — 7.5 (High)
- XSS — 6.1 (Medium)
- CSRF — 4.3 (Medium)
- OR — 4.3 (Medium)

The corresponding CVSS vectors and detailed scoring rationale are documented in the final VAPT report.

## Risk Assessment

The assessment identified security risks across several areas of the application, including:

- Authentication
- Authorization and access control
- Privilege management
- Database security
- Confidentiality of application data
- Integrity of user information
- Client-side security
- Account security
- User redirection

The Critical findings included privilege escalation, weaknesses in password recovery, and SQL Injection resulting in authentication bypass.

The High finding involved SQL Injection in the product search functionality and potential database information disclosure.

The Medium findings affected authorization, unauthorized basket access, client-side script execution, profile modification, and redirect functionality.

## Remediation Recommendations

The final report provides remediation recommendations for each confirmed vulnerability.

The recommendations focus on strengthening the application's security controls, including:

- Enforcing server-side authorization and role validation.
- Implementing proper access checks for user-specific resources.
- Strengthening password recovery mechanisms.
- Using parameterized queries and secure database interaction.
- Implementing appropriate input validation and output encoding.
- Implementing effective CSRF protection.
- Validating redirect destinations.
- Applying secure authentication and authorization practices.

## Final VAPT Report

The complete security assessment report is available at:

```text
report/VAPT-Report-Final.pdf

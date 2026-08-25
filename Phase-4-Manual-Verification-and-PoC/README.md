# Phase 4 — Manual Verification and Proof of Concept

## Objective

This phase manually verifies potential vulnerabilities identified during reconnaissance and vulnerability assessment.

The purpose is to determine whether the identified issues are actually exploitable and to collect proof-of-concept evidence demonstrating their security impact.

## Verified Vulnerabilities

| Vulnerability | Status |
|---|---|
| SQL Injection | Confirmed |
| Reflected XSS | Confirmed |
| Broken Access Control | Pending |
| Authentication-related vulnerability | Pending |

## Evidence Organization

```text
evidence/
├── sqli/
├── xss/
├── bac/
└── authentication/

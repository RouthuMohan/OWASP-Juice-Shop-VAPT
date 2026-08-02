# Phase 1 – Planning and Scoping

## Overview

This phase defines the scope, objectives, testing environment, and rules of engagement for the Vulnerability Assessment and Penetration Testing (VAPT) of OWASP Juice Shop.

The assessment is performed in a controlled local lab environment for educational and cybersecurity training purposes.

---

## Project Objective

The objective of this project is to perform a structured VAPT assessment of OWASP Juice Shop and identify, validate, exploit, and document security vulnerabilities within the application.

The project follows the following VAPT phases:

1. Planning and Scoping
2. Reconnaissance (Information Gathering)
3. Vulnerability Assessment
4. Exploitation / Penetration Testing
5. Reporting

---

## Target Information

| Item | Details |
|---|---|
| Target Application | OWASP Juice Shop |
| Target URL | `http://127.0.0.1:3000` |
| Environment | Local Lab |
| Assessment Type | Web Application VAPT |
| Testing Approach | Manual and Automated Testing |

---

## Scope

### In Scope

The following components are included in the assessment:

- OWASP Juice Shop web application
- Application endpoints and routes
- REST API endpoints
- Authentication and session mechanisms
- User-controlled input fields
- Application access controls
- Client-server HTTP communication
- Application security configurations

### Out of Scope

The following are excluded from the assessment:

- External websites and services
- Other devices on the local network
- Host operating system exploitation
- Denial-of-Service (DoS) testing
- Any system not belonging to the local OWASP Juice Shop lab

---

## Rules of Engagement

The following rules are followed during testing:

- Testing is restricted to the local OWASP Juice Shop instance.
- Testing activities are performed only within the defined scope.
- No attacks are performed against real-world or unauthorized systems.
- Denial-of-Service testing is excluded.
- Findings are documented with appropriate evidence.
- Testing is performed for educational and cybersecurity training purposes.

---

## Testing Methodology

The assessment follows a structured VAPT methodology:

### Phase 1 – Planning and Scoping
Define the target, scope, objectives, and testing boundaries.

### Phase 2 – Reconnaissance
Gather information about the target, technologies, services, directories, and application endpoints.

### Phase 3 – Vulnerability Assessment
Identify and validate potential security weaknesses in the application.

### Phase 4 – Exploitation
Perform controlled exploitation of confirmed vulnerabilities and collect proof of impact.

### Phase 5 – Reporting
Document findings, severity, evidence, impact, and recommended remediation.

---

## Expected Deliverables

The project will produce:

- Reconnaissance findings
- Vulnerability assessment results
- Confirmed vulnerability findings
- Proof-of-concept evidence
- Risk and impact analysis
- Remediation recommendations
- Final VAPT report

---

## Authorization

OWASP Juice Shop is intentionally vulnerable and is being hosted locally for security testing and educational purposes.

All testing documented in this project is restricted to the controlled lab environment.

---

## Phase Status

**Status:** Completed

The project scope, target, objectives, testing boundaries, and methodology have been defined. The assessment can proceed to **Phase 2 – Reconnaissance**.

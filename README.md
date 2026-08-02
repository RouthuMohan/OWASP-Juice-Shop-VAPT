# OWASP Juice Shop VAPT

A Vulnerability Assessment and Penetration Testing (VAPT) project performed on the OWASP Juice Shop application in a controlled local lab environment.

The project follows a structured VAPT methodology covering planning, reconnaissance, vulnerability assessment, exploitation, and reporting.

---

## Project Scope

| Item | Details |
|---|---|
| Target Application | OWASP Juice Shop |
| Target URL | `http://127.0.0.1:3000` |
| Testing Environment | Local Lab |
| Assessment Type | Web Application VAPT |
| Testing Approach | Manual and Automated Testing |

---

## VAPT Methodology

The project follows five phases:

### Phase 1 – Planning and Scoping ✅

Defines the target, objectives, scope, testing boundaries, rules of engagement, and assessment methodology.

**Status:** Completed

[View Phase 1 – Planning and Scoping](Phase-1-Planning-and-Scoping/README.md)

---

### Phase 2 – Reconnaissance (Information Gathering) ✅

Information about the target application and its attack surface was collected before vulnerability testing.

**Tools Used:**

- Nmap
- Browser
- Wappalyzer
- Burp Suite
- OWASP ZAP
- ffuf

**Activities Performed:**

- Target identification
- Port scanning
- Service detection
- Technology identification
- `robots.txt` analysis
- HTTP request and response analysis
- Directory and endpoint discovery
- Traditional spidering
- AJAX-based crawling

**Status:** Completed

[View Phase 2 – Reconnaissance](Phase-2-Reconnaissance/README.md)

---

### Phase 3 – Vulnerability Assessment

Potential security vulnerabilities will be identified and manually verified using the information collected during reconnaissance.

**Status:** Not Started

---

### Phase 4 – Exploitation / Penetration Testing

Confirmed vulnerabilities will be exploited in the controlled lab environment to demonstrate their security impact and collect proof-of-concept evidence.

**Status:** Not Started

---

### Phase 5 – Reporting

Confirmed findings will be documented with severity, evidence, impact, and remediation recommendations in the final VAPT report.

**Status:** Not Started

---

## Project Structure

```text
OWASP-Juice-Shop-VAPT/
│
├── README.md
│
├── Phase-1-Planning-and-Scoping/
│   └── README.md
│
├── Phase-2-Reconnaissance/
│   ├── README.md
│   └── images/
│
├── Phase-3-Vulnerability-Assessment/
│
├── Phase-4-Exploitation/
│
└── Phase-5-Reporting/

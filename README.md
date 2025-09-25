# Task-3
---

## Overview

This document contains the results of a **Nessus vulnerability scan** performed on multiple hosts within the internal network.
The scan identifies vulnerabilities, misconfigurations, and informational findings, categorized by severity.

* **Report File:** `vuln scan_f4asqq (1).pdf`
* **Tool Used:** Tenable Nessus
* **Author:** Vijay Chandra Kumar B
* **Date:** 25-09-2025

---

## Target Hosts Scanned

1. **Host 10.0.0.1** – 14 vulnerabilities (2 Medium, 12 Informational)
2. **Host 10.0.0.2** – 84 vulnerabilities (5 Critical/High, 3 Medium, 75 Informational)
3. **Host 10.0.0.3** – 5 vulnerabilities (all Informational)

---

## Severity Distribution

* **Critical:** 1
* **High:** 4
* **Medium:** 5
* **Low:** 0
* **Informational:** 92

---

## Key Findings & Mitigation Tips

### 🔹 Host 10.0.0.1

* **IP Forwarding Enabled (Medium):** Disable IP forwarding unless explicitly required for routing.
* **DNS Cache Snooping (Medium):** Restrict DNS server access and configure query filtering.
* **Info Leaks:** Limit unnecessary network services and disable unused protocols.

### 🔹 Host 10.0.0.2

* **Node.js Vulnerabilities (Critical/High):** Upgrade Node.js to the latest patched release.
* **Ruby RACK DoS (Medium):** Update Rack to version ≥ 2.2.14 / 3.x patched releases.
* **SSL Certificate Issues (Medium):** Replace untrusted/expired certificates with CA-signed ones.
* **Service/Software Enumeration:** Apply least privilege, firewall restrictions, and disable unneeded services.

### 🔹 Host 10.0.0.3

* **Informational Findings Only:** No immediate risk; monitor system regularly and keep software updated.

---

## References

Each finding in the report includes a direct link to the **Tenable Nessus Plugin ID** for remediation details.

Example:

* IP Forwarding Enabled → [Plugin 50686](https://www.tenable.com/plugins/nessus/50686)
* Node.js Multiple Vulnerabilities → [Plugin 190856](https://www.tenable.com/plugins/nessus/190856)

---

## How to Use This Report

* Open the PDF file (`vuln scan_f4asqq (1).pdf`) to review all findings.
* Prioritize **Critical and High severity issues** first (Node.js, SSL, Ruby RACK).
* Apply OS and application patches promptly.
* Disable or restrict unnecessary services to reduce attack surface.
* Use regular scanning and patch management to maintain security posture.

---

✅ This README provides a **concise summary with mitigation guidance** alongside the detailed PDF report.

---





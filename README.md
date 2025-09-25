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

1. **Host A** – 14 vulnerabilities (2 Medium, 12 Informational)
2. **Host B** – 84 vulnerabilities (5 Critical/High, 3 Medium, 75 Informational)
3. **Host C** – 5 vulnerabilities (all Informational)

---

## Severity Distribution

* **Critical:** 1
* **High:** 4
* **Medium:** 5
* **Low:** 0
* **Informational:** 92

---

## Key Findings

* **Host A:**

  * IP Forwarding Enabled (Medium risk)
  * DNS Server Cache Snooping (Medium risk)
  * Multiple OS and network info disclosures

* **Host B:**

  * Multiple **Node.js vulnerabilities** (Critical & High severity) across versions 18.x, 20.x, 21.x, 22.x, and 23.x
  * **Ruby RACK DoS vulnerability**
  * **SSL Certificate issues** (untrusted certificate)
  * Numerous informational findings (software detections, service enumeration, system configs)

* **Host C:**

  * Only informational findings (VMware detection, traceroute, NIC info)

---

## References

Each finding in the report contains a direct link to the **Tenable Nessus Plugin ID** for further details and remediation guidance.

Example:

* IP Forwarding Enabled → [Plugin 50686](https://www.tenable.com/plugins/nessus/50686)
* Node.js Multiple Vulnerabilities → [Plugin 190856](https://www.tenable.com/plugins/nessus/190856)

---

## How to Use This Report

* Open the PDF file (`vuln scan_f4asqq (1).pdf`) to review all findings.
* Focus remediation efforts first on **Critical and High vulnerabilities**, especially Node.js and SSL-related issues.
* Use the provided Nessus plugin reference links for mitigation steps.
* Apply security patches and hardening measures where necessary.

---



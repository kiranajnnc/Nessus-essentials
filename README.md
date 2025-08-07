
# 🔐 Vulnerability Assessment & Remediation – Localhost (127.0.0.1)

## 📋 Overview

This repository contains results and remediation documentation for a local vulnerability scan conducted as part of a cybersecurity internship. The scan was performed using *Tenable Nessus Essentials* on the localhost environment (127.0.0.1).

## 🛠 Tools Used

- *Nessus Essentials* – Vulnerability scanner for up to 16 IPs
- *CVSS v3.0* – Standardized vulnerability severity scoring
- *Markdown* – Documentation and remediation log format
- *Linux CLI* – For manual verification and upgrades

## 📅 Scan Details

- *Scan Tool*: Nessus Essentials  
- *Target*: 127.0.0.1  
- *Scan Date*: August 7, 2025  
- *Total Vulnerabilities Found:* 78  
  - Critical: 2  
  - High: 5  
  - Medium: 6  
  - Low: 0  
  - Info: 65+

## 📁 Repository Contents

| File Name                 | Description                                              |
|---------------------------|----------------------------------------------------------|
| nessus-scan-report.pdf  | Exported Nessus vulnerability scan report               |
| remediation-log.md      | Structured log of vulnerabilities and remediation steps |
| README.md               | Project overview and instructions                        |

## ✅ Remediation Summary

- All *Critical* and *High* severity vulnerabilities have been patched or mitigated.
- Medium severity issues were addressed or are being monitored.
- Informational findings are logged for ongoing awareness.
- Verification was performed via re-scanning and manual checks (e.g., node -v, sqlite3 --version).

## 🔧 Key Vulnerabilities Remediated

- Multiple *Node.js* vulnerabilities upgraded to stable versions (20.19.4+)
- *Ruby Rack* denial-of-service vulnerability patched
- *SQLite* memory corruption vulnerabilities fixed by upgrading packages
- SSL certificate issues resolved by installing properly trusted certificates

## 📌 Notes

- Scan was performed with authenticated credentials for accuracy.
- All remediation followed official vendor advisories.
- Verification included rescanning and command line checks.

## 4. Internal Questions Answered

*1. What is vulnerability scanning?*  
Vulnerability scanning is an automated process that inspects systems, networks, and applications to detect known security weaknesses before adversaries can exploit them.

*2. Differences between vulnerability scanning and penetration testing?*  
- Vulnerability scanning is automated and identifies known issues without exploiting them.  
- Penetration testing is manual (or semi-automated), exploits vulnerabilities to demonstrate real-world impact, and often involves social-engineering or privileged escalation.

*3. What are common vulnerability scanning and penetration testing tools?*  
- Scanners: OpenVAS, Nessus, Qualys, Rapid7 InsightVM.  
- Penetration testing: Metasploit, Burp Suite Pro, Cobalt Strike.

*4. What are some common vulnerabilities in personal computers?*  
- Missing OS and software patches  
- Default or weak credentials  
- Unencrypted remote-access services (RDP, Telnet)  
- Exposed management interfaces (SNMP, RPC)

*5. How do scanners detect vulnerabilities?*  
Scanners use signature databases (CVE lists), configuration checks, and service fingerprinting to match system outputs against known vulnerability patterns.

*6. What is CVSS?*  
The Common Vulnerability Scoring System (CVSS) provides a standardized numerical score (0.0–10.0) reflecting a vulnerability’s severity and exploitability.

*7. How often should vulnerability scans be performed?*  
At minimum, monthly for external-facing assets and quarterly for internal networks; after major system changes or emergency patches.

*8. How is a false positive vulnerability identified?*  
By verifying the finding manually—cross-checking with vendor documentation, testing exploit conditions, or using alternative scanning tools.

## 5. Key Concepts

- *Vulnerability Scanning*  
- *Risk Assessment*  
- *CVSS (Common Vulnerability Scoring System)*  
- *Remediation*  
- *Security Tools*  




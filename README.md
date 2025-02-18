# Cybersecurity-Nessus-Assessment

## Overview

This project showcases a comprehensive vulnerability assessment using Tenable Nessus, focusing on identifying, analyzing, and mitigating security risks in a simulated environment. The assessment aligns with NIST 800-171 and CMMC compliance frameworks, helping organizations strengthen their security posture and reduce potential attack vectors.

---

## Key Focus Areas:

- Credentialed vulnerability scans for deeper system insights
- Web application security assessment to detect potential risks
- Configuration reviews for OpenSSH, Apache, and Nginx to prevent exploitation
- Automated vulnerability reporting for proactive risk management

## Tools Used

* Nessus (for vulnerability scanning)

* Linux (Ubuntu, Kali)

* SMTP (for email reporting)

* OpenSSH, Apache, Nginx (web services assessment)

---

## Methodology

### Vulnerability Scanning with Nessus

- Scanned assets for misconfigurations, outdated software, weak encryption, and open ports.
- Mapped detected vulnerabilities to MITRE ATT&CK tactics for threat classification.
- Used Nmap for supplementary network reconnaissance.

### Compliance Alignment (NIST 800-171 & CMMC)

- Mapped scan results to NIST 800-171 & CMMC security controls.
- Identified gaps in access control, encryption, endpoint security, and log management.

### Risk Analysis & Prioritization

- Categorized vulnerabilities based on CVSS (Common Vulnerability Scoring System) scores.
- Assessed risk levels based on exploitability and impact on system integrity.
- Prioritized remediation efforts using a risk-based approach.

### Remediation Strategies

- Patching & Updates: Recommended applying security patches to mitigate known vulnerabilities.
- Hardening Configurations: Strengthened endpoint security by enforcing least privilege access and disabling unnecessary services.
- Network Security Improvements: Suggested firewall rule updates and network segmentation.

### Security Metrics & Reporting

- Generated compliance reports detailing security posture improvements.
- Tracked vulnerability trends over time to measure risk reduction.

---
## Assessment Process

### Credentialed Scan on Linux Server

* Configured SSH-based authentication for Nessus credentialed scans.

* Verified root access settings in /etc/ssh/sshd_config.

* Assessed vulnerabilities in OpenSSH versions and configurations.

* Identified misconfigurations such as weak password authentication settings.


### Web Application Security Assessment

* Conducted a web vulnerability scan using Nessus.

* Identified OWASP Top 10 issues (XSS, SQL Injection, etc.).

* Tested Apache & Nginx configurations for security gaps.

* Reviewed HTTP method restrictions in /etc/apache2/apache2.conf.


### Automated Email Reporting

* Configured SMTP settings in Nessus to send reports via email.

* Enabled TLS encryption for secure transmission (smtp.gmail.com:587).

* Implemented Python-based automation for sending scan reports.

---

## Key Findings & Impact
| Vulnerability              | CVSS Score     | Affected Systems  | Status                 |
| ------------------------   | -------------- | ----------------- | ---------------------- |
| Node.js RCE (CVE-2024)     | 9.8 (Critical) | Web Server        | Patch Required         |
| OpenSSH Weak Cipher Use    | 8.2 (High)     | Linux Servers     | Reconfiguration Needed |
| SSL Certificate Issues     | 6.5 (Medium)   | Web & API Servers | Upgrade to Trusted CA  |
| Apache mod_status Exposure | 5.3 (Medium)   | Apache Servers    | Restrict Access        |

---

## Results & Recommendations

### Critical Vulnerabilities (CVE Analysis)

1. Node.js (CVE-2024) - Remote Code Execution (RCE)

    - Fix: Upgrade to version 18.20.4+, 20.15.1+, or 22.4.1+.

2. nginx 1-Byte Memory Overwrite (RCE - CVE-2024)

    - Fix: Upgrade nginx to 1.20.1 or higher.


### High-Risk Vulnerabilities

1. Apache mod_status Information Disclosure

    * Fix: Disable mod_status or restrict access.

2. SSL Certificate Cannot Be Trusted

    * Fix: Install a valid SSL certificate from a trusted CA.


### Medium-Risk Vulnerabilities

1. nginx Information Disclosure

    * Fix: Update nginx to 1.17.7+.

2. aioHTTP XSS (Cross-Site Scripting)

    * Fix: Upgrade aioHTTP to 3.9.4+ and implement input validation.

---
## Conclusion

By implementing Nessus-based vulnerability assessments, we successfully identified and mitigated critical security risks in the Linux infrastructure and web applications. The automated reporting ensures continuous monitoring and proactive security posture improvement.

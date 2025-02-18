# Cybersecurity-Nessus-Assessment

## Overview

As cybersecurity analysts at CyberTech Solutions, we used Nessus to conduct a vulnerability assessment on Linux servers and web applications. Our goal was to identify security risks, analyze vulnerabilities, and automate security monitoring using credentialed scans and SMTP-based reporting.

---

## Tools Used

* Nessus (for vulnerability scanning)

* Linux (Ubuntu, Kali)

* SMTP (for email reporting)

* OpenSSH, Apache, Nginx (web services assessment)

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

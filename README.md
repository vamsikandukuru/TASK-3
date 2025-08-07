# Vulnerability Scanning

This project contains a vulnerability assessment performed on the Metasploitable 2 virtual machine using Nessus. The report highlights five critical vulnerabilities along with simple one-line remediation steps.

---

## Target Information

- **Subnets
- **IP Address**: 192.168.0.0/24
- **Scanner**: Nessus

---

## Top 5 Critical Vulnerabilities in Scanning & Remediation

| No. | Vulnerability                          | Description                                                                                     | Remediation                                                   |
|-----|----------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------|
| 1   | UnrealIRCd Backdoor Detection          | A known backdoor in UnrealIRCd allows remote code execution via a malicious command.           | Remove UnrealIRCd or upgrade to a secure version.             |
| 2   | VNC Server 'password' Password         | VNC server uses default weak password "password", allowing full remote access.                 | Set a strong, complex VNC password.                          |
| 3   | SSL Version 2 and 3 Protocol Detection | SSLv2/SSLv3 are outdated and insecure protocols prone to attacks.                              | Disable SSLv2/SSLv3 on all services and use TLS 1.2/1.3.     |
| 4   | Bind Shell Backdoor Detection          | A bind shell was detected, allowing attackers to connect and execute remote commands.          | Identify and remove the bind shell or block related ports.   |
| 5   | Canonical Ubuntu Linux SEoL (8.04.x)   | The system runs end-of-life Ubuntu 8.04 which no longer receives security updates.             | Upgrade the OS to a supported version like Ubuntu 22.04 LTS. |

---

##  Files Included

- nessus_report:  Nessus  report
- screenshots: Folder containing evidence of vulnerabilities
- README.md: Project documentation

---

##  Summary

This task demonstrates how to identify and mitigate critical vulnerabilities in legacy systems using Nessus. All listed issues are high risk and should be addressed immediately to prevent exploitation.

---

## 

Metasploitable 2 is intentionally vulnerable and should never be exposed to a public network.


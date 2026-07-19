# Lessons Learned

## Overview

The ransomware simulation provided valuable insight into how endpoint compromises can affect organizational assets and why layered defensive controls are essential.

Although the incident occurred in a controlled environment, the observations closely resemble real-world ransomware behavior.

---

# Key Findings

- Unsupported operating systems significantly increase organizational risk.
- Vulnerability management is essential to reduce exposure.
- Endpoint monitoring greatly improves incident visibility.
- Ransomware primarily targets data availability.
- Early detection reduces overall business impact.

---

# Security Recommendations

## Patch Management

Apply security updates promptly to eliminate known vulnerabilities.

---

## Disable Legacy Protocols

Disable SMBv1 where operationally possible.

---

## Endpoint Detection and Response (EDR)

Deploy EDR solutions capable of detecting:

- File encryption
- Suspicious process execution
- Behavioral anomalies

---

## Security Monitoring

Enable centralized logging through a SIEM platform.

Collect:

- Windows Event Logs
- Sysmon Logs
- PowerShell Logs
- Authentication Events

---

## Network Segmentation

Separate critical systems from user workstations to reduce lateral movement opportunities.

---

## Backup Strategy

Maintain:

- Offline backups
- Immutable backups
- Regular backup testing

---

## Incident Response Planning

Organizations should establish an Incident Response Plan that includes:

- Identification
- Containment
- Eradication
- Recovery
- Lessons Learned

---

# Personal Learning Outcomes

Through this project I gained practical experience in:

- Incident Response
- Windows Security
- Endpoint Investigation
- IOC Identification
- Evidence Collection
- Event Log Analysis
- Host-Based Forensics
- MITRE ATT&CK Mapping
- Security Documentation
- SOC Investigation Workflow

---

# Future Improvements

Future enhancements for this project include:

- Sysmon deployment
- Splunk log ingestion
- Sigma detection rules
- YARA rule development
- Wireshark traffic analysis
- Threat hunting queries
- Automated IOC extraction
- SIEM dashboard creation

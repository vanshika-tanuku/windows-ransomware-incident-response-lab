# Windows Ransomware Incident Response Lab

A controlled ransomware incident response lab demonstrating attacker behavior, forensic artifacts, MITRE ATT&amp;CK mapping, and defensive detection techniques in an isolated virtual environment.

---

## Overview

This project documents the investigation of a simulated ransomware incident within an isolated Windows 7 virtual machine. The objective was not to demonstrate offensive techniques, but to analyze the impact of ransomware from a Security Operations Center (SOC) perspective.

The lab simulates a ransomware infection in a controlled environment and walks through the investigation process, including:

- Incident identification
- Host investigation
- Evidence collection
- IOC extraction
- MITRE ATT&CK mapping
- Incident reporting
- Detection opportunities
- Security recommendations

---

## Objectives

- Build an isolated ransomeware analysis lab
- Simulate a ransomware incident
- Investigate the compromised endpoint
- Collect forensic evidence
- Document Indicators of Compromise (IOCs)
- Map attacker behavior to the MITRE ATT&CK framework
- Produce a professional incident report
- Recommend defensive measures

---

## Lab Environment

| Component | Details |
| --------- | ------- |
| Virtualization | Oracle VirtualBox |
| Attacker Machine | Kali Linux |
| Victim Machine | Windows 7 |
| Network | Internal Virtual Network |
| Analysis Type | Host-Based Incident Response |
| Malware | Simulated WannaCry Sample |
| Operating Mode | Offline / Isolated Lab|

---

## Lab Architecture

```
            VirtualBox

          Internal Network

      +-----------------------+
      |                       |
      |     Kali Linux        |
      |   (Attacker VM)       |
      |                       |
      +-----------+-----------+
                  |
                  |
                  |
      +-----------+-----------+
      |                       |
      |      Windows 7        |
      |    (Victim Machine)   |
      |                       |
      +-----------------------+
```

---
## Attack Scenario

During the investigation, the following observations were made:

- Windows 7 host successfully compromised in an isolated environment.
- Multiple user files became encrypted.
- Desktop wallpaper was modified.
- Ransom note was displayed.
- New ransomware-related files appeared within the user profile.
- Indicators of compromise were documented.
- Security event logs were reviewed.
- Host configuration was analyzed.
- Incident timeline was reconstructed.

---

## Investigation Workflow

```
Lab Setup
      ↓
Host Discovery
      ↓
Vulnerability Assessment
      ↓
Controlled Attack Simulation
      ↓
Host Investigation
      ↓
Evidence Collection
      ↓
IOC Analysis
      ↓
MITRE ATT&CK Mapping
      ↓
Impact Assessment
      ↓
Incident Report
      ↓
Defensive Recommendations
```

---

## Evidence Collected

- Network discovery results
- Vulnerability assessment
- Host information
- Windows Event Logs
- Security Logs
- Process Investigation
- Encrypted files
- Ransom note
- File system artifacts
- Desktop modifications
- Network configuration
- Incident screenshots

---

## MITRE ATT&CK Mapping

| Tactic | Technique |
|---------|-----------|
| Discovery | System Discovery |
| Initial Access | Exploitation of Public-Facing Service (Lab Simulation) |
| Execution | User Execution |
| Credential Access | OS Credential Dumping (Lab Observation) |
| Collection | Data Collection |
| Impact | Data Encrypted for Impact |

---

## Indicators of Compromise

Examples collected during the investigation include:

- Encrypted user files
- Modified desktop wallpaper
- Ransom note
- Ransomware executable
- Suspicious file extensions
- SMB activity
- Windows Event Logs
- Host artifacts

---

## Security Findings

The investigation identified several security weaknesses:

- Unsupported Windows 7 operating system
- SMB vulnerability present
- Missing security patches
- Lack of endpoint monitoring
- No endpoint detection and response (EDR)
- Insufficient host logging

---


## Skills Demonstrated

- Incident Response
- SOC Investigation
- Host-Based Forensics
- Windows Security
- Malware Analysis
- IOC Collection
- MITRE ATT&CK Mapping
- Vulnerability Assessment
- Documentation
- Security Reporting

---

## Lessons Learned

This project strengthened practical understanding of:

- Endpoint compromise investigation
- Ransomware behavior
- Evidence collection
- Incident documentation
- Security reporting
- Defensive analysis
- Blue Team methodologies

---

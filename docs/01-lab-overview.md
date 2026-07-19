# Lab Overview

## Purpose

The purpose of this laboratory is to simulate and investigate a ransomware incident within an isolated virtual environment. The project demonstrates how a Security Operations Center (SOC) analyst can investigate a compromised Windows endpoint, collect forensic evidence, identify Indicators of Compromise (IOCs), analyze the impact, and produce an incident report.

The environment was intentionally isolated using Oracle VirtualBox to ensure that all attack activity remained contained and posed no risk to external systems.

---

# Learning Objectives

This project was designed to achieve the following objectives:

- Build a controlled ransomware analysis environment
- Simulate a Windows ransomware incident
- Investigate the compromised endpoint
- Identify Indicators of Compromise (IOCs)
- Analyze the impact of ransomware on a Windows host
- Map observed behavior to the MITRE ATT&CK framework
- Document findings as an incident report
- Recommend defensive controls and mitigation strategies

---

# Lab Environment

| Component | Description |
|------------|-------------|
| Virtualization Platform | Oracle VirtualBox |
| Attacker Machine | Kali Linux |
| Victim Machine | Windows 7 |
| Network Type | Internal Virtual Network |
| Communication | SMB |
| Operating Mode | Offline / Isolated |

---

# Network Architecture

The lab consists of two virtual machines connected through an isolated VirtualBox Internal Network.

- Kali Linux acts as the attacker machine.
- Windows 7 acts as the victim endpoint.
- Both systems communicate only inside the isolated virtual network.
- Internet connectivity is disabled during testing to prevent unintended communication.

---

# Safety Considerations

This laboratory was conducted entirely within an isolated environment.

Safety measures included:

- VirtualBox snapshots before testing
- No Internet access
- No production systems involved
- Educational malware sample used solely for research
- VM restored immediately after investigation

---

# Scope

This project focuses on the investigation of a ransomware incident from a blue-team perspective.

The emphasis is placed on:

- Host investigation
- Evidence collection
- Incident analysis
- IOC identification
- Security recommendations

The repository does not serve as a guide for exploiting systems.

# Incident Report

## Incident Overview

| Field | Value |
|---------|-------|
| Incident Type | Ransomware |
| Severity | High |
| Investigation Type | Host-Based Incident Response |
| Environment | VirtualBox Isolated Lab |
| Status | Contained |

---

# Executive Summary

A ransomware incident was simulated within an isolated Windows 7 virtual environment to evaluate host-based investigation techniques and document defensive observations.

Following execution of the ransomware sample, user files became encrypted, the desktop environment was modified, and ransom-related artifacts were generated.

The investigation focused on identifying evidence of compromise, documenting attacker impact, collecting Indicators of Compromise (IOCs), and recommending defensive improvements.

---

# Incident Timeline

| Time | Activity |
|------|----------|
| T0 | Windows host operational |
| T1 | Vulnerable host identified |
| T2 | Simulated compromise completed |
| T3 | Ransomware executed |
| T4 | User files encrypted |
| T5 | Ransom note displayed |
| T6 | Host investigation initiated |
| T7 | Evidence collected |
| T8 | Snapshot restored |

---

# Evidence Collected

The following evidence was documented:

- Host information
- IP configuration
- Event Viewer logs
- Task Manager
- Encrypted user files
- Ransom note
- Desktop modifications
- Network configuration
- System information

---

# Key Findings

The investigation confirmed:

- Successful ransomware execution
- Encryption of user documents
- Encryption of media files
- Desktop wallpaper modification
- Ransom demand displayed
- Multiple ransomware artifacts created

---

# Indicators of Compromise

Observed indicators included:

- Encrypted `.WNCRY` files
- Ransom note
- Modified desktop wallpaper
- Ransomware artifacts
- SMB communication within the isolated lab

---

# Root Cause

The victim system was running an unsupported version of Windows with a known SMB vulnerability.

The absence of security updates allowed the simulated ransomware scenario to be reproduced within the isolated laboratory.

---

# Business Impact

The incident primarily affected:

- Availability of user data
- User productivity
- Access to personal documents

No production systems were involved.

---

# Containment

Containment actions included:

- Isolation of the virtual machine
- Preservation of forensic evidence
- Restoration using VirtualBox snapshot

---

# Recovery

Recovery consisted of restoring the victim machine to its clean snapshot.

No permanent data loss occurred because the environment was intentionally isolated for testing.

---

# Recommendations

Recommended improvements include:

- Upgrade unsupported operating systems
- Apply security patches promptly
- Disable SMBv1 where possible
- Deploy Endpoint Detection and Response (EDR)
- Enable Sysmon logging
- Centralize logs using a SIEM
- Maintain tested offline backups
- Develop and regularly test an incident response plan

---

# Conclusion

This project demonstrates a complete ransomware investigation workflow from a defender's perspective. The lab highlights the importance of proactive vulnerability management, endpoint visibility, structured evidence collection, and incident documentation.

Although performed in a controlled environment, the investigation methodology aligns with common SOC incident response practices and provides a foundation for developing practical blue-team skills.

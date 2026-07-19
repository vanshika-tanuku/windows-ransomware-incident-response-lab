# MITRE ATT&CK Mapping

The following table maps the observed attacker behavior to the MITRE ATT&CK Enterprise Framework.

| Tactic | Technique | ID | Observation |
|----------|-----------|------|-------------|
| Reconnaissance | Network Service Discovery | T1046 | Network hosts identified within the isolated environment |
| Initial Access | Exploitation of Remote Services | T1210 | Vulnerable SMB service exploited in lab |
| Execution | User Execution | T1204 | Ransomware executable launched |
| Discovery | File and Directory Discovery | T1083 | User directories enumerated |
| Credential Access | OS Credential Dumping | T1003 | Credential hash extraction observed during simulation |
| Collection | Data from Local System | T1005 | Sample user files accessed within the lab |
| Impact | Data Encrypted for Impact | T1486 | User files encrypted |
| Impact | Defacement | T1491 | Desktop wallpaper modified |
| Impact | Data Manipulation | T1565 | User files modified during encryption |

---

# ATT&CK Summary

The investigation demonstrates a typical ransomware attack lifecycle:

Reconnaissance

↓

Initial Access

↓

Execution

↓

Discovery

↓

Credential Access

↓

Collection

↓

Impact

The incident primarily affected the Availability component of the CIA Triad through encryption of user data.

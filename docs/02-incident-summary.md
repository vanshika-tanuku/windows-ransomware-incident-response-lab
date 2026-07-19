# Incident Summary

## Executive Summary

A simulated ransomware incident was successfully reproduced within an isolated Windows 7 virtual machine for educational and defensive research purposes.

Following execution of the ransomware sample, multiple user files became inaccessible due to encryption. The ransomware modified the desktop environment, created ransom-related artifacts, and displayed a ransom demand window.

The incident was investigated from the perspective of a Security Operations Center (SOC) analyst. Evidence was collected from the compromised endpoint to determine the scope of the attack, identify Indicators of Compromise (IOCs), and document the observed behavior.

---

# Incident Details

| Field | Value |
|---------|-------|
| Incident Type | Ransomware |
| Severity | High |
| Victim Host | Windows 7 |
| User | vboxuser |
| Environment | VirtualBox Internal Network |
| Status | Contained |
| Recovery Method | Snapshot Restoration |

---

# Initial Observations

The following observations were made immediately after the incident:

- Desktop wallpaper changed
- Ransom note displayed
- Multiple files encrypted
- User files inaccessible
- New ransomware artifacts present
- Host remained operational

---

# Scope of Impact

The following assets were affected:

- Desktop
- Documents
- Pictures
- Music
- User profile files

System files remained operational, allowing further investigation.

---

# Investigation Objectives

The investigation aimed to:

- Identify evidence of compromise
- Collect host artifacts
- Document attacker activity
- Identify Indicators of Compromise
- Assess business impact
- Recommend defensive improvements

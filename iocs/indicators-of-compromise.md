# Indicators of Compromise (IOCs)

## Overview

Indicators of Compromise (IOCs) are observable artifacts that suggest a system has been compromised. During this ransomware investigation, multiple host-based indicators were identified that can assist defenders in detecting similar incidents.

---

# Host Information

| Indicator | Value |
|------------|-------|
| Host Name | windows7 |
| Operating System | Windows 7 Home Basic |
| User Account | vboxuser |
| Network | VirtualBox Internal Network |

---

# File-Based Indicators

| Indicator | Observation |
|------------|-------------|
| File Extension | `.WNCRY` |
| Ransom Note | `@Please_Read_Me@` |
| Wallpaper | Modified after encryption |
| User Documents | Encrypted |
| Images | Encrypted |
| Music Files | Encrypted |
| Desktop Files | Encrypted |

---

# Process Indicators

Observed during investigation:

- Suspicious executable executed
- File encryption activity
- Multiple user files modified
- Desktop wallpaper changed

---

# Registry / System Artifacts

Observed artifacts:

- Ransom note files created
- Desktop modifications
- New ransomware-related files
- User profile artifacts

---

# Network Indicators

Observed activity:

- SMB communication between attacker and victim (isolated lab)
- Internal network communication only
- No Internet connectivity during testing

---

# Impact Indicators

The following indicators confirmed successful ransomware execution:

- User files inaccessible
- Desktop wallpaper modified
- Ransom note displayed
- Encrypted file extensions observed
- New ransomware artifacts present

---

# Detection Recommendations

SOC analysts should monitor for:

- Rapid file encryption
- Sudden file extension changes
- Creation of ransom notes
- Unauthorized executable launches
- Excessive SMB activity
- Multiple file modifications within a short period

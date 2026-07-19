# Network Analysis

## Overview

The purpose of this analysis was to review network-related observations from the simulated ransomware incident.

The environment consisted of an isolated VirtualBox Internal Network containing two virtual machines:

- Kali Linux
- Windows 7

No Internet connectivity was available during testing.

---

# Network Topology

| Machine | Role |
|----------|------|
| Kali Linux | Attacker |
| Windows 7 | Victim |

Communication occurred entirely within the internal virtual network.

---

# Observed Communication

During the investigation the following communication was observed:

- Host discovery
- SMB communication
- Remote session establishment
- Internal host communication

No external Internet traffic was generated.

---

# Protocols Observed

| Protocol | Purpose |
|-----------|----------|
| SMB | File sharing / communication |
| TCP | Session transport |
| ICMP | Host discovery (where applicable) |

---

# Security Observations

The Windows system exposed SMB services within the isolated network.

The vulnerable SMB implementation allowed the simulated compromise to occur.

---

# Network Risk Assessment

| Risk | Severity |
|------|----------|
| SMB Exposure | High |
| Legacy Operating System | High |
| Missing Security Updates | High |

---

# Detection Opportunities

Security teams should monitor for:

- Excessive SMB traffic
- Internal network scanning
- Unexpected host discovery
- Unusual lateral SMB communication
- Multiple failed SMB connections

---

# Recommended Defensive Controls

- Disable SMBv1
- Apply Microsoft security updates
- Restrict SMB using firewall policies
- Enable network intrusion detection
- Segment user workstations

# Windows Event Log Analysis

## Overview

Windows Event Viewer was reviewed to identify system activity related to the simulated ransomware incident.

The following logs were examined:

- Application
- Security
- System

---

# Application Log

Observed:

- Normal application events
- Service-related events
- Volume Shadow Copy Service (VSS) events

These events provide context for system activity during the investigation.

---

# Security Log

Observed:

- Successful user logon events
- User authentication records
- Normal security auditing events

No abnormal authentication attempts were observed during this investigation.

---

# System Log

Observed:

- Normal operating system activity
- Service status updates
- Device initialization events

No evidence of operating system instability was identified.

---

# Investigation Findings

The collected logs were used to:

- Establish the investigation timeline
- Verify system activity
- Correlate host observations
- Support incident documentation

---

# Limitations

The laboratory did not include:

- Sysmon
- Windows Defender logs
- EDR telemetry
- Centralized SIEM logging

As a result, visibility was limited to native Windows event logs.

---

# Recommendations

Future investigations should include:

- Sysmon
- Microsoft Defender for Endpoint
- Splunk or Microsoft Sentinel
- Centralized Windows Event Forwarding

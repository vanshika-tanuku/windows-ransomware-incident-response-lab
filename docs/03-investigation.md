# Investigation

## Phase 1 – Initial Observation

The investigation began after the victim system displayed ransomware indicators.

Observed changes included:

- Modified desktop wallpaper
- Ransom demand window
- Encrypted user files
- New ransom-related files

Screenshot:
screenshots/12_ransom_note_display.png

---

## Phase 2 – Host Identification

Basic system information was collected to identify the affected host.

Information collected:

- Computer Name
- Operating System
- User Account
- Network Adapter
- IP Address

Screenshots:

- screenshots/19_system_information.png
- screenshots/20_victim_network_configuration.png

---

## Phase 3 – Process Investigation

Running processes were examined using Windows Task Manager.

Objective:

- Identify suspicious processes
- Determine whether ransomware remained active
- Observe abnormal resource usage

Screenshot:

screenshots/16_process_investigation_task_manager.png

---

## Phase 4 – File System Analysis

The desktop and user directories were inspected.

Observed artifacts:

- .WNCRY encrypted files
- Ransom notes
- New ransomware files
- Modified desktop wallpaper

Screenshot:

screenshots/13_encrypted_user_files.png

---

## Phase 5 – Event Log Analysis

Windows Event Viewer was reviewed for evidence of system activity.

Logs reviewed:

- Application
- Security
- System

Objective:

- Identify abnormal events
- Correlate timestamps
- Support incident timeline

Screenshots:

- screenshots/17_security_event_logs.png
- screenshots/18_application_event_logs.png

---

## Phase 6 – Impact Assessment

Observed impact included:

- Loss of access to user files
- Encryption of documents
- Encryption of images
- Desktop modification
- User productivity disruption

No evidence of physical damage was observed.

---

## Phase 7 – Evidence Collection

Evidence collected during the investigation included:

- System Information
- IP Configuration
- Event Logs
- Desktop Artifacts
- Encrypted Files
- Task Manager
- Network Information

These artifacts were preserved for analysis and reporting.

# 🛡️ Wazuh SOC Home Lab

A hands-on Security Operations Center (SOC) home lab built to practice security monitoring, log analysis, alert investigation, and incident triage using **Wazuh SIEM**.

## 🎯 Project Objective

The goal of this lab is to simulate basic SOC analyst activities in a controlled environment, including:

- Endpoint monitoring
- Security event collection
- Authentication monitoring
- Alert investigation
- Event correlation
- Incident triage
- Security evidence documentation

## 🏗️ Lab Architecture

```text
                    ┌─────────────────────┐
                    │    Wazuh Manager    │
                    │    Ubuntu Server    │
                    │     192.168.44.131   │
                    └──────────┬──────────┘
                               │
                         VMware NAT
                               │
             ┌─────────────────┴─────────────────┐
             │                                   │
    ┌────────▼────────┐                ┌─────────▼────────┐
    │   Windows 11    │                │    Kali Linux    │
    │  Wazuh Agent    │                │ Security Testing │
    │   windows-11    │                │      Machine     │
    │    Agent 001    │                │                  │
    └─────────────────┘                └──────────────────┘
```
## 🔧 Technologies & Tools
Wazuh SIEM
Wazuh Agent
Windows 11
Ubuntu Server
Kali Linux
Windows Event Viewer
VMware

📂 Projects
1. Windows 4625 Authentication Failure Investigation

Investigated multiple failed Windows authentication attempts using Wazuh.

Detection:

Windows Security Event ID: 4625
Wazuh Rule ID: 60122
Rule Level: 5
Failed Attempts: 3
Logon Type: 2 - Interactive
Source Address: 127.0.0.1
Target User: Taif

The failed authentication attempts were followed by a successful login.

Verdict: Benign / Authorized Lab Activity

📁 Open Windows 4625 Investigation

📄 View Investigation Report

🚧 Upcoming Project

2. Linux SSH Brute-Force Detection

A Linux-based authentication monitoring lab will be added to demonstrate:

SSH failed login detection
Authentication log analysis
Repeated login attempt investigation
Wazuh alert generation
Basic brute-force investigation
SOC-style incident triage

Security Event
      ↓
Wazuh Agent
      ↓
Wazuh Manager
      ↓
Alert Generation
      ↓
Alert Triage
      ↓
Event Investigation
      ↓
Timeline Analysis
      ↓
Benign / Suspicious Assessment
      ↓
Incident Documentation


🧠 Skills Practiced

SIEM monitoring
Windows security event analysis
Authentication log investigation
Event ID analysis
Alert triage
Incident timeline creation
Basic MITRE ATT&CK context
Security documentation
SOC analyst investigation workflow

📸 Lab Evidence

Screenshots and investigation evidence are available inside the individual project directories.

⚠️ Disclaimer

This project was created in an authorized home lab environment for educational and cybersecurity training purposes.

No unauthorized systems or accounts were targeted.

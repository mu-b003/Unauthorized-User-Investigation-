# Unauthorized User Investigation

## Overview

This project documents a simulated Security Operations Center (SOC) investigation into unauthorized user creation and privilege escalation on a Linux system.

The investigation was performed in a personal cybersecurity lab using Ubuntu Server and Kali Linux running on VMware. It demonstrates how an attacker can gain administrative access, create a hidden backdoor account, and how these activities can be identified through log analysis.

---

## Objectives

- Install and configure SSH.
- Simulate an attacker gaining remote access.
- Create unauthorized user accounts.
- Escalate privileges using the sudo group.
- Investigate authentication and system logs.
- Build an incident timeline.
- Identify Indicators of Compromise (IOCs).
- Document the investigation process.

---

## Lab Environment

| Component | Description |
|----------|-------------|
| Host | VMware Workstation |
| Victim Machine | Ubuntu Server |
| Attacker Machine | Kali Linux |
| Investigation Type | Unauthorized User Investigation |
| Access Method | SSH |

---

## Attack Scenario

The simulation follows these stages:

1. SSH service installation.
2. Creation of the user **Omar**.
3. Granting Omar sudo privileges.
4. SSH login from Kali.
5. Creation of a hidden user named **door**.
6. Granting door sudo privileges.
7. Switching into the door account.
8. Creating a sample password file.
9. Closing the SSH session.
10. SOC investigation using Linux logs.

---

## Investigation Steps

The investigation included:

- Enumerating local users
- Checking group memberships
- Reviewing sudo assignments
- Searching journal logs
- Verifying account creation events
- Reviewing password changes
- Tracking session activity
- Building an attack timeline

---

## Indicators of Compromise (IOCs)

- Unauthorized account creation
- Hidden administrative account
- Multiple sudo privilege assignments
- Remote SSH login
- Suspicious user creation
- Password modifications
- Authentication log clearing
- Privilege escalation

---

## Key Findings

- Omar was granted administrative privileges.
- Omar logged in remotely through SSH.
- Omar created a hidden account named **door**.
- The door account received sudo privileges.
- Passwords were configured for the new account.
- Session logs confirmed successful account switching.
- Authentication logs had been cleared.
- The attack sequence was reconstructed using journal logs.

---

## Skills Demonstrated

- Linux Administration
- Incident Investigation
- Log Analysis
- SSH Investigation
- Privilege Escalation Detection
- User Account Investigation
- Digital Forensics
- SOC Analysis

---

## Repository Structure

```
Unauthorized-User-Investigation/
│
├── README.md
├── LICENSE
├── DISCLAIMER.md
├── reports/
├── evidence/
├── commands/
├── docs/
├── diagrams/
└── assets/
```

---

## MITRE ATT&CK Techniques

- Initial Access
- Valid Accounts
- Remote Services
- Account Manipulation
- Create Account
- Privilege Escalation
- Defense Evasion
- Indicator Removal

---

## Lessons Learned

- Monitor privileged account creation.
- Review sudo assignments regularly.
- Protect authentication logs.
- Audit SSH access.
- Investigate unexpected user accounts immediately.

---

## Educational Purpose

This project was created solely for cybersecurity education, SOC training, and defensive security research inside an isolated laboratory environment.

---

## Author

**Mubarak Bashr**

Cybersecurity Student | SOC Analyst (Learning) | Blue Team Enthusiast

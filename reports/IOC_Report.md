# Indicators of Compromise (IOC) Report

## Suspicious Accounts

| Account | Description |
|----------|-------------|
| Omar | Administrative account used during the attack |
| door | Unauthorized backdoor account |

---

## Privilege Escalation

- Omar added to sudo group.
- door added to sudo group.

---

## Suspicious Commands

- useradd
- usermod
- passwd
- su
- sudo

---

## Authentication Events

- Successful SSH login.
- Local account switching.
- Administrative command execution.

---

## Evidence Sources

- journalctl
- /etc/passwd
- id
- groups
- Authentication logs

---

## IOC Summary

The investigation confirmed unauthorized account creation, privilege escalation, and persistent administrative access.

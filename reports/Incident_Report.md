# Incident Report

## Incident Information

| Field | Value |
|------|------|
| Investigation | Unauthorized User Investigation |
| Platform | Ubuntu Server |
| Attacker | Kali Linux |
| Access Method | SSH |
| Investigation Type | Privilege Escalation |

---

# Executive Summary

A simulated attacker remotely accessed the victim machine using SSH, created a hidden administrative account, and attempted to establish persistence.

---

# Incident Timeline

1. SSH service installed.
2. Omar account created.
3. Omar granted sudo privileges.
4. SSH login.
5. door account created.
6. Password assigned.
7. door granted sudo privileges.
8. Session switched to door.
9. Investigation initiated.

---

# Evidence Collected

- User accounts
- Sudo assignments
- Password changes
- SSH sessions
- journalctl logs
- Authentication events

---

# Findings

- Unauthorized account creation confirmed.
- Privilege escalation confirmed.
- Administrative persistence established.
- Attack timeline reconstructed successfully.

---

# Root Cause

The Omar account received administrative privileges and was subsequently used to create an unauthorized privileged account.

---

# Recommendations

- Remove unauthorized accounts.
- Reset compromised credentials.
- Review sudo assignments.
- Monitor SSH activity.
- Enable centralized logging.

---

# Conclusion

The investigation successfully identified the attacker activities, reconstructed the attack timeline, and confirmed the presence of an unauthorized administrative backdoor.

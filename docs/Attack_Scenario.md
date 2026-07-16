# Attack Scenario

## Scenario Overview

An attacker obtained access to an existing privileged account and attempted to establish persistent administrative access.

---

## Attack Timeline

1. SSH service installed.
2. User **Omar** created.
3. Omar granted sudo privileges.
4. Remote SSH login from Kali Linux.
5. Hidden account **door** created.
6. Password assigned.
7. Sudo privileges granted.
8. Switched into the door account.
9. Created a sample password file.
10. Logged out.
11. SOC investigation began.

---

## Attacker Objectives

- Obtain persistent access.
- Create a hidden administrator account.
- Maintain remote access.
- Avoid detection.

---

## Expected Impact

- Unauthorized administrative access.
- Increased attack persistence.
- Security policy violation.

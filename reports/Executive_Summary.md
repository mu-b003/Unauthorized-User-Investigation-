# Executive Summary

## Overview

This investigation examined suspicious administrative activity on an Ubuntu Server following the creation of unauthorized user accounts and privilege escalation.

The incident was simulated within a controlled laboratory environment to demonstrate the investigation process performed by a Security Operations Center (SOC) analyst.

---

## Incident Summary

A legitimate administrator created a user account named **Omar** and granted it administrative privileges. Later, Omar remotely accessed the system via SSH and created another account named **door**, which was also granted sudo privileges.

System logs confirmed that the new account was used as a persistence mechanism and administrative backdoor.

---

## Key Findings

- Unauthorized administrative account created.
- SSH used for remote access.
- Privilege escalation confirmed.
- Password assigned to the backdoor account.
- Successful account switching using `su`.
- Authentication logs had been cleared.
- Journal logs successfully reconstructed the attack timeline.

---

## Impact

The attacker successfully established persistent administrative access to the system.

---

## Status

**Investigation Completed**

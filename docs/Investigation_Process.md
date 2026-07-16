# Investigation Process

## Objective

Identify how the unauthorized account was created and determine the extent of privilege escalation.

---

## Investigation Steps

### 1. User Enumeration

Verified all local accounts.

---

### 2. Privilege Verification

Checked sudo group membership.

---

### 3. Log Analysis

Reviewed journal logs for:

- useradd
- passwd
- usermod
- session activity

---

### 4. Timeline Reconstruction

Reconstructed the sequence of attacker actions.

---

### 5. Evidence Collection

Collected screenshots and command outputs.

---

## Tools Used

- journalctl
- grep
- id
- groups
- cat
- cut

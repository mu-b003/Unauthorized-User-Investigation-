# Investigation Commands

This file contains the commands used during the SOC investigation.

---

## List All Users

```bash
cut -d: -f1 /etc/passwd
```

Checks whether unauthorized users exist.

---

## Verify User Information

```bash
id door
```

Displays detailed information about the door account.

---

## Check User Groups

```bash
groups door
```

Verifies whether the account belongs to the sudo group.

---

## Search for User Creation Events

```bash
sudo journalctl | grep -Ei "useradd|adduser"
```

Finds account creation events.

---

## Search for Door Account Activity

```bash
sudo journalctl | grep "door"
```

Displays all log entries related to the door account.

---

## Search Password Changes

```bash
sudo journalctl | grep "passwd"
```

Identifies password modification events.

---

## Search Sudo Group Modifications

```bash
sudo journalctl | grep "usermod"
```

Shows when users were added to privileged groups.

---

## Search Executed Commands

```bash
sudo journalctl | grep "COMMAND="
```

Displays commands executed using sudo.

---

## Search Session Events

```bash
sudo journalctl | grep -E "su:|session opened|door"
```

Tracks account switching and login sessions.

---

## Final Verification

```bash
id door
```

Confirms that the suspicious account still exists and retains sudo privileges.

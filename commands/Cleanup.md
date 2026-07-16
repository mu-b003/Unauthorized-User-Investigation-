# Cleanup Commands

These commands can be used after completing the lab to restore the environment.

---

## Remove Backdoor Account

```bash
sudo userdel -r door
```

Deletes the door account and its home directory.

---

## Remove Omar from Sudo Group

```bash
sudo gpasswd -d Omar sudo
```

Revokes administrative privileges from Omar.

---

## Lock Omar Account

```bash
sudo passwd -l Omar
```

Locks the Omar account to prevent logins.

---

## Restart SSH Service

```bash
sudo systemctl restart ssh
```

Restarts the SSH service after cleanup.

---

## Verify User Removal

```bash
cut -d: -f1 /etc/passwd
```

Confirms that the door account has been removed.

---

## Verify Sudo Membership

```bash
groups Omar
```

Checks that Omar no longer belongs to the sudo group.

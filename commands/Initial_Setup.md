# Initial Setup

This file contains the commands used to prepare the victim machine before the investigation.

---

## Update Package Lists

```bash
sudo apt update
```

Updates the package index from the configured repositories.

---

## Install OpenSSH Server

```bash
sudo apt install openssh-server -y
```

Installs the OpenSSH server to allow remote SSH access.

---

## Restart SSH Service

```bash
sudo systemctl restart ssh
```

Restarts the SSH service after installation.

---

## Verify SSH Status

```bash
sudo systemctl status ssh
```

Confirms that the SSH service is active and listening on port 22.

---

## Create User

```bash
sudo adduser Omar
```

Creates a new local user named **Omar**.

---

## Verify Existing Users

```bash
cut -d: -f1 /etc/passwd
```

Lists all user accounts on the system.

---

## Grant Sudo Privileges

```bash
sudo usermod -aG sudo Omar
```

Adds Omar to the sudo group.

---

## Clear Authentication Log

```bash
sudo truncate -s 0 /var/log/auth.log
```

Empties the authentication log file.

---

## Check Victim IP Address

```bash
ip a
```

Displays the network interfaces and IP address.

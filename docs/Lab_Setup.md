# Lab Setup

## Overview

This investigation was conducted in a controlled virtual laboratory designed to simulate a real-world Security Operations Center (SOC) investigation.

---

## Environment

| Component | Description |
|----------|-------------|
| Virtualization | VMware Workstation |
| Victim Machine | Ubuntu Server |
| Attacker Machine | Kali Linux |
| Network | NAT |
| SSH Port | 22 |

---

## Software Used

- Ubuntu Server
- Kali Linux
- OpenSSH Server
- systemd-journald
- journalctl
- Linux Authentication Logs

---

## Network Information

### Victim

- Hostname: Ubuntu Server
- IP Address: 192.168.81.129

### Attacker

- Hostname: Kali Linux

---

## Investigation Goal

Simulate unauthorized account creation and privilege escalation, then investigate the attack using Linux system logs.

# Recommendations

## Immediate Actions

- Remove unauthorized accounts.
- Reset compromised passwords.
- Revoke unnecessary sudo privileges.

---

## Monitoring

- Monitor new user creation.
- Audit sudo membership regularly.
- Monitor SSH logins.
- Enable centralized logging.

---

## Hardening

- Disable password authentication for SSH.
- Use SSH keys.
- Enforce strong password policies.
- Enable Multi-Factor Authentication where possible.

---

## Detection

Create alerts for:

- useradd
- usermod
- passwd
- sudo privilege changes
- SSH logins

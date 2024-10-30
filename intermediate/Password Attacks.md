
### 3. `intermediate/Password Attacks.md`
```markdown
# Password Attacks

> **Overview**: Password attacks are attempts to crack or guess a user's password. This document discusses various techniques used in password attacks and ways to defend against them.

## Table of Contents
- [Brute Force Attack](#brute-force-attack)
- [Dictionary Attack](#dictionary-attack)
- [Rainbow Table Attack](#rainbow-table-attack)
- [Password Cracking Tools](#password-cracking-tools)
- [Best Practices for Password Security](#best-practices-for-password-security)
- [Resources](#resources)

---

### Brute Force Attack
A brute force attack tries every possible combination until the correct password is found. It is time-intensive and may be mitigated with account lockout mechanisms.

**Example**:
Using Hydra to brute-force SSH:
```bash
hydra -l <username> -P <password-list> ssh://<target-ip>

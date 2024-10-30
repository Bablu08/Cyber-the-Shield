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
```

### Dictionary Attack
A dictionary attack uses a list of common passwords or words, assuming the target's password is a common one.

**Example:** Using John the Ripper with a wordlist:
```bash
john --wordlist=<wordlist.txt> <hashfile>
```

### Rainbow Table Attack
Rainbow tables are precomputed tables for reversing cryptographic hash functions, primarily used to crack password hashes quickly.

- Prevention: Use salted hashes to prevent rainbow table attacks.

### Password Cracking Tools
- John the Ripper: Powerful password cracker for various hash types.
- Hydra: Fast and flexible network login cracker.
- Hashcat: Advanced GPU-accelerated password recovery tool.

### Best Practices for Password Security
- Use long, complex passwords.
- Enable multi-factor authentication (MFA).
- Avoid using the same password across multiple sites.

### Resources
- Password Cracking Tools by Kali Linux
- Cybersecurity Password Best Practices

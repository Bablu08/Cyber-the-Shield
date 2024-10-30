## Intermediate Topics

### 1. `intermediate/Web Vulnerabilities.md`
# Web Vulnerabilities

> **Overview**: A guide to common web vulnerabilities and how they are exploited.

## Table of Contents
- [SQL Injection](#sql-injection)
- [Cross-Site Scripting (XSS)](#cross-site-scripting-xss)
- [Cross-Site Request Forgery (CSRF)](#cross-site-request-forgery-csrf)
- [Resources](#resources)

---

### SQL Injection
A vulnerability allowing attackers to manipulate a database by injecting malicious SQL.

**Example**:
```sql
SELECT * FROM users WHERE username = 'admin' OR '1'='1';

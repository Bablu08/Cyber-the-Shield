# Web Vulnerabilities

> **Overview**: This document provides an overview of common web vulnerabilities, their impact, and how they are typically exploited. Understanding these vulnerabilities is crucial for identifying security flaws in web applications.

## Table of Contents
- [SQL Injection](#sql-injection)
- [Cross-Site Scripting (XSS)](#cross-site-scripting-xss)
- [Cross-Site Request Forgery (CSRF)](#cross-site-request-forgery-csrf)
- [Command Injection](#command-injection)
- [Insecure Direct Object References (IDOR)](#insecure-direct-object-references-idor)
- [Resources](#resources)

---

### SQL Injection
SQL Injection (SQLi) occurs when an attacker can execute arbitrary SQL commands on a database by injecting malicious input. This vulnerability can lead to unauthorized data access, data modification, or even deletion.

**Example**:
```sql
SELECT * FROM users WHERE username = 'admin' OR '1'='1';
```

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
- Impact: Unauthorized data access, data manipulation, and potential system compromise.
- Prevention: Use parameterized queries and prepared statements.

### Cross-Site Scripting (XSS)
XSS occurs when an attacker injects malicious scripts into a web page viewed by other users. This can be used to steal session cookies, capture user input, or redirect users to malicious sites.

**Example**:
```html
<script>alert('XSS');</script>
```
- Types: Stored XSS, Reflected XSS, DOM-based XSS.
- Prevention: Proper input sanitization and encoding of output.

###Cross-Site Request Forgery (CSRF)
CSRF tricks a user into performing actions they didn’t intend to, such as submitting a form or changing their account settings, by exploiting their authenticated session.

**Example**: A malicious link that performs a request:
```html
<a href="http://example.com/change-email?email=hacker@example.com">Click here</a>
```


### 2. `intermediate/Enumeration and Scanning.md`
```markdown
# Enumeration and Scanning

> **Overview**: Techniques for identifying and gathering information about network resources.

## Techniques
- **Port Scanning**: Using Nmap for open ports.
- **Service Enumeration**: Identifying services on open ports.
- **Banner Grabbing**: Gathering information about services.

**Example Nmap Commands**:
```bash
nmap -sS -p 22,80,443 192.168.1.1
nmap -A 192.168.1.1


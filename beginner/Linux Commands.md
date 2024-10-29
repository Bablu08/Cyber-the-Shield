# Linux Commands

> **Overview**: A guide to essential Linux commands for cybersecurity tasks.

## Table of Contents
- [Introduction to Linux](#introduction-to-linux)
- [Basic Commands](#basic-commands)
- [File Permissions](#file-permissions)
- [Network Commands](#network-commands)
- [Resources](#resources)

---

### Introduction to Linux
Linux is the preferred operating system in cybersecurity due to its flexibility and open-source nature. 

### Basic Commands
**1.File and Directory Management:**
- `ls`: Lists directory contents.
- `cd <directory>`: Changes directory.
- `pwd`: Prints current directory.
- `mkdir <directory>`: Create a new directory.
- `rmdir <directory>`: Remove an empty directory.
- `rm <file>`: Remove a file.
- `cp <source> <destination>`: Copy a file or directory.
- `mv <source> <destination>`: Move or rename a file or directory.
- `cat <file>`: Display the contents of a file.

**2.System Information:**
>Display system information.
```bash
uname -a
```
>Display running processes.
```bash
top
```
>Show disk space usage.
```bash
df -h
```

### File Permissions
Permissions determine who can access or modify files. Use `chmod` to change permissions:
- `chmod 755 filename`: Sets permissions to allow the owner to read/write/execute, others can only read/execute.

### Network Commands
- `ping <host>`: Tests connectivity to a host.
- `ifconfig` or `ip addr`: Shows IP configuration.
- `netstat`: Displays network connections and open ports.

### Resources
- [Linux Command Reference](https://linuxcommand.org/)

---



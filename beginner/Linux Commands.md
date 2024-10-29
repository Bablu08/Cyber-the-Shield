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

**2. System Information:**
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
>Show memory usage.
```bash
free -h
```
>Display the current logged-in user.
```bash
whoami
```

**3. Networking:**
>Display network interfaces 
```bash
ifconfig
```
>Show all network interfaces.
```bash
ip a
```
>Send ICMP echo requests to a host.
```bash
ping <host>
```
>Trace the route packets take to a network host.
```bash
traceroute <host>
```
>Show listening ports and network connections.
```bash
netstat -tuln
```

**4. Package Management:**
>Update package lists.
```bash
apt update
```
>Upgrade installed packages.
```bash
apt upgrade
```
>Install a new package.
```bash
apt install <package>
```
>Remove a package.
```bash
apt remove <package>
```

**5. Permissions:**
>Change file permissions.
```bash
chmod <permissions> <file>
```
>Change file ownership.
```bash
chown <user>:<group> <file>
```

**6. Text Processing:**
>Search for a pattern in a file.
```bash
grep <pattern> <file>
```
>Display text to the terminal.
```bash
echo <text>
```
>Open a file in the Nano text editor.
```bash
nano <file>
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



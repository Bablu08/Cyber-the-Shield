# Basic Scripting

> **Overview**: Scripting basics for automation in cybersecurity.

## Table of Contents
- [Introduction to Bash Scripting](#introduction-to-bash-scripting)
- [Creating Simple Scripts](#creating-simple-scripts)
- [Control Structures](#control-structures)
- [Example Scripts](#example-scripts)
- [Resources](#resources)

---

### Introduction to Bash Scripting
Bash scripting can automate repetitive tasks, making it valuable in cybersecurity.

### Creating Simple Scripts
>Create a file with `.sh` extension, like `script.sh`, and add:
```bash
echo "Hello, World!"
```
>2. Basic Backup Script:
```bash
tar -cvf backup_$(date +%F).tar /path/to/directory
echo "Backup completed!"
```
>3. Network Scanner Script:
```bash
echo "Scanning network..."
for ip in {1..254}; do
    ping -c 1 192.168.1.$ip | grep "64 bytes" &
done
wait
echo "Scan completed!"
```
>4. Directory Cleanup Script:
```bash
find /path/to/directory -type f -name "*.tmp" -delete
echo "Temporary files deleted!"
```
>5. System Update Script:
```bash
echo "Updating system..."
apt update && apt upgrade -y
echo "System updated!"
```

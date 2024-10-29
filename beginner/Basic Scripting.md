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
Create a file with `.sh` extension, like `script.sh`, and add:
```bash
#!/bin/bash
echo "Hello, World!"
```
Basic Backup Script:
```bash
#!/bin/bash
tar -cvf backup_$(date +%F).tar /path/to/directory
echo "Backup completed!"
```

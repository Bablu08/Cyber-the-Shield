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

if [ condition ]; then
    echo "Condition met"
fi

for i in {1..5}; do
    echo "Iteration $i"
done

for port in {1..1024}; do
    (echo > /dev/tcp/127.0.0.1/$port) 2>/dev/null && echo "Port $port is open"
done


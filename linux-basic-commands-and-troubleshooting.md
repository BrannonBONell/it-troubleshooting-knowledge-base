# Linux Basic Commands and Troubleshooting

# Introduction

Linux is widely used in:
- cloud infrastructure
- web servers
- DevOps
- cybersecurity
- AI infrastructure
- enterprise environments

Basic Linux troubleshooting and command-line familiarity are important skills for IT and cloud roles.

---

# Common Linux Distributions

Examples:
- Ubuntu
- Debian
- CentOS
- Rocky Linux
- Fedora
- Arch Linux

---

# Navigating the File System

# Show Current Directory

```bash
pwd
```

Displays the current working directory.

---

# List Files and Directories

```bash
ls
```

Useful options:

```bash
ls -la
```

Shows:
- hidden files
- permissions
- ownership
- timestamps

---

# Change Directory

```bash
cd /path/to/directory
```

Examples:

```bash
cd /home
cd ..
cd ~
```

---

# File Management

# Create File

```bash
touch filename.txt
```

---

# Create Directory

```bash
mkdir foldername
```

---

# Copy Files

```bash
cp source.txt destination.txt
```

---

# Move or Rename Files

```bash
mv oldname.txt newname.txt
```

---

# Delete File

```bash
rm filename.txt
```

---

# Delete Directory

```bash
rm -r foldername
```

Use caution with recursive deletion.

---

# Viewing File Contents

# Display File

```bash
cat filename.txt
```

---

# View Large Files

```bash
less filename.txt
```

Navigation:
- q = quit
- arrow keys = scroll

---

# View First Lines

```bash
head filename.txt
```

---

# View Last Lines

```bash
tail filename.txt
```

Useful for logs.

---

# User and Permission Basics

# View Current User

```bash
whoami
```

---

# File Permissions

```bash
ls -l
```

Example output:

```text
-rwxr-xr--
```

Permission types:
- r = read
- w = write
- x = execute

---

# Change Permissions

```bash
chmod 755 script.sh
```

---

# Change Ownership

```bash
sudo chown user:user filename.txt
```

---

# Sudo

```bash
sudo command
```

Allows administrative privileges.

---

# System Information

# Check Disk Space

```bash
df -h
```

---

# Check Memory Usage

```bash
free -h
```

---

# Check CPU Information

```bash
lscpu
```

---

# View Running Processes

```bash
top
```

Alternative:

```bash
htop
```

---

# Networking Commands

# Show IP Address

```bash
ip a
```

---

# Test Connectivity

```bash
ping google.com
```

---

# DNS Lookup

```bash
nslookup google.com
```

---

# View Open Ports

```bash
ss -tuln
```

---

# Package Management

# Ubuntu/Debian

Update packages:

```bash
sudo apt update
```

Upgrade packages:

```bash
sudo apt upgrade
```

Install package:

```bash
sudo apt install package-name
```

---

# CentOS/RHEL/Rocky

Install package:

```bash
sudo dnf install package-name
```

---

# Service Management

# Check Service Status

```bash
systemctl status service-name
```

Example:

```bash
systemctl status ssh
```

---

# Start Service

```bash
sudo systemctl start service-name
```

---

# Stop Service

```bash
sudo systemctl stop service-name
```

---

# Restart Service

```bash
sudo systemctl restart service-name
```

---

# Log Troubleshooting

# View System Logs

```bash
journalctl
```

---

# Follow Live Logs

```bash
journalctl -f
```

---

# View SSH Logs

```bash
journalctl -u ssh
```

---

# Common Troubleshooting Scenarios

# Scenario 1
Server cannot reach internet.

Possible causes:
- incorrect gateway
- DNS issue
- firewall issue
- interface down

Check:
- ip a
- ping
- DNS resolution

---

# Scenario 2
Disk space full.

Check:

```bash
df -h
```

Identify large directories:

```bash
du -sh /*
```

---

# Scenario 3
High CPU usage.

Check:

```bash
top
```

Identify:
- runaway processes
- memory leaks
- excessive services

---

# Scenario 4
SSH connection fails.

Check:
- ssh service status
- firewall rules
- network connectivity
- correct IP address

Useful commands:

```bash
systemctl status ssh
ss -tuln
```

---

# Important Linux Directories

# /home
User home directories.

# /etc
Configuration files.

# /var/log
System logs.

# /tmp
Temporary files.

# /bin
Essential binaries.

# /usr
User applications and utilities.

---

# Key Troubleshooting Mindset

1. Read error messages carefully
2. Check logs first
3. Verify network connectivity
4. Confirm services are running
5. Isolate one issue at a time
6. Document troubleshooting steps

---

# Beginner Linux Skills That Help IT Careers

- navigating directories
- editing configuration files
- restarting services
- reading logs
- managing packages
- basic networking commands
- permissions management

These skills are highly relevant for:
- help desk
- cloud support
- DevOps
- Linux administration
- AI infrastructure
- cybersecurity

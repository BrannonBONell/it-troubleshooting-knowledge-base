# Windows Command Line and System Tools

# Introduction

Windows command-line tools are commonly used in:
- IT support
- help desk
- networking
- system administration
- cloud support
- troubleshooting

Understanding these tools helps diagnose:
- network issues
- system failures
- performance problems
- connectivity issues

---

# Command Prompt vs PowerShell

# Command Prompt (CMD)
Traditional Windows command-line interface.

---

# PowerShell
More advanced scripting and automation environment.

Used heavily in:
- enterprise IT
- cloud administration
- Active Directory
- automation

---

# Opening Command Prompt

Press:

```text
Windows + R
```

Type:

```text
cmd
```

---

# Opening PowerShell

Press:

```text
Windows + X
```

Select:
- Windows PowerShell
OR
- Terminal

---

# Basic Navigation Commands

# Show Current Directory

```powershell
pwd
```

---

# List Files

```powershell
dir
```

---

# Change Directory

```powershell
cd foldername
```

---

# Go Back One Directory

```powershell
cd ..
```

---

# Networking Commands

# ipconfig

Displays network configuration.

```powershell
ipconfig
```

Useful for:
- checking IP address
- gateway
- DNS settings

---

# ipconfig /all

Detailed network information.

```powershell
ipconfig /all
```

---

# Release DHCP Address

```powershell
ipconfig /release
```

---

# Renew DHCP Address

```powershell
ipconfig /renew
```

---

# Flush DNS Cache

```powershell
ipconfig /flushdns
```

Useful for:
- DNS resolution problems
- website connectivity issues

---

# ping

Tests network connectivity.

```powershell
ping google.com
```

Useful for:
- connectivity testing
- latency checks
- troubleshooting

---

# tracert

Shows route traffic takes.

```powershell
tracert google.com
```

Useful for:
- routing issues
- latency troubleshooting

---

# nslookup

Tests DNS resolution.

```powershell
nslookup google.com
```

Useful for:
- DNS troubleshooting
- verifying DNS records

---

# System Information Commands

# systeminfo

Displays detailed system information.

```powershell
systeminfo
```

Useful for:
- OS version
- uptime
- memory
- patch levels

---

# tasklist

Displays running processes.

```powershell
tasklist
```

---

# taskkill

Terminates processes.

```powershell
taskkill /PID 1234 /F
```

---

# Disk Management Commands

# chkdsk

Checks disk integrity.

```powershell
chkdsk /f
```

Useful for:
- file system issues
- disk corruption

---

# sfc /scannow

Checks and repairs system files.

```powershell
sfc /scannow
```

Useful for:
- corrupted Windows files
- system instability

---

# DISM Repair

Repairs Windows image corruption.

```powershell
DISM /Online /Cleanup-Image /RestoreHealth
```

---

# User and Permission Commands

# whoami

Displays current logged-in user.

```powershell
whoami
```

---

# hostname

Displays computer name.

```powershell
hostname
```

---

# net user

Displays local user accounts.

```powershell
net user
```

---

# Event Viewer

# Opening Event Viewer

Press:

```text
Windows + X
```

Select:
- Event Viewer

---

# Common Logs

# System Logs
Hardware and driver issues.

---

# Application Logs
Software/application errors.

---

# Security Logs
Authentication and login events.

---

# Common Event IDs

# Event ID 41
Kernel-Power unexpected shutdown.

Common causes:
- PSU instability
- overheating
- crashes

---

# Event ID 6008
Unexpected shutdown.

---

# Resource Monitoring Tools

# Task Manager

Useful for:
- CPU usage
- memory usage
- startup applications

Shortcut:

```text
Ctrl + Shift + Esc
```

---

# Resource Monitor

Detailed performance monitoring.

Launch:

```powershell
resmon
```

---

# Performance Monitor

Launch:

```powershell
perfmon
```

Useful for:
- long-term performance analysis
- bottleneck detection

---

# Common Troubleshooting Scenarios

# Scenario 1
No internet access.

Check:
- ipconfig
- ping gateway
- DNS resolution

---

# Scenario 2
Slow computer.

Check:
- Task Manager
- startup applications
- disk usage
- memory usage

---

# Scenario 3
Frequent crashes.

Check:
- Event Viewer
- temperatures
- driver updates
- sfc /scannow

---

# Scenario 4
Website inaccessible.

Test:
- ping
- nslookup
- tracert

Determine:
- DNS issue
- routing issue
- server issue

---

# Important IT Troubleshooting Mindset

1. Gather information first
2. Read error messages carefully
3. Check logs
4. Isolate variables
5. Test step-by-step
6. Document findings

---

# Why These Skills Matter

Windows troubleshooting skills are valuable for:
- help desk
- technical support
- cloud support
- system administration
- MSP environments
- remote IT support

Basic command-line knowledge separates candidates from many entry-level applicants.

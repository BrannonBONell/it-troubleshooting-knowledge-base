# VPN and Remote Access Troubleshooting

# What is a VPN?

VPN stands for Virtual Private Network.

A VPN creates a secure encrypted connection between a user and a remote network.

VPNs are commonly used for:
- remote work
- secure access to company resources
- accessing internal applications
- secure communication

---

# Common VPN Types

# Remote Access VPN
Used by remote employees to connect to company networks.

---

# Site-to-Site VPN
Connects entire networks together.

Common in:
- branch offices
- enterprise environments

---

# Common VPN Applications

Examples:
- Cisco AnyConnect
- OpenVPN
- GlobalProtect
- WireGuard
- FortiClient

---

# Common VPN Problems

- cannot connect
- authentication failures
- slow connection
- disconnected sessions
- unable to access internal resources

---

# Initial Troubleshooting Process

# 1. Verify Internet Connectivity

Test:
```powershell
ping google.com
```

If internet does not work:
- VPN will not function properly.

---

# 2. Verify VPN Credentials

Check:
- username
- password
- MFA prompts

Common issues:
- expired passwords
- locked accounts
- incorrect MFA approval

---

# 3. Restart VPN Client

Close and reopen VPN application.

Simple restarts often resolve:
- stuck sessions
- authentication issues
- temporary software problems

---

# 4. Reboot System

Reboots can resolve:
- adapter issues
- DNS problems
- VPN service failures

---

# Common VPN Troubleshooting Commands

# ipconfig

```powershell
ipconfig /all
```

Verify:
- IP assignment
- DNS settings
- VPN adapter status

---

# ping

```powershell
ping internal-server-name
```

Tests:
- connectivity
- DNS resolution
- internal resource access

---

# nslookup

```powershell
nslookup internal-server
```

Useful for:
- DNS troubleshooting
- verifying internal DNS

---

# tracert

```powershell
tracert google.com
```

Useful for:
- routing problems
- latency analysis

---

# Common Troubleshooting Scenarios

# Scenario 1
VPN connects but internal websites fail.

Possible causes:
- DNS issue
- split tunneling configuration
- firewall restrictions

---

# Scenario 2
User cannot authenticate.

Possible causes:
- expired password
- MFA issue
- locked account

---

# Scenario 3
VPN disconnects frequently.

Possible causes:
- unstable internet
- Wi-Fi issues
- VPN server load
- ISP interruption

---

# Remote Desktop Basics

# What is RDP?

RDP = Remote Desktop Protocol

Allows remote access to Windows systems.

---

# Common RDP Problems

- incorrect credentials
- firewall blocking
- remote desktop disabled
- VPN connectivity issues

---

# Basic RDP Troubleshooting

1. Verify target computer online
2. Test ping connectivity
3. Verify VPN connection
4. Confirm Remote Desktop enabled
5. Check firewall rules

---

# Security Best Practices

- use MFA
- avoid public Wi-Fi when possible
- disconnect VPN when not needed
- use strong passwords
- keep VPN client updated

---

# Why VPN Knowledge Matters

VPN troubleshooting skills are valuable for:
- remote IT support
- help desk
- cloud support
- system administration
- cybersecurity

Remote connectivity support is extremely common in modern IT environments.

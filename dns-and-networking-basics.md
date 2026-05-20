# DNS and Networking Basics

# What is DNS?

DNS stands for Domain Name System.

DNS translates human-readable domain names into IP addresses.

Example:

google.com → 142.250.x.x

Without DNS, users would need to memorize IP addresses for websites and services.

---

# Basic Network Flow

When a user visits a website:

1. Device checks local DNS cache
2. Request goes to configured DNS server
3. DNS server finds IP address
4. Browser connects to destination server
5. Website loads

---

# Common Networking Devices

# Router
A router connects different networks together.

Common functions:
- Internet access
- NAT
- DHCP
- Traffic routing

Home example:
- Connects local home network to ISP

---

# Switch
A switch connects devices within the same local network.

Examples:
- PCs
- printers
- servers
- access points

Switches use MAC addresses to forward traffic efficiently.

---

# Modem
A modem connects the local network to the ISP connection.

Examples:
- cable modem
- fiber ONT
- DSL modem

---

# Access Point
Provides wireless network connectivity.

Common examples:
- Wi-Fi routers
- enterprise wireless APs

---

# DHCP

DHCP stands for Dynamic Host Configuration Protocol.

DHCP automatically assigns:
- IP address
- subnet mask
- gateway
- DNS server

Without DHCP:
devices would require manual IP configuration.

---

# Public vs Private IP Addresses

# Private IP Examples
- 192.168.x.x
- 10.x.x.x
- 172.16.x.x - 172.31.x.x

Used inside local networks.

---

# Public IP
Public IP addresses are internet-routable addresses assigned by ISPs.

---

# Common Networking Commands

# ipconfig

Displays network configuration.

```powershell
ipconfig
```

Useful for:
- checking IP address
- checking gateway
- checking DNS server

---

# ipconfig /all

Displays detailed adapter information.

```powershell
ipconfig /all
```

---

# ping

Tests network connectivity.

```powershell
ping google.com
```

Useful for:
- connectivity testing
- latency testing
- DNS troubleshooting

---

# tracert

Shows path traffic takes to destination.

```powershell
tracert google.com
```

Useful for:
- identifying routing problems
- diagnosing latency issues

---

# nslookup

Queries DNS information.

```powershell
nslookup google.com
```

Useful for:
- verifying DNS resolution
- troubleshooting DNS issues

---

# Common Network Troubleshooting Steps

# 1. Check Physical Connections
Verify:
- Ethernet cable connected
- Link lights active
- Modem/router powered on

---

# 2. Verify IP Address

Use:

```powershell
ipconfig
```

Common issue:
- APIPA address (169.254.x.x)

This often indicates DHCP failure.

---

# 3. Test Connectivity

Test:
- localhost
- gateway
- public IP
- domain name

Example:

```powershell
ping 8.8.8.8
ping google.com
```

If IP works but domain fails:
- likely DNS issue

---

# 4. Restart Networking Equipment

Power cycle:
- modem
- router
- switch

This resolves many temporary issues.

---

# 5. Flush DNS Cache

```powershell
ipconfig /flushdns
```

Useful when:
- websites fail to resolve
- DNS records changed

---

# Common IT Support Scenarios

# Scenario 1
User cannot access websites.

Possible causes:
- DNS failure
- ISP outage
- gateway issue
- firewall issue

---

# Scenario 2
User has Wi-Fi but no internet.

Possible causes:
- router WAN issue
- ISP outage
- DNS problem

---

# Scenario 3
Slow network connection.

Possible causes:
- bandwidth saturation
- faulty cable
- high latency
- driver issue

---

# Key Networking Concepts

# NAT
Network Address Translation allows many devices to share one public IP.

---

# Gateway
The gateway is the device traffic uses to leave the local network.

Usually:
- router IP

---

# MAC Address
A unique hardware identifier assigned to network adapters.

---

# Subnet Mask
Determines which portion of an IP address belongs to the local network.

---

# Basic Troubleshooting Mindset

Always troubleshoot in layers:

1. Physical
2. IP configuration
3. Gateway
4. DNS
5. Internet connectivity
6. Application layer

Do not assume the internet is the issue before testing local connectivity first.

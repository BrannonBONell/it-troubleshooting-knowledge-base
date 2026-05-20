# Active Directory Basics and Troubleshooting

# What is Active Directory?

Active Directory (AD) is Microsoft's directory service used to manage:
- users
- computers
- groups
- permissions
- policies
- authentication

Active Directory is commonly used in:
- corporate environments
- enterprise networks
- schools
- healthcare organizations
- government systems

---

# Core Active Directory Concepts

# Domain

A domain is a centralized network environment that manages users and devices.

Example:

company.local

---

# Domain Controller (DC)

A Domain Controller is a server running Active Directory services.

Responsibilities:
- authentication
- authorization
- user management
- policy enforcement

---

# Organizational Unit (OU)

Containers used to organize:
- users
- computers
- departments

Example:
- HR
- IT
- Finance

---

# Users

User accounts allow employees to:
- log in
- access resources
- use email
- access applications

---

# Groups

Groups simplify permission management.

Examples:
- Help Desk
- Accounting
- Domain Admins

---

# Group Policy (GPO)

Used to apply rules and settings across systems.

Examples:
- password policies
- desktop restrictions
- software deployment
- security settings

---

# Common Active Directory Tasks

# Unlock User Account

Common issue:
User enters incorrect password too many times.

Typical solution:
- unlock account
- reset password if necessary

---

# Reset User Password

Help desk responsibility in many environments.

Best practices:
- verify user identity
- require password change after login

---

# Add User to Group

Used to grant access to:
- shared folders
- applications
- printers
- permissions

---

# Disable User Account

Typically done when:
- employee leaves company
- security concern exists

---

# Common Help Desk Scenarios

# Scenario 1
User cannot log in.

Possible causes:
- incorrect password
- locked account
- expired password
- disconnected from domain

Troubleshooting:
1. Verify username
2. Check caps lock
3. Confirm network connectivity
4. Check AD account status
5. Reset password if needed

---

# Scenario 2
User cannot access shared drive.

Possible causes:
- missing permissions
- incorrect group membership
- network issue

Troubleshooting:
1. Verify network access
2. Check group membership
3. Confirm share permissions
4. Test with another user

---

# Scenario 3
Computer cannot join domain.

Possible causes:
- DNS issue
- incorrect credentials
- connectivity problem
- duplicate hostname

Troubleshooting:
1. Verify DNS settings
2. Ping domain controller
3. Check firewall
4. Confirm credentials

---

# DNS and Active Directory

DNS is critical for Active Directory functionality.

Common symptoms of DNS problems:
- login failures
- domain join failures
- authentication errors

Useful checks:

```powershell
ipconfig /all
nslookup domain.local
ping domaincontroller
```

---

# Basic PowerShell Commands

# View Current User

```powershell
whoami
```

---

# Check Computer Name

```powershell
hostname
```

---

# Network Configuration

```powershell
ipconfig /all
```

---

# Test Connectivity

```powershell
ping domaincontroller
```

---

# Common Active Directory Tools

# Active Directory Users and Computers (ADUC)

Used to:
- manage users
- manage groups
- reset passwords
- unlock accounts

---

# Group Policy Management

Used to:
- configure GPOs
- apply security policies
- manage system configurations

---

# Event Viewer

Useful for:
- authentication troubleshooting
- login failures
- security auditing

---

# Active Directory Security Best Practices

# Least Privilege
Users should only have access necessary for their role.

---

# Multi-Factor Authentication
Improves account security.

---

# Disable Unused Accounts
Reduces security risk.

---

# Strong Password Policies
Encourage:
- password complexity
- expiration policies
- lockout policies

---

# Basic Home Lab Ideas

# Beginner Lab
- Windows Server VM
- Windows 10/11 VM
- Create domain
- Add users/computers

---

# Skills to Practice
- password resets
- account unlocks
- group management
- domain joins
- DNS troubleshooting

---

# Why Active Directory Matters

Active Directory knowledge is valuable for:
- help desk
- IT support
- cloud support
- system administration
- cybersecurity
- enterprise IT

Many entry-level IT jobs expect basic familiarity with:
- user accounts
- permissions
- password resets
- domain environments

---

# Key Troubleshooting Mindset

1. Verify connectivity first
2. Check DNS configuration
3. Confirm account status
4. Verify permissions/groups
5. Review logs and error messages
6. Test one variable at a time

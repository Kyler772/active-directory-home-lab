# Active Directory Home Lab
![Windows Server](https://img.shields.io/badge/Windows_Server-2022-blue)
![Active Directory](https://img.shields.io/badge/Active_Directory-AD_DS-blue)
![VirtualBox](https://img.shields.io/badge/VirtualBox-Lab-orange)
![Jira](https://img.shields.io/badge/Jira-Service_Management-blue)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

## Overview

This project demonstrates the deployment and administration of a Windows Active Directory environment using Windows Server 2022 and VirtualBox. The lab simulates a small enterprise network where a Domain Controller manages authentication, user accounts, security groups, shared resources, and common Help Desk requests.

To further simulate a real-world IT environment, support requests were documented and resolved using Jira Service Management, following a structured ticket lifecycle from incident creation through resolution and verification.

---

## Project Objectives

- Deploy a Windows Server 2022 Domain Controller
- Configure Active Directory Domain Services (AD DS)
- Configure DNS for centralized name resolution
- Join a Windows 10 client to the domain
- Create and manage Active Directory users and security groups
- Configure shared folders and NTFS permissions
- Simulate common Help Desk support requests
- Document troubleshooting and resolutions using Jira Service Management

---

## Technologies Used

- Windows Server 2022
- Windows 10 Pro
- Oracle VirtualBox
- Active Directory Domain Services (AD DS)
- DNS
- Group Policy
- NTFS Permissions
- SMB File Sharing
- Jira Service Management

---

## Lab Architecture

```
                     VirtualBox
                         │
                Internal Network (AD-Lab)
                   ┌───────────────┐
                   │               │
               DC01             CLIENT01
        Windows Server      Windows 10 Pro
         Active Directory      Domain Joined
               DNS
```

---

## Environment Configuration

### Domain Controller

| Setting | Value |
|----------|-------|
| Hostname | DC01 |
| Operating System | Windows Server 2022 |
| Domain | lab.local |
| IP Address | 192.168.10.10 |
| DNS | 192.168.10.10 |

### Client Workstation

| Setting | Value |
|----------|-------|
| Hostname | CLIENT01 |
| Operating System | Windows 10 Pro |
| IP Address | 192.168.10.20 |
| DNS | 192.168.10.10 |
| Domain | lab.local |

---

# Active Directory Configuration

The following Active Directory components were configured:

- Active Directory Domain Services
- DNS
- Organizational Units (OUs)
- Domain Users
- Security Groups
- Shared Folder Permissions

Example users created:

- John Doe
- Jane Smith
- Emily Carter

Example security groups:

- IT
- HR

---

# Simulated Help Desk Tickets

## Ticket 1 — Password Reset

### Scenario

User was unable to log in after forgetting their password.

### Resolution

- Verified user account
- Reset password in Active Directory
- Required password change at next logon
- Verified successful authentication

**Skills Demonstrated**

- Active Directory User Management
- Identity Administration
- Help Desk Documentation

---

## Ticket 2 — Account Lockout

### Scenario

User account became locked after multiple failed login attempts.

### Resolution

- Confirmed account lockout
- Unlocked account
- Verified successful login

**Skills Demonstrated**

- Account Security
- User Authentication
- Active Directory Administration

---

## Ticket 3 — Shared Folder Access

### Scenario

User reported "Access Denied" when attempting to access the Finance shared folder.

### Resolution

- Reviewed NTFS permissions
- Reviewed Share permissions
- Updated security group membership
- Verified user access

**Skills Demonstrated**

- NTFS Permissions
- Share Permissions
- Security Groups
- Access Control

---

## Ticket 4 — New Employee Onboarding

### Scenario

HR requested creation of a new Active Directory account for a new employee.

### Resolution

- Created user account
- Assigned Organizational Unit
- Added security group memberships
- Configured temporary password
- Verified successful login
- Verified shared folder access

**Skills Demonstrated**

- User Provisioning
- Group Membership Management
- Active Directory Administration

---

## Ticket 5 — DNS Troubleshooting

### Scenario

A workstation was unable to communicate with Active Directory due to incorrect DNS configuration.

### Resolution

- Verified IP configuration
- Diagnosed DNS misconfiguration
- Updated Preferred DNS Server
- Verified successful communication with the domain

**Skills Demonstrated**

- Windows Networking
- DNS
- Active Directory Troubleshooting
- Root Cause Analysis

---

# Skills Demonstrated

- Windows Server Administration
- Active Directory
- DNS Configuration
- Domain Administration
- User Lifecycle Management
- Security Groups
- NTFS Permissions
- SMB File Sharing
- Windows Authentication
- Group Policy
- Help Desk Troubleshooting
- Jira Service Management
- Technical Documentation

---

# Lessons Learned

This project reinforced several core concepts used in enterprise Windows environments:

- DNS is critical for Active Directory functionality.
- Security groups simplify permission management.
- Proper NTFS and Share permissions are required to secure shared resources.
- Effective documentation is an essential part of IT support.
- Structured troubleshooting reduces resolution time and improves consistency.

---

# Future Improvements

Future enhancements planned for this lab include:

- Group Policy deployment
- Folder Redirection
- DHCP Server
- Print Server
- WSUS
- PowerShell automation
- Microsoft Entra ID (Azure AD)
- Microsoft 365 administration

---

# Screenshots

Screenshots documenting each phase of the project are available in the `/screenshots` directory.

---

# Documentation

Detailed project documentation, ticket write-ups, and supporting materials are available in the `/docs` directory.

---

# Author

Kyler Watson

UAH Computer Science Graduate 

Aspiring IT Support / Systems Administrator

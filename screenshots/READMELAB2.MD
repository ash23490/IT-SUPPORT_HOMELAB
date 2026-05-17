# Lab 2 - IT Support Operations & Troubleshooting

## Overview

This lab simulated real-world IT support and helpdesk operations within a Windows Active Directory environment using virtualized Windows Server and Windows 10 systems.

The lab focused on troubleshooting, centralized administration, Active Directory management, file sharing, Group Policy configuration, and remote support workflows commonly performed by IT Support Technicians and Junior System Administrators.

---

# Environment

- VirtualBox
- Windows Server 2019
- Windows 10 Client
- Active Directory Domain Services (AD DS)
- DNS
- Group Policy Management Console (GPMC)
- PowerShell
- Remote Desktop (RDP)

---

# Core Tasks Completed

## Active Directory User Administration
- Created and managed domain users and security groups
- Reset passwords and unlocked accounts
- Diagnosed disabled account issues
- Verified and managed group memberships

---

## Shared Folder & Permissions
- Configured shared network folders
- Implemented NTFS and Share permissions
- Created role-based access using Active Directory security groups
- Tested shared resource accessibility from domain-joined clients

---

## Network Drive Mapping
- Mapped shared network drives manually
- Verified persistent mapped drive connectivity
- Simulated enterprise shared resource workflows

---

## Group Policy Management
- Configured Account Lockout Policies
- Applied centralized domain policies using GPMC
- Explored enterprise Group Policy deployment concepts
- Practiced Group Policy updates and policy refresh procedures

---

## Remote Desktop & Remote Administration
- Configured Remote Desktop access
- Diagnosed RDP authentication and trust relationship issues
- Explored centralized RDP management using Group Policy concepts
- Practiced remote workstation administration

---

## Authentication & Trust Troubleshooting
- Diagnosed secure channel trust failures
- Repaired domain trust relationships using PowerShell
- Verified authentication using domain credentials
- Troubleshot stale security token and permission propagation issues

---

# Troubleshooting Scenarios

## Scenario 1 - Domain Authentication Failure
Symptoms:
- Users unable to authenticate
- Secure channel verification failures
- Trust relationship errors

Resolution:
- Verified DNS functionality
- Tested secure channel communication
- Repaired workstation trust using:

```powershell
Test-ComputerSecureChannel -Repair

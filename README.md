# Active Directory Homelab

## Overview
This project documents a cloud-hosted Active Directory homelab built in Microsoft Azure using Windows Server 2025 and Windows 11 virtual machines.

The lab was created to practice enterprise IT administration, troubleshooting, networking, Group Policy, and PowerShell automation in a realistic Windows domain environment.

---

## Technologies Used

- Windows Server 2025
- Windows 11
- Microsoft Azure
- Active Directory Domain Services (AD DS)
- DNS
- Group Policy (GPO)
- PowerShell
- SMB File Sharing
- NTFS Permissions
- Virtual Networking

---

## Lab Architecture

### Domain Controller
- Windows Server 2025 VM
- Configured as Domain Controller
- DNS Server installed
- Active Directory configured

### Client Machine
- Windows 11 VM
- Joined to Active Directory domain
- Used for user authentication and testing

---

## Skills Demonstrated

- Active Directory user and group management
- Domain joining Windows clients
- DNS configuration and troubleshooting
- Group Policy configuration
- Network drive mapping
- NTFS and Share permissions
- Password resets and account unlocks
- PowerShell administration
- Help desk troubleshooting workflows

---

## Key Configurations

### Active Directory
- Created Organizational Units (OUs)
- Created domain users and security groups
- Assigned group-based permissions

### File Shares
Configured shared department folders:
- HR
- Finance
- IT

Implemented:
- Share permissions
- NTFS permissions
- Group-based access control

### Group Policy
Configured:
- Automatic network drive mapping
- User-based access policies

### DNS Troubleshooting
Resolved hostname resolution issues using:
- nslookup
- ipconfig /flushdns
- DNS record verification

---

## PowerShell Examples

### Unlock AD Account
```powershell
Unlock-ADAccount -Identity jsmith
```

### Add User to Group
```powershell
Add-ADGroupMember -Identity HR_Users -Members jsmith
```

### Force Group Policy Update
```powershell
gpupdate /force
```

## Troubleshooting Scenarios

- User unable to access shared drive
- DNS resolution failures
- GPO drive mapping issues
- Account lockouts
- Incorrect NTFS permissions
- Domain join troubleshooting

---

## Screenshots

(Add screenshots here)

Examples:
- Active Directory Users and Computers
- GPO Drive Mapping
- Shared Folder Permissions
- PowerShell Commands
- Mapped Network Drives

---

## Lessons Learned

This lab improved my understanding of:
- Enterprise Windows environments
- Identity and access management
- Group-based permissions
- Windows troubleshooting
- Active Directory administration
- PowerShell automation

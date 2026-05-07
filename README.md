# IT-SUPPORT_HOMELAB
# IT Support &amp; Active Directory Home Lab
Built a virtualized Windows Server Active Directory environment using ORACLE VirtualBox to replicate a real-world IT support and system administration tasks.

The lab includes:
- Domain Controller setup
- DNS configuration
- Active Directory user management
- Domain-joined Windows 10 client
- Helpdesk troubleshooting simulations
- Secure channel and authentication troubleshooting

  ## Technologies Used

- VirtualBox
- Windows Server 2019
- Windows 10
- Active Directory Domain Services (AD DS)
- DNS
- PowerShell
- Command Prompt

## Lab 1 - Active Directory Infrastructure
- Installed and configured Windows Server 2019
- Promoted server to Domain Controller
- Created company.local domain
- Configured DNS services
- Created organizational units and domain users
- Joined Windows 10 client machine to domain

- ## Lab 2 - IT Support & Troubleshooting
- Simulated real-world IT support scenarios including:

- Domain login failures
- DNS troubleshooting
- Secure channel repair
- User authentication troubleshooting
- Active Directory password resets
- Domain trust verification

- ## Troubleshooting Experience
- During the lab, I encountered several authentication and domain communication issues.

Key troubleshooting steps included:
- Diagnosing DNS resolution issues
- Verifying Active Directory DNS zones
- Repairing broken domain trust relationships using PowerShell
- Testing secure channel communication
- Identifying incorrect user logon names causing authentication failures
This process really taught me that sometimes the smallest issues are the ones that make the system fail, i figured that the secure channel was broken which i fixed through a command in powershell (Test-ComputerSecureChannel -Repair -Credential company\administrator), still the problem remained username or password incorrect. it was after that i figured out i was writing asher which of course was my username but the login username was set to ash. the way i figured out is i logged on the client virtual machine as administrator and ran a command in powershell to directly reset the password of the username asher. the powershell returned that no such user exists so i found my root cause of the problem

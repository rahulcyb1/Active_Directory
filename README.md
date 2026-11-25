# Active Directory Administration & Group Policy Lab

A hands-on Windows Active Directory lab focused on user and group management, account security, Group Policy administration, shared-folder permissions and network drive mapping.

## Project Overview

- **Domain:** `soc.lab`
- **Domain Controller / File Server:** `SOC-AD`
- **Environment:** Windows Server and Windows client (WIN 11)

## Objectives

- Manage domain users, Organizational Units (OUs) and security groups.
- Configure password and account lockout policies.
- Perform password resets and account unlocks.
- Apply Group Policy Objects (GPOs) using security filtering.
- Restrict Command Prompt access for targeted users.
- Configure SMB shared folders with NTFS permissions.
- Monitor account-lockout events using Splunk.
- Deploy and verify network drive mapping through Group Policy Preferences.

## Repository Structure

```text
Active-Directory-Lab/
│
├── Account-Password administration/
│   ├── #1 Password & Account lockout policy.png
│   ├── #2 Account Unlock.png
│   ├── #3 Detecting Account Lockout using Splunk.png
│   ├── #4 Password Reset.png
│   └── README.md
│
├── Group Policy Objects (GPO)/
│   ├── #1 GPO Configuration.png
│   ├── #2 Apply GPO to target specific group.png
│   ├── #3 Assigning required permission for the target group.png
│   ├── #4 Forcing the GPO enforcement.png
│   ├── #5 Verifying the GPO enforcement.png
│   ├── #6 Drive mapping to group user.png
│   ├── #7 Verifying drive mapping.png
│   └── README.md
│
├── Shared Folder Configuration/
│   ├── #1 Shared_folder_provision.png
│   ├── #2 Shared_folder_permission.png
│   ├── #3 Verifying shared folder access.png
│   └── README.md
│
├── User-Group management/
│   ├── README.md
│   ├── logon time restriction.png
│   └── user-group creation and addition.png
│
└── README.md
```

## Project Implementation

### 1. User & Group Management

- Created domain users and department-based security groups.
- Organized accounts using Organizational Units.
- Assigned users to appropriate security groups.
- Configured user logon-hour restrictions.

[View User & Group Management](./User-Group%20management/README.md)

### 2. Account & Password Administration

- Configured domain password and account lockout policies.
- Performed password resets and account unlocks.
- Investigated account-lockout activity using Windows Security events and Splunk.

[View Account & Password Administration](./Account-Password%20administration/README.md)

### 3. Group Policy Objects (GPO)

- Created and linked Group Policy Objects.
- Configured security filtering for the IT department group.
- Restricted Command Prompt access.
- Applied and verified policies using `gpupdate /force`.
- Configured network drive mapping through Group Policy Preferences.

**Verified:** The IT shared folder was successfully mapped as drive `Z:` and accessed through File Explorer.

[View GPO Configuration](./Group%20Policy%20Objects%20\(GPO\)/README.md)

### 4. Shared Folder Configuration

- Created an SMB shared folder on the domain server.
- Configured group-based NTFS permissions.
- Tested access using assigned and non-assigned group accounts.

**Network Share:** `\\SOC-AD\shared`

[View Shared Folder Configuration](./Shared%20Folder%20Configuration/README.md)

## Skills Demonstrated

- Active Directory Domain Services (AD DS)
- Organizational Unit and user administration
- Security group management
- Password and account lockout policies
- Group Policy Objects and security filtering
- Group Policy Preferences
- SMB and NTFS permissions
- Network drive mapping
- Windows Security event analysis
- Splunk event monitoring

## Project Outcome

Implemented and tested core Active Directory administration and Windows security controls in a lab environment, demonstrating account management, policy enforcement, group-based resource access, security-event monitoring, and successful network drive mapping.

**Purpose:** Hands-on learning and demonstration of foundational Windows infrastructure and cybersecurity administration.


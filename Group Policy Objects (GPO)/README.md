# Group Policy Objects (GPO)

## Overview
Configured Group Policy Objects (GPOs) to manage user settings and automate network drive mapping in the Active Directory environment.

## Project Evidence

### 1. GPO Configuration
- Screenshot: `#1 GPO Configuration.png`
- Created and configured Group Policy setting to block command prompt access.

### 2. Apply GPO to a Specific Group
- Screenshot: `#2 Apply GPO to target specific group.png`
- Used security filtering to target the intended user group.

### 3. Assign Required Permissions
- Screenshot: `#3 Assigning required permission for the target group.png`
- Configured the permissions required for the target group to read and apply the GPO.

### 4. Force GPO Update
- Screenshot: `#4 Forcing the GPO enforcement.png`
- Triggered a Group Policy update to apply the configured settings.

### 5. Verify GPO Application
- Screenshot: `#5 Verifying the GPO enforcement.png`
- Checked whether the configured policy was successfully applied.

### 6. Configure Network Drive Mapping
- Screenshot: `#6 Drive mapping to group user.png`
- Configured a network drive mapping for the intended group of users.

### 7. Verify Network Drive Mapping
- Screenshot: `#7 Verifying drive mapping.png`
- Verified successful mapping of the IT shared folder as **Z:** in File Explorer.

## Result
- Configured and targeted GPOs using security filtering.
- Verified policy application.
- Successfully mapped and accessed the IT shared folder through the **Z:** network drive.

# Windows Environment

## Overview
WAGO SCADA provides installation packages for the 64-bit Windows operating system.

### Recommended Systems for Installation:
- Windows Server 2012 R2
- Windows Server 2016
- Windows Server 2019
- Windows Server 2022
- Windows 10 *(Not supported in Home Edition)*
- Windows 11 *(Not supported in Home Edition)*

---

## Installation Steps:
1. Run the installation package program as an administrator.
2. Select the installation language.
3. Perform a port check. If the port is occupied, the installation cannot proceed.
4. Read and accept the license agreement.
5. Choose the installation location; the default path is:  
   `C:\Program Files\WAGO SCADA`
6. Select the WAGO SCADA application data directory.
7. Prepare for installation.
8. Complete the installation.
9. After completion, the default access to the WAGO SCADA site is:  
   `http://localhost:8066`.  
   After installation, you will enter the configuration wizard interface.

---

## Configuration Steps:
1. **Create an administrator user**:  
   Remember the username and password, as you will use them to log in for the first time.
2. **Port configuration**:  
   Configure HTTP and HTTPS ports, and remember the access port.
3. After completing the above steps, wait for the program to load, and then log in to the default-created workspace using the user created in Step 1.

> **Note**: After each installation, a new empty workspace will be created by default. To return to the original workspace, you must log in to the new workspace first and manually open the original workspace from the workspace list.

---

## Security Configuration (Optional)
To enhance system security, it is recommended to set permissions on the service directory and application data directory, allowing only specific users to access or modify them. This ensures sensitive data is well-protected and minimizes potential risks.

### Steps for Security Configuration:

1. **Create a dedicated service account**:  
   - Create a dedicated account in Windows local users and groups (e.g., `WagoScadaSvc`).

2. **Set service installation directory permissions**
   - Navigate to the service installation directory (e.g., `C:\Program Files\WAGO SCADA`).
   - Right-click and select: `Properties → Security`.  
   - Based on the actual security requirements:  
     - Retain necessary users or groups, and delete unnecessary ones *(e.g., `Users`, `Everyone`)*.
     - Add the `WagoScadaSvc` user and grant **Read, Write, and Modify** permissions.
     - Ensure the changes are applied to all subfolders and files.

     > **Note**: This step must be completed before changing the service logon account; otherwise, the service may fail to start or restart.

3. **Modify the service logon account**:
   - Open `Services` (`services.msc`), locate the WAGO SCADA service.
   - Right-click the service → `Properties` → `Log On` → select "This account".
   - Enter `. \WagoScadaSvc` and the password.  
   - Save and restart the service.

4. **Set application data directory permissions**:
   - Navigate to the application data directory chosen during installation *(e.g., `C:\ProgramData\WAGOSCADA`)*.
   - Right-click and select: `Properties → Security`.
   - Based on actual security requirements:  
     - Retain necessary users or groups and delete unnecessary ones *(e.g., `Users`, `Everyone`)*.
     - Add the `WagoScadaSvc` user and grant **Read, Write, and Modify** permissions.
     - Ensure the changes are applied to all subfolders and files.

5. **Verify configuration**:
   - Access the WAGO SCADA site *(e.g., `http://localhost:8066`)* and confirm that the site is running normally.

---

## Uninstallation Steps:
1. Open the software uninstall list from the Control Panel.  
   Locate WAGO SCADA and proceed with the uninstallation.
2. Confirm the uninstallation to complete the removal of the application.

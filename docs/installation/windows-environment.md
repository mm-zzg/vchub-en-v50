<img width="67" height="20" alt="image" src="https://github.com/user-attachments/assets/1f9c7a8f-dbd0-4404-a345-8aadeb1b4e82" /># Windows Environment

VC Hub provides installation packages for the 64-bit Windows operating system.

Recommended Systems for Installation:

- Windows Server 2012 R2
- Windows Server 2016
- Windows Server 2019
- Windows Server 2022
- Windows 10  (Not supported in Home Edition)
- Windows 11  (Not supported in Home Edition)

#### **Installation Steps:**

1. Run the installation package program as an administrator.
2. Select the installation language.

<img width="372" height="179" alt="image" src="https://github.com/user-attachments/assets/dba75d4c-342f-4dbb-a1af-23b34ac46509" />


3. Perform a port check, if the port is occupied, the installation cannot proceed. 

<img width="601" height="465" alt="image" src="https://github.com/user-attachments/assets/94a6df97-6d65-4520-8886-83bb8de76ae5" />


4. Read and accept the license agreement.

<img width="599" height="467" alt="image" src="https://github.com/user-attachments/assets/fa502ccd-9bb1-4931-a3ff-5e3234fb5c9b" />

5. Choose the installation location; the default path is: "C:\Program Files\WAGO Visualization And Control Hub".

<img width="598" height="465" alt="image" src="https://github.com/user-attachments/assets/c99f75c0-98e9-48ad-93c8-33c36dac6f75" />


6. Select the VC Hub application data directory.

<img width="600" height="465" alt="image" src="https://github.com/user-attachments/assets/32bc1467-86c0-4ed4-a827-7f29ecfd8347" />


7. Prepare for installation.

<img width="600" height="466" alt="image" src="https://github.com/user-attachments/assets/5dde45db-1db1-405c-ba39-726cd30703e5" />


8. The installation is complete.

<img width="602" height="469" alt="image" src="https://github.com/user-attachments/assets/8eb83193-602e-48e4-8e0e-a9b178d7ad51" />


9.  After completion, the default access to the VC Hub site is: `http://localhost:8066`. After the installation, you will enter the configuration wizard interface.

#### Configuration **Steps**:

1. Create an administrator user. Remember this username and password, as you will use them to log in for the first time. 

<img width="731" height="626" alt="image" src="https://github.com/user-attachments/assets/b0b7fb2e-de45-4074-ac2b-5d47574719b7" />


2. Port configuration, configure HTTP, HTTPS ports, and remember the access port. 

<img width="727" height="623" alt="image" src="https://github.com/user-attachments/assets/a1416428-c526-4635-8dc1-6cd0cb858acb" />


3. After completing the above steps, wait for the program to load, and then you can log in to the default-created workspace with the user created in step 1.

| **Note**: After each installation, a new empty workspace will be created by default. To return to the original workspace, you need to log in to the new workspace first and then manually open the original workspace from the workspace list. |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

#### Security Configuration (Optional)

To further enhance system security, it is recommended to perform the following steps after configuration to set permissions on the **service directory **and** application data directory**, allowing only specific users to access or modify them. This ensures that sensitive data is well protected and potential risks are minimized.

1. Create a dedicated service account

      Create a dedicated account in Windows local users and groups (e.g., VCHubSvc):

<img width="931" height="684" alt="image" src="https://github.com/user-attachments/assets/4145b04f-2443-4fe4-93f7-d28cd4143492" />


2. Set service installation directory permissions

Navigate to the service installation directory (e.g., C:\Program Files\WAGO Visualization And Control Hub), right-click the mouse, select "Properties" → "Security"

   - Based on the actual security requirements, select the users or groups to be retained, and delete the unnecessary ones (such as Users, Everyone).
   - Add the VCHubSvc user and grant Read, Write, and Modify permissions.
   - Ensure the changes are applied to all subfolders and files.
            Note: This step must be completed before changing the service logon account; otherwise, the service may fail to start or restart.

3. Modify the service logon account

      In Services (services.msc), locate the VC Hub service → right-click → Properties → Log On → select "This account":

   - Enter .\VCHubSvc and the password.
   - Save and restart the service.
4. Set application data directory permissions

     Navigate to the application data directory chosen during installation (e.g., C:\ProgramData\WAGOVisualizationAndControlHub), in the right-click menu, click "Properties"

    → "Security":

   - Based on the actual security requirements, select the users or groups to be retained, and delete the unnecessary ones (such as Users, Everyone).
   - Add the VCHubSvc user and grant Read, Write, and Modify permissions.
   - Ensure the changes are applied to all subfolders and files.
5. Verify configuration

      Access the VC Hub site (e.g., `http://localhost:8066`) and confirm that the site is running normally.

#### **Uninstallation Steps:**

1. Enter the software uninstall list from the Control Panel. Find VC Hub and proceed with the uninstallation.

<img width="1018" height="244" alt="image" src="https://github.com/user-attachments/assets/7f9cdd5b-ce60-4557-b81b-c4f9e3143c8b" />


2. Confirm the uninstallation to complete the removal of the application.

<img width="476" height="173" alt="image" src="https://github.com/user-attachments/assets/8c147bbc-49e8-4529-9b3f-8b0401d59dea" />







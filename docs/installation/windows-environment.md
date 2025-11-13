# Windows Environment

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

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/BjhJa6EB/resources/lSrVgCuRH-Bi-DKP-NTTZwCTTsdVGyXQ_Fcfr_IiAKA.png?token=W.3fbm3_f-WIBk-p8lXWjPS9RRSSqCt5ZLVnZCwFOmpxahYN2wtJWgSiHPwP-IdoKVZBvFbLzDIZYE0CKZ5pyWNf2kzQ)

3. Perform a port check, if the port is occupied, the installation cannot proceed. 

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/BjhJa6EB/resources/hXIRxB8zGBCZLewD9ugNzUXi5EjzkNRgV0UMYMPelDM.png?token=W.3fbm3_f-WIBk-p8lXWjPS9RRSSqCt5ZLVnZCwFOmpxahYN2wtJWgSiHPwP-IdoKVZBvFbLzDIZYE0CKZ5pyWNf2kzQ)

4. Read and accept the license agreement.

5. Choose the installation location; the default path is: "C:\Program Files\WAGO Visualization And Control Hub".

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/BjhJa6EB/resources/uEO0mjp1nZjaZ0KZxdWhhwFz3IUxPQDt2Am1qvE7fKY.png?token=W.3fbm3_f-WIBk-p8lXWjPS9RRSSqCt5ZLVnZCwFOmpxahYN2wtJWgSiHPwP-IdoKVZBvFbLzDIZYE0CKZ5pyWNf2kzQ)

6. Select the VC Hub application data directory.

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/BjhJa6EB/resources/2hNWBl-yCqZM6e93-lETDUTrgXegzJClVdpsE-zfaM8.png?token=W.3fbm3_f-WIBk-p8lXWjPS9RRSSqCt5ZLVnZCwFOmpxahYN2wtJWgSiHPwP-IdoKVZBvFbLzDIZYE0CKZ5pyWNf2kzQ)

7. Prepare for installation.

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/BjhJa6EB/resources/DM4kj7VXamZgyUOyoyI1SgvlocMFO_5RBRkSEnrGpJ4.png?token=W.3fbm3_f-WIBk-p8lXWjPS9RRSSqCt5ZLVnZCwFOmpxahYN2wtJWgSiHPwP-IdoKVZBvFbLzDIZYE0CKZ5pyWNf2kzQ)

8. The installation is complete.

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/BjhJa6EB/resources/mIOJzni9MnJD0fv_EO2McyDVA3IhZHEe-6kqTYEmMj8.png?token=W.3fbm3_f-WIBk-p8lXWjPS9RRSSqCt5ZLVnZCwFOmpxahYN2wtJWgSiHPwP-IdoKVZBvFbLzDIZYE0CKZ5pyWNf2kzQ)

9.  After completion, the default access to the VC Hub site is: "http://localhost:8066". After the installation, you will enter the configuration wizard interface.

#### Configuration **Steps**:

1. Create an administrator user. Remember this username and password, as you will use them to log in for the first time. 

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/BjhJa6EB/resources/i8Fpp7XWTXNk9EZxyqW1t2WxZ9gORUtgzMbEr0qcoTU.png?token=W.3fbm3_f-WIBk-p8lXWjPS9RRSSqCt5ZLVnZCwFOmpxahYN2wtJWgSiHPwP-IdoKVZBvFbLzDIZYE0CKZ5pyWNf2kzQ)

2. Port configuration, configure HTTP, HTTPS ports, and remember the access port. 

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/BjhJa6EB/resources/btb2wq84MheO3r4LNa8UmHv6OMaD2q7WbKnuTmhbQtU.png?token=W.3fbm3_f-WIBk-p8lXWjPS9RRSSqCt5ZLVnZCwFOmpxahYN2wtJWgSiHPwP-IdoKVZBvFbLzDIZYE0CKZ5pyWNf2kzQ)

3. After completing the above steps, wait for the program to load, and then you can log in to the default-created workspace with the user created in step 1.

**Note**: After each installation, a new empty workspace will be created by default. To return to the original workspace, you need to log in to the new workspace first and then manually open the original workspace from the workspace list. 


#### Security Configuration (Optional)

To further enhance system security, it is recommended to perform the following steps after configuration to set permissions on the **service directory **and** application data directory**, allowing only specific users to access or modify them. This ensures that sensitive data is well protected and potential risks are minimized.

1. Create a dedicated service account

      Create a dedicated account in Windows local users and groups (e.g., VCHubSvc):

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/BjhJa6EB/resources/dt1gt0xOCVmBuSOycwhblnAqqaywMZCQbsjNVktpw24.png?token=W.3fbm3_f-WIBk-p8lXWjPS9RRSSqCt5ZLVnZCwFOmpxahYN2wtJWgSiHPwP-IdoKVZBvFbLzDIZYE0CKZ5pyWNf2kzQ)

2. Set service installation directory permissions

Navigate to the service installation directory (e.g., C:\Program Files\WAGO Visualization And Control Hub), right-click the mouse, select "Properties" → "Security"

   - Based on the actual security requirements, select the users or groups to be retained, and delete the unnecessary ones (such as Users, Everyone).
   - Add the WagoScadaSvc user and grant Read, Write, and Modify permissions.
   - Ensure the changes are applied to all subfolders and files.
            Note: This step must be completed before changing the service logon account; otherwise, the service may fail to start or restart.

3. Modify the service logon account

      In Services (services.msc), locate the VC Hub service → right-click → Properties → Log On → select "This account":

   - Enter .\WagoScadaSvc and the password.
   - Save and restart the service.
4. Set application data directory permissions

     Navigate to the application data directory chosen during installation (e.g., C:\ProgramData\WAGOVisualizationAndControlHub), in the right-click menu, click "Properties"

    → "Security":

   - Based on the actual security requirements, select the users or groups to be retained, and delete the unnecessary ones (such as Users, Everyone).
   - Add the WagoScadaSvc user and grant Read, Write, and Modify permissions.
   - Ensure the changes are applied to all subfolders and files.
5. Verify configuration

      Access the VC Hub site (e.g., http://localhost:8066) and confirm that the site is running normally.

#### **Uninstallation Steps:**

1. Enter the software uninstall list from the Control Panel. Find VC Hub and proceed with the uninstallation.

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/BjhJa6EB/resources/0B43Unm15LFV4YFGeS0vBDGmg1pKd_Ik6MwlfZxkjQo.png?token=W.3fbm3_f-WIBk-p8lXWjPS9RRSSqCt5ZLVnZCwFOmpxahYN2wtJWgSiHPwP-IdoKVZBvFbLzDIZYE0CKZ5pyWNf2kzQ)

2. Confirm the uninstallation to complete the removal of the application.

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/BjhJa6EB/resources/8dF5OqJcJjFo9hIWpmhkLRStQrvRk_pJB1G7MLbHsu0.png?token=W.3fbm3_f-WIBk-p8lXWjPS9RRSSqCt5ZLVnZCwFOmpxahYN2wtJWgSiHPwP-IdoKVZBvFbLzDIZYE0CKZ5pyWNf2kzQ)






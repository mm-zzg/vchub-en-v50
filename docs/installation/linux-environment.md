# Linux Environment

VC Hub provides an installation package for the Linux environment, with the file name wagovisualizationandcontrolhub-x.x.x-linux-x64-installer.run.

#### **Installation Steps:**

1. Copy the installation package to a directory on the Linux server.
2. Grant the file owner the permission to execute the installation file 

<img width="1566" height="27" alt="image" src="https://github.com/user-attachments/assets/23201de1-fe7c-478a-9c7c-c1525d69d1ce" />


3. Run the installation package in the directory using the command ./ followed by the file name. 

<img width="1362" height="30" alt="image" src="https://github.com/user-attachments/assets/22535401-5edd-45f3-a72d-c9fb91aeee59" />


4. Select the installation language.

<img width="1371" height="120" alt="image" src="https://github.com/user-attachments/assets/733ba351-aa04-4873-bb50-178ae88ec4aa" />


5. Customize the installation directory or use the default directory. If the installation directory does not exist, the installer will create it automatically.

<img width="1197" height="207" alt="image" src="https://github.com/user-attachments/assets/f9cd8ceb-48ab-40d8-a8f0-41f06437af48" />


<img width="1344" height="153" alt="image" src="https://github.com/user-attachments/assets/13b29be6-f23c-4914-8f28-1a7fa06ba3a3" />


6. Customize the data directory or use the default directory.

<img width="1143" height="81" alt="image" src="https://github.com/user-attachments/assets/c32df722-01b5-4803-acab-8c7416e90c9d" />


7. Wait for the installation to complete. This process may take some time, so please be patient. 

<img width="1869" height="177" alt="image" src="https://github.com/user-attachments/assets/d69959c6-4183-441b-93d5-a3a8182d3565" />


8. The installation is complete.

<img width="1254" height="102" alt="image" src="https://github.com/user-attachments/assets/c321674b-0302-4870-afc6-8077c6aa79f0" />

9. After completion, the default access to the VC Hub site is: `http://localhost:8066`. After the installation, you will enter the configuration wizard interface.

**Notes:** 

1. The program is supervised and managed by the systemd service manager that comes with the Linux system. Ensure that the systemd on the server is running properly.
2. The installation script includes operations such as creating scripts, so make sure you have sufficient permissions.

## Configuration:

1. Read and agree the license agreement

2. Create an administrator user. Remember this username and password, as you will use them to log in for the first time. 

<img width="990" height="831" alt="image" src="https://github.com/user-attachments/assets/b0ca6757-e573-4ea1-8f33-c4f1c509c160" />


3. Port configuration, configure HTTP, HTTPS ports, and remember the access port. 

<img width="984" height="827" alt="image" src="https://github.com/user-attachments/assets/8f4e1688-8cfb-40f6-8f63-5fb87d371806" />




4. After completing the above steps, wait for the program to load, and then you can log in to the default workspace with the administrator user created in step 2.

**Note**: If you perform an upgrade installation, a new empty workspace will be created by default. To return to the original workspace, you need to log in to the new workspace first and then manually open the original workspace from the workspace list. 


#### Security Configuration (Optional)

To further enhance system security, it is recommended to perform the following steps after configuration to set permissions on the **service directory **and** application data directory**, allowing only specific users to access or modify them. This ensures that sensitive data is well protected and potential risks are minimized.

1.  Create a Dedicated Service Account

    Create a dedicated system account (e.g., wago_vc_hub) with no interactive login, used only to run service processes:

```Plain Text
sudo useradd -r -s /sbin/nologin wago_vc_hub
```
 
    Then, configure passwordless sudo for this account via the sudoers file:

```Plain Text
wago_vc_hub ALL=(ALL) NOPASSWD: ALL
```
 
2. Set Service Installation Directory Permissions

    Assign ownership of the service installation directory (e.g., /usr/local/bin/wagovisualizationandcontrolhub-x.x.x-linux-x64) to wago_vc_hub and restrict access to other users:

```Plain Text
sudo chown -R wago_vc_hub:wago_vc_hub /usr/local/bin/wagovisualizationandcontrolhub-x.x.x-linux-x64
sudo chmod -R 750 /usr/local/bin/wagovisualizationandcontrolhub-x.x.x-linux-x64
```
 
   **Note:** Perform this step before changing the service run account, otherwise the service may lose access.

3. Modify Service Run Account

  Configure the service to run under the wago_vc_hub account:

```Plain Text
sudo systemctl edit visualizationandcontrolhub.service
```
 
Add the following lines under the [Service] section:

```Plain Text
User=wago_vc_hub
Group=wago_vc_hub
```
 
Then reload the systemd configuration and restart the service:

```Plain Text
sudo systemctl daemon-reexec
sudo systemctl restart visualizationandcontrolhub.service
```
 
4. Set Application Data Directory Permissions

    Assign ownership of the data directory (e.g., /usr/share/wagovisualizationandcontrolhub) to wago_vc_hub and ensure read/write access while restricting other users:

```Plain Text
sudo chown -R wago_vc_hub:wago_vc_hub /usr/share/wagovisualizationandcontrolhub
sudo chmod -R 750 /usr/share/wagovisualizationandcontrolhub
```
 
5. Verify Configuration

   Check that the service is running under the wago_vc_hub account and confirm the site is accessible:

```Plain Text
systemctl status visualizationandcontrolhub.service
```
 
  Open a browser and visit the VC Hub site (e.g., `http://localhost:8066`) to verify it is running correctly.

#### **Uninstallation Steps:**

1. Go to the parent directory of the installation directory.
2. Grant the file owner the permission to execute the file "visualizationandcontrolhub-uninstall.sh"

<img width="1314" height="30" alt="image" src="https://github.com/user-attachments/assets/24bed512-59fd-4b17-8f71-80218ad1a1cd" />


3. Run the script "visualizationandcontrolhub-uninstall.sh".

<img width="1278" height="408" alt="image" src="https://github.com/user-attachments/assets/175c0ceb-813a-41b3-88c8-e3998aa9c1b5" />


4. After these operations, all program-related files will be removed, and the process supervisory service will also be removed.

**Notes:**

The uninstallation script includes operations such as deleting files, so ensure you have sufficient permissions.


# Linux Environment

VC Hub provides an installation package for the Linux environment, with the file name wagoscada-x.x.x-linux-x64-installer.run.

#### **Installation Steps:**

1. Copy the installation package to a directory on the Linux server.
2. Grant the file owner the permission to execute the installation file 

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/G3XMsK9P/resources/AO3_WyuE4OyqPdALLN_T0L-QFkllmgUlsqCom7EH9kc.png?token=W.uKaf8l56Zl_yatBygqePA0wHOxrqdqqH6ghpU0i3nMjEPIvAdNOwOSHxUL3c5iy4_1kHkTw41694jfoaXH19MpfAlw)

3. Run the installation package in the directory using the command ./ followed by the file name. 

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/G3XMsK9P/resources/9MbXmv_lTPa5LsV9aJbJRB4-Yp2crugITg5ytFi33tw.png?token=W.uKaf8l56Zl_yatBygqePA0wHOxrqdqqH6ghpU0i3nMjEPIvAdNOwOSHxUL3c5iy4_1kHkTw41694jfoaXH19MpfAlw)

4. Select the installation language.

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/G3XMsK9P/resources/9wUq5xyd-za04TP66M72ZZgU8vfTY8Y530V7K6LTAUw.png?token=W.uKaf8l56Zl_yatBygqePA0wHOxrqdqqH6ghpU0i3nMjEPIvAdNOwOSHxUL3c5iy4_1kHkTw41694jfoaXH19MpfAlw)

5. Customize the installation directory or use the default directory. If the installation directory does not exist, the installer will create it automatically.

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/G3XMsK9P/resources/NxTiUwxnsPGSqm7PARBMKuf7opHpyNzJA5P1t9MGx0Y.png?token=W.uKaf8l56Zl_yatBygqePA0wHOxrqdqqH6ghpU0i3nMjEPIvAdNOwOSHxUL3c5iy4_1kHkTw41694jfoaXH19MpfAlw)

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/G3XMsK9P/resources/CDTsfls4lX2uqBaA2xGbtTBcpeEQmAt8J2I2jI8t6EE.png?token=W.uKaf8l56Zl_yatBygqePA0wHOxrqdqqH6ghpU0i3nMjEPIvAdNOwOSHxUL3c5iy4_1kHkTw41694jfoaXH19MpfAlw)

6. Customize the data directory or use the default directory.

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/G3XMsK9P/resources/uA0EJplanMvXdqJwoDpjq2E7MSFJlCkRaAA7uhOU6ps.png?token=W.uKaf8l56Zl_yatBygqePA0wHOxrqdqqH6ghpU0i3nMjEPIvAdNOwOSHxUL3c5iy4_1kHkTw41694jfoaXH19MpfAlw)

7. Wait for the installation to complete. This process may take some time, so please be patient. 

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/G3XMsK9P/resources/4aB0YlU9qh0mJ8W45byIxWvNuvnd01ZOZmRznecZA6c.png?token=W.uKaf8l56Zl_yatBygqePA0wHOxrqdqqH6ghpU0i3nMjEPIvAdNOwOSHxUL3c5iy4_1kHkTw41694jfoaXH19MpfAlw)

8. The installation is complete.

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/G3XMsK9P/resources/7fzgopSlKLZuJ0jzNFtJRzzkoMi9l-qIj3nwQZtLM8s.png?token=W.uKaf8l56Zl_yatBygqePA0wHOxrqdqqH6ghpU0i3nMjEPIvAdNOwOSHxUL3c5iy4_1kHkTw41694jfoaXH19MpfAlw)

9. After completion, the default access to the VC Hub site is: "http://localhost:8066". After the installation, you will enter the configuration wizard interface.

**Notes:** 

1. The program is supervised and managed by the systemd service manager that comes with the Linux system. Ensure that the systemd on the server is running properly.
2. The installation script includes operations such as creating scripts, so make sure you have sufficient permissions.

## Configuration:

1. Read License Agreement

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/G3XMsK9P/resources/bCUeY3P8oZNjW-H1Ub4ug3wzpaI_bNEyGOsAq9L5ieE.png?token=W.uKaf8l56Zl_yatBygqePA0wHOxrqdqqH6ghpU0i3nMjEPIvAdNOwOSHxUL3c5iy4_1kHkTw41694jfoaXH19MpfAlw)

2. Create an administrator user. Remember this username and password, as you will use them to log in for the first time. 

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/G3XMsK9P/resources/vN56AKxuo2vW48LNBoITn5Xr2Eb1UaIOp4dDqKURwZs.png?token=W.uKaf8l56Zl_yatBygqePA0wHOxrqdqqH6ghpU0i3nMjEPIvAdNOwOSHxUL3c5iy4_1kHkTw41694jfoaXH19MpfAlw)

3. Port configuration, configure HTTP, HTTPS ports, and remember the access port. 

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/G3XMsK9P/resources/HKaRCPMZOQyROlWsR8lgmAbe7m1X2-hHRasXgCdwzqE.png?token=W.uKaf8l56Zl_yatBygqePA0wHOxrqdqqH6ghpU0i3nMjEPIvAdNOwOSHxUL3c5iy4_1kHkTw41694jfoaXH19MpfAlw)



4. After completing the above steps, wait for the program to load, and then you can log in to the default workspace with the administrator user created in step 2.

| **Note**: If you perform an upgrade installation, a new empty workspace will be created by default. To return to the original workspace, you need to log in to the new workspace first and then manually open the original workspace from the workspace list. |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

#### Security Configuration (Optional)

To further enhance system security, it is recommended to perform the following steps after configuration to set permissions on the **service directory **and** application data directory**, allowing only specific users to access or modify them. This ensures that sensitive data is well protected and potential risks are minimized.

1.  Create a Dedicated Service Account

    Create a dedicated system account (e.g., wago_scada) with no interactive login, used only to run service processes:

```Plain Text
sudo useradd -r -s /sbin/nologin wago_scada
```
 
    Then, configure passwordless sudo for this account via the sudoers file:

```Plain Text
wago_scada ALL=(ALL) NOPASSWD: ALL
```
 
2. Set Service Installation Directory Permissions

    Assign ownership of the service installation directory (e.g., /usr/local/bin/wagoscada) to wago_scada and restrict access to other users:

```Plain Text
sudo chown -R wago_scada:wago_scada /usr/local/bin/wagoscada
sudo chmod -R 750 /usr/local/bin/wagoscada
```
 
   Note**:** Perform this step before changing the service run account, otherwise the service may lose access.

3. Modify Service Run Account

  Configure the service to run under the wago_scada account:

```Plain Text
sudo systemctl edit wagoscada.service
```
 
Add the following lines under the [Service] section:

```Plain Text
User=wago_scada
Group=wago_scada
```
 
Then reload the systemd configuration and restart the service:

```Plain Text
sudo systemctl daemon-reexec
sudo systemctl restart wagoscada.service
```
 
4. Set Application Data Directory Permissions

    Assign ownership of the data directory (e.g., /usr/share/WAGOSCADA) to wago_scada and ensure read/write access while restricting other users:

```Plain Text
sudo chown -R wago_scada:wago_scada /usr/share/WAGOSCADA
sudo chmod -R 750 /usr/share/WAGOSCADA
```
 
5. Verify Configuration

   Check that the service is running under the wago_scada account and confirm the site is accessible:

```Plain Text
systemctl status wagoscada.service
```
 
  Open a browser and visit the VC Hub site (e.g., http://localhost:8066) to verify it is running correctly.

#### **Uninstallation Steps:**

1. Go to the parent directory of the installation directory.
2. Grant the file owner the permission to execute the file "wagoscada-uninstall.sh"

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/G3XMsK9P/resources/xd11MyGmn9OA6PthQy1nBLU3cmFcXycVd01EEEic-7U.png?token=W.uKaf8l56Zl_yatBygqePA0wHOxrqdqqH6ghpU0i3nMjEPIvAdNOwOSHxUL3c5iy4_1kHkTw41694jfoaXH19MpfAlw)

3. Run the script "wagoscada-uninstall.sh".

![img](https://docs.wagoscada.cn/wiki/api/wiki/editor/QHXVK91b/G3XMsK9P/resources/C4WIxPVkApX4ebQzDghHpKAC5LlLp69UycLWmS_6AIQ.png?token=W.uKaf8l56Zl_yatBygqePA0wHOxrqdqqH6ghpU0i3nMjEPIvAdNOwOSHxUL3c5iy4_1kHkTw41694jfoaXH19MpfAlw)

4. After these operations, all program-related files will be removed, and the process supervisory service will also be removed.

**Notes: **

The uninstallation script includes operations such as deleting files, so ensure you have sufficient permissions.


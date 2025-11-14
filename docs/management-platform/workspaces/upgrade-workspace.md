# Upgrade Workspace

#### Overview

When workspaces in the system are on versions lower than the current system version, users won’t be able to open, copy, or edit them. To address this, an upgrade is necessary to ensure compatibility and access. Users can initiate the upgrade by clicking the green upgrade arrow button next to the corresponding version number. The process is handled server-side, where the workspace is seamlessly updated to match the current system version. This upgrade retains all existing data from the older version, ensuring that no information is lost while enabling full functionality in the latest system environment.

#### How to Operate

As shown in the figure below, there are two workspaces in the list. The workspace named "Default" has a version of 4.3.0, which is lower than the system version displayed in the lower right corner (4.4.0). Since it meets the upgrade criteria, a green upgrade arrow button is displayed next to the version number.

<img width="1807" height="204" alt="image" src="https://github.com/user-attachments/assets/75267928-d0da-4210-8e33-3290d923071c" />


After the user clicks the upgrade button, the system will prompt a dialog asking whether to Backup. The user can choose to either "Upgrade" or "Backup and Upgrade" based on their needs.

<img width="516" height="164" alt="image" src="https://github.com/user-attachments/assets/8ddf7caa-a0e2-4222-bdb9-063b21d31950" />

After clicking the "Upgrade" or "Backup and Upgrade" button, the upgrade arrow will change to "Upgrading..." indicating that the system is currently upgrading the workspace in the background.

<img width="1557" height="167" alt="image" src="https://github.com/user-attachments/assets/d80afaa9-3c18-4522-8032-737e74bac4e2" />


If the user selects "Upgrade" , then after a successful upgrade, only the updated workspace named "Test" with the new version 4.1.0 will appear in the list, while the old version 4.0.0 of the "Test" workspace will be removed.

<img width="1556" height="189" alt="image" src="https://github.com/user-attachments/assets/6ed12fd2-6b79-4e5c-8ac0-c00b6e0e06fa" />


If the user selects "Backup and Upgrade," then after a successful upgrade, the list will contain both the updated workspace named "Test" with the new version 4.1.0 and an additional backup of the old version 4.0.0, named "Test_{Backup Time}_bak," as shown in the figure below.

<img width="1562" height="248" alt="image" src="https://github.com/user-attachments/assets/ad21f044-70c3-41a6-b1c7-94f2dc703607" />



If any error occurs during the backend upgrade of the workspace, the upgrade will fail. A red "Upgrade Failed" message will appear next to the upgrade arrow to alert the user. The user can click on the adjacent exclamation mark button to view detailed information about the failure.

<img width="1550" height="186" alt="image" src="https://github.com/user-attachments/assets/d5c35d68-b8c1-4145-85e8-6d103df9eb6d" />



<img width="412" height="158" alt="image" src="https://github.com/user-attachments/assets/d945be0e-8cd7-45df-b592-2b53a7442ea1" />


Users can attempt to resolve the issues based on the failure information. After resolving the issues, the user can click the upgrade arrow button again to retry the upgrade process.

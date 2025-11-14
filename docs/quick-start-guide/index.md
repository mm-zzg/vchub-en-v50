# Quick Start Guide

We have outlined some simple steps to guide you through configuring your project. You can run a project in a short amount of time.

#### **1. Create a Project**

Click the "Add" button in the project list to create a project.

<img width="1907" height="302" alt="image" src="https://github.com/user-attachments/assets/adb1b2ec-68b2-4286-8673-a5daed813e82" />


#### **2** **. Add a Database**

After the installation of VC Hub, a SQLite database will be automatically created, which you can use for basic testing. You can also click "Database" -> "Database Connection" page and then click the "New" button to create a new database connection. 

#### **3. Add Assets**

After the installation of VC Hub, a default asset will be automatically created, which you can use for basic testing. You can also click "Tags" -> "Assets" page and then click the "New" button to create new assets.

#### **4. Open the Editor**

On the project list page, click the "Design" button for the project.

<img width="1895" height="239" alt="image" src="https://github.com/user-attachments/assets/c5546d2d-9098-4b0d-a825-be9c0fb6f618" />


Open the configuration editor to display the following interface.

<img width="1920" height="941" alt="image" src="https://github.com/user-attachments/assets/ad7fcdd6-8cfb-4953-a62a-ec071703c024" />


#### **5. Create a New Page**

Click "New Page" to quickly create a new page.

<img width="246" height="372" alt="image" src="https://github.com/user-attachments/assets/a227ee58-3ad6-4cd4-9cf5-1de2f181e181" />


In the **Tools** window on the left side of the designer, add for example "Rect" , "Label" , "Value Display",and "Historical Trend Chart" controls to the page. You can also use the search functionality.

<img width="1915" height="604" alt="image" src="https://github.com/user-attachments/assets/dc56dbc1-12e9-4589-b24f-057c7b7cc6eb" />


#### **6. Create a Tag**

In the asset dropdown box of the asset window in the configuration editor, select an asset and then click the add button to add a memory tag to that asset. Tag name: liquid.

<img width="376" height="706" alt="image" src="https://github.com/user-attachments/assets/1d87b78d-4022-4ec3-b4ef-612cca9a687f" />


Enable the simulated property for this tag, using simulated value as the tag value. Types supported are **Random**, **Increment**, **Decrement**, and **Fixed.**

<img width="1090" height="495" alt="image" src="https://github.com/user-attachments/assets/e44da068-a6f8-44eb-b723-4204617ef49c" />


#### **7. Enable History for Tags**

At the top of the tag editing page, enable history recording to store the value of the tag historically.

<img width="1092" height="571" alt="image" src="https://github.com/user-attachments/assets/79ff5d78-3ab6-4ea0-999c-6c7d3dd1fb7b" />


#### **8. Bind Tag**

Bind tags to controls on the page.

1. Set the display content of the text label to: "Liquid level:"

<img width="1579" height="452" alt="image" src="https://github.com/user-attachments/assets/8daad4c6-6f35-4a52-8786-c8e25116b32c" />


2.  In the animation of the rectangle, select the fill animation. Click the value binding button and bind the created tag:liquid.

<img width="1919" height="723" alt="image" src="https://github.com/user-attachments/assets/20fc173a-9004-4e74-8723-f2f7c1b50bbf" />


3. In the value display control, click the value binding button and bind the created tag:liquid. Afte binding, the binding icon will turn from gray to green.

<img width="1549" height="480" alt="image" src="https://github.com/user-attachments/assets/0aaeb96d-847a-462c-a750-8aa8a8020a5e" />


4. In the historical chart control, click the value binding button and bind the created tag:liquid. 

<img width="1324" height="494" alt="image" src="https://github.com/user-attachments/assets/16361bcd-19c5-4d86-8794-a1ab69ac3d69" />


Note: For more information on binding, please refer to the Property Binding page. 

#### **9. Preview/Run**

Click the preview button in the page tool bar to view the preview effect. You can also click the run button for the project in the project list to view the running page.









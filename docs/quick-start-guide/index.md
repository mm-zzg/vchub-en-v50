# Quick Start Guide

We have outlined some simple steps to guide you through configuring your project. You can run a project in a short amount of time.

#### **1. Create a Project**

Click the "Add" button in the project list to create a project.

<img width="1907" height="302" alt="image" src="https://github.com/user-attachments/assets/3d4d73d1-f44d-49bc-abba-526385d57a5d" />



#### **2** **. Add a Database**

After the installation of VC Hub, a SQLite database will be automatically created, which you can use for basic testing. You can also click "Database" -> "Database Connection" page and then click the "New" button to create a new database connection. 

#### **3. Add Assets**

After the installation of VC Hub, a default asset will be automatically created, which you can use for basic testing. You can also click "Tags" -> "Assets" page and then click the "New" button to create new assets.

#### **4. Open the Editor**

On the project list page, click the "Design" button for the project.

<img width="1895" height="239" alt="image" src="https://github.com/user-attachments/assets/a5a3ecc9-ee42-4f46-803b-d5b522e3d0d6" />



Open the configuration editor to display the following interface.

<img width="1920" height="941" alt="image" src="https://github.com/user-attachments/assets/74598900-7862-4936-b110-4a2b76559155" />



#### **5. Create a New Page**

Click "New Page" to quickly create a new page.

<img width="246" height="372" alt="image" src="https://github.com/user-attachments/assets/822c7b78-ad39-4a2b-887e-497fe4f56b63" />



In the **Tools** window on the left side of the designer, add for example "Rect" , "Label" , "Value Display",and "Historical Trend Chart" controls to the page. You can also use the search functionality.

<img width="1915" height="604" alt="image" src="https://github.com/user-attachments/assets/5709271c-9561-4d4a-91d9-f93f5437f8f6" />



#### **6. Create a Tag**

In the asset dropdown box of the asset window in the configuration editor, select an asset and then click the add button to add a memory tag to that asset. Tag name: liquid.

<img width="376" height="706" alt="image" src="https://github.com/user-attachments/assets/de955e06-6229-44d7-85bb-0b556bb4b5fa" />



Enable the simulated property for this tag, using simulated value as the tag value. Types supported are **Random**, **Increment**, **Decrement**, and **Fixed.**

<img width="1090" height="495" alt="image" src="https://github.com/user-attachments/assets/05d14416-cd92-4b60-b27c-0d03d9ede78b" />



#### **7. Enable History for Tags**

At the top of the tag editing page, enable history recording to store the value of the tag historically.

<img width="1092" height="571" alt="image" src="https://github.com/user-attachments/assets/ee5f32cb-3b12-4a4d-b501-4bd5049cdfca" />



#### **8. Bind Tag**

Bind tags to controls on the page.

1. Set the display content of the text label to: "Liquid level:"

<img width="1579" height="452" alt="image" src="https://github.com/user-attachments/assets/516ac065-21cf-4372-b5b7-d0f0b32081d0" />



2.  In the animation of the rectangle, select the fill animation. Click the value binding button and bind the created tag:liquid.

<img width="1919" height="723" alt="image" src="https://github.com/user-attachments/assets/cfd8b9b7-863f-496b-baf7-8b5585747d64" />



3. In the value display control, click the value binding button and bind the created tag:liquid. Afte binding, the binding icon will turn from gray to green.

<img width="1549" height="480" alt="image" src="https://github.com/user-attachments/assets/b6a7a4d7-900a-4ee2-94f1-c4c056c7f4a3" />



4. In the historical chart control, click the value binding button and bind the created tag:liquid. 

<img width="1324" height="494" alt="image" src="https://github.com/user-attachments/assets/3faa187d-b0b4-4ad8-b55e-b1ffebf85ce7" />



Note: For more information on binding, please refer to the Property Binding page. 

#### **9. Preview/Run**

Click the preview button in the page tool bar to view the preview effect. You can also click the run button for the project in the project list to view the running page.


![quick-start-guide](../assets/images/quick-start-guide.gif)








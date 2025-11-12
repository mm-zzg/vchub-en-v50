
# Version Update Notes

WAGO SCADA is constantly evolving and being updated, with each new version bringing new features and bug fixes. Here, you can quickly preview the new features and resolved issues of the corresponding versions.

---

## Determining Your Current Version

You can find out the version number of WAGO SCADA you are currently using in the following two ways:

1. **Bottom Right Corner of the Management Platform**
   The version number can be found in the bottom right corner of the management platform.

2. **Top Right Corner of the Configuration Editing Interface**
   Click on the exclamation mark icon in the top right corner of the configuration editing interface to view the version number information.

---

## Features Overview

### **WYSIWYG Configuration Editor**
WAGO SCADA provides a WYSIWYG (What You See Is What You Get) configuration editor, allowing real-time preview of configuration effects.

### **Standardized Alarms**
- Includes limit alarms, rate of change alarms, and equal value alarms.
- Provides real-time and historical configuration controls.

### **Object-Oriented Tag Creation**
- Supports direct creation of tags.
- Allows object-oriented tag creation to build field applications using the concept of assets.

### **Multi-Database Support**
WAGO SCADA enables the configuration of various databases for historical data storage, such as MySQL and SQL Server.

### **Networking and Redundancy**
- Supports large-scale configurations and high-availability scenarios.
- Facilitates complex field configuration projects through SCADA networking.

### **3D Digital Twin**
- Supports 3D configuration, similar to 2D configuration.
- Allows building of digital twin scenarios using advanced 3D APIs.

---

## New Features by Version

### **Version 4.3.X**

- **SVG Editor**: Modify and save attributes of SVG images, such as color, size, text content, and visibility.
- **Toggle Button**: Switches between ON and OFF states when clicked. Useful for controlling Boolean-type devices like start/stop or on/off switches.
- **2-State Button**: Represents two distinct states (e.g., ON/OFF or Start/Stop), with configurable styles for each state.
- **Multi-State Button**: Contains multiple states and allows switching between them, with configurable appearance styles for each state.
- **Historical Data Storage of Raw Values**: Supports storing original raw values of variables for historical data.
- **Screen Functions and Expression Functions**: Centralize common logic into reusable functions, reducing repeated logic and maintenance costs.
- **Binding Support for Enabling/Disabling Animations**: Property bindings can control enabling or disabling of animations for components.

---

### **Version 4.2.X**

- **Permissions**: Supports single sign-on and project/page permissions setting.
- **SQL Query**: Enables querying data from third-party databases, with support for parameterized dynamic result sets bound to controls.
- **Table Control**: Displays data in a customizable table format, with styling and interactive elements.
- **Bidirectional Binding**: Tags, indirect tags, and properties can reflect changes bidirectionally between controls and tags.
- **Parameterized Data Source Binding**: Use parameters for flexible tag paths, automatically updating paths when parameter values change.
- **Batch Editing Control Properties**: Batch modify properties for multiple controls, such as labels.
- **Editable System Tags**: System tags can be edited and configured for alarms, historical storage, and more.
- **OPC UA**: Added discovery service function.
- **Camera Configuration**: Set up WebRTC streamer for camera streaming, separate from the WAGO SCADA server.
- **Alarm Notifications Integration**: Send alarm notifications to WeCom (group/account) or DingTalk (group/account).

---

### **Version 4.1.X**

- **Alarm Notifications**: Notifications sent to specific users via email or SMS when system alarms occur.
- **Symbols**: Create detailed models of devices or systems using symbols and sub-symbols for efficient monitoring. Supports user-defined symbols.
- **Workspace Upgrades**: Upgrade historical workspaces to align with the current package version.
- **Open API**: Share data with external applications or partners via APIs for seamless integration.
- **Property Binding Enhancements**: Supports "Dynamic Tag" binding and "Cell Update" binding.
- **Batch Operation Tags**: Add and edit tags in bulk using Excel.


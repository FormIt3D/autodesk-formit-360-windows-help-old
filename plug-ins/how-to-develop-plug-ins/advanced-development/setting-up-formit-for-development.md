# Setting up FormIt for Development



In order to test and build plugins in FormIt desktop app, you'll need FormIt for Window v17.0 or later.

### **Display script editor and script output**

Toggle the Script Editor and Script Output in FormIt for Windows:

**Window **menu > check **Script Editor** and **Script Output**

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/EnableDevelopmentWindows.PNG)

Once toggled, the Script Editor and Script Output will appear at the bottom of the FormIt window.

Switch between the Script Editor and Script Output by using the buttons at the bottom.

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/ScriptEditorDefaultState.PNG)

You can also get both panels to show up side-by-side by clicking the button next to the "x" in the upper right corner to detach one of the panels, then drag and drop the panels next to each other:

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/ScriptEditor+ScriptOutputConfiguration.gif)

### **Script Editor**

The Script Editor provides a simple development environment where you can write and test code.

The Script Editor stores written code inside a scratch.js file in the directory where the FormIt exe is located.

At the top are two buttons:

* **Run **![](<../../../.gitbook/assets/image (4).png>)**: **Executes all code written in the window.
* **Run Selection **![](<../../../.gitbook/assets/image (15).png>)**:  **Executes only the selected/highlighted lines of code.

****

### **Script Output**

The Script Output window will display any messages printed to the console from plugins.

You can clear the output by running `console.clear();` in the Script Editor.

## Working with Sample Plugins

If you've cloned the repositories and set up a web server from the previous steps, you can now get the local plugins to show up in FormIt.

You can load or install any of the plugins, but for the purposes of this exercise, you'll install both a panel-based and toolbar-based plugin. We'll assume your npm http-server is running on port 8080 hosting both example repositories.

### **Load vs. Install**

`FormIt.LoadPlugin();` loads the plugin only for that session. It will be unloaded automatically when the app is closed and restarted.

* Great for temporarily manifesting a plugin for testing, for this session only.

`FormIt.InstallPlugin();` makes the plugin persist between sessions using a registry key.

* Use `FormIt.UninstallPlugin(); `to uninstall.
* Great for plugins you'll use frequently between sessions.
* On Windows, the following registry keys are used to persist plugins:
  * Plugins: Computer\HKEY\_CURRENT\_USER\Software\Autodesk\FormIt 360\Plugins\InstalledPlugins

In the following examples, unless otherwise noted, feel free to use _Install_ and _Load_ interchangeably depending on whether you want the results of the exercise to be persistent or not.



### **Toolbar plugin sample**

In the Script Editor, run the following:

If running a local server:

* `FormIt.LoadPlugin("http://localhost:8080/FlipAlong");`



If loading from the [FormIt Github repo](https://github.com/FormIt3D/) (requires an internet connection):

* `FormIt.LoadPlugin("https://formit3d.github.io/FlipAlong");`



You should see the Flip Along toolbar appear at the top of the application window:

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/FlipAlongToolbar.PNG)

### ****

### **HTML Panel plugin sample**

In the Script Editor, run the following:

If running a local server:

* `FormIt.LoadPlugin("http://localhost:8080/PropertiesPlus");`



If loading from the [FormIt Github repo](https://github.com/FormIt3D/) (requires an internet connection):

* FormIt.LoadPlugin("https://formit3d.github.io/PropertiesPlus");
* You should see the Properties Plus panel appear on the right side of the application window

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PropertiesPlusPanel.png)

### ****

### **Modal + Modeless Dialog Plugin Sample**

Dialog plugins are unique, they can only be loaded, not installed.

In the Script Editor, run the following:

If running a local server:

* Modal: `FormIt.LoadPlugin("http://localhost:8080/FormItExamplePlugins/ModalDialog");`
* Modeless: `FormIt.LoadPlugin("http://localhost:8080/FormItExamplePlugins/ModelessDialog");`



If loading from the [FormIt Github repo](https://github.com/FormIt3D/) (requires an internet connection):

* Modal: `FormIt.LoadPlugin("https://formit3d.github.io/FormItExamplePlugins/ModalDialog");`
* Modal: `FormIt.LoadPlugin("https://formit3d.github.io/FormItExamplePlugins/ModelessDialog");`

``

You should see the Hello Block! panel from the HTML Panel example appear on screen as either a modal or modeless dialog.

# Enable development window in FormIt desktop app



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

****

### **Script Editor**

The Script Editor provides a simple development environment where you can write and test code.

The Script Editor stores written code inside a scratch.js file in the directory where the FormIt exe is located.

At the top are two buttons:

* **Run **![](<../../../../.gitbook/assets/image (4).png>)**: **Executes all code written in the window.
* **Run Selection **![](<../../../../.gitbook/assets/image (15).png>)**:  **Executes only the selected/highlighted lines of code.

****

### **Script Output**

The Script Output window will display any messages printed to the console from plugins.

You can clear the output by running `console.clear();` in the Script Editor.

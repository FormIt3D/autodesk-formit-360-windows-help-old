# Testing Plugins

If your web server is running [per the instructions above](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html#SettingUpEnvironment), you can test your in-progress plugins easily using the built-in [Script Editor](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html#SettingUpFormIt) in FormIt for Windows:

We recommend using FormIt.LoadPlugin("URL"); when testing, which loads plugins temporarily for this session (they will disappear when FormIt is restarted). Once testing is complete, you can persist the plugin between sessions using FormIt.InstallPlugin("URL");.

* **FormIt for Windows v17 and newer**
*
  * **Toolbar Plugins**
  *
    * Load your plugin into FormIt to see the latest UI and test the latest functionality:
    *
      * FormIt.LoadPlugin("http://localhost:8080/YourPluginName");
    * Make some changes, then load the plugin again using the command above.
    *
      * You can load many instances of the same plugin in the current session as you test, each with its own UI.
      * Be sure to use the latest UI instance to ensure you're testing your most recent changes.
  * **HTML Panel Plugins**
  *
    * Load your plugin into FormIt to see the latest UI and test the latest functionality:
    *
      * FormIt.LoadPlugin("http://localhost:8080/YourPluginName");
    * Make some changes, then simply right-click the panel and select "Hard Reload" to reload the panel with the latest HTML, CSS, and scripts.

**Previewing Your Plugin with the Plugin Manager**

To preview how your plugin would appear in the Plugin Manager (updated title, description, etc) before it's pushed to GitHub, you can paste the localhost URL into the box at the bottom of the Plugin Manager:

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerInstallLocal.png)

Then look for your plugin in the Installed section at the top:

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerInstalledList.png)

**Force Clearing the Web Cache for .JSON Files**

If you modify the title or description inside the manifest.json file for a plugin or repo, you may need to force clear the cache in FormIt for Windows to see those changes take effect the next time you reload the Plugin Manager.

FormIt for Windows stores its web cache here:

* C:\Users\user\AppData\Local\Autodesk\FormIt 360\QtWebEngine\Default
* You'll need to enable hidden items in Windows Explorer to see the AppData folder.

To delete the web cache, simply delete the "Default" folder above, then reload the Plugin Manager to see the updated titles and descriptions.

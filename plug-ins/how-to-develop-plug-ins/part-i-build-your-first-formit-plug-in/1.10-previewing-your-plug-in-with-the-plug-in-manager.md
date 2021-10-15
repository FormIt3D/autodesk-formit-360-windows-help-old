# 1.10 - Previewing Your Plug-in with the Plug-in Manager

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

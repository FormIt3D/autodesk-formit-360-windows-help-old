# Previewing your Plugin with the Plugin Manager

### Install/preview locally hosted plugin from Plugin Manager

To preview how the plugin would appear in the Plugin Manager (updated title, description, etc) before it's pushed to GitHub, you can paste the localhost URL into the box at the bottom of the Plugin Manager:

![](<../../../../.gitbook/assets/image (6).png>)

Then look for your plugin in the Installed section at the top:

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerInstalledList.png)

### **Force clearing web cache for .JSON files**

If you modify the title or description inside the manifest.json file for a plugin or repo, you may need to force clear the cache in FormIt for Windows to see those changes take effect the next time you reload the Plugin Manager.

FormIt for Windows stores its web cache here, you will need to enable hidden items in Windows Explorer to see the AppData folder.

* C:\Users\user\AppData\Local\Autodesk\FormIt 360\QtWebEngine\Default

To delete the web cache, simply delete the "Default" folder above, then reload the Plugin Manager to see the updated titles and descriptions.

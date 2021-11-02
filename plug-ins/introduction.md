# Introduction to Plugins

![](../.gitbook/assets/gg4.gif)

Plugins are custom software additions that expand FormIt's core functionality. Plugins can enhance, empower, and simplify your 3D modeling workflows in FormIt.&#x20;

Plugins can be used to generate objects, make modifications to existing objects, or extract information about an object. Plugins can also use rich web interfaces to display data and provide controls and inputs directly in the application.&#x20;

## Accessing Plugins

Plugins are available in the [Plugin Manager](broken-reference) in the desktop and web versions of FormIt, as long as you are connected to the internet. Plugins are composed of a series of files and folders hosted on GitHub, or on a local server when building your own.&#x20;

![](../.gitbook/assets/c17.PNG)

### Plugins Require Internet Access

External plugins (plugins not hosted locally) require an internet connection to initially load, which means:

* External plugins will not load if no internet connection is detected when FormIt starts. Once loaded, some external plugins can continue to work in offline mode for that session, but others might break until connectivity is restored.&#x20;
* External plugins load the latest code on the server at every run, so their functionality will update whenever the author pushes a change. Plugins are loaded asynchronously, which means the order of the plugins in the FormIt interface may change with each new session.

## Open Source

Plugins are open-source, allowing you to use the plugins in the [Plugin Manager](broken-reference) free of charge, publish and share your plugins easily, and find other plugins on GitHub to understand how they're built.&#x20;

If you are a developer and want more information on how to publish your plugins, see [Hosting a Plugin on GitHub](how-to-develop-plug-ins/advanced-development/hosting-a-plugin-on-github.md).&#x20;

If you want to make a plugin for private use, you can develop and host it using a local service. For more information, see [Using an IDE. ](how-to-develop-plug-ins/advanced-development/using-an-ide.md)

![](../.gitbook/assets/c18.PNG)



## Contact Us

If you need any help with FormIt plugins, drop us a line on the [FormIt Forum](https://forums.autodesk.com/t5/formit-forum/bd-p/142).

![](../.gitbook/assets/c19.PNG)

&#x20;

&#x20;

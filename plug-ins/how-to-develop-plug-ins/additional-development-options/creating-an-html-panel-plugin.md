# Creating an HTML Panel Plugin

![](<../../../.gitbook/assets/PANEL BASED PLUGIN.gif>)

A panel-based plugin that displays an HTML page has a _manifest.json_ file with the following structure:

```
{
    "PluginName": "Hello Block!",
    "PluginType": "Panel",
    "PluginDescription": "Creates a panel with an HTML form that allows dimensional input for a 3D block which will get generated at the world origin.",
    "Scripts": [
        "PLUGINLOCATION/block.js"
    ],
    "Panel": "PLUGINLOCATION/hello_block.html",
    "PanelIcon": "PLUGINLOCATION/hello_block.png"
}               
```

In addition to the [standard JSON properties](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html#GeneralPluginSetup), a panel-based plugin includes these special JSON properties:

* "Panel" tells FormIt that this plugin is a panel, and links to the location of the HTML file that should be loaded in the panel.
* The HTML file will need links in the header to the appropriate JavaScript files, as well as to a CSS file for styling.
* The HTML file will render in the FormIt panel as it would in a browser.
* You can see examples of rich HTML interfaces in our [FormIt3D organization](https://github.com/FormIt3D/).
* "PanelIcon" defines an icon for this plugin to appear in the tab on the right side of the application. If undefined, FormIt creates an automatic icon using the initials from the name of the plugin.

Once your HTML, CSS, and JavaScript files are set up, you can begin testing your HTML panel plugin by [loading it or installing it](../advanced-development/setting-up-formit-for-development.md#load-vs.-install).

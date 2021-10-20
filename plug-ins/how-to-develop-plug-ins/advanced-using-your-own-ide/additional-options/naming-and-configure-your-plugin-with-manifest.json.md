# Plugin setup with manifest.json

FormIt plugins are comprised of a key core component called a _manifest.json_ file.&#x20;

The manifest file is a [JSON object](http://www.json.org) that tells the FormIt infrastructure what files to fetch and what kind of plugin to create.



### Manifest.json structure and properties

A _manifest.json_ file has the following structure, but has additional properties depending on whether it's a [toolbar-based](../additional-options/creating-toolbar-based-plugin.md) or a [HTML panel-based plugin](../additional-options/creating-an-html-panel-based-plugin.md)

```
{
    "PluginName": "[PluginName]",
    "PluginType": "[PluginType]"
    "PluginDescription": "[PluginDescription]",
    "Scripts": [
        "PLUGINLOCATION/[script1].js",
        "PLUGINLOCATION/[script2].js",
        ...
        "PLUGINLOCATION/[scriptn].js"
    ]
}               
```

A typical plugin includes these JSON properties:

* "PluginName" represents the name of the plugin for internal and most display purposes, including for the [Plugin Manager](https://formit3d.github.io/FormItExamplePlugins/index.html).
* "PluginType" represents the type of the plugin, so users know what to look for when they install the plugin, and is used in the [Plugin Manager](https://formit3d.github.io/FormItExamplePlugins/index.html) description.
* "PluginDescription" is used by the [Plugin Manager](https://formit3d.github.io/FormItExamplePlugins/index.html) to communicate the plugin's capabilities before installing it.
* "Scripts" lists the required external scripts associated with the plugin that will be loaded into the FormIt application and can be executed when plugin functionality is invoked.

Start your plugin development by creating a manifest.json file in your plugin folder. Next, you'll need to decide if you are making a toolbar or panel-based plugin.

**Note:** the use of PLUGINLOCATION throughout the manifest.json file above is essential and also case sensitive. FormIt will replace PLUGINLOCATION with the server location for the plugin.

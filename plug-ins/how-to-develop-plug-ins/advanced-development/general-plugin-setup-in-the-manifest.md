# General Plugin Setup in the Manifest

FormIt plugins are composed of a key core component called a _manifest.json_ file.&#x20;

The manifest file is a [JSON object](http://www.json.org) that tells the FormIt infrastructure what files to fetch and what kind of plugin to create.

### Manifest.json Structure and Properties

A manifest.json file has the following structure. It has additional properties depending on whether it's a [toolbar-based](../additional-development-options/creating-a-toolbar-based-plugin.md) or an [HTML panel-based plugin](../additional-development-options/creating-an-html-panel-plugin.md).

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
* "PluginType" represents the type of the plugin, letting users know in the [Plugin Manager](https://formit3d.github.io/FormItExamplePlugins/index.html) description what to look for when they install the plugin.
* "PluginDescription" is displayed in the [Plugin Manager](https://formit3d.github.io/FormItExamplePlugins/index.html) to communicate the plugin's capabilities.
* "Scripts" lists the required external scripts associated with the plugin that will be loaded into the FormIt application and can be executed when plugin functionality is invoked.

![](<../../../.gitbook/assets/image (4).png>)

Start your plugin development by creating a manifest.json file in your plugin folder. Next, you'll need to decide whether you are making a toolbar-based or panel-based plugin.

![](<../../../.gitbook/assets/image (13).png>)

**Note:** The use of PLUGINLOCATION throughout the manifest.json file above is essential and is case sensitive. FormIt will replace PLUGINLOCATION with the server location for the plugin.

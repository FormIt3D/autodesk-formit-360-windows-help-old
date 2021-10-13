# Creating a Toolbar Plugin

A toolbar-based plugin has a _manifest.json_ file with the following structure:

```
{
    "PluginName": "Flip Along",
    "PluginType": "Toolbar",
    "PluginDescription": "Creates a toolbar with X, Y, and Z buttons to quickly flip selected geometry in the direction of the selected axis.",
    "ToolbarURL": "PLUGINLOCATION/toolbar.json",
    "Scripts": [
        "PLUGINLOCATION/flipalong.js"
    ]
}               
```

In addition to the [standard JSON properties](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html#GeneralPluginSetup), a toolbar-based plugin includes these special JSON properties:

* "ToolbarURL" tells FormIt that this plugin is a toolbar, and links to the location of another JSON file that describes the toolbar's functionality.

After creating a manifest file like the one described above, you'll need to create the _toolbar.json_ file which defines the toolbar buttons, their names, text, icons, and the onClick function assigned to each button. The toolbar's JSON file will have the following format:

```
{
    "name": "Flip Along Toolbar",
    "buttons": [
        {
            "name": "Flip Along X",
            "command": "FlipAlongPlugin.ButtonX",
            "iconText": "X",
            "iconURL": "[Icon URL]"
        },
        {
            "name": "Flip Along Y",
            "command": "FlipAlongPlugin.ButtonY",
            "iconText": "Y",
            "iconURL": "[Icon URL]"
        },
        {
            "name": "Flip Along Z",
            "command": "FlipAlongPlugin.ButtonZ",
            "iconText": "Z",
            "iconURL": "[Icon URL]"
        }
    ]
}               
```

The _toolbar.json_ file includes these JSON properties:

* "name" represents the name of the overall toolbar, and is used internally to associate all the buttons to the single toolbar menu.
* "buttons" represent individual buttons added inside of the toolbar. A toolbar can have any number of buttons.
*
  * "name" is used to define the button's internal name which is used to associate the button to the toolbar, as well as to the button's onClick function.
  * "command" is used to define the function of the button, which can come in one of two forms: a JavaScript function (which can be defined in a script contained in the _manifest.json_ "Scripts" field), or a FormIt Command i.e. "Draw: Circle". You can obtain a list of FormIt commands by running the Messages plugin.
  * "iconText" is used to set the tooltip and description text in the button. If an icon URL is not provided, the text will create an auto-generated icon of formatted text.
  * "iconURL" can be set to use a custom icon for the button.

After the buttons have all been defined in the _toolbar.json_ file, the plugin is ready to go. If there are any additional JavaScript functions you would like to define, add them to the same folder as the _manifest.json_ file and be sure to add the file reference to the "Scripts" field of the manifest file as well so that FormIt can find the files.

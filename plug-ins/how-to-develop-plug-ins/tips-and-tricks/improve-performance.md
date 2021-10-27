# Improve Performance

## **FormIt Side vs Web Side**

FormIt runs multiple JavaScript engines simultaneously:

* The FormIt application has its own JavaScript engine
* Each plugin Toolbar has its own JavaScript engine.
* Each plugin Panel has its own JavaScript engine (Chromium)

Plugins can specify where the JavaScript is loaded:

![](../../../.gitbook/assets/d13.png)

### FormIt-side:

Specified using [manifest.json](https://github.com/FormIt3D/FormItExamplePlugins/blob/master/HelloBlockAsync/v23\_0/manifest.json#L8)

```
    "Scripts": [
        "PLUGINLOCATION/blockFormItSide.js",
        "https://formit3d.github.io/FormItExamplePlugins/SharedPluginFiles/PluginUtils18_0.js"
    ]

```

### Web-side:

Specified using[ index.html](https://github.com/FormIt3D/FormItExamplePlugins/blob/master/HelloBlockAsync/v23\_0/index.html#L7)

Web Side scripts are loaded from the web page.&#x20;

Web Side scripts can call into the FormIt Side JavaScript using multiple async calls.

### Three methods to call FormIt-side commands from a Web-based plugin:

#### Method 1 (FormItInterface.CallMethod)

CallMethod takes a function name and the arguments that will run on the FormIt Side.  The passed in function will be called with the result of the function call.

```
    var args = {
        "w": 10,
        "l": 10,
        "h": 10
    }
    FormItInterface.CallMethod("CreateBlock", args, function(result)
    {
        // Result of the function call
    });
```

Pros: No await needed.&#x20;

Cons: A callback is needed to get the result and is called “who knows when”. Scripts defined in two different places. Requires plugin logic to be split into two different files.

## Quick Reloading

💡** **You can reload a plugin on the web without reloading the whole app (same as in Windows) via right-clicking and selecting `Reload Frame`

![](../../../.gitbook/assets/d11.png)

# Creating an Add-In

An Add-In is a plugin that also loads DLLs that expose new JavaScript APIs.&#x20;



### Download FormIt API

To build DLLs that support FormIt, the FormIt API is needed. The FormIt API can be downloaded from the [Autdesk Developers Network](https://www.autodesk.com/developer-network/overview). A login is needed to access the download.&#x20;

Once logged in, the FormIt API is available under SOFTWARE.

&#x20;

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/FormItAPIDownload.jpg)

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/FormItAPIMenuItem.jpg)

An Add-In has access to the [FormIt API](https://formit3d.github.io/FormItExamplePlugins/docs/FormItCPPAPI/index.html) and [FormIt Modeling Kernel C++ API](https://formit3d.github.io/FormItExamplePlugins/docs/FormItCPPAPI/group\_\_mod\_\_wsm\_\_api\_\_ref.html).

An add-in has the following structure:

```
            // FormIt looks for REGISTERAPIMETHODS to load new JS APIs
            REGISTERAPIMETHODS
            {
                // Declare new namespace for the new JS APIs
                REGISTERNAMESPACE("HelloDLL")
                // Create a JS API with no arguments
                APIMETHOD(HelloDLL, API1, "") {}
                // Create a JS API with 1 argument
                APIMETHOD(HelloDLL, API2, "arg1") {}
                // Create a JS API with 2 argument
                APIMETHOD(HelloDLL, API3, "arg1, arg2") {}
                ...
                ...
            }
        
```

To get the arguements into C++ variables use SCRIPTCONVERTER-

```
            // Create a JS API with 2 argument
            APIMETHOD(HelloDLL, API3, "arg1, arg2")
            {
                // NOTE: The arg names above ^^^^ have to match the args in the macros below.
                // arg1 expects a bool
                SCRIPTCONVERTER(bool, arg1);
                // arg2 expects an int
                SCRIPTCONVERTER(int, arg2);
                return JSON_UNDEFINED;
            }
        
```

Either JSON\_UNDEFINED or any json object can be returned. Use to\_json to convert your C++ variable to json

```
            // Create a JS API with 2 argument
            APIMETHOD(HelloDLL, API3, "arg1, arg2")
            {
                // NOTE: The arg names above ^^^^ have to match the args in the macros below.
                // arg1 expects a bool
                SCRIPTCONVERTER(bool, arg1);
                // arg2 expects an int
                SCRIPTCONVERTER(int, arg2);

                std::string myValue = "Test";
                return to_json(myValue);
            }
        
```

Once the DLL is defining all the needed JS APIs, the plugin must tell FormIt what DLLs need loaded. This is done in the [manifest](https://github.com/FormIt3D/HelloAddIn/blob/main/v22\_0/manifest.json#L8).

```
        "DLLs" : ["PLUGINLOCATION/MyClass.dll", "PLUGINLOCATION/HelloDLL.dll"]
        
```

[HelloAddIn](https://github.com/FormIt3D/HelloAddIn) is a working example that explains how to make an Add-In.

[HelloWSMAddIn](https://github.com/FormIt3D/HelloWSMAddIn) is a working example that explains how to make an Add-In with the [FormIt Modeling Kernel C++ API](https://formit3d.github.io/FormItExamplePlugins/docs/FormItCPPAPI/group\_\_mod\_\_wsm\_\_api\_\_ref.html).

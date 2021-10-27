# How Do I Connect to Other Services?

## **Connecting Plugins With Dynamo**

FormIt 2022.1 and newer offers access to JavaScript APIs and custom functions from Dynamo via two new nodes:

### **CallJSAPI** <a href="calljsapi" id="calljsapi"></a>

The **CallJSAPI** node allows you to invoke FormIt JavaScript APIs directly from Dynamo.

![](https://formit.autodesk.com/page/formit-dynamo/dynamo-formitCallJSAPI-GetTotalGrossArea.png)

For function names and parameters, take a look at our JavaScript documentation, which is divided into two parts: [FormIt API](https://formit3d.github.io/FormItExamplePlugins/docs/FormItJSAPI/group\_\_mod\_\_jsapi\_\_formit.html) and [WSM API](https://formit3d.github.io/FormItExamplePlugins/docs/FormItJSAPI/group\_\_mod\_\_jsapi\_\_wsm.html) (modeling kernel).

### **CallPluginJS** <a href="callpluginjs" id="callpluginjs"></a>

Conversely, the **CallPluginJS** node allows you to invoke custom functions from a loaded plugin, or a script snippet that's been executed from the Script Editor window.

![](https://formit.autodesk.com/page/formit-dynamo/dynamo-formitCallPluginJS.png)

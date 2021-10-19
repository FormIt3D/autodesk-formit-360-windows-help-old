# Host local server

Before you can preview a clone plugin in FormIt, you need to host it on a local server in order to deploy it in both FormIt web/desktop

### **Start local server from IDE**

You have the option of starting the server inside Visual Studio Code, instead of from a separate terminal window, in your Visual Studio Code, open your project folder (to make s:

View > Terminal (or shortcut Ctrl + \`)

![](broken-reference)

Simply run the command to start your npm http-server from previous steps:&#x20;

```
http-server
```

1. You can verify your server by navigate to the following: http://localhost:8080/YourPluginFolder/manifest.json
2.  FormIt for Windows only requires a simple HTTP server to host plugins on a local web server.

    An HTTP server that works well is npm's [http-server](https://www.npmjs.com/package/http-server), which you can install by:

    * First, download and install [NodeJS](https://nodejs.org/en/) if it's not already installed (one-time setup).
    *
      * If you encounter errors in the following steps, try restarting your computer for the NodeJS installation to complete.
    * In the Command Prompt, enter the following to install npm's _http-server_ globally (one-time setup):
    *
      * npm install http-server -g
    * In Command Prompt, navigate to the directory containing the folders of repos you've cloned.
    * Run the following:
    *
      * http-server



**Verify the Web Server**

* In a web browser, navigate to the following: [\
  &#x20;   http://localhost:8080/YourPluginFolder/manifest.json\
  ](http://localhost:8080/YourPluginFolder/manifest.json)
* You should see a json object in the browser window.
* If you use a different web server than npm, the default address/port might be different.


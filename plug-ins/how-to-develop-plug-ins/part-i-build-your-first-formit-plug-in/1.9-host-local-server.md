# Host local server

Before you can use it in formit, you need to host it on a server, perhaps a local server in order to deploy it in the formit web/desktop

**Start your server from the IDE**

Now, you have the option of starting the server you installed previously right inside Visual Studio Code, instead of from a separate terminal window:

1. View > Terminal (or shortcut Ctrl + \`)
2.  You should already be in the correct folder, so simply run the command to start your npm http-server from previous steps: 

    ```
    http-server
    ```
3. You can verify your server by navigate to the following: http://localhost:8080/YourPluginFolder/manifest.json
4.  FormIt for Windows only requires a simple HTTP server to host plugins on a local web server.

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




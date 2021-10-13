# Setting up your Environment



Plugin development is supported in FormIt for Windows and FormIt for Web.

#### Get the Source Code

* You can clone various first-party FormIt plugin repos, which demonstrate different UI types and some advanced functionality that can be achieved with plugins.
* Each first-party plugin is now stored in its own repo. You'll find them all here:
* [FormIt3D Organization Repos](https://github.com/FormIt3D)
* You can also download [GitHub Desktop](https://desktop.github.com), which provides an easy-to-use interface for cloning repos, seeing changes to files, and pushing/pulling changes between your local computer and online repos.

#### Start a Web Server

**FormIt for Windows**

FormIt for Windows only requires a simple HTTP server to host plugins on a local web server.

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

* In a web browser, navigate to the following:
*
  * http://localhost:8080/YourPluginFolder/manifest.json
* You should see a json object in the browser window.
* If you use a different web server than npm, the default address/port might be different.

**FormIt for Web**

To develop on FormIt Web, simply run the following command instead:

* http-server --cors

You can verify the web server in the same way as outlined above for Windows.

#### Install an IDE

Write your code in an integrated development environment (IDE) that helps identify issues, correct syntax errors, and includes a terminal for running your local server.

A free IDE that works well for FormIt plugin development is Microsoft's [Visual Studio Code](https://code.visualstudio.com/Download).

Once installed:

* File > Open Folder
* Select the folder that contains your plugin files and folders.

**Optionally start your server from the IDE**

Now, you have the option of starting the server you installed previously right inside Visual Studio Code, instead of from a separate terminal window:

* View > Terminal (or shortcut Ctrl + \`)
* You should already be in the correct folder, so simply run the command to start your npm http-server from previous steps:
* http-server
* You can confirm your server is running correctly by following the "Verify the Web Server" steps above.

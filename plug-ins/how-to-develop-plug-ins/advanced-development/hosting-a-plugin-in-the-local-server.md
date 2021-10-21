# Hosting a Plugin in the Local Server

Before you can preview a clone plugin in FormIt, you need to host it on a local server in order to deploy it in both FormIt web/desktop

### **View terminal from IDE**

You have the option of starting the server inside Visual Studio Code, instead of from a separate terminal window, make sure the right folder is opened in Visual Studio Code before opening a terminal:

View > Terminal (or shortcut Ctrl + \`)

![](<../../../.gitbook/assets/image (4) (1).png>)

### Setup http server

An HTTP server that works well is npm's [http-server](https://www.npmjs.com/package/http-server)

First you will need to download and install [NodeJS](https://nodejs.org/en/) (this is a one-time setup, do this if NodeJS is not already installed)

If you encounter errors in the following steps, try restarting your computer for the NodeJS installation to complete.

In the Command Prompt, enter the following to install npm's _http-server_ globally (also a one-time setup)

* `npm install http-server -g`

![](<../../../.gitbook/assets/image (14) (1).png>)

### Start local server

Once the setup is complete, simply run the following command in the terminal to start your npm http-server

* `http-server`

![](<../../../.gitbook/assets/image (21).png>)



### Develop for FormIt for Web

To develop on FormIt Web, simply run the following command instead:

* `http-server --cors`

![](<../../../.gitbook/assets/image (5).png>)

###

### Verify your server

You can verify your server by navigating to the following address in your web browser:&#x20;

* http://localhost:8080

You should see your project folder files in the browser window.

\*\*If you use a different web server than npm, the default address/port might be different.

![](<../../../.gitbook/assets/image (13) (1).png>)


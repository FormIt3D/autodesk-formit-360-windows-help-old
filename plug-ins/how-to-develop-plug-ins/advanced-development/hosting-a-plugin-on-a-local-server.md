# Hosting a Plugin on a Local Server

Before you can preview a cloned plugin in FormIt, you need to host it on a local server.

### **View the Terminal in IDE**

You have the option of starting the server inside Visual Studio Code, instead of a separate terminal window.** **Before opening a terminal, make sure the right folder is opened in Visual Studio Code.

View > Terminal (or shortcut Ctrl + \`)

![](<../../../.gitbook/assets/image (4) (1).png>)

### Set Up an HTTP Server

An HTTP server that works well is npm's [http-server](https://www.npmjs.com/package/http-server).

First, you will need to download and install [NodeJS](https://nodejs.org/en/), if it's not already installed.

If you encounter errors in the following steps, try restarting your computer to complete the NodeJS installation.

In the Command Prompt, enter the following to install npm's _http-server_ globally (a one-time setup).

* `npm install http-server -g`

![](<../../../.gitbook/assets/image (14) (1) (1).png>)

### Start the Local Server

Once the setup is complete, run the following command in the terminal to start your npm http-server:

* `http-server`

![](<../../../.gitbook/assets/image (21).png>)

Tip 1: In case of any issues with running the http-server (installed globally or locally), it may be helpful to run it directly via npx:

* `npx http-server`

Tip 2: For Windows 10/11 users, if you encounter an error when running a script on your new machine, this may be due to the settings being disabled. To fix this:

* Launch PowerShell script as an administrator&#x20;
* Enter: `Set-ExecutionPolicy RemoteSigned `

### Develop for FormIt Web

To develop for FormIt Web, simply run the following command instead:

* `http-server --cors`

![](<../../../.gitbook/assets/image (5).png>)

### Verify Your Server

You can verify your server by navigating to the following address in your web browser:&#x20;

* http://localhost:8080

You should see your project folder files in the browser window.

\*\*If you use a different web server than npm, the default address/port might be different.

![](<../../../.gitbook/assets/image (13) (1).png>)


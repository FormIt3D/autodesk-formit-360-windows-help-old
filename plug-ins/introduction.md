# Introduction to Plugins

## What Are Plugins?

 Plug-ins are additions that expand FormIt's core functionality. Created to help enhance/empower/simplify the modeling process, productivity, or workflow when 3d modeling in FormIt. Plug-ins can be used for generating objects, making modifications or extracting info & properties of an object. Features of plug-ins may be as simple as fillet 2 edges, or as advance as generating a string of light fixtures. You may find plug-ins developed by the communities or Autodesk from GitHub. You may even create your own plug-ins to suit the needs of different project.

![](../.gitbook/assets/g1.gif)

## Where are they available?

They are available both on desktop or web version, as long as you have an internet connection. You can find them on the [plugin manager](how-to-use-plug-ins/the-plugin-manager.md)

**(DIFFERENCES BETWEEN DESKTOP AND WEB?)** 

## Are they open source?

Plugins are open source.....Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

**(LICENSE MORE INFO?)**

## Connectivity to services

Talk about connectivity to different services.

**(WHICH ONES SHOULD WE TALK ABOUT?)**

## **Using Formit Plugins for Concept Modeling** 

Are you a developer looking for a concept modeling environment? If you are interested in developing plug-ins go to the following section on[ how to develop plugins](how-to-develop-plug-ins/)

**(ADD SPECIFIC SECTION ABOUT CONCEPT MODELING)**

## How Plugins Work

Plugins are comprised of a series of files and folders hosted on GitHub, or on a local server when building your own.

### Plugins and connection

External plugins (plugins not hosted locally) require an internet connection to initially load, which means:

External plugins will not load if no internet connection is detected when FormIt starts. Once loaded, some external plugins can continue to work in offline mode for that session, but others might break until connectivity is restored. External plugins load the latest code on the server at every run, so their functionality will update whenever the author pushes a change. Plugins are loaded asynchronously, which means the order of the plugins in the FormIt interface may change with each new session. 

The Plugin Manager uses registry keys on Windows to store your installed repositories and plugins.

### Resetting the plugin manager

If you need to reset your Plugin Manager to its defaults, delete the following registry key:

* Computer\HKEY_CURRENT_USER\Software\Autodesk\FormIt 360\Plugins
* Note this will uninstall all user-added repos and plugins, resetting the Plugin Manager to include only the built-in repos and plugins.

## Need any help?

If you need any help with Formit Plugins drop us a line on the [Autodesk forums](https://forums.autodesk.com/t5/formit-forum/bd-p/142)



 

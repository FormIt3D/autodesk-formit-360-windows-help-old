# 1.12 - Publish your project and hosting on GitHub

Built a useful plugin that you want to share? Host your repository on GitHub so others can install your plugins from the [Plugin Manager](https://formit3d.github.io/FormItExamplePlugins/index.html)!

**Hosting Your Repo + Plugins on GitHub**

* Sign up for a free [GitHub account](https://github.com/join).
* Download [GitHub Desktop](https://desktop.github.com), a free tool for cloning repos, seeing changes to files, and pushing/pulling changes between your local computer and online repositories.
* Create a new repo to host your plugin on GitHub.
* Use GitHub Desktop to clone your new (empty) GitHub repository to your local machine.
* Develop your plugin by adding new files to the repo folder locally.
* Use GitHub Desktop to push your plugin files and directories to your repository.
* Enable GitHub Pages in your repository so FormIt can load and display your GitHub-hosted plugins.
*
  * Go to your new GitHub plugins repo, i.e. https://github.com/Joe/JoesPlugins
  * In the top-right corner, click the Settings tab.
  * Scroll down to the GitHub Pages section, enable GitHub Pages, and use the _master_ branch.

At this point, you can continue adding, modifying, and testing plugins locally, and when you're ready to publish, use GitHub Desktop or another Git client to push your changes to your GitHub repo. Anyone consuming your repo and plugins will always get the latest code when they start FormIt.



For project created in an IDE instead of [Plugin Playground](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html#PluginPlayground), you can publish your plugin by:

*   Adding a **formit-plugin** topic to your plugin's repository

    ![plugin topic](https://formit3d.github.io/FormItExamplePlugins/docs/images/topic.png)
*   Enabling GitHub pages on your project. This can be found and set in the Setting tabs of your repository.

    Under the **GitHub Pages** section, choose the branch you want to use. Typically choose **master** or **main**.

    ![install pages](https://formit3d.github.io/FormItExamplePlugins/docs/images/pages.png)

If you'd like your plugin to appear under the list of recommended plugins in the Plugin Manager, add an additional topic to your repository, **formit-plugin-recommended**. The FormIt team will then review your plugin.

###

# 插件

使用“插件管理器”从 FormIt 团队安装有用的插件，或了解如何[**构建您自己的 FormIt 插件**](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)**。**

#### FormIt 插件管理器

“FormIt 插件管理器”用作发现和管理 Formit 插件的中心。

只要 FormIt 可以访问 Internet，则当 FormIt 启动时就会自动加载“插件管理器”。

通过单击应用程序窗口右侧的“插件管理器”选项卡图标，可以访问该插件管理器：

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerTab.PNG)

#### “插件管理器”会对不同类型的插件进行分类：

* **已安装的插件**
* **建议的插件**
   * FormIt 团队建议用于扩展 FormIt 的核心功能并解锁新工作流的插件。
   * 社区开发的插件在获得 FormIt 团队批准后将显示在此处。以后将对此进行详细介绍。
* **公共插件**
   * 由社区构建的插件，但尚未由 FormIt 团队审阅或批准。

#### “插件管理器”是使用一系列可展开和可收拢的界面进行设计的，这使管理插件及其存储库变得轻松：

* **管理插件：**
   * 单击插件名称，即可查看其说明。
   * 切换开关，即可安装或卸载它。
      * 该插件将显示为应用程序顶部的工具栏、右侧的面板或中间的对话框，具体取决于插件类型。
* 如果您正在[开发自己的插件](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)，可以将其私有 URL 添加到底部的字段中，然后点击 (+)：

![FormIt 插件管理器](https://formit3d.github.io/FormItExamplePlugins/docs/images/addNew.png)

#### 插件的工作方式

* 插件是基于 Web 的，在 FormIt for Windows 和 FormIt for Web 中可用。
* 插件由托管在 GitHub 或本地服务器（构建自己的插件时）上的一些列文件和文件夹组成。
* 外部插件（插件不在本地托管）需要 Internet 连接，才能初始加载，这意味着：
   * 如果在 FormIt 启动时未检测到 Internet 连接，则将加载外部插件。
   * 加载后，一些外部插件可以继续在脱机模式下为该任务工作，但其他外部插件可能会中断工作，直到恢复连接。
   * 外部插件在每次运行时都在服务器上加载最新代码，因此只要作者推送更改，其功能就会更新。
* 插件异步加载，这意味着 FormIt 界面中插件的顺序可能会随每个新任务而变化。
* “插件管理器”使用 Windows 上的注册表项，来存储您安装的储存库和插件。
   * 如果需要将“插件管理器”重置为其默认值，请删除以下注册表项：
      * Computer\HKEY\_CURRENT\_USER\Software\Autodesk\FormIt 360\Plugins
      * 请注意，这将卸载用户添加的所有存储库和插件，从而重置“插件管理器”以仅包含内置的存储库和插件。


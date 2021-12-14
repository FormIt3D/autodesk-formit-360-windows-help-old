# 常见问题解答

## 关于 FormIt

**什么是 FormIt 和 FormIt Pro？**

FormIt 是用于建筑设计的三维建模、可视化、分析和计算环境。

FormIt 功能：

* 强健的实体建模引擎，具有针对建筑设计优化的强大工具和工作流
* 增强的环境可视化以展示设计选项，包括使用场景保存的模型状态
* 使用必应地图的位置、卫星图像和三维地形
* Autodesk 材质库中的材质
* 模型组织和可见性工具，如组、图层和场景
* 分析工具，包括：
   * 无间隙面和背面验证，用于实体模型诊断和修复
   * 日光和阴影
   * 日光分析
   * 能量分析
* Autodesk 产品集成：
   * BIM 360 Docs
   * Insight（能量分析）
   * [Dynamo](https://formit.autodesk.com/page/formit-dynamo)
   * [Revit](https://formit.autodesk.com/page/formit-revit)
* 文件格式支持：
   * 打开/输入
      * AXM、DWG、FBX、SAT、STL、OBJ、WSM、SketchUp、图像
   * 导出
      * AXM、FBX、OBJ、STL、SAT、DAE、DXF

FormIt 可在 [iOS](https://itunes.apple.com/us/app/autodesk-formit-360/id575282599?mt=8) 和[浏览器](https://app.formit.autodesk.com/)中免费使用。需要 **FormIt Pro** 固定期限的使用许可，才能使用 [FormIt for Windows](https://formit.autodesk.com/page/download)，这一版本的 FormIt 的功能最强大也最丰富。**FormIt Pro** 固定期限的使用许可还支持在 iOS 和 Web 上使用其他功能，如日光和能量分析。**FormIt Pro** 包含在 [Autodesk 工程建设软件集](https://www.autodesk.com.cn/collections/architecture-engineering-construction/overview) 中。

**FormIt for Android 发生了什么情况？**

为了精简 FormIt 产品，我们不得不做出停止 Android 应用程序的艰难决定。如果已安装，它将继续运行，但不再可从 Play Store 获取。

**如何获取 FormIt？**

要运行 Windows 版本，您必须有权访问 **FormIt Pro**，它是[工程建设行业软件集](https://www.autodesk.com.cn/collections/architecture-engineering-construction/overview)固定期限的使用许可的一部分。因此，如果您的办公室有 Revit，则很可能您已经有权访问 FormIt！可以[直接从我们的网站下载 FormIt for Windows](https://formit.autodesk.com/page/download)，也可以从 Autodesk 桌面应用程序下载。

此外，还可以从我们的网站直接免费运行 Web 版本：[http://formit.autodesk.com](http://formit.autodesk.com)

可以从 Apple App Store 免费下载 iOS 版本（仅限 iPad）。

**如果我是学生或教师，是否可以免费获得 FormIt Pro 访问权限？**

是的！您可以通过 [Autodesk 教育门户](https://www.autodesk.com.cn/education/edu-software/overview?sorting=featured&page=1)访问 FormIt Pro 固定期限的使用许可。

**如何学习使用 FormIt？**

最好从 [FormIt Primer 教程](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html)开始。

本入门手册有多个部分，从初学者（创建整个现代住宅）到更高级的操作（以更高级的方式使用 Revit 和 Dynamo）。

在 FormIt Friday 网络讲座系列中，我们还提供有 20 多个视频。可以在 [YouTube 频道](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH)上找到这些视频。

## 使用 Revit

**FormIt 如何与 Revit 配合使用？**

FormIt 是一款独立的三维草图绘制和设计应用程序，但它创建的数据可以[使用 FormIt Add-In for Revit](https://formit.autodesk.com/page/formit-revit) 轻松转换为 Revit。

**输入到 Revit 时会发生什么情况？**

自 2016 年开始，Revit 会随附一个用于使用 FormIt 数据的附加模块。将 FormIt AXM 文件输入 Revit 时，该附加模块会查看文件中的每个对象，然后使用相应 API 在 Revit 中重新创建。默认情况下，FormIt 中的所有内容都分类为“体量”。

FormIt 转换器会获取每个体量对象，并使用 [Direct Shape API](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/CHS/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html) 在 Revit 中创建体量族。

“Direct Shape”是 IFC 工作流中所使用的不可编辑对象。尽管它不可编辑，但它具有在 FormIt 和 Revit 之间传输完整材质纹理的显著优势。[此处获取教程](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html)，该教程详细介绍了 FormIt 到 Revit 的工作流。

**FormIt 是否可以创建墙、楼板和其他 Revit 系统族？**

并非直接创建。如上所述，每个对象都默认为“体量”类别。创建墙、楼板等的步骤您应使用转换器附加模块将模型输入 Revit，然后使用原生 Revit 工具从基本体量模型创建系统族。

**Revit 是否可以将数据发送回 FormIt？**

可以。要将数据输入回 FormIt，请将 Revit 文件的全部或_部分_（最好）输出为 SAT 文件格式。通常，不需要将所有 Revit 数据发送到 FormIt。相反，在 Revit 中创建仅包含最少数据（例如，楼板和墙）的过滤视图，然后再保存为 SAT。

## 使用其他应用程序

**为什么默认文件格式为“.AXM”？**

FormIt 正式命名之前的内部代号为 XModeler - 因此我们创建的文件格式是 Autodesk X Modeler 或 AXM（简写）。

**FormIt 可以输入哪种类型的三维格式？**

* Windows：AXM、DWG、FBX、OBJ、SAT、SKP、STL
* Web：OBJ、STL
* iOS：OBJ、STL、SAT

**FormIt 可以输出哪些类型的格式？**

* Windows：FBX、OBJ、SAT、STL、DAE、DXF
* Web：OBJ、SAT、STL
* iOS：OBJ

**FormIt 如何与 Dynamo 配合使用？**

[了解 FormIt 和 Dynamo 如何协同工作](https://formit.autodesk.com/page/formit-dynamo)，以创建计算设计工作流。

**FormIt 与 SketchUp 相比如何？**

* [**与 Revit 的互操作性更好**](../tool-library/revit.md) ****
* [**Dynamo 集成**](../tool-library/dynamo.md)（用于计算设计）
* Autodesk Insight 支持用于[**日光分析**](../tool-library/solar-analysis.md)和[**能量分析**](../tool-library/energy-analysis.md)的原生工具
* 更强健的实体建模内核，支持高级建模操作
* 原生高级建模工具，如[**扫掠、覆盖、放样**](../tool-library/cover-sweep-loft.md)、偏移/壳实体和三维过渡/圆角以及[**展平面**](../tool-library/flatten-face.md)
* 多个可见[**剖切平面**](../tool-library/section-planes.md)
* 诊断工具，如[**显示无间隙问题和显示背面**](../tool-library/visual-styles.md)
* [**输出模型的各个部分**](../tool-library/export-data.md)（基于所选内容和/或可见内容）
* 原生 OBJ、SAT 和 STL 输出

**是否可以使用自己的 SketchUp 键盘快捷键？**

是的！FormIt for Windows 具有完全可编辑的键盘映射。默认情况下，许多常用的 SketchUp 快捷键已存在，但可以在“编辑”>“首选项”菜单中进行编辑。

**是否可以使用自己的 DWG 文件？**

是的！FormIt 可输入二维和三维 DWG 文件。

## 常见支持问题

**如何获取支持？**

可以先与 Autodesk 经销商联系，也可以在 [FormIt 论坛](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=zh-CN)上联系我们。最好先搜索您遇到的问题，如果尚未解答，请发布新主题，FormIt 团队会回复。

**如果无法登录，该怎么办？**

* 此[论坛帖子](https://forums.autodesk.com/t5/formit-forum/having-trouble-logging-into-formit-for-windows-try-these-steps/td-p/7179572?profile.language=zh-CN)介绍了常见登录问题
* 如果您的 PC 具有可切换的图形处理器 (GPU)，请务必确保 FormIt 始终使用性能更高的 GPU。以下是有关 [AMD](https://community.amd.com/docs/DOC-1581#jive_content_id_Assigning_Applications_to_GPUs) 和 [NVIDIA](http://nvidia.custhelp.com/app/answers/detail/a_id/2615/kw/manage%203d%20settings/related/1) 的说明

**如果 Insight 能量分析失败，该怎么办？**

如果 Insight 能量分析报告错误或无法返回任何结果，请[查看我们的 Insight 能量分析页面](https://formit.autodesk.com/page/formit-insight)，以了解常见疑难解答提示。


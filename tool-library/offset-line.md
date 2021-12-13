# 偏移线

使用“偏移线”工具绘制平行线或偏移线。这对于创建二维形状非常有用，稍后可以拉伸该形状以使其看起来像三维墙。

![](../.gitbook/assets/image%20%283%29.png)

**“偏移线”**工具的工作方式与[**“线”**](https://windows.help.formit.autodesk.com/tool-library/line-tool)工具类似：

* 单击以设置第一个点，然后移动光标并放置后续点，从而捕捉到现有几何图形或推断轴。
* 将显示生成形状的预览。第二个点和第三个点确定其余点要跟随的平面，因此结果为平面。
* 继续添加点，然后按 **Esc** 键或双击以完成工具。
* 将清理和合并任何自交，从而保留一个可拉伸面。

![放置 2 个点并拖动第 3 个点后](../.gitbook/assets/walls1.png)

输入线以红色绘制，默认放置于偏移线的中心。

通过点击 **Tab** 键，可以更改偏移线的对齐方式及其厚度。这将调用**“工具选项”**对话框：

![“偏移线”工具的选项](../.gitbook/assets/walls2.png)

例如，将**“对齐”**更改为**“左”**，将**“厚度”**更改为“6"”，偏移线将绘制在输入线的左侧，相距 6 英寸。

![](../.gitbook/assets/walls3.png)

## 实用提示

可以通过捕捉到放置的第一个点，来绘制闭合形状。将自动清理生成的拐角：

![](../.gitbook/assets/walls4.png)

可以自由地绘制彼此顶部的输入线。工具完成后，将清理生成的交点。

![](../.gitbook/assets/walls5.png)

![](../.gitbook/assets/walls6.png)

固有地，“偏移线”工具必须在平面上生成几何图形，因此前几个点确定其余点将跟随的平面。

例如，开始在立方体的侧面绘制，以使用该面的平面。在放置三个非共线点后，将为其余输入固定输入平面。请注意，在面上绘制时，生成的形状将插入到该面中，从而将其分割为多个面。要防止插入，在其上进行绘制的面必须是[组](https://windows.help.formit.autodesk.com/tool-library/groups)的一部分。

![在垂直面上绘制](../.gitbook/assets/walls7.png)

![工具结束后，将插入线，并且可以进一步操纵分割面](../.gitbook/assets/walls8.png)

还可以使用“偏移线”工具，在平面图形中进行追踪。将平面作为图像输入。

* 调整图像大小，以使平面具有正确的比例。有关更多详细信息，请单击[此处](https://windows.help.formit.autodesk.com/building-the-farnsworth-house/work-with-images-and-the-ground-plane)。
* 可以使用[“正交相机”](orthographic-camera.md)，以在正交[俯视图](orthographic-views.md)中进行跟踪。

![](../.gitbook/assets/walls9.png)

![](../.gitbook/assets/walls10.png)




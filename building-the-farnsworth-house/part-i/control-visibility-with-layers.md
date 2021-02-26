# 1.6 - Control Visibility with Layers

_Much like AutoCAD and Photoshop, Layers in FormIt allow you to manage the visibility of objects in your model. In this chapter, we are going to create a layer to save and hide the building mass for future analysis._

_If you did not complete the last section, download and open the_ _**1.6 - Control Visibility with Layers.axm**_ _file from the_ _**FormIt Primer Part 1 Datasets**._

## **Create Layers**

1 - To create the new layers:

1. Go to the **Layers Palette** and click the **+** sign three times to create three layers.
2. Double-click the layer names to rename them **Massing**, **Main Building Floor**, and **Plan Image.**

![](../../.gitbook/assets/0%20%2813%29.png)

_**Note:**_ _You can click on a layer name and drag it up or down to re-order the layers._

2 - To assign the **Massing - Main Building** group to the **Massing** layer:

1. In the canvas, select the **Massing - Main Building** group.
2. In the **Layers Palette** choose the **Massing** layer from the “**Selection On:”** drop-down menu. Similarly, assign the **Plan Image** group to the **Plan Image** layer.

![](../../.gitbook/assets/1%20%289%29.png)

## **Duplicate Group**

_We will now start the process of modeling the building in more detail. The first step is to create the floor geometry based on the building massing we already have._

1 - Select the **Massing - Main Building** group again. Press **Ctrl + C \(Copy\)** to copy, and then **Ctrl + Shift + V \(Paste in Place\)** to paste the mass in the same place.

2 - To dissociate the new group geometry from the original group: right-click to access the **Context Menu**, and choose the **Make Unique \(MU\)** option.

![](../../.gitbook/assets/2%20%2812%29.png)

_**Note**: The new group is no longer associated with the original. Changes to the new group will not alter the original group._

## **Create the Floor Geometry**

1 - Reassign group’s layer:

1. Single-click to select either of the **Massing – Main Building** groups.
2. Put the group on the **Main Building Floor** layer using the “**Selection On:”** drop-down in the **Layers Palette**.
3. Uncheck the **Massing** layer to hide its geometry and keep it safe from any accidental edits.

![](../../.gitbook/assets/3%20%2812%29.png)

2 - Double-click the visible **Massing – Main Building** group to edit it. Re-name the group **Floor** in the **Properties Palette**.

![](../../.gitbook/assets/4%20%286%29.png)

3 - **Single-click** the geometry’s **top face** to select it. Click again and start dragging the face down. As you drag the face down, type **11’-2”**, and the **Dimension Dialog** will appear. Click on **OK** after entering the value. The resulting floor should be 1' thick. Double-click off in space to exit the group.

![](../../.gitbook/assets/5%20%286%29.png)


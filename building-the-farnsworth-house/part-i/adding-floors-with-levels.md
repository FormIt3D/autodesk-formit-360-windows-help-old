# 1.4 - Add Floors with Levels

_Levels allow you to slice masses with individual floor datums and calculate gross area per building mass. FormIt Levels and their custom names will translate to Revit Levels when the file gets converted to Revit._

_If you did not complete the last section, download and open the **1.4 - Add Floors with Levels.axm axm** file from the **Farnsworth House Data Set**._

## **Create, and Customize Levels**

1 - To create levels:

1. Go to the **Level Palette** in the **Palette Bar**.
2. Click **+** \(**Add Level**\) four times to create four Levels.
3. Double-click each level’s current elevation to modify them to: **0’-0", 2'-2", 4’-6"** and **17’-8"**.
4. Double-click each level’s current name and rename them: **Ground, Terrace, Main Building,** and **Top of Roof.**

![](../../.gitbook/assets/0%20%285%29.png)

_**Note**: You can click the_ _**++**_ _icon to create multiple levels, with a specified and uniform distance apart. This is handy for multi-story buildings_.

## **Apply Levels to Geometry**

_In the previous steps, we only created levels. Now we are ready to apply those levels to the geometry we have created._

1 - To apply levels to the exiting geometry:

1. Select the entire upper terrace mass by double-clicking it.
2. In the **Properties Palette**, click **Use Levels**. This step will pre-select all levels that currently intersect the selected geometry.
3. Now the currently selected geometry has three levels applied to it \(**Main Building, Terrace,** and **Ground**\), but for this exercise, we only want to apply **Ground**. Uncheck **Main Building** and **Terrace**.
4. This process ensures that only the area intersected by **Ground** is considered for the gross area calculation, which can be seen in the **Area by Level** field.

![](../../.gitbook/assets/1%20%284%29.png)

_**Note**: If you do not see blue level lines on your mass, type_ _**DL**_ _to_ _**Display Levels**._

![](../../.gitbook/assets/2%20%283%29.png)


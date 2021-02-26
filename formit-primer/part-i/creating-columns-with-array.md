# 1.8 - Create Columns with Array

_In this exercise, we will sketch a detailed element - an I-beam column. Then we will use the Array tool to quickly create multiple equally-spaced copies._

_If you did not complete the last section, download and open the_ _**1.8 – Create Columns with Array.axm**_ _file from the_ _**FormIt Primer Part 1 Datasets**._

## **Sketch the Column Profile**

1 - To facilitate the drafting process:

1. Go to the **Top View \(VT\)**.
2. Switch the view mode to **Orthographic \(VO\)**.
3. Turn off the **Main Building** **Floor** and **Roof** layers. This step will prevent the new geometry from snaping to the existing geometry on those layers.
4. Zoom into the upper left corner of the **imported floor plan** image so you can view the column in detail.
5. Turn off the **Snap to Grid \(SG\)** feature \(if you have it on\). This will help with drawing the detail lines.

![](../../.gitbook/assets/0%20%2813%29.png)

_To draw the column, we will first draw one half, then mirror it to quickly create the other symmetrical half._

2 - To create the first half of the I-beam, use the **Line tool \(L\)** to make the following sketch using the specified dimensions. Don’t worry about the exact position of the column on the plan image just yet.

![](../../.gitbook/assets/1%20%2818%29.png)

3 - To mirror the shape you have just drawn:

1. Double-click to select all the faces and edges of the drawn geometry.
2. Right-click and select the **Mirror Tool \(MI\)**.
3. Click on the center orange grip of the **Mirror Widget** and place it at the geometry’s bottom left corner.
4. Use the bottom arrow from the double-sided arrow button in the Widget to rotate the mirroring-axis -90 degrees \(clockwise\).
5. Single-click off in space, or press **Esc** to finish the mirroring process. The result should look like an I-beam profile with a line down the middle. Press **Esc** again to clear the selection.

![](../../.gitbook/assets/2%20%285%29.png)

![](../../.gitbook/assets/3%20%287%29.png)

_**Note**: The final geometry location and orientation is previewed with the ghosted blue shape while you are adjusting the mirror widget. You can use this preview as a reference to mirror the geometry to the intended location._

4 - To join both sides into a single geometry, remove the line dividing them by clicking on it to select it and then pressing **Delete**. Now the two surfaces are joined into a single surface.

5 - To move the geometry to its final location:

1. If off, turn on the **Plan Image** and **Roof** layers, to use them as a guide.
2. Double-click the column profile to select its face and all of its lines. Start moving the selection along the green axis \(**Y Axis**\). Hold **Shift** and move the profile until it aligns with the Roof, then click to place it.
3. Similar to the previous step, move the geometry once again, this time locking it to the red axis \(**X Axis**\).
4. Click to place it on top of the I-Beam drawn in the **Plan Image**. Getting it close is fine, like in the following image, the horizontal position does not need to be perfect.

_**Note:**_ _The_ _**Shift**_ _key will lock the geometry to move along only one axis, in this case, the green \(**Y Axis**\). This will ensure the column profile does not accidentally move up and align to the top of the roof plane._

![](../../.gitbook/assets/4%20%289%29.png)

## **Extrude and Array the Column**

1 - To facilitate the next drafting process, switch the view mode back to **Perspective \(VP\)** and **Orbit \(O\)** to position the camera as to visualize the I-Beam profile from the northwest. Use the north arrow at the bottom left corner to help you position the view.

![](../../.gitbook/assets/5%20%281%29.jpeg)

_**Note:**_ _To learn how to navigate around the sketch, we recommend checking out the_ _**Navigate the Scene**_ _chapter._

2- Select the column profile face and extrude the face up to **17’-8”**.

_**Note:**_ _If while moving the column profile, it aligned itself to the roof, extrude the face down by_ _**17’-8”**  
instead of up._

3 - Zoom out and turn the **Roof** layer on \(if off\). The top of the column should line up with the top of the roof.

![](../../.gitbook/assets/6%20%289%29.png)

4 - To keep the model organized and tidy, select the column geometry again and do the following:

1. **Group \(G\)** and name it **Column Tall**.
2. Create a new **Layer** called **Column** and add the group to it.
3. Import the material **Metal - Brushed - Colorized** and paint the group with it.

![](../../.gitbook/assets/7%20%284%29.png)

_**Note:**_ _See previous chapters for more information on_ _**Groups**,_ _**Layers**, and_ _**Materials**._

4 - Click **Esc** to clear the paintbrush tool.

## **Array the Columns**

1 - Go to the **Top View \(VT\)** and switch the camera mode to **Orthographic \(VO\)** again.

2 - Turn off the **Roof** layer.

3 - To start the array process:

1. Single-click to select the column group. Right-click to bring the **Context Menu** and choose **Array \(AR\)**.
2. In the **Array Properties** dialog, use the following settings:
   * **Length Between Copies**
   * **Linear** \(default\)
   * **Group each solid then array** \(default\)
   * **Number of Copies: 3**
   * Press **OK** to close the dialog.

![](../../.gitbook/assets/8%20%283%29.png)

4 - To place the new elements:

1. Single-click on the column to start the **Array**. Move the cursor along the red axis \(**X axis**\).
2. Set dimension to **22'**. You now have **four** columns **22'** apart.
3. **Esc** to clear your selection.

![](../../.gitbook/assets/9%20%286%29.png)

5 - To select all the **Tall Column** groups at once, hover your mouse over one of them and press the **Tab** key once. Notice that all 4 column’s bounding boxes have been highlighted. Single-click on the column your mouse is hovering over and they will all be selected. This is a quick way to select all instances of the same group at once.

6 - Perform another **Array \(AR\)** to create the columns at the other side of the building. This time make 1 copy along the green axis across the building. Set dimension to **29'- 4 5/8”.**

_**Note:**_ _29’ 4 5/8” = 8 5/8” \(column depth\) + 28’-8” \(main building width\)._

7 - To visualize the whole building, go to the **3D View \(V3\)** and set it to **Perspective \(VP\)**. If off, turn on the **Main Building Floor**, **Roof**, **Lower Terrace**, and **Column** layers.

![](../../.gitbook/assets/10%20%287%29.png)

## **Create the Terrace Columns**

_Now we will duplicate the main building columns to create similar, but shorter, versions for the terrace._

1 - To facilitate drafting, we recommend going back to an **Orthogonal \(OV\)** and **Top View \(VT\)** setting.

2 - To create the new columns:

1. Hold **Ctrl** or **Shift**, click on the 3 columns closest to the **Lower Terrace Floor** to select them.
2. Single-click on any one of the columns to start moving all 3 selected columns at once. Press the **Ctrl** key once to create a **quick copy**. A ghost preview of the copy will appear.
3. Move the copies down along the green axis \(**Y Axis**\) by **23’-4 3/8**”. Press **Esc**.
4. Without deselecting, move the copied columns along the red axis \(**X Axis**\) by **22’** to place them in their final position.
5. Again, with the 3 new columns still selected, right-click one of the copied columns and select **Make Unique \(MU\)**. These columns are now associated with each other, but unique from the originals.

_**Note:**_ _Holding_ _**Shift**_ _or_ _**Ctrl**_ _allows you to select multiple elements at once, or remove elements from your current selection._

![](../../.gitbook/assets/11%20%287%29.png)

3 - Modify the new column group:

1. Double-click to edit one of the new groups and rename it **Column Short.**
2. Adjust the height of the new column to align to the top of the **Lower Terrace** **Floor** \(3’-2”\). To do that, select and drag the column’s face down along the blue axis \(**Z axis**\) and hold **Shift**. Hover the cursor anywhere on the top face of the **Lower Terrace Floor** and the column’s height will automatically align to the Lower Terrace. Once the height is set, click to finish.

![](../../.gitbook/assets/12%20%284%29.png)

_**Note:**_ _You can check the height of the short columns by using the_ _**Measure \(ME\)**_ _tool. Alternatively, you can select one of the column’s vertical edge and see its length in the_ _**Properties Palette**._

4- Using the techniques you just learned, copy the furthest short column to the opposite side of the **Lower Terrace Floor** to create the last remaining column.

![](../../.gitbook/assets/13%20%284%29.png)


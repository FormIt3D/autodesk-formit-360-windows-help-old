### Group Objects

When you draw lines on an existing object, the new lines "stick" to the existing objects. To avoid this "stickiness", you have to Group existing objects first. But this is not all Groups are good for! Copies of Groups maintain their connection to the original, such that editing any copy updates all of them. This concept is similar to Components in SketchUp and Families in Revit.

If you did not complete the last section, download and open the **farnsworth02.axm** file from the [FormIt Primer folder](https://autodesk.app.box.com/s/thavswirrbflit27rbqzl26ljj7fu1uv/1/9025446442).

#### Create a Group

1. Select the upper terrace mass by **double clicking** it

2. **Right click** and **Group (G)**

    ![](./images/c2f57781-ec11-4fbd-87b0-c5fd33ad8b07.png)

3. Select the mass with a **single click** and notice that you are in the Move tool

#### Move a Group

4. Turn Grid Snapping back on by typing **SG** keyboard shortcut

4. Click once on the lower corner of the mass, then move your cursor 'up' and you should see a blue axis line appear

5. With the blue axis visible, press the **Tab key** and enter **4'-6"**. This will move the entire mass up off of the ground plane

    ![](./images/293f6046-366c-43ca-858b-389f0c260be6.png)

#### Edit a Group

4. **Double-click** the mass to edit it. You are now in a Group Edit mode

5. Rename the Group in the [**Properties Palette**](../tool-library/tool-bars-extended.md) 

6. Name the Group **"main building"**. We'll talk about the Category option in future steps

    ![](./images/93c9106d-7676-4cd7-b5e2-b00a56c4e30f.png)

5. Close out of Group Edit mode by clicking on the **check mark** in the panel on the upper left corner of the canvas - or double click off in space

    ![](./images/3b0e7944-9cb1-4852-9b3b-aedf75fc5270.png)

**Note**: *Each Group has their own undo/redo "stack" that is distinct from the overall project - you can click the undo and redo arrows in this panel.*

#### Apply Levels to a Group

1. If you had applied Levels to geometry in the previous exercise, then you will have to re-apply Levels to the new group you just created

2. Select the **main building** group by **single-click** on it

2. Go to the [**Properties Palette**](../formit-introduction/tool-bars.md) and check **Use Levels**

3. Check only the **Floor 1** Level and uncheck the other Levels

    ![](./images/8b2036b8-b627-44a2-ada8-b901cdb380d2.png)

3. The **Area by Level** field will display gross area of the currently selected object(s) and the area of each individual level

    * If you do not see area reported on the Floor 1 Level, then your geometry may not intersect 4' 6"
     
    * If you do not see blue level lines on the object, go to the **Settings menu &gt; Visual Style &gt; Display Levels (DL)**

5. **Deselect** the Group by clicking **Esc** or single clicking off in space - 

6. Now the **Properties Palette** reports the **Gross Area** of the overall sketch - not just the area of the selected object

    ![](./images/GrossArea.png)



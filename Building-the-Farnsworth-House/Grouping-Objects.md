### Group Objects

When you draw lines on an existing object, the new lines "stick" to the existing objects. To avoid this "stickiness", you have to Group existing objects first. But this is not all Groups are good for! Copies of Groups maintain their connection to the original, such that editing any copy updates all of them. This concept is similar to Components in SketchUp and Families in Revit.

If you did not complete the last section, download and open the **farnsworth02.axm** file from the [FormIt Primer folder](https://autodesk.app.box.com/s/thavswirrbflit27rbqzl26ljj7fu1uv/1/9025446442).

#### Create a Group

1. Select the upper terrace mass by **double clicking** it

2. **Right click** and **Group (G)**

    ![](./images/c2f57781-ec11-4fbd-87b0-c5fd33ad8b07.png)

3. Select the mass with a **single click** and notice that you are in the Move tool. 

#### Move a Group

4. Turn on Grid Snapping by clicking SG

4. Click once on the lower edge of the mass. then move your cursor 'up' and you should see a blue axis line appear

5. Press and hold the **Shift key** when the blue Z axis guide appears to lock onto that axis

6. Press the **Tab key** and enter **4'-6"**. This will move the entire mass up 

    ![](./images/293f6046-366c-43ca-858b-389f0c260be6.png)

4. It is important to name Groups as you will have many of them to keep track of. To name the Group, **double-click** to start the edit mode and then open the [**Properties Palette**](../tool-library/tool-bars-extended.md) to name the Group **"main building"**. <br>
    ![](./images/93c9106d-7676-4cd7-b5e2-b00a56c4e30f.png)

5. Close the edit mode by clicking on the **check mark** in the upper left. 

    ![](./images/3b0e7944-9cb1-4852-9b3b-aedf75fc5270.png)



**Note**: *Each Group has their own undo/redo "stack" that is distinct from the top level project.*

#### Apply Levels to a Group

1. Select the **main building by single-clicking** and open the [**Properties Palette**](../formit-introduction/tool-bars.md) of the Palette Bar.

2. Check the **Use Levels ON**. This will "slice" these masses by the levels you choose. Click **Check All**.

3. The **Area by Level** will display gross area of the currently selected object(s) and the area of each individual level.

4. If you do not see blue level lines on the object, go to the **Settings menu &gt; Visual Style &gt; Display Levels (DL)**.

     ![](./images/8b2036b8-b627-44a2-ada8-b901cdb380d2.png)

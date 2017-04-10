### Adding Detail
FormIt is a great massing tool - and it is **also** a great modeling tool. We'll start to add detail to the Farnsworth house in the form of doors and mullions for the glass box. We'll cover some additional tools, and practice the process of adding new geometry, layers, materials, and group management.

If you did not complete the last section, download and open the **farnsworth04.axm** file from the [FormIt Primer folder](https://autodesk.app.box.com/s/thavswirrbflit27rbqzl26ljj7fu1uv/1/9025446442).

#### Door Frames
We are going to create a 2" metal frame and mullions around the glass box. These mullions will overlap with the glass box, and that is intentional

1. Create a new layer called **glass walls** and put the glass box onto this layer

1. **Turn off** the **Roof** layer so we can see the entire glass box. Turn on the **North Arrow** with the **DN** keyboard shortcut

2. Use the [**Rectangle tool (R)**](../tool-library/rectangle-tool.md) to draw a surface over the western face of glass. _**Note**: Since the glass box is grouped, then this new rectangle will **not "stick"** to the glass box_

3. **Single click** to select the new face, then **single click** to start a drag face. **Push** the face 2" towards the interior. Click **Esc** to clear the selection. 

4. If you have trouble selecting the new face, turn off the **glass walls** layer, or hover on the face, hit the **space bar** to choose different selection candidates

    ![](./images/24f63252-b1e6-4071-ba24-961269bf4490.png)
    
3. **Single click** the face you just created. **Right click** to access the context menu. Use the [**Offset Face tool (OF)**](../tool-library/extrude-cut-and-offset-faces.md)

4. Move your mouse toward the inside of the face. Hit the **Tab key** and enter **2"** to create a new rectangle. Click **Esc** to clear the selection

5. **Single click** to select the interior rectangle you just created. Click again to start a drag face. **Push** this face through the model to remove it

6. **Double click** to select the mullion frame. **Group (G)** the selection

    ![](./images/UpperTerraceSketch_15.png)
    
7. Create a layer named **mullions** and  put the new group on it

8. Edit the mullion group by **double clicking** it. Name it **EW Frame** in the **Properties palette**

6. Import and paint the **mullion group** with the material **Metal &gt; Anodized – Gray**

7. **Quick copy**, **Array** or **Mirror** the mullion to the eastern side of the building

Repeat the steps above for the **North and South** sides of the glass box. You may want to turn off the **columns** layer. The mullion frames will overlap each other at the corners and this is intentional

#### Create Mullions

1. Using the same methods in the previous exercise, create a 2" thick and deep mullion **11'-10 ¾"** from the North West corner. 

    ![](./images/7657c4da-7a46-4b50-9458-d08286f9efa4.png)

2. Make the mullion the entire height of the glass walls (11'10").

3. Group and name the assembly **mullion**.

4. Import and paint the column with the material **Metal &gt; Anodized – Gray**.

5. [**Array**](../tool-library/tilt-array-copy-and-paste.md) them three times at a distance of **11'**.

6. Use the **hover + Tab key** to select all mullion instances and **copy** to the south side of the wall.

#### Create Door
Using the same methods as in the previous two exercises, create a 3'-6" double door centered in the western wall.

![](./images/a4f7bb20-db89-4638-a3ad-4ae05c63d351.png)

---
####Related Topics:

[**Cover Sweep Loft**](../tool-library/cover-sweep-loft.md)
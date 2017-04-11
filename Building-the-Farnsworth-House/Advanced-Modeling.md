### Advanced Modeling
In our Farnsworth House exercises we've focused on basic modeling tools like Sketching, Drag Face, Move, Array, and Offset Face. We've also covered the essential workflows involving Groups, Layers, Materials and Levels. In this section we'll introduce you to the Advanced Modeling tools **Sweep** and **Fillet**

If you did not complete the last section, download and open the **farnsworth05.axm** file from the [FormIt Primer folder](https://autodesk.app.box.com/s/thavswirrbflit27rbqzl26ljj7fu1uv/1/9025446442).

####Sweep
Use the Sweep tool to create a cornice along the roof

1. With the **Rectangle (R)** tool, create a **6" high by 4 5/8"** profile at any corner of the roof

    ![](./images/a7297208-cefe-42e7-95ca-1e8ea122ac38.png)

2. Create another **Rectangle (R)** profile that is **2" x 2"** 

    ![](./images/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54.png)

3. **Single click** to select the line between the profiles. Use the **Delete** key to remove the line - this creates a single outline 

    ![](./images/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_2.png)

4. Select the [**Sweep tool (SW)**](../tool-library/cover-sweep-loft.md) from the [**Advanced Modeling menu**](../formit-introduction/tool-bars.md)

    ![](./images/8a17017b-b824-48ac-ba24-064a24e7a6ad.png)

5. The **Advanced Geometry** toolbar appears in the upper left corner of the canvas with helper text instructions

    ![](./images/e8badff2-acd9-4393-af5f-adae2424ad47.png)

6. **Single click** to select the face you just drew. This will be the **profile** you want to sweep

    ![](./images/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_3.png)

7. The **Advanced Geometry** toolbar changes once you select a face. Now it is prompts you to select a **path** for the sweep

    ![](./images/df9fc338-15c0-4953-9ec1-c977117efc4d.png)

6. **Single click** to select the **top face of the roof**. The tool infers the edges of the face as the path. The sweep is created after picking the roof 

    ![](./images/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_4.png)

7. Double click to select the entire cornice element. **Group (G)** the cornice. Edit the group and name it **cornice**

    ![](./images/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_5.png)

8. Paint the cornice group with the material **Concrete &gt; White** to match the roof. Put the **cornice group** on the **roof** layer

You need to adjust the **height of the columns** to end into the cornice. Edit one of the tall column groups, select the top face, and bring it down to the correct height. You may also need to adjust the location of the columns so they are flush to the slabs. Now is a good time to make these minor adjustments.

####Fillet
Now you'll learn the Fillet tool to create a rounded edge to give a softer look to a piece of furniture

1. Turn **off** the **roof** layer so you can see inside the house

2. Create a **4' x 7'** **Rectangle (R)** in the North East corner of the house. Select the face and extrude it **1'-6" high** 

    ![](./images/UpperTerraceSketch_20.png)

2. Select the [**Fillet tool (FI)**](../tool-library/cover-sweep-loft.md) from the **Advanced Modeling tools** in the [**Action Tool Bar**](../formit-introduction/tool-bars.md)

    ![](./images/f7e388e3-4ad0-4fef-a701-0d3176adc2c5.png)

3. Change the default **fillet** value to 1" in the dialog that appears

4. **Single click** the top face of the bed. The fillet is created automatically after selecting the face

    ![](./images/UpperTerraceSketch_21.png)
    
5. **Double click** to select the entire bed. **Group (G)** the bed, then edit the group and name it **Bed**, set the category to **Furniture** 

6. Exit the group, and put the bed on a new layer called **furniture** 

####Merge and Smooth Edges

7. **Double click** to edit the group. Select the entire bed with a **double click**. **Right click** and choose **Merge (MG)** from the context menu

    ![](./images/UpperTerraceSketch_215.png)
    
6. Now, **Single click** to select the remaining arc and edge at the corner. Then **right click** and choose **Smooth Edges (SE)** 

    ![](./images/UpperTerraceSketch_216.png)

7. Turn the **roof** layer back on, your Farnsworth house is coming along nicely!

    ![](./images/UpperTerraceSketch_22.png)

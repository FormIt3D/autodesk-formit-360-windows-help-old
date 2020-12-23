# Advanced Modeling

In our Farnsworth House exercises we've focused on basic modeling tools like Sketching, Drag Face, Move, Array, and Offset Face. We've also covered the essential workflows involving Groups, Layers, Materials and Levels. In this section we'll introduce you to the Advanced Modeling tools **Sweep** and **Fillet**

If you did not complete the last section, download and open the **farnsworth05.axm** file from the [FormIt Primer folder](https://autodesk.app.box.com/s/thavswirrbflit27rbqzl26ljj7fu1uv/1/9025446442).

## Sweep

Use the Sweep tool to create a cornice along the roof.

1. With the **Rectangle \(R\)** tool, create a **6" high by 4 5/8"** profile at any corner of the roof.

   ![](../.gitbook/assets/a7297208-cefe-42e7-95ca-1e8ea122ac38.png)

2. Create another **Rectangle \(R\)** profile that is **2" x 2".**

   ![](../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54.png)

3. **Single click** to select the line between the profiles. Use the **Delete** key to remove the line - this creates a single outline.

   ![](../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_2.png)

4. Select the [**Sweep tool \(SW\)**](../tool-library/cover-sweep-loft.md) from the [**Advanced Modeling menu**](../formit-introduction/tool-bars.md)**.**

   ![](../.gitbook/assets/8a17017b-b824-48ac-ba24-064a24e7a6ad.png)

5. The **Advanced Geometry** toolbar appears in the upper left corner of the canvas with helper text instructions.

   ![](../.gitbook/assets/e8badff2-acd9-4393-af5f-adae2424ad47.png)

6. **Single-click** to select the face you just drew. This will be the **profile** you want to sweep.

   ![](../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_3.png)

7. The **Advanced Geometry** toolbar changes once you select a face. Now it is prompts you to select a **path** for the sweep.

   ![](../.gitbook/assets/df9fc338-15c0-4953-9ec1-c977117efc4d.png)

8. **Single-click** to select the **top face of the roof**. The tool infers the edges of the face as the path. The sweep is created after picking the roof.

   ![](../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_4.png)

9. Double click to select the entire cornice element. **Group \(G\)** the cornice. Edit the group and name it **cornice.**

   ![](../.gitbook/assets/5e1ad684-a3db-4c30-882c-6fdd9a1b9f54_5.png)

10. Paint the cornice group with the material **Concrete &gt; White** to match the roof. Add the **cornice group** to the **roof** layer.

You need to adjust the **height of the columns** to end in the cornice. Edit one of the tall column groups, select the top face, and bring it down to the correct height. You may also need to adjust the location of the columns so they are flush to the slabs. Now is a good time to make these minor adjustments

## Fillet

Now you'll learn the Fillet tool to create a rounded edge to give a softer look to a piece of furniture

1. Turn **off** the **roof** layer so you can see inside the house.
2. Create a **4' x 7'** **Rectangle \(R\)** in the North East corner of the house. Select the face and extrude it **1'-6" high.**

   ![](../.gitbook/assets/upperterracesketch_20.png)

3. Select the [**Fillet tool \(FI\)**](../tool-library/cover-sweep-loft.md) from the **Advanced Modeling tools** in the [**Action Tool Bar**](../formit-introduction/tool-bars.md)**.**

   ![](../.gitbook/assets/f7e388e3-4ad0-4fef-a701-0d3176adc2c5.png)

4. Change the default **fillet** value to 1" in the dialog that appears.
5. **Single-click** the top face of the bed. The fillet is created automatically after selecting the face.

   ![](../.gitbook/assets/upperterracesketch_21.png)

## Groups Tree

Instead of editing the group to name and categorize it, let's use the **Groups Tree** which allows you to quickly conduct multiple model management tasks.

1. **Double-click** to select the entire bed. Add the bed to **Group \(G\).**
2. Click the **Groups Tree** icon from the palettes on the right.

   ![](../.gitbook/assets/groupstree.png)

3. If you select the bed group in the canvas, it will highlight in the **Groups Tree** list \(the opposite is also true, if you select a group in the list, it will highlight in the canvas\).
4. You can **double-click** the name in the list and change it to **Bed** - all instances of the group will update - in our case there is only one.
5. While the **Bed group** is selected in the list, you can set the category to **Furniture** from the drop-down list at the top of the Groups Tree palette.

   ![](../.gitbook/assets/groupstree_palette.png)

## Merge Edges, Smooth Edges, and Selection Filtering

We'll now hide unwanted edges on our furniture, to give it a smoother, softer look.

1. **Double-click** to edit the group. Select the entire bed with a **double-click**. **Right-click** and choose **Merge \(MG\)** from the context menu.

   ![](../.gitbook/assets/upperterracesketch_215.png)

2. Use the **Selection Filter** to constrain a window selection to only pick-up **Edges.**

   ![](../.gitbook/assets/25b2428d-bc93-4ae4-9b8a-d8f3749ddb43.png)

3. **Drag the mouse** from the upper left to the lower right corner to perform a **window selection**. Window select the arc and edge at each corner of the bed. Hold down **Ctrl** or **Shift** to add to the selection set.
4. **Right click** and choose **Smooth Edges \(SE\)**

   ![](../.gitbook/assets/upperterracesketch_216.png)

5. To make these edges visible again, **single-click** to select the top face of the bed, **right-click** and choose **Facet Smooth Edges** \(UE\).

   ![](../.gitbook/assets/upperterracesketch_217.png)

6. Change your **Selection Filter** back to include Faces and Groups again. Turn the **roof** layer back on. Your Farnsworth house model is coming along nicely!

   ![](../.gitbook/assets/upperterracesketch_22.png)


### Import/Export and Content Library
In this section we will import models existing models from the SketchUp warehouse, and use the FormIt Content Library to place Families we've converted from Revit. **Note** that SKP files import to FormIt with Materials, Groups and Components, Layers and Scenes in tact

If you did not complete the last section, download and open the **farnsworth07.axm** file from the [FormIt Primer folder](https://autodesk.app.box.com/s/thavswirrbflit27rbqzl26ljj7fu1uv/1/9025446442).

#### Import SKP files
First we'll go through the process of adding a piece of downloaded content to your own personal content library

4. Start a new session of FormIt - you can either **Save (Ctrl + S)** your existing work, and start a **New file (Ctrl + N)**, or start another session of the app, so you have two running side by side

5. In an empty FormIt scene, click File &gt; Import &gt; **Import 3D Model (Ctrl + I)** and Import **mies\_ottoman.SKP** from **FormIt Primer/content/SKP**

     ![](./images/6d0397d3-3c97-46cd-90f9-878c34e90195.png)

5. **Double click** to edit the **ottoman** group. Name the group **Mies Ottoman** and set the category to **Furniture**

6. Ensure **Snap to Grid (SG)** is on. Draw a reference **Line (L)** starting at the origin point defined by the X, Y, Z axis. Click anywhere to place the second point

7. **Single click** to select the **ottoman** group. Click the lowest corner of the leg to set the **start point** of a **move command** 

     ![](./images/6d0397d3-3c97-46cd-90f9-878c34e90195_2.png)
     
7. **Single click** to place the **ottoman** group at the origin. Clear the selection with an **Esc**, then delete the reference line  

     ![](./images/6d0397d3-3c97-46cd-90f9-878c34e90195_3.png)

7. Turn off the **Grid (DG)** and the **X, Y, Z axes (DZ)** and do a **Zoom All (ZA)**. FormIt will store the current [**Visual Styles**](/Building-the-Farnsworth-House/Visual-Settings.md) for the **Content Library** thumbnail preview image

     ![](./images/6d0397d3-3c97-46cd-90f9-878c34e90195_4.png)

8. **Save As (Ctrl + Shift + S)**. Put the file in the **content\Seating** folder with the name **Mies Ottoman.AXM**. Note that an **example** is there in case you want to review

You can follow the same steps above with the **Mies_van_der_Rohe_Couch** and the **mob_cadeira_barcelona** files in the **content\SKP** folder

####Link a Content Library

1. Open the [**Content Library Palette**](../formit-introduction/tool-bars.md)

     ![](./images/ContentLibrary.png)

2. Click the **+** icon to link a Content Library folder. Click the **+** icon in the dialog to define a path to a local folder 

3. Select the **FormIt Primer\content** folder and click OK

     ![](./images/15e16abd-9b7a-4762-9364-0f31e81ded8a.png)

####Place Content from the Library

1. Turn off the **roof** layer so you can see inside the house

3. Look in the **Content Library** palette and choose the **content** folder** you just linked from the drop down menu

     ![](./images/627dd398-eefa-4407-842f-e42c2e4350f1.png)

1. **Single click** the **components** folder to open it. **Drag and drop** the **core** file into the canvas. Place it in the middle of the floor

     ![](./images/UpperTerraceSketch_29.png)

2. Go to the **Top View (ZT)** and turn off the **Floor 1** layer to see the plan image below

3. Select the **core** and move it along the **red axis** until it roughly lines up to the plan below. You may want to turn off **Snap to Grid (SG)** 

     ![](./images/UpperTerraceSketch_30.png)

3. **Move the core** along the **green axis** until it is roughly in place, using the plan as a guide. You should also adjust the location of the bed while you're here!

Make sure to **move along the red and green axes** while working in Top View. Otherwise you may snap to elements above or below, and the object you're moving will jump in the Z direction

####Place Furniture from the Library

4. Go back to the **perspective view (ZD)**, turn on the **Floor 1** layer 

5. Look into the **Content Library** palette. Click into the **Seating** sub-folder

     ![](./images/ba020113-7f1e-4b8e-a11c-f336dbb68e41.png)

5. Select the **Corbu Chair** and a few of the ** **place two** instances of it. 

     ![](./images/1f193941-4bf0-4394-8316-e5a103fa8949.png)
     
     
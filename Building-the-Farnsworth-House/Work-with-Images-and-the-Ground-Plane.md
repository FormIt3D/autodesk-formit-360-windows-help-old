### Project set up with Images and Grid

You may import PNG images onto the ground plane by using the File &gt; Import menu. However, to gain more control over the scale and position, we will place a material texture onto a plane that we will draw ourselves. The **plan.png** image is 3600 pixels wide by 2400 pixels high. By measuring the scale on the plan, we see that 1' is 25 pixels. This will allow us to scale the image properly in the scene


1. Click the Top View icon from the Navigation Bar to see the scene from above

    ![](./images/TopView.png)    

2. Choose the [**Rectangle tool (R)**](../tool-library/rectangle-tool.md) from the 3D Sketch toolbar and draw a rectangle **144'** by **96'**

    ![](./images/rectangleToolbar.png)  

3. While the dimension is visible, click the **Tab key** to access a dialog where you can input exact dimensions. Click **OK** to commit the dimension. Click **Esc** to clear the Rectangle tool

    ![](./images/RectangleCanvas.png)

2. Open the [**Material Palette**](../formit-introduction/tool-bars.md) and click the **+** icon to create a new material

    ![](./images/NewMaterial.png)

3. Name the new material **Floor Plan**

4. Import the image texture. Find the Texture preview tile and click the **folder icon**, browse to **plan.png** in the **FormIt Primer release\Part 1 datasets\drawings** folder, click OK

4. Change the scale of the image. Enter **144'** in the Horizontal field and **96'** in the Vertical field, click OK to finish the material

    ![](./images/8f0f2e11-ecfb-484d-94f6-0930c8ad7b20.png)

5. In the [**Material Palette**](../formit-introduction/tool-bars.md) **single click** on the **Floor Plan material** tile to paint with this material

6. Click on the **rectangle** you sketched to paint it with the material. Click **Esc** to clear the paintbrush tool

6. Now we'll rotate the rectangle to align with the Satellite image. **Double-click** the **rectangle** to select it 

7. **Right click** to bring up the context menu. Choose [**Rotate (Q)**](../tool-library/placing-and-modifying-objects/rotate.md)

    ![](./images/eab003c6-c95c-4003-9068-0eb43f41a263.png)

8. The Rotate widget appears in the middle of the rectangle. Select the widget by clicking once on the orange grip in the middle. Move the widget to the bottom left corner of the rectangle. It will snap to the corner. Click to place it

9. Hit the Tab key and input **9 degrees** the rectangle will rotate counter clockwise

    ![](./images/eab003c6-c95c-4003-9068-0eb43f41a263_2.png)

7. Now we will align the grid with the Satellite image and the floor plan. **Right click** on the **ground plane** and choose [**Set Axes (SZ)**](../tool-library/world-axes.md). 

    ![](./images/SetAxis.png)

8. The Set Axis widget appears. Move the axis to the bottom left corner of the of the rectanle. Click to place it

9. Click the grip at the end of the red axis. Move the grip so that it snaps to the bottom edge of the plane. Click off in space to commit this change

    ![](./images/ed8afd35-af8a-4cf3-b3a7-71def22f9b2e.png)

9. The satellite image, the rectangle and the grid are now aligned – which will make 3D sketching much easier

    ![](./images/SiteFinished.png)


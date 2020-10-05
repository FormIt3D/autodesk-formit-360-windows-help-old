# Offset Line

Draw parallel, or offset, lines using the Offset Line tool. This is useful to create 2D shapes that can later be extruded to look like 3D walls.

![](../.gitbook/assets/image%20%283%29.png)

The **Offset Line** tool works similar to the [**Line** ](https://windows.help.formit.autodesk.com/tool-library/line-tool)tool: 

* Click to set the first point and then move your cursor and place the subsequent points, snapping to existing geometry or to inference axes. 
* A preview of the resulting shape is shown. The second and third points determine the plane for the rest of the points to follow, so the result is planar.
* Continue adding points, and **Escape** or double click to finish the tool
* Any self-intersections will be cleaned up and merged, leaving you with one extrudable face.

![After placing 2 points and dragging the 3rd point](../.gitbook/assets/walls1.png)

The input line is drawn in red, and by default is placed in the center of the offset lines. 

You can change the alignment of the offset lines and their thickness by hitting the **Tab** key. This will invoke the **Tool Options** dialog:

![Options for the Offset Line tool](../.gitbook/assets/walls2.png)

Change the **Alignment** to **Left** and the **Thickness** to 6", for example, and the offset lines will be drawn to the left of the input lines, 6 inches apart.

![](../.gitbook/assets/walls3.png)

## Useful Tips

You can draw a closed shape by snapping to the first point placed. The resulting corner will be cleaned up automatically:

![](../.gitbook/assets/walls4.png)

You can freely draw the input lines on top of each other. When the tool is finished the resulting intersections are cleaned up.

![](../.gitbook/assets/walls5.png)

![](../.gitbook/assets/walls6.png)

Inherently, the Offset Line tool must generate geometry on a plane, so the first few points determine the plane that the remaining points will follow. 

Start drawing on the side of a cube, for example, to use the plane of that face. After three non colinear points are placed the input plane is fixed for the remainder of the input. Note, that when drawing on a face the resulting shape is inserted into the face, splitting it into multiple faces. To prevent the insertion, the face you draw on must be part of a [Group](https://windows.help.formit.autodesk.com/tool-library/groups).

![Drawing on a vertical face](../.gitbook/assets/walls7.png)

![After the tool is ended, the lines are inserted and the split faces can be further manipulated](../.gitbook/assets/walls8.png)

You can also use the Offset Line tool to trace from a plan drawing. Import the plan as an image. 

* Resize the image so that the plan has the proper scale. This is described in more detail [here](https://windows.help.formit.autodesk.com/building-the-farnsworth-house/work-with-images-and-the-ground-plane). 
* You can use the [Orthographic Camera](orthographic-camera.md) to trace in an orthographic [top view](orthographic-views.md)

![](../.gitbook/assets/walls9.png)

![](../.gitbook/assets/walls10.png)




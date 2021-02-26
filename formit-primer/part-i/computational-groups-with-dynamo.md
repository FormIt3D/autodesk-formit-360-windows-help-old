# 1.10 - Computational Groups with Dynamo

_In this chapter, we will leverage the computational power of_ [_**Dynamo**_](http://dynamobim.org/) _to place and modify flexible groups that are tied to OOTB Dynamo Graphs Samples._

_If you did not complete the last section, download and open the_ _**1.10 – Computational Groups with Dynamo.axm**_ _file from the_ _**FormIt Primer Part 1 Datasets**._

_You can_ [_**learn more here**_](http://formit.autodesk.com/page/formit-dynamo) _about how FormIt and Dynamo work together for computational design workflows._

## **Create Lower Terrace Stairs**

1 - Make sure the **Lower Terrace, Main Building Floor**, and **Plan Image** layers are turned on, since that is where we are going to add the stairs.

2 - To place a stair group tied to one of the OOTB Dynamo Samples:

1. Open the **Dynamo Palette** in the Palette Bar. You should see a few built-in Dynamo objects in the **Dynamo Samples** directory
2. Single-click the **Stairs** Dynamo sample to bring it to the model space. FormIt will run the graph behind-the-scenes and generate the stair geometry from this graph.
3. Move your cursor over the canvas, and once the stair is loaded, a ghosted preview of the stair geometry will now be moving alongside your mouse. Move your cursor over the canvas, near the terrace, and click to place the stair. Press **Esc** to clear the selection. Note that after placing the stairs the **Properties Palette** will automatically open.

![](../../.gitbook/assets/0%20%2815%29.png)

_**Note:**_ [_**You can also link local directories**_](https://formit.autodesk.com/page/formit-dynamo#dynamo-getting-started) _containing Dynamo graphs, and run your own local Dynamo graphs just like these samples._

3 - To update the stairs dimensions:

1. With the stair group selected, modify the inputs available under the Dynamo **INPUTS** section at the bottom of the **Properties Palette** to match as shown below. Most groups created via Dynamo Scrips will have a Dynamo section included in their properties when selected.
   * Add Top Landing = False
   * Add Middle Landing = False
   * Add Bottom Landing = False
   * Floor-to-Floor Height = 2.6
   * Stair Width = 12
   * Riser Height = 0.6
   * Tread Length = 1.25
   * Tread Overlap = 0.25
   * Tread Thickness = 0.25
   * Height Between Middle Landings = \(not relevant since no middle landing is being created\)
   * Middle Landing Length = \(not relevant since no middle landing is being created\)
   * Top/Bottom Landing Length = \(not relevant since no landing is being created\)
2. Click on the **Run** button to re-run the Dynamo script using the updated input values.
3. Move the group as needed to place the stair in the correct location accordingly to the **Plan Image**. Take care not to change the elevation of the stair group at all as you move it. Refer to previous chapters to learn more about tricks and techniques when moving model elements.

![](../../.gitbook/assets/1%20%2811%29.png)

_**‌Note:**_ _The_ _**Floor-to-Floor Height**_ _input is an approximation of the stair’s total height. The_ _**Riser Height**_ _is the parameter that actually defines the height of the stairs. In this example we set the_ _**Floor-to-Floor Height**_ _as 2.6’ but the final stair height is 3.0’ \(0.6’ \(**Riser Height**\) x 5 \(number of risers\)\). Since the span between the ground and the terrace top of floor is 3’-2”, the remaining 2” is contained in the upper riser._

## **Create Main Building Stairs**

_In the previous steps we created a stair with no landings. Now we will create a stair that uses an upper landing that aligns with the_ _**Main Building Floor**._

1 - Start by making a copy of the stairs we just made:

1. Select the existing stair and then click anywhere on the **Plan Image** to start a move command. This will cause FormIt to use the elevation of the **Plan Image** as the starting reference height for place our new copy. Press **Ctrl** to make a **quick copy**.
2. Move the cursor over closer to the main building above the terrace. Note that now the terrace’s top face is the new reference plane. Click to place the group.

![](../../.gitbook/assets/2%20%289%29.png)

_**Note:**_ _Since the_ _**Plan Image**_ _is at the_ _**Ground Level**_ _plane, the_ _**Move Tool**_ _will use that plane as a reference for its start point. Note the_ _**On Face**_ _tooltip in the above image, indicating that the Plan Image face is selected as the starting reference, and the top face of the_ _**Lower Terrace Floor**_ _is selected as the ending reference._

2 - Use the **Make Unique \(MU\)** tool so that when we change this stair’s Dynamo inputs it will not affect the lower stair. Reposition the group as needed so that it is close to its final location – we will fine tune this later. You can toggle the **Lower Terrace** layer visibility to see the plan below to help position it, but again be careful not to change the new stair’s elevation as you move it.

3 - In the **Properties Palette** update the **Dynamo Inputs** as shown below and run the script once more.

* Add Top Landing = True
* Floor-to-Floor Height = 2.333
* Riser Height = 0.466
* Tread Length = 1.5
* Top/Bottom Landing Length = 2.5

![](../../.gitbook/assets/3%20%281%29.jpeg)

_**Note:**_ _If you set_ _**Add Bottom Landing**_ _to_ _**true**_ _and re-run the script, the bottom landing’s top face should align with the_ _**Lower Terrace Floor**’s top face. This is happening because – differently from the previous stairs - we adjusted the_ _**Riser Height**_ _to match the_ _**Floor-to-Floor Height**_ _to the true height we want \(2’-4” or 2.333’\)._

2 - Reposition the group again to its final position. The top landing should be flush with the **Main Building Floor**.

3 - To finalize the stairs, add the **Stone - Travertine** material to it to match the floors. To learn more about how to apply materials, see previous chapters.


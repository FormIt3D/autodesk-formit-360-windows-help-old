# Computational Groups with Dynamo

In this section we will leverage the computational power of [Dynamo](http://dynamobim.org/) to place and modify flexible groups.

If you did not complete the last section, download and open the **farnsworth06.axm** file from the [FormIt Primer folder](https://autodesk.app.box.com/s/thavswirrbflit27rbqzl26ljj7fu1uv/1/9025446442).

## Place and Modify Dynamo Content

1. Open the [**Dynamo Palette**](../formit-introduction/tool-bars.md) in the Palette Bar

   ![](../.gitbook/assets/99a4e906-2dd3-4a71-bcc9-578018dc5fb8.png)

2. Click the **+** icon to **add Dynamo content** from a URL
3. Paste the following URL into the dialog [https://www.dynamoreach.com/share/5780fb888794379c4b65b941](https://www.dynamoreach.com/share/5780fb888794379c4b65b941). This will refresh the Dynamo panel to include a **Simple Stair tool**

   ![](../.gitbook/assets/simplestair.png)

4. Single click the **Simple Stair**. FormIt will load the Dynamo graph, this will take a few seconds
5. Once the stair is loaded, move your cursor over the canvas, near the terrace. Click to place the stair. Click **Esc** to clear the selection

   ![](../.gitbook/assets/7f47eb16-9bde-4a17-bf63-898774c31338.png)

6. Edit the Simple Stair group, just like you would a normal group, by **double clicking** into it
7. The [**Properties Palette**](../formit-introduction/tool-bars.md) automatically toggles to view the stair's parameters. Modify the settings so they are the same as the picture below

   ![](../.gitbook/assets/c068120a-7b4b-4816-ba48-8f7a8066262c.png)

## Locate the Stair Group

1. **Single click** to select the stairs, click one of the top corners to start the move tool

   ![](../.gitbook/assets/upperterracesketch_23.png)

2. **Move** the top of the stairs so it aligns with the edge of the terrace

   ![](../.gitbook/assets/upperterracesketch_24.png)

3. Next, **center** the stairs between the two columns. This could be done with **guide lines** as we did in the previous exercise, but we'll introduce the **Measure \(ME\)** tool

   ![](../.gitbook/assets/measure.png)

4. Start the **Measure \(ME\)** tool. Your first click should be the edge of the lower terrace. This is where you are measuring **from**
5. You second click should be the **mid point** of the stair. A dimension string will appear

   ![](../.gitbook/assets/upperterracesketch_25.png)

6. Press the **Tab key** and enter **16' 7"**. The measure tool will move the geometry using the reference and target points you provided

## Locate the Upper Stair Group

1. **Single click** to select the stair group, click the same mid point to start the **move tool**
2. Press the **Ctrl key** once to make a **quick copy** - and move the ghost preview geometry to the upper terrace

   ![](../.gitbook/assets/upperterracesketch_26.png)

3. Right click on copied group and select **Make Unique \(M U\)**
4. **Double click** to edit the copied group. Change the **Floor to Floor height** setting to **1.75**. You will need to **move** the stairs up to align with the upper terrace floor
5. Create a new **layer** called **stairs** and put both stairs on that layer
6. Paint both of the **stair** groups with the material **Travertine** to match the floors

   ![](../.gitbook/assets/upperterracesketch_28.png)


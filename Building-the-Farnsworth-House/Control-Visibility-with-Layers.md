### Control Visibility with Layers
Much like AutoCAD and Photoshop, Layers in FormIt allow you to manage the visibility of objects in your scene. We are going to create a layer to save and hide the building mass for analysis in the future.

### Create Layers

1. Go to the [**Layers Palette**](../formit-introduction/tool-bars.md) and click the **+** sign three times to create three layers

2. Double click the layer names to rename them **Massing**, **Floor 1**, and **Plan Image**
     
     ![](./images/10c435cf-fcc2-4a4b-9135-094dea903da2.png)

3. Select the **main building** mass and choose the **massing layer** from the **Selection On** drop down in the Layers palette

### Duplicate Group

4. Create a copy of the Group by selecting it with a **single click** 

5. Press **Ctrl+C** to copy, and then **Ctrl+Shift+V** to paste the mass in the same place

5. The **new** copy is still selected. **Right click** and choose **Make Unique (MU)**. 

     ![](./images/3f46a20c-a1ab-44a1-8ba3-d2cdb050f1bd.png)

**Note**: The new Group is now severed from the original and will not update with the other one



6. Select the **newly created group** and choose **Floor 1** from the menu. This will be the basis for the first floor.

7. Move it to exact spot of the original Group by selecting the lower left corner. 

8. Uncheck the **massing** layer to hide it.

9. Edit the **Floor 1 Group** and select the **top face**. Move it down **11'-2"**. The resulting floor should be 1' thick.

10. Select the plan image group and create and assign it to a new **Plan Image** layer.
# Properties Plus Plugin

_This plugin is a more featured version of the standard_ _**Properties Palette**. If you select multiple groups and/or types of geometry, this plugin will provide you with a breakdown of what has been selected, as well as allow for the bulk renaming of groups and group instances._

1 **-** First we will look at the properties of a door group from our main model. Re-open **Encode Campus Sample Model.axm** and go back to the **Eye Level – Long Alley** scene. To start utilizing the **Properties Plus** plugin:

1. Open the **Properties Plus Palette** by clicking on the property with a ‘plus’ symbol icon.
2. Make sure that **Update on Selection Change** is checked.
3. Select one of the double glass door groups, named **Door**, on the right side of the alley.
4. Under the **Selection Count** area, **Total Objects** tells us that we have one (**1**) object selected.
5. Just below that we can find more information on what types of objects have been selected. In this case, there is one (**1**) group selected, but that group has four (**4**) instances somewhere in the model.

![](<../../../.gitbook/assets/10 (2).png>)

_**Note:**_ _Checking the number of instances of the selected group can be very handy to prevent accidentally changing multiple elements when you actually only wanted to change the selected element, but forgot to make it unique first._

2 - This plugin allows us to edit a group or group instance’s name without having to go into group edit mode, and rename multiple instances at once. As we learned previously, every group has a name, but every instance of that group can also have a unique ‘instance’ name. Since there will most likely be many types of doors in this model, we want to give this group, and some of its instances, more specific names.

1. With the first glass **Door** group still selected, add another **Door** group to your current selection by holding **Shift** or **Ctrl** and single-clicking on the other double glass **Door** group near the first.
2. Notice that now, the **Properties Plus Palette** has updated its **Selection Count** to show that there are two (**2**) instances selected, but still only one (**1**) unique **Family** (AKA group) selected. (Even though this plugin is using the term **Family**, which should be familiar to Revit users, in this context it means the same thing as a FormIt group.)
3. Under the **Group Family** area, update the **Name** field to be **Doors – Double Glass Storefront**. This will update the name group’s name for all instances, no matter where they are or whether they are currently selected or not, without having to double-click and edit the group.
4. Since these two instances are both doors into the Groove Coffee area, lets rename just these two instances by entering **Groove Coffee Door** into the **Name** field under the **Multiple Group Instances** area.

**Note:** In the standard **Properties Palette**, there is no way to rename multiple instances of a group at once. This can be extremely handy when you want to rename tens or hundreds of instances with the same name at once.

![](<../../../.gitbook/assets/11 (6).png>)

_**Note:**_ _If you mouse leaves the palette, you will no longer be able to edit the selected textbox. This is true for all palettes, so make sure to keep your cursor within the palette boundary while editing anything inside of a palette._

3 - Now if you select a Groove Coffee glass door or a different glass door and look at their properties in the regular **Properties Palette**, you will see that the name of the **Group** has been updated for every instance, but only the Groove Coffee doors have their instance **Name** property updated from its default value.

![](<../../../.gitbook/assets/12 (3).png>)

4 - Finally, let’s look at how this plugin sorts different types of elements:

1. Quickly draw a **Line (L)**, **Rectangle (R)**, and **Cube (Alt + B)** anywhere you would like in the model. These will be temporary, so their precise location is not important.
2. Re-open the **Properties Plus Palette** if it was closed, and then press **Crtl + A** to select all visible elements in the model.
3. Look in the **Selection Count** area, and notice that the selected elements are separated into **Edges** (lines), **Faces**, **Bodies**, (3D shapes made of faces and edges, like the cube)**,** **Groups**, and more.

![](<../../../.gitbook/assets/13 (3).png>)

_**Note:**_ _This plugin also detects_ _**Vertices**, which can be created using another plugin called_ _**Generate Vertex**. If you would like to experiment, install the_ _**Generate Vertex Plugin**_ _and repeat the steps above._

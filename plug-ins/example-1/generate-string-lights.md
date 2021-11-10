# Generate String Lights

_In this chapter, we are going to sample a few of the plugins that come with FormIt to make some improvements to the_ _**Encode Campus Sample Model.axm**. If you have not already, you can download the file from the_ [_FormIt Primer Part II DataSet_](https://formit-help.s3.amazonaws.com/FormIt+Primer+Part+2+Datasets.zip)__

_This neat plugin lets you quickly add hanging lights to your model based on a line or curve._

1 - Before adding any new lights, let's check out the intended result using a premade scene in the model.

1. To jump to the scene containing existing string lights, open the **Scenes Palette** and double click on the scene named **Eye Level – Short Alley**.
2. Notice the string lights that came with this model – that is what we are going to recreate, but somewhere else.
3. In the **Layer Palette**, turn on the **Helper Geometry** layer so you can see the original lines used to generate these string lights.

![](<../../.gitbook/assets/3 (10).png>)

2 - Now let’s navigate to the other alley and add some lights. In the **Scenes Palette** open the **Eye Level – Long Alley** scene. Notice that this alley does not yet have any string lights.

3 - To create a new string of lights:

1. Open the newly installed **Generate String Lights Palette** by clicking on the string light icon. By default, the icons for new plugins appear at the bottom.
2. Change the **Number of Fixtures** option to **10**.
3. Double-click on one of the helper lines to edit the pre-created **String Lights – Long Alley** group. Then single-click on one of the pre-drawn helper lines to select it.
4. Click the **Generate String Lights** button inside the plugin’s palette, and a new string of lights should appear! Note that each string of lights is created as its own unique group.

![](<../../.gitbook/assets/4 (6).png>)

_**Note:**_ _It is OK that some of the lines are going through the “Groove Coffee” sign, because the string light plugin creates a catenary curve that will sag realistically below the sign._

4 - Try creating some more string lights by using the other pre-made helper line and/or creating some of your own helper lines. Play around with the plugin’s settings to get different results.

5 - To help keep the model organized, when finished we recommend grouping all the helper lines and placing that group on the **Helper Geometry** layer, as well as assigning all string light groups to the **Context – Exterior Lighting** layer. This will prevent the helper lines from showing up in any of the ‘Eye Level’ scenes where we do not want to see them. When finished, the results should look something like the next screenshot.

![](<../../.gitbook/assets/5 (3).png>)

_**Note:**_ _Unlike geometry created from a Dynamo script, which can be updated and regenerated through the_ _**Properties Palette**, objects created by a plugin are (for the most part) just regular FormIt geometry. Once created, they can only be edited using FormIt’s built in modeling tools._

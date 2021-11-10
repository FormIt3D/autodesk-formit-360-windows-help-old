# Manage Cameras Plugin

_In this chapter, we are going to sample a few of the plugins that come with FormIt to make some improvements to the_ _**Encode Campus Sample Model.axm**. If you have not already, you can download the file from the_ [_FormIt Primer Part II DataSet_](https://formit-help.s3.amazonaws.com/FormIt+Primer+Part+2+Datasets.zip)__

Throughout the primer, we have been using scenes as valuable tools to navigate and control visibility throughout the model. This plugin allows us to see and edit the elevation of our current camera, export cameras for each scene as 3D objects, and copy these scenes between models.

1 - First, we will adjust the **Eye Level – Long Alley** scene so that its camera is actually at eye level:

1. If not already there, go back to the **Eye Level – Long Alley** scene by double-clicking on it inside the **Scenes Palette**.
2. Open the **Manage Cameras Palette** by clicking on the camera with a gear icon.
3. Change the **Height Above Ground** to **5’-8”**.

![](<../../.gitbook/assets/6 (6).png>)

_**Note:**_ _If your model has levels, this plugin will also show the height above the nearest level below the_ _**Main Camera**._

2 - Then:

1. Go back to the **Scenes Palette**.
2. Make sure the **Eye Level – Long Alley** scene is still selected (otherwise single-click to select it).
3. Click on the **Update Scene** button to save the new camera height to this scene.

![](<../../.gitbook/assets/7 (1).png>)

_**Note:**_ _You can also adjust the angle and position of a scene’s camera by toggling the_ _**Edit Scene Cameras**_ _button at the top of the_ _**Scenes Palette**_ _(between the update and play buttons)._

3 - Next let’s export our scenes to a new model. First we have to create camera objects for all scenes using the **Manage Cameras** plugin:

1. Open the **Manage Cameras Palette** again.
2. Make sure the **Copy Cameras to Clipboard** option is checked.
3. Click on the **Export Scenes to Cameras** button. This may take a few seconds.
4. If your entire canvas went white, it is because your **Main Camera** was aligned with one of the scene cameras. **Zoom (Z)** out until you can see the 3 main buildings and the newly created camera objects. Note that the camera objects are automatically placed into one large group named **Cameras**. Inside that group, each individual camera is placed in its own group with the same name as the scenes it was created from.

![](<../../.gitbook/assets/8 (7).png>)

4 – Let’s copy these scenes to a new model. Since the camera data was saved to the clipboard, there is not much we have to do:

1. **Save** **(Ctrl + S)** your current model, and the close it.
2. Start a new empty sketch by selecting **New Sketch (Ctrl + N)** from the **File** dropdown in the **Main Menu** bar.
3. Open the **Manage Cameras** plugin, if its not already open, and make sure the **Look for Cameras on Clipboard** option is checked.
4. Click on the **Import Scenes from Cameras** button near the bottom of the plugin, and the scenes from our other model will be imported. To check, open the **Scenes Palette** and/or turn on the **Camera** layer. You will see that all the scenes and 3D camera objects have been imported into this model.

![](<../../.gitbook/assets/9 (7).png>)

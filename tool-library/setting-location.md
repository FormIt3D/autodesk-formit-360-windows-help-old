# Setting Location

Setting your your project's location in the world it is important for the accuracy of your model and downstream analyses, including:

* Location is used to import a satellite image which can be used to trace an existing site or building
* Location is used for accurate positioning of the sun in the sky, affecting calculation of shadows and shade studies
* Location is used for Solar Analysis and Energy Analysis to provide accurate analytical calculations

You'll need to be signed in with your Autodesk account to access location and satellite imagery services. 

### Importing Terrain

The FormIt 2021.3 release adds the ability to import terrain from the **Set Location** dialog. By default, imported terrain is placed on a Terrain layer. Toggle this layer to see your imported terrain.

![](../.gitbook/assets/terrain_solid.png)

### Getting Started With Location

* Launch the **Set Location** dialog from the **Location** tool in the toolbar, or with the keyboard shortcut SL.

![](../.gitbook/assets/location-toolbar.png)

* Begin by typing the location of your project into the search box in the upper left hand corner of the _Set Location_ window. 

![](../.gitbook/assets/location-step-1%20%281%29.png)

* Select one of the auto-populating location options, or hit Enter to choose the first one
* You'll zoom in to the location you searched for automatically

### Set Location Only vs. Import Satellite Image

Once you've searched for a location, you can choose one of two options:

*  **Set Location Only** will set the location in the file without importing satellite imagery
* **Import Satellite Image** will set the location, and will also import satellite imagery using a zoom level and extents you can configure

### Importing Satellite Imagery

* Click **Import Satellite Image** at the top right of the **Set Location** window
* A preview of the satellite imagery will appear in the center of the window, along with an indication of where the FormIt origin will appear, relative to the imagery

![](../.gitbook/assets/location-step-2.png)

* Drag the satellite imagery within the square to adjust its position
* Once the square area encapsulates the imagery you want, click **Finish Importing**
* The image will be imported to scale, with true north facing up, centered at the FormIt canvas origin. You can change the transparency and Z-ordering of the imported image by double clicking it and going to the [**Properties Palette**](../formit-introduction/tool-bars.md). 

![](../.gitbook/assets/location-step-3.png)

### Updating Satellite Imagery

After importing satellite imagery the first time, you can use the Set Location window to adjust the zoom level or extents of the satellite imagery.

* Start the **Set Location** window again by accessing it from the toolbar, as outlined above
* Click **Import Satellite Image**
* You'll see the current satellite image zoom level and extents, as shown in the FormIt canvas
* Simply adjust the position or zoom, and click **Finish Importing** as you did before
* When the image is re-imported into the canvas, it will move to the correct location relative to the original image position \(and may no longer be centered at the origin\):

![](../.gitbook/assets/location-step-4.png)


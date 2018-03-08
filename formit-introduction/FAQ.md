# Frequently Asked Questions

## What FormIt is and how to get it

%accordion% What is the difference between Formit, FormIt 360, and FormIt Pro? %accordion%

The "360" in FormIt has been retired ."**FormIt**" refers to the entire product. The free versions are on Web and iOS.

**FormIt PRO **refers to a subscription available only if you purchase the Autodesk AEC Industry Collection.

The subscription enables some additional features on iOS and Web and also enables you to run the Windows client.

%/accordion%

%accordion% What platforms does FormIt work on? %accordion%

Windows, Web, and iOS

%/accordion%

%accordion% What happened to the Android version?%accordion%

In an effort to streamline the FormIt product offering, we had to make the hard decision to discontinue the Android app.

If you have it installed, it will continue to run. However, you will no longer be able to install it from the Play Store as of January 30, 2018.

Any files you saved to Autodesk 360 Drive from the Android app are still available. You can access them using any of the current apps, including the free Web version.

%/accordion%

%accordion% How do I get FormIt? %accordion%

To run the Windows version, you must have access to FormIt Pro, which is part of our AEC Industry Collection subscription

So, if your office has Revit, there is a good chance you have access to FormIt already! 

You can download it directly from our website or from the Autodesk Desktop App. 

The Web version can be run directly for free from our website: http://formit.autodesk.com 

The iOS version can be downloaded for free from the Apple App Store (iPad only). 

%/accordion%

%accordion% If I am a student or educator, can I get access for FormIt Pro for no cost? %accordion%

Yes! You can access the FormIt Pro subscription through the [Autodesk Education Portal](https://www.autodesk.com/education/free-software/formit-pro).

%/accordion%

%accordion% How do I learn FormIt? %accordion%

The best place to start is the [FormIt Primer tutorial](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html). 

There are multiple parts ranging from beginner (creating an entire modern house) to more advanced (working with Revit and Dynamo in more advanced ways).

We also have over 20 videos in our FormIt Friday webinar series. These can be found on our [YouTube channel](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH).

%/accordion%

## Working with Revit

%accordion% How does FormIt work with Revit? %accordion%

This is where things get really interesting! It's a bit of a long answer, so we made [this video] (https://youtu.be/teKsLX99_FA) to explain it 

For a short version: FormIt is a completely separate 3D sketching and design application. The file that FormIt creates 

can be read into Revit to automatically create individual families which maintian materials from FormIt.

%/accordion%

%accordion% What happens when you import into Revit? %accordion%

Starting in 2016, Revit ships with an add-in for working with FormIt data. When you import a FormIt AXM file into Revit, 

it looks at each object in the file and re-creates it in Revit using the API. By default, everything in FormIt is categorized

as Mass. The FormIt Converter takes each Mass object and creates a Mass family in Revit using the [Direct Shape API](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/ENU/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html).

What is Direct Shape? It is a non-editable object used in IFC workflows. Although it is not editable, it has the distinct 

advantage of transferring full material textures between FormIt and Revit. [Here is a tutorial](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html) that explains the FormIt to Revit workflow in more detail.

%/accordion%

%accordion% How do I get FormIt? %accordion%

%/accordion%
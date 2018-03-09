# Frequently Asked Questions

## What FormIt is and how to get it

%accordion% What is the difference between Formit, FormIt 360, and FormIt Pro? %accordion%

The "360" in FormIt has been retired."**FormIt**" refers to the entire product. The free versions are on Web and iOS. **FormIt PRO ** refers to a subscription available only if you purchase the Autodesk AEC Industry Collection. The subscription enables some additional features on iOS and Web and also enables you to run the Windows client.

%/accordion%

%accordion% What platforms does FormIt work on? %accordion%

Windows, Web, and iOS

%/accordion%

%accordion% What happened to the Android version?%accordion%

In an effort to streamline the FormIt product offering, we had to make the hard decision to discontinue the Android app. If you have it installed, it will continue to run. However, you will no longer be able to install it from the Play Store as of January 30, 2018. Any files you saved to Autodesk 360 Drive from the Android app are still available. You can access them using any of the current apps, including the free Web version.

%/accordion%

%accordion% How do I get FormIt? %accordion%

To run the Windows version, you must have access to FormIt Pro, which is part of our [AEC Industry Collection](https://www.autodesk.com/collections/architecture-engineering-construction/overview) subscription. So, if your office has Revit, there is a good chance you have access to FormIt already! You can download it directly from our website or from the Autodesk Desktop App.

The Web version can be run directly for free from our website: [http://formit.autodesk.com](http://formit.autodesk.com)

The iOS version can be downloaded for free from the Apple App Store \(iPad only\).

%/accordion%

%accordion% If I am a student or educator, can I get access for FormIt Pro for no cost? %accordion%

Yes! You can access the FormIt Pro subscription through the [Autodesk Education Portal](https://www.autodesk.com/education/free-software/formit-pro).

%/accordion%

%accordion% How do I learn FormIt? %accordion%

The best place to start is the [FormIt Primer tutorial](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html).

There are multiple parts ranging from beginner \(creating an entire modern house\) to more advanced \(working with Revit and Dynamo in more advanced ways\).

We also have over 20 videos in our FormIt Friday webinar series. These can be found on our [YouTube channel](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH).

%/accordion%

## Working with Revit

%accordion% How does FormIt work with Revit? %accordion%

This is where things get really interesting! It's a bit of a long answer, so we made [this video](https://youtu.be/teKsLX99_FA) to explain it.

For a short version: FormIt is a completely separate 3D sketching and design application. The file that FormIt creates can be read into Revit to automatically create individual families which maintian materials from FormIt.

%/accordion%

%accordion% What happens when you import into Revit? %accordion%

Starting in 2016, Revit ships with an add-in for working with FormIt data. When you import a FormIt AXM file into Revit, it looks at each object in the file and re-creates it in Revit using the API. By default, everything in FormIt is categorized as Mass.

The FormIt Converter takes each Mass object and creates a Mass family in Revit using the [Direct Shape API](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/ENU/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html).

What is Direct Shape? It is a non-editable object used in IFC workflows. Although it is not editable, it has the distinct advantage of transferring full material textures between FormIt and Revit. [Here is a tutorial](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html) that explains the FormIt to Revit workflow in more detail.

%/accordion%

%accordion% Can FormIt create walls, floors and other Revit system families? %accordion%

Not directly. As stated above, each object defaults to Mass category. To create walls, floors, etc. you should import the model into Revit using the converter add-in and use native Revit tools to create system families from the underlying mass model.

%/accordion%

%accordion% Can Revit send data back to FormIt? %accordion%

Yes. To import data back into FormIt, export all, or preferably _part_ of your Revit file to the SAT file format. There is usually no need to send ALL of your Revit data to FormIt. Instead, create a filtered view in Revit that only includes the minimal data \(for instance, floors and walls\) before saving to SAT.

## Working with other apps

%/accordion%

%accordion% Why is the default file format ".AXM" %accordion%

The internal codename before FormIt was officially named was XModeler - so the file format we created was Autodesk X Modeler - hence AXM

%/accordion%

%accordion% What kind of 3D formats can FormIt import? %accordion%

* Windows:  AXM, OBJ, DWG, STL, SAT, SKP
* Web: OBJ, STL
* iOS: OBJ, STL, SAT

%/accordion%

%accordion% What kind of formats can FormIt export? %accordion%

* Windows: FBX, OBJ, SAT, STL, DAE, DXF
* Web: OBJ, SAT, STL
* iOS: OBJ

%/accordion%

%accordion% How does FormIt work with Dynamo? %accordion%

Dynamo Studio, the standalone version that runs separately from Revit, can publish scripts to [https://dynamo.autodesk.com](https://dynamo.autodesk.com). These scripts can be run \(but not edited\) inside FormIt. See this [tutorial](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Computation-Groups-with-Dynamo.html) page for more detail.

%/accordion%

%accordion% How is FormIt similar to SketchUp? %accordion%

* Better interop with Revit 
* Dynamo integration
* Native Solar Analysis and Energy Analysis powered by Autodesk Insight
* A more robust solid modeling system
* Native advanced modeling tools, like Sweep, Cover, Loft, Offset/Shell Solid, and 3D Blend/Fillet
* Diagnostic tools, like Display Watertight issues, Display Back Faces, and Flatten.
* Export pieces of the model based on what is selected and/or visible
* Native STL export for 3D printing

%/accordion%

%accordion% Can I use my SketchUp keyboard shortcuts? %accordion%

Yes! FormIt for Windows has a completely editable keyboard map. Many common SketchUp shortcuts are already there by default, but you can edit them in the Edit &gt; Preferences menu.

%/accordion&gt;

%accordion% Can I use my DWG files? %accordion%

Yes! FormIt imports 2D and 3D DWG files.

%/accordion&gt;

## Common support questions

%accordion% How do I get support? %accordion%

As with most Autodesk products, it is best to start with your reseller. Another great place to find common questions and solution is our [FormIt Forum](https://forums.autodesk.com/t5/formit-forum/bd-p/142). Did not find an answer by searching? Post your question and our team is there every day answering questions.

%/accordion&gt;

%accordion% What do I do if I cannot log in? %accordion%

* This [Forum Post](https://forums.autodesk.com/t5/formit-forum/having-trouble-logging-into-formit-for-windows-try-these-steps/td-p/7179572) covers common login issues
* If you have PC with switchable graphics processor \(GPU\) it is important to ensure that FormIt always uses the higher performance GPU. Here are instructions for [AMD](https://community.amd.com/docs/DOC-1581#jive_content_id_Assigning_Applications_to_GPUs) and [NVIDIA](http://nvidia.custhelp.com/app/answers/detail/a_id/2615/kw/manage 3d settings/related/1)

%/accordion&gt;

%accordion% What do I do if the Insight Energy Analysis seems to fail? %accordion%

If the Insight Energy Analysis reports and error or fails to return any results, here are a few things to try

* If you are working on a local version of the file, try to save the file to A360 Drive first, and then try again to Generate Insight
* If your file is already saved to A360 Drive. Try to re-save with a different file name and then try again to Generate Insight
* If you are working on the Windows client, try opening the file with Web cient and try again to Generate Insight. The Web client provides better progress feedback about 

%/accordion&gt;


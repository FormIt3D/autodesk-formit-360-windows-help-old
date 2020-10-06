# Frequently Asked Questions

## About FormIt

**What is FormIt and FormIt Pro?**

FormIt is a 3D modeling, visualization, analysis, and computation environment for architectural design. 

FormIt features:

* A robust solid modeling engine, with powerful tools and workflows optimized for building design
* Enhanced environmental visualization to illustrate design options, including saved model states using Scenes
* Location, satellite imagery, and 3D terrain using Bing Maps
* Materials from the Autodesk Material Library
* Model organization and visibility tools like Groups, Layers, and Scenes
* Analysis tools, including:
  * Watertight and Back Faces validation for solid model diagnostics and repair
  * Sun and Shadows
  * Solar Analysis
  * Energy Analysis
* Autodesk product integrations:
  * BIM 360 Docs
  * Insight \(Energy Analysis\)
  * [Dynamo](https://formit.autodesk.com/page/formit-dynamo)
  * [Revit](https://formit.autodesk.com/page/formit-revit)
* File format support:
  * Open/Import
    * AXM, DWG, FBX, SAT, STL, OBJ, WSM, SketchUp, Image
  * Export
    * AXM, FBX, OBJ, STL, SAT, DAE, DXF

FormIt is available for free on [iOS](https://itunes.apple.com/us/app/autodesk-formit-360/id575282599?mt=8) and [in your browser](https://app.formit.autodesk.com/). A **FormIt Pro** subscription is required to use [FormIt for Windows](https://formit.autodesk.com/page/download), the most powerful and feature-rich version of FormIt. The **FormIt Pro** subscription also enables additional features on iOS and Web, like Solar and Energy Analysis. **FormIt Pro** is included in the [Autodesk AEC Collection](https://www.autodesk.com/collections/architecture-engineering-construction/overview).

**What happened to FormIt for Android?**

In an effort to streamline the FormIt product offering, we had to make the hard decision to discontinue the Android app. If you have it installed, it will continue to run, but it is no longer available from the Play Store.

**How do I get FormIt?**

To run the Windows version, you must have access to **FormIt Pro**, which is part of our [AEC Industry Collection](https://www.autodesk.com/collections/architecture-engineering-construction/overview) subscription. So, if your office has Revit, there is a good chance you have access to FormIt already! You can [download FormIt for Windows directly from our website](https://formit.autodesk.com/page/download) or from the Autodesk Desktop App.

Additionally, the Web version can be run directly for free from our website: [http://formit.autodesk.com](http://formit.autodesk.com)

The iOS version can be downloaded for free from the Apple App Store \(iPad only\).

**If I am a student or educator, can I get access for FormIt Pro for no cost?**

Yes! You can access the FormIt Pro subscription through the [Autodesk Education Portal](https://www.autodesk.com/education/free-software/formit-pro).

**How do I learn FormIt?**

The best place to start is the [FormIt Primer tutorial](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html).

There are multiple sections of the Primer, ranging from beginner \(creating an entire modern house\) to more advanced \(working with Revit and Dynamo in more advanced ways\).

We also have over 20 videos in our FormIt Friday webinar series. These can be found on our [YouTube channel](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH).

## Working with Revit

**How does FormIt work with Revit?**

FormIt is a separate 3D sketching and design application, but it creates data that can be converted easily to Revit [using the FormIt Add-In for Revit](https://formit.autodesk.com/page/formit-revit).

**What happens when you import into Revit?**

Starting in 2016, Revit ships with an add-in for working with FormIt data. When you import a FormIt AXM file into Revit, this add-in looks at each object in the file and re-creates it in Revit using the API. By default, everything in FormIt is categorized as Mass.

The FormIt Converter takes each Mass object and creates a Mass family in Revit using the [Direct Shape API](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/ENU/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html).

Direct Shape is a non-editable object used in IFC workflows. Although it is not editable, it has the distinct advantage of transferring full material textures between FormIt and Revit. [Here is a tutorial](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html) that explains the FormIt to Revit workflow in more detail.

**Can FormIt create walls, floors and other Revit system families?**

Not directly. As stated above, each object defaults to Mass category. To create walls, floors, etc. you should import the model into Revit using the converter add-in and use native Revit tools to create system families from the underlying mass model.

**Can Revit send data back to FormIt?**

Yes. To import data back into FormIt, export all or, preferably, _part_ of your Revit file to the SAT file format. There is usually no need to send ALL of your Revit data to FormIt. Instead, create a filtered view in Revit that only includes the minimal data \(for instance, floors and walls\) before saving to SAT.

## Working with other apps

**Why is the default file format ".AXM"?**

The internal codename before FormIt was officially named was XModeler - so the file format we created was Autodesk X Modeler, or AXM for short.

**What kind of 3D formats can FormIt import?**

* Windows:  AXM, DWG, FBX, OBJ, SAT, SKP, STL
* Web: OBJ, STL
* iOS: OBJ, STL, SAT

**What kind of formats can FormIt export?**

* Windows: FBX, OBJ, SAT, STL, DAE, DXF
* Web: OBJ, SAT, STL
* iOS: OBJ

**How does FormIt work with Dynamo?**

[Learn how FormIt and Dynamo work together](https://formit.autodesk.com/page/formit-dynamo) to create computational design workflows.

**How does FormIt compare to SketchUp?**

* Better [**interop with Revit**](../tool-library/revit.md) ****
* [**Dynamo integration**](../tool-library/dynamo.md) for computational design
* Native tools for [**solar analysis**](../tool-library/solar-analysis.md) and [**energy analysis powered**](../tool-library/energy-analysis.md) by Autodesk Insight
* A more robust solid modeling kernel that enables advanced modeling operations
* Native advanced modeling tools like [**Sweep, Cover, Loft**](../tool-library/cover-sweep-loft.md), Offset/Shell Solid, and 3D Blend/Fillet and [**Flatten Faces**](../tool-library/flatten-face.md)
* Multiple visible [**section planes** ](../tool-library/section-planes.md)
* Diagnostic tools like [**Display Watertight issues and Display Back Faces**](../tool-library/visual-styles.md)
* [**Export pieces of the model**](../tool-library/export-data.md) based on what is selected and/or visible
* Native OBJ, SAT, and STL export

**Can I use my SketchUp keyboard shortcuts?**

Yes! FormIt for Windows has a completely editable keyboard map. Many common SketchUp shortcuts are already there by default, but you can edit them in the Edit &gt; Preferences menu.

**Can I use my DWG files?**

Yes! FormIt imports 2D and 3D DWG files.

## Common support questions

**How do I get support?**

You can start with your Autodesk reseller, or find us on the [FormIt Forum](https://forums.autodesk.com/t5/formit-forum/bd-p/142). It's best to search for the question you have first, and if it hasn't been answered, post a new topic and the FormIt team will respond.

**What do I do if I cannot log in?**

* This [Forum Post](https://forums.autodesk.com/t5/formit-forum/having-trouble-logging-into-formit-for-windows-try-these-steps/td-p/7179572) covers common login issues
* If you have a PC with a switchable graphics processor \(GPU\) it is important to ensure that FormIt always uses the higher performance GPU. Here are instructions for [AMD](https://community.amd.com/docs/DOC-1581#jive_content_id_Assigning_Applications_to_GPUs) and [NVIDIA](http://nvidia.custhelp.com/app/answers/detail/a_id/2615/kw/manage%203d%20settings/related/1)

**What do I do if Insight Energy Analysis fails?**

If the Insight Energy Analysis reports an error or fails to return any results, here are a few things to try:

* [Ensure your model is solid and manifold](https://formit.autodesk.com/blog/post/repairing-solid-models).
* Try opening the file in FormIt Web using Google Chrome and try to run Energy Analysis again. 
  * If it fails, press the F12 key to open Developer tools, go to the Console tab, and take a screenshot of the errors or warnings in the console. [Post the screenshot on the forums](https://forums.autodesk.com/t5/formit-forum/bd-p/142).


# 1.15 - Working With Revit

_One of FormIt's most exciting features is the ability to move your model from a flexible modeling environment like FormIt, to a powerful parametric environment like Revit. In this chapter, we will go through a few exercises that move various elements from FormIt to Revit, and from Revit to FormIt._

_This chapter will make use of sample Revit families. If you have not already, you can download them from the **Farnsworth House Data Set.** If you did not follow the whole tutorial up until this point, you can also download and open the **1.15 – Working With Revit.axm** file from the **FormIt Primer Part 1 Datasets**._

_In these exercises, we will use Revit 2022, which has improved interoperability capabilities with FormIt. Previous versions of Revit will not have some or any of the features shown in this tutorial, and will have different UI._

## From Revit to FormIt

### Convert Revit Families for Use in FormIt

If you \(or your firm\) have a trove of Revit Families that you want to use in FormIt, then you will be interested in this section, which discusses how to batch export RFA files to FormIt.

 _**Note:**_ _The steps below show the interface and the necessary steps when using Revit 2022, but the_ _**Convert RFA to FormIt**_ _tools has been available since Revit 2016._

1 – Open a New Revit Project or Family. Then:

1. From the **Add-Ins** ribbon, find the **FormIt Converter** panel and click on the **Convert RFA to FormIt** button. The **Convert Revit Families Dialog** will pop-up.
2. In the **Path to Revit Family File** field, browse to wherever you saved the following folder on your computer: **Farnsworth House Data Set &gt; Supporting Files &gt; Revit**.
3. In the **Path to FormIt Content** field, browser to **Farnsworth House Data Set &gt; Supporting Files &gt; FormIt &gt; Custom FormIt Content**. If you have not completed chapter **1.11 Import Models with Content Library**, you may need to create the **Custom FormIt Content** folder, or choose another destination.
4. Click **OK** to start the conversion process.

![](../../.gitbook/assets/0%20%2823%29.png)

_**Notes:**_

* _This process will take some time as Revit opens the_ _**RFA**_ _in the first path, then converts and saves it as an_ _**AXMF**_ _format for FormIt._
* _In this exercise, we are only converting a single file, but you can use this process to batch-convert all_ _**RFAs**_ _in the selected folder \(including any_ _**RFAs**_ _in nested folders\)._

2 - Once the process is completed, go back to FormIt. There you will see the new content appear in the **Content Library Palette**, inside the **FormIt &gt;** **Custom FormIt Content** folder we previously linked. If you saved your converted **AXMF** file\(s\) to a different location, or did not complete chapter **1.11 Import Models with Content Library**, you may need to add that folder to your content library to see its contents. Refer to chapter 1.11 for instructions on how to add folders to your content library.

![](../../.gitbook/assets/1%20%2824%29.png)‌

**Note**: _Not all categories from Revit are supported for export. The 'free standing' or ‘level based’ families are supported, but the 'host based' families like doors and windows are not. Mass, Casework, Entourage, Furniture, Furniture System, Generic Model, Parking, Site, and Specialty Equipment are all supported. Any unsupported families in the selected fold will simply be skipped._

## From FormIt to Revit

_There are two different ways to bring geometry from FormIt to Revit. You can import an existing_ _**.axm**, into either a Revit project or Revit family file, which will behave similarly to an imported model or CAD file. Alternatively, you can launch FormIt from within Revit, and bring each FormIt group into Revit as an individual Generic Model element. The second method is covered in the **Part II** chapter_ _**2.8**_ _**Advanced Revit Workflows**._

### Importing the Farnsworth House to Revit

1 – To import an FormIt file \(**.axm**\) to Revit, start a new Revit project and open the default 3D view. Then:

1. Go to the **Insert Tab**, and click on the **Import CAD** button. The **Import CAD Formats** window will open.
2. Make sure the **Files of type** dropdown is set to **FormIt Files \(\*.axm\)**.
3. Navigate to and select the Farnsworth **.axm** file you have been working on. If you have not been following along with the Primer Part I, you can also open **1.15 – Working With Revit.axm** file the **Farnsworth House Data Set &gt; Chapter Files** folder.
4. Make sure that **Import FormIt Levels** is checked.
5. Once the settings are defined, click **Open**, and the FormIt geometry will be brought into Revit as a single element.

![](../../.gitbook/assets/2%20%2824%29.png)

Importing a FormIt file using the import CAD button.

![](../../.gitbook/assets/3%20%2821%29.png)  
Imported .axm element. Note that the Levels from the FormIt model are also imported into Revit.

_Similar to other CAD formats, the layers in the original file are imported to Revit. This feature allows you to define different visibility settings for each layer to easily manipulate the graphic appearance of your FormIt file in any Revit view._

2 – To adjust the imported .axm file’s layer visibility:

1. Go to the **Visibility/Graphic Overrides \(VG or VV\)** window, **Imported Categories** tab, expand your imported FormIt file, and uncheck the **Planting** layer to turn off the layer in the current view, and click **OK**.
2. Change the **Visual Style** to **Realistic**, and you will see that all the FormIt materials have been imported into Revit.

![](../../.gitbook/assets/4%20%2820%29.png)

3 - In fact, the imported FormIt materials will now be available in this Revit project, tagged with the Class **FormIt**. Just open the **Material Browser** and search for “FormIt” and you will see them all. These can now be used in your Revit project just like any other material.

![](../../.gitbook/assets/5%20%2819%29.png)


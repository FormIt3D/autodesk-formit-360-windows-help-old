### Import Data from FormIt into Revit

1. Still inside Revit, choose **Import FormIt 360 to RVT** from the add-in. ![](./images/9a7673f7-a265-49c8-b665-325e9618ac65.png)
2. Choose **farnsworth07.axm** from **** the FormIt Primer folder.
3. This process will take a few minutes as Revit converts each object in the FormIt file into individual Mass, Generic, and Furniture family instances. 
![](./images/cce7e450-4f6b-4f05-bdb1-88c385f58040.png)
4. If we inspect the various objects, we will see that most are mass families. The Columns however, are Generic family. This will allow us to edit the family and convert to another category such as Structural Column.
5. The various furniture objects are Furniture category. There is one more tool that we can use to automatically swap out the ones that were converted in the previous exercise. Select **Reload Families** from the add-in. ![](./images/fbd116b0-fbb7-4d89-a15a-83ae42639705.png)
6. In the dialog, select **FormIt Primer\\content.** This will point the converter at all sub-folders under this folder. Press OK. This process will take a number of minutes as it looks at each family and tries to make a match and reload the proper RFA file in its place. 
![](./images/a97d2f55-e13c-4c34-b885-789f272949cc.png)

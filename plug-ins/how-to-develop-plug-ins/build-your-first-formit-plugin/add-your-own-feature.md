# Add your own feature

### Sample files and code

The html file (left) allows you to modify the user interface of your plugin, the js file (middle) is where you write the code for how the function works and the css file (right) includes styles to determine the appearance of your html elements.

![](<../../../.gitbook/assets/image (10) (1).png>)

###

### Add a function to create cylinder&#x20;

Let's add a feature to this plugin for creating cylinder.

First, configure the input field and UI button in the html file, copy the following code and paste it after line 23 and before _\<!-- Do not remove below scripts unless you know what you're doing- - >_

```
<p>Cylinder: Create a cylinder at the origin.</p>
<div>
    <input id="Radius" type=number value=2 />
    <label>Radius</label>
</div>
        
<div>
    <input id="CHeight" type=number value =0.5 />
    <label>Height</label>
</div>
        

<input id="CreateCylinderBtn" type=button value="Create Cylinder" />
        
```

![](<../../../.gitbook/assets/image (20) (1) (1).png>)

Next, add the function in the js file. Copy the following code and paste it at the end of the file (after line 16)

```
// Create cylinder
const createCylinder = async (r,h) =>
{
    const posCenter = await WSM.Geom.Point3d(0,0,0);

    const histID = await FormIt.GroupEdit.GetEditingHistoryID();
    console.log(histID,posCenter,r,h);

    const cyl = await WSM.APICreateCylinder(histID,posCenter,r,h);
}


// Execute function when 'create cylinder' button is clicked
document.getElementById("CreateCylinderBtn").addEventListener("click", ()=>
{
    console.log('create cylinder clicked')

    const r = Number(document.getElementById("Radius").value);
    const h = Number(document.getElementById("CHeight").value);

    createCylinder(r,h);

});
```

![](<../../../.gitbook/assets/image (19) (1).png>)

###

### Run and preview plugin

When you’re ready to see the results, click the Play Arrow button ![](<../../../.gitbook/assets/image (18) (1) (1).png>) again and you will see the update of your plugin in the same window.

![](<../../../.gitbook/assets/image (5).png>)

###

### FormIt plugins API

For a complete documentation on the FormIt plugins API please refer: [https://formit3d.github.io/FormItExamplePlugins/docs/FormItJSAPI/](https://formit3d.github.io/FormItExamplePlugins/docs/FormItJSAPI/)

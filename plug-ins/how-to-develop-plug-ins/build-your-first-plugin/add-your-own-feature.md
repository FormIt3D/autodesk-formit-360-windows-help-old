# Adding Your Own Features

### Inside the HTML, JavaScript, and CSS Panels

When you click Edit in the Plugin Playground sample plugin, you will see the HTML, JavaScript (JS), and CSS panels. The HTML panel (left) enables you to modify the user interface of your plugin. The JS panel (middle) enables you to write functions that can communicate to FormIt using the FormIt JS Plugin API. Finally, the CSS panel (right) will determine the style of your HTML.

![](<../../../.gitbook/assets/image (10) (1) (1).png>)

### Adding a Function to Create a Cylinder&#x20;

Let's add a feature to this plugin to create a cylinder.

First, let's configure the input field and UI button in the HTML panel. Copy the following code and paste it after line 23 and before _\<!-- Do not remove below scripts unless you know what you're doing- - >_

This will add some basic UI elements to our plugin.

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

![](<../../../.gitbook/assets/image (20) (1) (1) (1).png>)

Next, let's add two functions in our JS panel. Copy the following code and paste it at the end of the file (after line 16).

This will create a cylinder in our FormIt workspace.

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

![](<../../../.gitbook/assets/image (19) (1) (1) (1).png>)

### Running and previewing

When you’re ready to see the results, click the Play button ![](<../../../.gitbook/assets/image (18) (1) (1) (1) (1) (1).png>) again and you will see your updates to the plugin in the same panel.

![](<../../../.gitbook/assets/image (5) (1).png>)

### FormIt plugins API

For complete documentation on the FormIt plugins API, see the [useful links](../useful-links.md) section.

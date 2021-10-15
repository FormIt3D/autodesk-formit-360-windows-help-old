# Coding to add your own feature

1\. Make some modifications to this code, we can try add a function to create cylinder.

2\. Add the input field and UI button in the html section

```
// Input fields

<p>Cylinder: Create a cylinder at the origin.</p>
<div>
    <input id="Radius" type=number value=2 />
    <label>Radius</label>
</div>
        
<div>
    <input id="CHeight" type=number value =0.5 />
    <label>Height</label>
</div>
        
// Buttom for create cylinder

<input id="CreateCylinderBtn" type=button value="Create Cylinder" />
        
```

3\. Add the function in the js section

```
// Create cylinder

const createCylinder = async (r,h) =>
{
    const posCenter = await WSM.Geom.Point3d(0,0,0);

    const histID = await FormIt.GroupEdit.GetEditingHistoryID();
    console.log(histID,posCenter,r,h);

    const cyl = await WSM.APICreateCylinder(histID,posCenter,r,h);
}


// Execute function when 'create cylinder' button is click
document.getElementById("CreateCylinderBtn").addEventListener("click", ()=>
{
    console.log('create cylinder clicked')

    const r = Number(document.getElementById("Radius").value);
    const h = Number(document.getElementById("CHeight").value);

    createCylinder(r,h);

});
```

4\. When you’re ready to see the results, click the Play Arrow button again.

![](<../../../.gitbook/assets/image (5).png>)

2\. For more documentation on the FormIt plug-ins API: [https://formit3d.github.io/FormItExamplePlugins/docs/FormItJSAPI/](https://formit3d.github.io/FormItExamplePlugins/docs/FormItJSAPI/)

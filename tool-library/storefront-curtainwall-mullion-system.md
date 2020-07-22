# Storefront/Curtainwall Mullion System

![](../.gitbook/assets/dynamo-storefront-system-options.gif)

## Powered by Dynamo

The ability to quickly create storefront/curtainwall mullion systems in FormIt is powered by Dynamo. You can find the Storefront Curtainwall system in the Dynamo Samples directory in the Dynamo panel:

![](../.gitbook/assets/storefront-curtainwall-button%20%281%29.png)

## Selecting "Glass" For Mullion System

Starting in FormIt 2021.2, the Storefront Curtainwall system uses the new [SelectFromFormIt node](https://formit.autodesk.com/page/formit-dynamo#dynamo-formit-nodes), allowing you to select a piece of "glass" \(a single face or an extruded solid\) around which to generate a mullion system.

![A simple plane of &quot;glass&quot; with an opening for doors at the bottom.](../.gitbook/assets/storefron-system-1_glass-only.png)

When you click the Storefront Curtainwall thumbnail \(notice the icon indicating that a selection is required\), FormIt will prompt you to select the glass geometry to continue:

![](../.gitbook/assets/storefront-curtainwall-prompt.png)

A few notes and caveats about how selecting glass works:

* Currently, only planar surfaces are supported. If you select a series of surfaces \(for example, a "curved" surface comprised of smaller planar surfaces\), the script will find the largest planar face and will use that.
* If your glass is solid - i.e. a single face extruded very slightly to convey a bit of thickness - the script will find the biggest surface, so the resulting mullions will generate on one side of the glass solid.
* You can sketch openings for doors, and remove the resulting surface from the glass boundary, and the resulting mullions will respect the door opening, leaving it blank for the addition of doors.
* Due to Dynamo limitations, this script won't work if the glass geometry has openings in the middle.

## Tips and Tricks

When selecting geometry for a Dynamo graph in FormIt, certain organizational tricks can simplify the experience and allow for easy instancing of results:




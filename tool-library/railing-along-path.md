# Railing Along Path

## Powered By Dynamo

In FormIt 2021 and newer, you can generate a railing along a path, and quickly customize the results in-place. Railing Along Path is powered by Dynamo, which means the resulting railing is easily configurable to get the results you want, and re-running the logic will update the geometry in-place.

![](../.gitbook/assets/railing-along-path.gif)

## Starting Railing Along Path

* Go to the Dynamo panel in FormIt for Windows, and ensure you're in the Dynamo Samples directory
* Click the Railing Along Path sample
* On the left side of the screen, you'll see a prompt to "Select path for railing"
  * You should select only a series of contiguous edges, or a Group containing only a series of edges.
  * Once you've got the path selected, click the "finish" button, or hit Enter/Return.
* The Dynamo panel will indicate it's processing the changes. When it's done, you'll have a Dynamo-generated railing in a FormIt Group, ready for modifying \(see below\).

## Iterating In Place

After running Railing Along Path, you'll notice its results are set to default values. Maybe these work for you, but you can heavily customize the railing to suit your needs.

When Railing Along Path runs, it creates a new Group containing the results, and FormIt will automatically select the Group and show the available options for that Railing Along Path instance.

You can always return to the Railing Along Path properties by selecting the Group and switching to the Properties panel, or by editing the Group which will automatically show Properties.

![](../.gitbook/assets/railing-along-path-options.png)

### Railing Height

The overall height of the railing. Uses the current FormIt units.

### Post Spacing

The spacing between main vertical posts. Uses the current FormIt units.

### Add Posts at Path Vertices

When **true**, posts will be added at each vertex of the selected path, and the calculation for the next post positioning resets at that point.

For example, if you selected a series of 3 edges, a post will appear at each of the two inner points. This is useful if the vertices indicate a change of direction \(like going up stairs or turning corners\) where a post would naturally occur.

When **false**, posts will only be added along the path starting from one end, and measuring the distance along the path, ignoring vertices along the way. This is useful if you've selected an arc, spline, or circle, where the vertices are not important, and you want the post spacing to ignore them.

### Reverse Path Direction

When calculating the positioning of the posts, the direction of the chosen path will determine which end of the path will start the post spacing measurement.

In cases where the post spacing results in leftover space on an undesirable end of the path, you can change this value to **true** to flip the curve, and start the post spacing measurement at the opposite end.

### Post Width + Depth

The size \(in plan\) of the rectangular vertical post profiles. Uses the current FormIt units.

### Handrail Width + Height

The size \(in section\) of the rectangular handrail profile. Uses the current FormIt units.

### Baluster Orientation

When true, balusters will be oriented horizontally, like cables. When false, the balusters will be oriented vertically, for a more traditional aesthetic.

### Baluster width + Depth

The size of the baluster's rectangular profile. Uses the current FormIt units.

### Baluster Spacing

The amount of space between each baluster. Uses the current FormIt units.

### Bottom Rail Start Height

The distance between the bottom of the railing, and the bottom rail that supports the balusters. Uses the current FormIt units.

### Run

After editing the options, click the "Run" button to run the underlying Dynamo graph, and generate new results. This button will turn blue when parameters have changed, so you know it needs to be clicked to see the updates in the final geometry.‌

### Edit Embedded Graph

Clicking this will launch the Dynamo graph editor environment, so you can view and edit the underlying Dynamo graph to more quickly change parameters and see live updates, or to inspect/adjust the logic.


# Groups

One of the most basic yet important techniques in FormIt workflows involves grouping. Groups allow you to keep your geometry from sticking together and allow you to set up parent/child relationships between copied elements so that if you update one element, both elements update. Learn more about groups [here](../formit-primer/part-i/grouping-objects.md).

Groups can be created and edited in two ways: either from the context menu of a selected group, or from the main toolbar.

## Groups Interactions

To **create a group**, select the elements you'd like to group together — this can include edges, faces, solids, or other groups — and right-click. Choose the **Group \(G\)** tool from the context menu. Imported images and satellite images cannot be grouped.

To **select a group**,  single-click the group. Note the dashed lines that appear when selecting a group — these lines indicate the group's total size.

To **edit a group**, double-click the group. This launches an edit mode where you can only view and snap to elements outside of the current group, but cannot select them. You can also hide the elements outside of the current group by using the **H** keyboard shortcut.

You can create **groups within groups:** these are called **nested groups** and can be created within the group edit mode. To move up one level in nested groups, click anywhere outside of the groups.

To **exit group edit mode,** double-click anywhere outside of the group.

You can **copy a group** to create a relationship between the original group and its copy: if you edit any copied groups, the same changes will affect all related groups.

To **sever the relationship between copied groups**, select the group or groups you would like to make separate, right-click, and choose **Make Unique** from the context menu. You can also select Make Unique from the Groups toolbar.

To **select all related groups**, hover over a group and press the Tab key. When all related groups become highlighted, click on the groups to select them. You can then perform an action on all groups at once.

The [**Groups Tree**](groups-tree.md) provides a single place to view and manage all of the groups in a project.

## Groups Context menu and Toolbar access

## ![](../.gitbook/assets/grouptoolbar.png)

**Group Elements**

To create a group from the Groups toolbar item, select one or more elements, select the **Create Group** icon, and then select the **Finish** icon. Alternatively, you can select **Create Group** from the Groups tool bar item, then select elements you would like to group and select the **Finish** icon.

To **edit a group from the Groups toolbar item**, select the **Edit Group** icon and then click the group you want to edit. When you are done making edits, select the **Finish** icon. This tool allows you to choose the specific group you'd like to edit, even if it is deeply nested.

**To make a group unique from the toolbar,** select the **Make Unique** icon in the Groups toolbar item. Additionally, you can select **Make Unique** from the Groups toolbar item and then select the group you would like to make unique and click the **Finish** icon.

**To ungroup a group from the Groups toolbar item,** select the group you want to change and choose the **Ungroup** icon from the Groups toolbar menu.This ungroups your current selection, but does not ungroup any nested groups. Alternatively, you can select **Ungroup** from the toolbar, select the group you want to change, and then select the **Finish** icon.

**To ungroup all groups nested below your currently selected group,** select a group with nested groups and choose **Ungroup All Nested** from the Groups toolbar.

**To ungroup all groups in your model,** select the **Ungroup All** tool from the Groups toolbar.

## Groups and Revit

If you're familiar with Revit **families**, then you are familiar with the concept of groups in FormIt. FormIt groups have features you can use to transfer them intelligently into Revit.

**FormIt Group Categories**

You can specify the **categories** for groups in FormIt so that your FormIt groups become families of the same categories when you import them into Revit. You can assign categories to your FormIt groups by selecting a group, entering **Group Edit** mode, and using the **Properties** panel to choose categories. You can also assign categories in the **Groups Tree** panel.

**FormIt Group Names**

You can also use the **Properties** panel to specify a name for your FormIt group. This can be helpful in navigating your own model, and when you import your model to Revit you can easily filter elementsusing the name of the group.

Note that **nested groups in FormIt are not imported into Revit as nested groups**. This prevents deeply-nested Revit families.


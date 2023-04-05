# Overview

The **Live Inventory** page provides an aggregated view of all of your **Integration Assets** in an **Asset Class**. This page has several search features that allow you to filter and view information about specific assets. Access this page by selecting the **Live Inventory** icon on the **Navigation bar** and clicking the **Devices** or **Users** link from the dropdown.

![Navigating to the Live Inventory page](https://my.sev.co/docs/Inventory_NavToInventory.gif)

<br>

***



# Inventory Views

The Live Inventory page has three ways for you to view your assets: **List**, **Geo** _(map)_, and **Network**.

<br>

## List

Of the three views, List view provides the most comprehensive snapshot of your assets. In this view, you will be able view **asset details**, **Integrations**, and more.

![Inventory Page in List View](https://my.sev.co/docs/SevcoWalkthrough_LiveInventoryPage_Labeled.png)

<br>

In this view, each **Row** represents a unique **asset** in your Organization. Select the caret (<img src="https://my.sev.co/docs/Inventory_ListView_Caret.png" width="20px">) to reveal additional information about it.

**Columns** represent each of your configured Integrations and the cells within them are used to indicate if and when a particular asset was last observed by an Integration. **Lighter cells** represent assets that have been observed more recently while **darker cells** represent ones that have been observed less recently. If a cell is **black**, it means the asset has never been observed by the Integration.

![Device Details preview](https://my.sev.co/docs/SevcoWalkthrough_DeviceDetailsPreview.png)

<br>

## Geo

Geo view allows you to view assets by their geographical location. Select a teal **map point** to zoom in on an area where multiple assets are located. 

![Selecting an icon on the "Geo" map to zoom in and filter by region](https://my.sev.co/docs/Inventory_GeoView_ZoomInOnRegion.gif)

<br>

If only one asset is present in a location, you may click on it to view **details** about it. If two or more assets are present in a location, select the **See details** link to view their information in **List** view.

![Clicking on a single device to view Device Details then selecting a group of devices to view it in "List" view](https://my.sev.co/docs/Inventory_GeoView_SelectDevices.gif)

<br>

## Network

Network view organizes your assets into three catagories: **On-Premise**, **Cloud**, and **Unknown**. Assets in the latter category are then broken down further and organized by country. 

![Network View](https://my.sev.co/docs/Inventory_NetworkView.png)

<br>

***



# Integration Venn Diagram

The Integration Venn Diagram tool compares asset data from up to **five Integrations** then organizes it into a venn diagram to visually communicate what assets are recognized by each Integration. Integrations can be added and removed from the **Integrations** dropdown menu. You may also remove an Integration by selecting its icon to the right of the dropdown.

Upon inspection, you'll likely notice that not all of your assets are recognizable to each of the Integrations you've selected. **Don't panic!** It isn't uncommon for assets to be unaccounted for by one or more Integrations – in fact, it is one of the many problems the Sevco platform was built to solve!

![Opening the "Sources" Dropdown then selecting and deselecting Source checkboxes. Next, selecting Source icons to remove them](https://my.sev.co/docs/SevcoWalkthrough_LiveInventory_DeselectSources.gif)

From here you can select various sections of the Venn Diagram to view a list of the assets in them and assess any coverage gaps.

<br>

___



# Filters

In addition to the Venn Diagram tool, the Live Inventory page also has a number of filters you can use in your asset searches. These filters include:

- OS Platform
- OS Release
- Tag Names
- Mac Manufacture
- Region
- Country
- Domain

Select the **Include** button (**+**) to _only_ include assets falling under a specific filter category in your results and the **Exclude** button (**x**) to remove them from your results all together. 

![Selecting Include & Exclude filtering icons](https://my.sev.co/docs/Inventory_Filters_Include%26ExcludeZoom.gif)

<br>

___



# Query Builder

For more granular searches that may not be accomplishable using the Venn Diagram or filtering tools, you may wish to write a query. 

The **Query Builder** is located at the top of the Live Inventory page and has a number of rules and parameters that can be used to create and execute complex queries to find gaps in asset coverage that may not be as obvious.

![Opening the Query Builder](https://my.sev.co/docs/SevcoWalkthrough_OpenQueryPanel_2-0.gif)

<br>

The Query Builder has four main parameters that can be used to assemble a query:

- **Scope:** The Scope parameter allows you to specify that you would only like to include assets from a specific Integration in your query results. _This field is optional_.
- **Attribute:** The Attribute parameter is where you will select the what data attribute(s) _(i.e. IP Address)_ you would like to build your query around.
- **Condition:** The condition field is used to define the conditions your selected Attribute must meet. Only assets with Attributes meeting this condition will be displayed in your results.
- **Value:** Once you've selected an Attribute and Condition, you will need to define the **Value** you will be using to determine if a Condition is satisfied. Please note that this field will not display when the **Exists** or **Does not exist** Condition is selected, as the value is already defined in the Condition itself.

![Selecting a Query Attribute](https://my.sev.co/docs/SevcoWalkthrough_Query_SelectAttribute_2-0.gif)

<br>

For more complex queries, you will want to take advantage of the **Add Rule** and **Add Group** options.

- The **Add Rule** option allows you to add additional conditions to your query. Once you've added a rule, you can use the **and / or** to decide if the rule must be met in addition to your previous rule or if the system can include assets meeting either set of conditions in your results.
- The **Add Group** option allows you to group rules in complex queries. You may wish to use this, if you are writing a query where some conditions must be met while other are optional. 

![Building a query using the "or" Group option](https://my.sev.co/docs/Inventory_QueryBuilder_AddGroup.gif)

<br>

After a query has been run, it will appear in the **Recent Queries** tab of the Query Builder. If you plan on running a query on a regular basis, hover over it and select the **Save** button to add it to either the **My Queries** or **Org-wide queries** tab. Once a query has been saved, you will also be able to apply **actions** to it as well. [Click here](doc:manage-query-reports) to learn more about these processes.

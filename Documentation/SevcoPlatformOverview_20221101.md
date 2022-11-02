# Overview

The purpose of this article is to provide a general overview of the Sevco platform's pages and functionality. This walk through assumes that you have already completed the initial setup for your Organization and are already collecting asset data. If you have not already done so, please refer to our [Quick Start Guide](doc:quick-start-guide) for instructions.

The Sevco platform is rapidly evolving, as we continue adding new features and making improvements to existing ones. As such, supporting documentation may lag behind from time to time. If you are unable to find information about a particular page or feature, please don't hesitate to reach out to us at [support@sevco.io](mailto:support@sevco.io) or utilize our in-app [Support Chat](#help-menu).

<br>

____

# Dashboard

The **Dashboard** provides a high-level overview of both the history and current status of your **Assets** and configured **Sources**. Additionally, it can also redirect you to other pages in the Sevco platform where you can review information in greater detail.

![Dashboard page](/images/Dashboard.png)

## Asset Totals

Asset totals for **Devices** and **Users** are located at the top of the Dashboard. On the left, you can find the total number of Devices or Users in your Organization. The **timeline** on the right provides insight into asset totals from previous days. Each day is represented by a bar on the timeline. Hovering over a bar displays asset totals for that day.

![Hovering over bar on Device Total history timeline](/images/Dashboard_AssetCount_Hover.gif)

<br>

## Enterprise Endpoint Controls Coverage Report

The **Enterprise Endpoint Controls Coverage Report** section of the Dashboard provides insight into device coverage by Sources falling under the **Enterprise Endpoint** category. **Endpoint Security**, **Configuration Management**, and **Directory Services** source types are included in this category and coverage can be reviewed by **operating system (OS)** or **Network location**

* The total number of **devices** associated with a **Network Location** or **Operating System** are listed in the far-left column.

* The **Percentages** and **totals** in each **cell** represent devices with coverage by a **Source** in the Enterprise Endpoint **category** it is listed under.

![Enterprise Controls Coverage](/images/ControlsCoverageMatrix.png)

<br>

Use the tabs to navigate between the **OS** and **Network Location** views.

![Switching between OS and Network Location view](/images/ControlsCoverage_SwitchingViews.gif)

Select the **Explore coverage gaps** link in any cell to be redirected to the [**Device Inventory**](doc:use-the-sevco-platform#live-inventory) page where you can view additional information about its corresponding devices.

![Clicking 'Explore coverage gaps link'](/images/ControlsCoverage_ExploreCoverage.gif)


<br>

## Source Inventory Overview

The **Source Inventory Overview** section provides a snapshot of the Sources you've configured. In this section, you will find information about the total number of assets identified by each Source, disabled Sources, and Source errors. 

You can also view asset totals from previous days by hovering over a Source's **timeline**.

![Hover over Source timeline](/images/Dashboard_SourceCount_Hover.gif)

<br>


Select a Source to view its **Source Inventory** page, where you can find additional information about it.

![Selecting a Source](/images/Dashboard_SourceCount_Click.gif)

<br>

____

# Live Inventory 

The **Live Inventory** page provides an aggregated view of all of your **Source Assets** in an **Asset Class**. This page has several search features that allow you to filter and view information about specific assets. Access this page by selecting the **Live Inventory** icon on the **Navigation bar** and clicking the **Devices** or **Users** link from the dropdown.

![Navigating to the Live Inventory page](/images/Inventory_NavToInventory.gif)

<br>


## Inventory Views

The Live Inventory page has three ways for you to view your assets: **List**, **Geo** _(map)_, and **Network**.

<br>


### List

Of the three views, List view provides the most comprehensive snapshot of your assets. In this view, you will be able view **asset details**, **Sources**, and more.

![Inventory Page in List View](/images/SevcoWalkthrough_LiveInventoryPage_Labeled.png)

<br>


In this view, each **Row** represents a unique **asset** in your Organization. Select the caret (<img src="/images/Inventory_ListView_Caret.png" width="20px">) to reveal additional information about it.

**Columns** represent each of your configured Sources and the cells within them are used to indicate if and when a particular asset was last observed by a Source. **Lighter cells** represent assets that have been observed more recently while **darker cells** represent ones that have been observed less recently. If a cell is **black**, it means the asset has never been observed by the Source.

![Device Details preview](/images/SevcoWalkthrough_DeviceDetailsPreview.png)

<br>



### Geo

Geo view allows you to view assets by their geographical location. Select a teal **map point** to zoom in on an area where multiple assets are located. 

![Selecting an icon on the "Geo" map to zoom in and filter by region](/images/Inventory_GeoView_ZoomInOnRegion.gif)

<br>


If only one asset is present in a location, you may click on it to view **details** about it. If two or more assets are present in a location, select the **See devices** link to view their information in **List** view.

![Clicking on a single device to view Device Details then selecting a group of devices to view it in "List" view](/images/Inventory_GeoView_SelectDevices.gif)

<br>


### Network

Network view organizes your assets into three catagories: **On-Premise**, **Cloud**, and **Unknown**. Assets in the latter category are then broken down further and organized by country. 

![Network View](/images/Inventory_NetworkView.png)

<br>


## Source Venn Diagram

The Source Venn Diagram tool compares asset data from up to **five sources** then organizes it into a venn diagram to visually communicate what assets are recognized by each Source. Sources can be added and removed from the **Sources** dropdown menu. You may also remove a Source by selecting its icon to the right of the dropdown.

Upon inspection, you'll likely notice that not all of your assets are recognizable to each of the Sources you've selected. **Don't panic!** It isn't uncommon for assets to be unaccounted for by one or more sources – in fact, it is one of the many problems the Sevco platform was built to solve!

![Opening the "Sources" Dropdown then selecting and deselecting Source checkboxes. Next, selecting Source icons to remove them](/images/SevcoWalkthrough_LiveInventory_DeselectSources.gif)

From here you can select various sections of the Venn Diagram to view a list of the assets in them and assess any coverage gaps.

<br>


## Filters

In addition to the Venn Diagram tool, the Live Inventory page also has a number of filters you can use in your asset searches. These filters include:

- OS Platform
- OS Release
- Tag Names
- Mac Manufacture
- Region
- Country
- Domain

Select the **Include** button (**+**) to _only_ include assets falling under a specific filter category in your results and the **Exclude** button (**x**) to remove them from your results all together. 

![Selecting Include & Exclude filtering icons](/images/Inventory_Filters_Include%26ExcludeZoom.gif)

<br>


## Query Builder

For more granular searches that may not be accomplishable using the Venn Diagram or filtering tools, you may wish to write a query. 

The **Query Builder** is located at the top of the Live Inventory page and has a number of rules and parameters that can be used to create and execute complex queries to find gaps in asset coverage that may not be as obvious.

![Opening the Query Builder](/images/SevcoWalkthrough_OpenQueryPanel.gif)

<br>


The Query Builder has four main parameters that can be used to assemble a query:

- **Scope:** The Scope parameter allows you to specify that you would only like to include assets from a specific Source in your query results. _This field is optional_.
- **Attribute:** The Attribute parameter is where you will select the what data attribute(s) _(i.e. IP Address)_ you would like to build your query around.
- **Condition:** The condition field is used to define the conditions your selected Attribute must meet. Only assets with Attributes meeting this condition will be displayed in your results.
- **Value:** Once you've selected an Attribute and Condition, you will need to define the **Value** you will be using to determine if a Condition is satisfied. Please note that this field will not display when the **Exists** or **Does not exist** Condition is selected, as the value is already defined in the Condition itself.

![Selecting a Query Attribute](/images/SevcoWalkthrough_Query_SelectAttribute.gif)

<br>


For more complex queries, you will want to take advantage of the **Add Rule** and **Add Group** options.
- The **Add Rule** option allows you to add additional conditions to your query. Once you've added a rule, you can use the **and / or** to decide if the rule must be met in addition to your previous rule or if the system can include assets meeting either set of conditions in your results.
- The **Add Group** option allows you to group rules in complex queries. You may wish to use this, if you are writing a query where some conditions must be met while other are optional. 

![Building a query using the "or" Group option](/images/Inventory_QueryBuilder_AddGroup.gif)

<br>


After a query has been run, it will appear in the **Recent Queries** tab of the Query Builder. If you plan on running a query on a regular basis, select the **star** next to it to add it to the **Saved Queries** tab. Once a query has been saved, you will also be able to for it as well.   

![Recent Queries list](/images/SevcoWalkthrough_RecentQueries.png)

<br>


<br>

____

# Telemetry

While the [**Live Inventory**](#live-inventory) page provides a snapshot of the current state of your assets, the **Telemetry** page tracks assets at the event level and shows how their attributes have changed in the time leading up to that point.

![Telemetry page](/images/SevcoWalkthrough_TelemetryPage.png)

<br>


## Telemetry Filters

On the left side of the page, there are several filters you can use to search for specific telemetry events.

- **Sources:** this filter allows you to include and exclude telemetry events from specific Sources. For example, you may only wish to view telemetry events related to Crowdstrike.
- **Attributes:** this filter allows you to search for telemetry events involving changes to specific attributes. For example, using changes to a Source's **agent version** to determine if an asset is running the most up-to-date version of it.
- **Event Types:** this filter allows to include and exclude specific telemetry event types. For example, if you've recently configured a new Source for your Organization, you may wish to filter for the `SourceMembershipAdd` event type.

Like the filters on the **Live Inventory** page, you can select the **Include** button (**+**) to _only_ include assets falling under a specific filter category in your results and the **Exclude** button (**x**) to remove them from your results all together. 

<br>


## Event History

The right side of the page provides a visual representation of events over time and is responsive to telemetry-filtering selections and queries. Use the **date picker** or click and drag over a specific section of the **Event Bar Graph** to view events within a specific time frame. All events meeting the conditions you've established will be listed in the **Event List** 

![Telemetry bar graph filtered by date, with event list below](/images/SevcoWalkthrough_Telemetry_SelectTimeframe.gif)

<br>


## Telemetry Queries

Like the **Live Inventory** page, the Telemetry page also features a **query builder** that can be used to run complex searches that may not be accomplishable using the telemetry filtering tools.

![Telemetry Query Builder](/images/Telemetry_QueryBuilder.png)

<br>

____

# Asset Details

In addition to the information found on the Live Inventory page, you can also view additional information about specific **assets** on their **Details** page. 

Asset Details pages can be accessed by identifying the asset you would like to view in the **Asset List** on the **Live Inventory** page, opening its dropdown, and selecting the **See Details** link.

![Navigating to an Asset's details page](/images/AssetDetails_NavigateToPage.gif)

<br>

The **left panel** of the Details page displays information that has been aggregated from all of its associated **Sources**. 

Notice how this Device has three **Internal IPs** listed. If we look at data collected from **Illumio**, **Automax** and **MalwareBytes** we will find that they have identified `10.20.199.156` as the Device's Internal IP.

![Switching between Sources and highlighting matching Internal IP addresses](/images/AssetDetails_Sources_InternalIPExample.gif)

<br>


However, when we look at **Lansweeper** we will also see a second Internal IP, `10.41.212.101` listed. Both of these are included in the left panel.

![Viewing Lansweeper, which has an additional Internal IP address, and showing that it is also listed in the left panel](/images/AssetDetails_Sources_InternalIPExample_twoIPs.gif)

<br>

As we stated earlier, the **right panel** of the Details page allows you to review information about assets by Source. Users can select a Source at the to view the most recent information it has collected about an asset.

Additionally, the right panel also allows you to view any **telemetry events** associated with that asset by Source. This feature functions very similarly to the [Event History](#event-history) section of the **Telemetry** page.

![Navigating between Sources to view associated Telemetry events](/images/AssetDetails_ShowTelemetryData_Example.gif)


<br>

____


# Source Inventory

**Source Inventory** pages are source-specific and only display **asset data** from a single source. Source Inventory pages can be used to search for an monitor assets associated with a Source. Additionally, you can also review information about and a Source's health (**Status**) and reconfigure it as-needed.

![Source Inventory Page](/images/SourceInventoryPage.png)

<br>

To access a Source Inventory page, select the **Source Inventory** icon on the **Navigation bar** then select the Source you would like to view information about from the **dropdown**. This is also where you can [configure new sources](doc:adding-a-source).

![Source Inventory Menu](/images/SourceInventoryMenu_Open.gif)

> ⚠️
> Make sure to pay attention to the **Devices** and **Users** tabs at the top of the Source Inventory dropdown, as Sources are separated by **asset type**. 


<br>



On the left side of the page, there are several filters you can use to search for specific Source assets:

- OS Platforms
- OS Releases
- Mac Manufacturers

Additionally, the page has a **query builder** that can be used to run complex searches that may not be accomplishable using filtering tools alone.

![Source Inventory query builder](/images/SourceInventory_QueryBuilder.png)

<br>

Each **Row** on the Source Inventory page represents a unique **asset**. Select the caret (<img src="/image/Inventory_ListView_Caret.png" width="20px">) to reveal additional information about an asset.

![Source asset details](/images/SourceInventory_ViewAssetDetails.png)

<br>

____

# Profile
The Profile page can be used to manage **MFA settings** for your profile such as enabling and disabling the requirement and resetting your **MFA token**. This is also where you can manage **API keys**.

![Profile page](/images/ProfilePage.png)

<br>

____

# Admin

> ℹ️ 
> Pages covered in this section are only accessible to users with **Admin** accounts. If your account is **Read Only**, you will need to contact an Admin to view them.

<br>

## Configured Sources
Information about Source health is located on the **Configured Sources** page, which can be accessed by selecting the **Admin** icon (<img src="adminicon.png" width="20px">) on the **Navigation bar** and clicking the **Sources** link from the dropdown.

![Navigate to Configured Sources](/images/ConfiguredSourcesPage.png)

<br>

> _[Click here](doc:monitoring-source-health) to learn more about this page._

<br>

## Members

The **Members** page is used to manage **User** (Member) accounts in your Organization. Here you can view and make changes to the existing accounts as well as invite new users to join your Organization. This page can be accessed by clicking the **Admin** icon (<img src="adminicon.png" width="20px">) on the **Navigation bar** then select the **Members** link from the dropdown menu.

![Navigate to Members page](/images/MembersPage.png)

<br>

> _[Click here](doc:manage-users) to learn more about this page._

<br>

## Runners

The **Runners** page is where you can install and monitor the Runners needed for the Sevco platform to communicate with and retrieve data from on-premise sources. This page can be accessed by clicking the **Admin** icon (<img src="/images/adminicon.png" width="20px">) on the **Navigation bar** then select the **Runners** link from the dropdown menu.

![Runners page](/images/RunnersPage.png)

<br>

> _[Click here](doc:manage-runners) to learn more about this page._



<br>

____

# Help Menu

Please refer to our **Help** menu for information or support needs.

## Documentation & FAQs

You can access this documentation site from the Sevco platform by selecting the **Documentation & FAQs** link on the **Help Menu**.


## Support & Updates

Select the **Support & Updates** link to access our in-app chat. This is where you can submit questions, request support, and report platform issues.


![](/images/Intercom_OpenHelpMenu_RequestSupport.gif)

This is also where you can find information about platform improvements, new features, and bug fixes as well as links to release notes. A yellow **Notification** icon will appear next to the **Help Menu** as well as the **Support & Updates** link to notify you when new updates are published.

![](/images/Intercom_OpenHelpMenu_Notification.gif)

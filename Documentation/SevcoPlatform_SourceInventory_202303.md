# Overview

**Source Inventory** pages are integration-specific and only display **asset data** from a single **Source** integration-type. Source Inventory pages can be used to search for an monitor assets associated with a Source. Additionally, you can also review information about a Source's health (**Status**) and reconfigure it as-needed.

![Source Inventory Page](https://my.sev.co/docs/SourceInventoryPage.png) 

<br>

To access an Source Inventory page, select the **Source Inventory** icon on the **Navigation bar** then select the **Integration** you would like to view information about from the **dropdown**.

![Source Inventory Menu](https://my.sev.co/docs/IntegrationsOverview_NavToSourceInventory.gif)

<br>

> ⚠️ 
> 
> Make sure to pay attention to the **Devices**, **Users**, and **Software** tabs at the top of the Source Inventory dropdown, as Integrations are separated by **asset type**.

<br>

___



# Filters & Configuration Panel

The **left-panel** of the page contains filters you can use to search for specific Integration assets.

| Asset Type   | Filters                                                |
| ------------ | ------------------------------------------------------ |
| **Devices**  | • OS Platforms<br>• OS Releases<br>• Mac Manufacturers |
| **Software** | • Software Vendor<br>• OS Platform<br>• OS Release     |
| **Users**    | • Groups<br>• Roles<br>• Domains                       |

<br>

It is also where you can access an Integration's **configuration panel**. Select the **Configure** link to view this information.

![Selecting Configure Link to view logs](https://my.sev.co/docs/SoftwareInventory_OpenConfigMenu.gif)

<br>

___



# Query Builder

Additionally, the page has a **query builder** that can be used to run complex searches that may not be accomplishable using filtering tools alone.

![Source Inventory query builder](https://my.sev.co/docs/SourceInventory_QueryBuilder.png)

<br>

___



# Asset Details

Each **Row** on the Source Inventory page represents a unique **asset**. Select the caret (<img src="https://my.sev.co/docs/Inventory_ListView_Caret.png" width="20px">) to reveal additional information about an asset.

![Source asset details](https://my.sev.co/docs/IntegrationInventory_ViewAssetDetails.png)

<br>

___



# Raw Asset Data

Additionally, you can also view an **raw asset data** on this page. Once a **row** has been expanded, select the **Raw** button to access this information

![Selecting the RAW button to view RAW data for an asset](https://my.sev.co/docs/ViewRawSourceAssetData.gif)

<br>

___



# Software Inventory

The **Software Inventory** page shares many of the same features as the **Device** and **User** Source Inventory pages. It provides up-to-date information about software that has been installed on **Devices** in your Organization.

Once an Integration has been configured to collect Software assets, the Sevco platform will aggregate a list of Devices associated with any software that has been identified.

![Image of the Software Inventory page](https://my.sev.co/docs/SoftwareInventory.png)

<br>

## Viewing Device Details

To view a list of Devices with a specific software installed, select the **See devices** link that corresponds with it.

A popup will appear with a list of all Devices that have the software installed. 

![Selecting the "see devices" link](https://my.sev.co/docs/SoftwareInventory_SelectSeeDevices.gif)

<br>

Hover over then select a Device to view additional details about it on the [**Live Inventory**](doc:sevco-platform-live-inventory) and [**Device Details**](doc:sevco-platform-asset-details) pages.

![Select device link to view info on Live Inventory and Device Details pages](https://my.sev.co/docs/SoftwareInventory_SelectSeeDetails.gif)
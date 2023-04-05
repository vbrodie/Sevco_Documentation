# Overview

The purpose of this article is to provide a general overview of the Sevco platform's pages and functionality. This walk through assumes that you have already completed the initial setup for your Organization and are already collecting asset data. If you have not already done so, please refer to our [Quick Start Guide](doc:quick-start-guide) for instructions.

The Sevco platform is rapidly evolving, as we continue adding new features and making improvements to existing ones. As such, supporting documentation may lag behind from time to time. If you are unable to find information about a particular page or feature, please don't hesitate to reach out to us at [support@sevco.io](mailto:support@sevco.io) or utilize our in-app [Support Chat](#help-menu).

<br>

___



# Dashboard

The **Dashboard** provides a high-level overview of both the history and current status of your **Assets** and configured **Integrations**. Additionally, can also be used to monitor **Enterprise Endpoint** coverage as well as  redirect you to other pages in the Sevco platform where you can review information in greater detail.

![Dashboard page](https://my.sev.co/docs/Dashboard.png)

<br>

## Query Reports

In addition to the main **Dashboard** page, there is also an additional **Query Reports** page that can be accessed by selecting the **Query Reports** tab at the top of the Dashboard. This page tracks specific queries over time. It features a handful of **Global Queries** that can be viewed by anyone in your Organization. Additionally, you may also add [custom queries](doc:manage-query-reports) to the **My Queries** and **Org-wide Queries** lists.

![Screenshot of the Tracked Queries page](https://my.sev.co/docs/QueryReportsPage_202302.png)

<br>

> _[Click here](doc:sevco-platform-dashboard) to learn more about the Sevco Dashboard._

<br>

___



# Live Inventory

The **Live Inventory** page provides an aggregated view of all of your **Device** and **User Assets**. This page has several search features that allow you to filter and view information about specific assets including:

- Multiple ways to view your assets, including in a **List**, by **Location**, and by **Network**.
- A **Venn Diagram** tool for comparing asset coverage between different **Source Integration** platforms
- Attribute filters
- A robust **query builder** for complex searches

![Image of Live Inventory page](https://my.sev.co/docs/SevcoPlatform_LiveInventoryPage.png)



<br>

You can access the Live Inventory page by selecting the **Live Inventory** icon on the **Navigation bar** and clicking the **Devices** or **Users** link from the dropdown.

![Navigating to the Live Inventory page](https://my.sev.co/docs/Inventory_NavToInventory.gif)

<br>

> _[Click here](doc:sevco-platform-live-inventory) to learn more about the Live Inventory page._

<br>

___



# Telemetry

While the [**Live Inventory**](doc:sevco-platform-live-inventory) page provides a snapshot of the current state of your assets, the **Telemetry** page tracks assets at the event level and shows how their attributes have changed in the time leading up to that point.

- On the **left side** of the page, you will find several filters that can be used to search for specific telemetry events by **Source**, **Attribute**, and **Event Type**.
- The **right side** of the page contains a responsive **Event History** that provides a visual representation of your events overtime.
- Like the **Live Inventory** page, the Telemetry page also features a **query builder** that can be used to run complex searches.

![Telemetry page](https://my.sev.co/docs/SevcoWalkthrough_TelemetryPage.png)

<br>

> _[Click here](doc:sevco-platform-telemetry) to learn more about the Telemetry page._

<br>

___



# Asset Details

In addition to the information found on the Live Inventory page, you can also view additional information about specific **assets** on their **Details** page. 

Asset Details page can be accessed by identifying the asset you would like to view in the **Asset List** on the **Live Inventory** page, opening its dropdown, and selecting the **See Details** link.

![Navigating to an Asset's details page](https://my.sev.co/docs/AssetDetails_NavigateToPage.gif)

<br>

The **left panel** of the Details page displays information that has been aggregated from all of its associated **Integrations**. 

![Switching between Integrations and highlighting matching Internal IP addresses](https://my.sev.co/docs/AssetDetails_Sources_InternalIPExample.gif)

<br>

The **right panel** of the Details page allows you to review information about assets by Integration. Users can select an Integration at the to view the most recent information it has collected about an asset.

Additionally, the right panel also allows you to view any **telemetry events** associated with that asset by Integration. This feature functions very similarly to the [Event History](doc:sevco-platform-telemetry#event-history) section of the **Telemetry** page.

![Navigating between Integrations to view associated Telemetry events](https://my.sev.co/docs/AssetDetails_ShowTelemetryData_Example.gif)

<br>

### Software

 Integrations that have been configured to collect **Software** assets will have an additional **Software** tab. Select this tab to view a complete list of software associated with a **Device**.

 ![Selecting Software tab](https://my.sev.co/docs/AssetDetails_SelectSoftwareTab.gif)

<br>

> _[Click here](doc:sevco-platform-asset-details) to learn more about the Asset Details page._

<br>

___



# Source Inventory

**Source Inventory** pages are integration-specific and only display **asset data** from a single **Source** integration-type. Source Inventory pages can be used to search for an monitor assets associated with a Source. Additionally, you can also review information about a Source's configuration health (**Status**) and reconfigure it as-needed.

![Source Inventory Page](https://my.sev.co/docs/SourceInventoryPage.png) 

<br>

To access an Source Inventory page, select the **Source Inventory** icon on the **Navigation bar** then select the **Integration** you would like to view information about from the **dropdown**.

![Source Inventory Menu](https://my.sev.co/docs/IntegrationsOverview_NavToSourceInventory.gif)

<br>

> ⚠️ 
> 
> Make sure to pay attention to the **Devices**, **Users**, and **Software** tabs at the top of the Source Inventory dropdown, as Integrations are separated by **asset type**.

<br>

> _[Click here](doc:sevco-platform-source-inventory) to learn more about the Source Inventory page._

<br>

___



# Profile

The **Profile** page can be used to manage **MFA settings** for your profile such as enabling and disabling the requirement and resetting your **MFA token**. This is also where you can manage **API keys**.

![Profile page](https://my.sev.co/docs/ProfilePage_202303.png)

<br>

___



# Admin

> ℹ️ 
> 
> Pages covered in this section are only accessible to users with **Admin** accounts. If your account is **Read Only**, you will need to contact an Admin to view them.

<br>

## Integrations

The **Integrations** page can be accessed by selecting the **Admin** icon (<img src="https://my.sev.co/docs/AdminIcon.png" width="20px">) on the **Navigation bar** and clicking the **Integrations** link from the dropdown.

![Navigate to Configured Integrations](https://my.sev.co/docs/Integrations_NavToIntegrations.gif)

<br>

Once you are on the Integrations page, you can access a list of all Integrations currently supported by the Sevco platform by selecting the **Add new** button at the top-left corner of the page.

![](https://my.sev.co/docs/Integrations_OpenAddNewMenu.gif)

<br>

This is also where you can monitor the health of the Integrations you've already configured.

![](https://my.sev.co/docs/Integration_ConfigurationPanel_ViewLogs.gif)

<br>

> _[Click here](doc:manage-integrations) to learn more about this page._

<br>

## Members

The **Members** page is used to manage **User** (Member) accounts in your Organization. Here you can view and make changes to the existing accounts as well as invite new users to join your Organization. This page can be accessed by clicking the **Admin** icon (<img src="https://my.sev.co/docs/AdminIcon.png" width="20px">) on the **Navigation bar** then select the **Members** link from the dropdown menu.

![Navigate to Members page](https://raw.githubusercontent.com/vbrodie17/Sevco_Documentation/main/images/NavigateToMembersPage.gif)

<br>

> _[Click here](doc:manage-users) to learn more about this page._

<br>

## Runners

The **Runners** page is where you can install and monitor the Runners needed for the Sevco platform to communicate with and retrieve data from on-premise Integrations. This page can be accessed by clicking the **Admin** icon (<img src="https://my.sev.co/docs/AdminIcon.png" width="20px">) on the **Navigation bar** then select the **Runners** link from the dropdown menu.

![Runners page](https://my.sev.co/docs/RunnersPage.png)

<br>

> _[Click here](doc:manage-runners) to learn more about this page._

<br>

## Tags

The **Tags** page is where you can create and manage Tags that can be applied to **assets** on the **Live Inventory** and **Asset Details** pages in Sevco. Likewise, any tags created and assigned to an asset from the two pages will automatically appear on the Tags page. This page can be accessed by clicking the **Admin** icon (<img src="https://my.sev.co/docs/AdminIcon.png" width="20px">) on the **Navigation bar** then select the **Tags** link from the dropdown menu.

![Tags Page](https://my.sev.co/docs/SevcoPlatform_TagsPage.png)

> ℹ️ 
> 
> While a tag can be removed from an **asset** or **query action**, you will need to delete the tag in the **Tags** page to completely remove it from your environment.

<br>

## Tenants

> ℹ️ 
> 
> The **Tenant Management** page is only available for **service partners** who manage multiple Sevco Organizations.

The **Tenant Management** page allows **service partners** to keep track of multiple **Organizations** or "Tenants" using a single account. You can use this page to create new Organizations or manage existing one. Additionally, this is where you can add new members to your tenant-management **team** and assign roles and permissions.

The **Tenants** page can be accessed by selecting the **Tenant Management** icon (<img src="https://my.sev.co/docs/TenantMgmtIcon.png" width="20px">) on the **Navigation bar**.

![Screenshot of page](https://my.sev.co/docs/TenantMgmtPage.png)

<br>

> _[Click here](doc:manage-tenants) to learn more about this page._

<br>

## Audit Log

The **Audit Log** provides a chronological list of all **events** that have taken place in your environment along with event details, timestamps, and the users associated with them. This page can be accessed by clicking the **Admin** icon (<img src="https://my.sev.co/docs/AdminIcon.png" width="20px">) on the **Navigation bar** then select the **Audit Log** link from the dropdown menu.

![Audit Log](https://my.sev.co/docs/SevcoPlatform_AuditLog.png)

<br>

___



# Help Menu

Please refer to our **Help** menu for information or support needs.

## Documentation & FAQs

You can access this documentation site from the Sevco platform by selecting the **Documentation & FAQs** link on the **Help Menu**.

## Support & Updates

Select the **Support & Updates** link to access our in-app chat. This is where you can submit questions, request support, and report platform issues.

![](https://my.sev.co/docs/Intercom_OpenHelpMenu_RequestSupport.gif)

This is also where you can find information about platform improvements, new features, and bug fixes as well as links to release notes. A yellow **Notification** icon will appear next to the **Help Menu** as well as the **Support & Updates** link to notify you when new updates are published.

![](https://my.sev.co/docs/Intercom_OpenHelpMenu_Notification.gif)
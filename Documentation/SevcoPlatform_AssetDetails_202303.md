# Overview

In addition to the information found on the Live Inventory page, you can also view additional information about specific **assets** on their **Details** page. 

Asset Details pages can be accessed by identifying the asset you would like to view in the **Asset List** on the **Live Inventory** page, opening its dropdown, and selecting the **See Details** link.

![Navigating to an Asset's details page](https://my.sev.co/docs/AssetDetails_NavigateToPage.gif)

<br>

___



# Data Aggregation

The **left panel** of the Details page displays information that has been aggregated from all of its associated **Integrations**. 

Notice how this Device has three **Internal IPs** listed. If we look at data collected from **Illumio**, **Automax** and **MalwareBytes** we will find that they have identified `10.20.199.156` as the Device's Internal IP.

![Switching between Integrations and highlighting matching Internal IP addresses](https://my.sev.co/docs/AssetDetails_Sources_InternalIPExample.gif)

<br>

However, when we look at **Lansweeper** we will also see a second Internal IP, `10.41.212.101` listed. Both of these are included in the left panel.

![Viewing Lansweeper, which has an additional Internal IP address, and showing that it is also listed in the left panel](https://my.sev.co/docs/AssetDetails_Sources_InternalIPExample_twoIPs.gif)

<br>

___



# Source Telemetry

As we stated earlier, the **right panel** of the Details page allows you to review information about assets by Integration. Users can select a **Source Integration** at the top of the page to view the most recent information it has collected about an asset.

Additionally, the right panel also allows you to view any **telemetry events** associated with that asset by Integration. This feature functions very similarly to the [Event History](doc:sevco-platform-telemetry#event-history) section of the **Telemetry** page.

![Navigating between Integrations to view associated Telemetry events](https://my.sev.co/docs/AssetDetails_ShowTelemetryData_Example.gif)

<br>

## Asset History

> ℹ️ 
> 
> **Asset History** functionality is only available for **Devices** at this point in time.

<br>

The Asset Details page has an additional **Asset History** feature for **Devices**. This feature allows users to compare the current **attribute values** of a device against values captured in past telemetry **events**.

![Example of Device Snapshot](https://my.sev.co/docs/AssetDetails_DeviceSnapshot.png)

<br>

Telemetry events can be captured as frequently as every minute. As such, it may take several clicks to get to the event you are interested in viewing. 

Select the **bar** on the timeline that corresponds with the **day** of the event you would like to review. Next, the **hour** followed by the exact **minute** it took place.

![GIF highlighting timeline](https://my.sev.co/docs/AssetDetails_DeviceSnapshot_ViewSnapshot.gif)

<br>

Once the event has been selected, its timeline bar will turn **yellow** and a **timestamp** will appear in the header. Past data that differs from current data will also be displayed in **yellow**. 

Take the image below for example, where we can see that the **Internal IP** reported on `12/01/2022 09:14 AM` differs from the Internal IP currently associated with the device.

![Highlighting Differences in IP and report date](https://my.sev.co/docs/AssetDetails_DeviceSnapshot_InternalIPExample.gif)

<br>

Once you have finished viewing a snapshot, you can reset the timeline by selecting the **Reset to current device** button.

![Select Reset button](https://my.sev.co/docs/AssetDetails_DeviceSnapshot_ResetToCurrent.gif)

<br>

## Software

 Integrations that have been configured to collect **Software** assets will have an additional **Software** tab. Select this tab to view a complete list of software associated with a **Device**.

 ![Selecting Software tab](https://my.sev.co/docs/AssetDetails_SelectSoftwareTab.gif)

<br>

 _[Click here](doc:sevco-platform-source-inventory#software-inventory) to learn more about **Software** assets._
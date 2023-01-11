---

copyright:
  years: 2017, 2023
lastupdated: "2023-01-11"

keywords:

subcollection: DataTransferService

---

{{site.data.keyword.attribute-definition-list}}

# Sorting or filtering the shipments list
{: #sort-or-filter-shipments-list}

The Shipments screen within the [{{site.data.keyword.cloud_notm}} console](/login){: external} displays the shipments that are associated with Data Transfer Service requests. All shipping requests from the last 30 days are displayed. Shipments can be sorted and filtered to view older shipments or specific shipment types.

## Sorting and filtering
{: #sorting}

1. Access the Shipments screen within the [{{site.data.keyword.cloud_notm}} console](/login){: external}.
2. Determine whether the view is to be filtered for specific details or sorted by shipment status.
   - If you want to sort by shipment status, you can select one of the following options from the **Display** list: **Open Shipping Requests**, **Closed Shipping Requests**, **Canceled Shipping Requests** or **All Shipping Requests**.
   - If you want to filter for specific details, select one, or more of the **filter options** available and click **Filter**.


![DTS Shipment Screen](/images/DTSShipmentScreen.png){: caption="Figure 1 shows the shipment screen." caption-side="bottom"}

|Filter option|Entry information|
|-------------|-----------------|
|Shipped date|Select the timeframe of the shipment.|
|Shipped from|Select the location where the shipment originates from.|
|Carrier|Select the courier (for example FedEx, UPS, or USPS) that transports the shipment.|
|Shipment type|Select the type of shipment.|
|Shipped To|Select the location to which the shipment was sent.|
|Tracking number|Enter the tacking number that was provided by the courier.|
|Item Description|Enter the description of the item that is shipped.|
{: caption="Table 1. Filter options." caption-side="top"}
{: summary="Table 1 shows the filter options available in the Shipment screen. The left column lists the available options and the right side column provides their descriptions."}


After you filtered the Shipments List, all shipments that correspond with the parameters that are set by the filter are displayed in the Shipment List. Click **Modify**, and update the filter options if you want to change the list. To clear all parameters that are set by the filter, click **Clear All**.

If the results were sorted by the shipment status, all shipments that are within the selected status are displayed. Select a new status from the list to update the displayed results at any time.

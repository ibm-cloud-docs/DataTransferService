---

copyright:
  years: 2017, 2024
lastupdated: "2024-10-31"

keywords:

subcollection: DataTransferService

---

{{site.data.keyword.attribute-definition-list}}

# Sorting or filtering the shipments list
{: #sort-or-filter-shipments-list}

The Data Transfer Service is deprecated. As of 04 November 2024, you can't create new requests for this service. Any existing requests will be serviced as per the terms of offering.
{: deprecated}

## Accessing the Shipments screen
{: #access-shipments-screen}

The Shipments screen within the [{{site.data.keyword.cloud_notm}} console](/login){: external} displays all shipments that are associated with data transfer service requests. From this screen, you can view shipments and you can confirm return shipments upon receipt.

To access the Shipments screen:

1. Access the [{{site.data.keyword.cloud_notm}} console](/login){: external} with your unique credentials.
2. Select **Account** > **Manage** > **Shipments** from the Navigation Bar.

On the Shipments screen, all shipping requests within the last 30 days are displayed with their details. Shipments can be sorted or filtered by status, age, or specific shipment details. Additionally, you can confirm the receipt of return shipments on this screen.

![Shipments Screen](/images/DTSShipmentScreen1.svg){: caption="Figure 1 shows the shipments screen." caption-side="bottom"}

## Sorting and filtering
{: #sorting}

1. Access the Shipments screen within the [{{site.data.keyword.cloud_notm}} console](/login){: external}.
2. Determine whether the view is to be filtered for specific details or sorted by shipment status.
   - Windows  you can select one of the following options from the **Display** list.
     - Open Shipping Requests
     - Closed Shipping Requests
     - Canceled Shipping Requests
     - All Shipping Requests
   - If you want to filter for specific details, select one or more of the **filter options** available and click **Filter**.

![DTS Shipment Screen](/images/DTSShipmentScreen.svg){: caption="The shipment screen." caption-side="bottom"}

|Filter option|Entry information|
|-------------|-----------------|
|Shipped date|Select the time frame of the shipment.|
|Shipped from|Select the location where the shipment originates from.|
|Carrier|Select the courier (for example FedEx, UPS, or USPS) that transports the shipment.|
|Shipment type|Select the type of shipment.|
|Shipped To|Select the location to which the shipment was sent.|
|Tracking number|Enter the tacking number that was provided by the courier.|
|Item Description|Enter the description of the item that is shipped.|
{: caption="Filter options." caption-side="top"}
{: summary="Table 1 shows the filter options available in the Shipment screen. The first column lists the available options and the second column provides their descriptions."}

After you filtered the Shipments List, all shipments that correspond with the parameters that are set by the filter are displayed in the Shipment List. Click **Modify**, and update the filter options if you want to change the list. To clear all parameters that are set by the filter, click **Clear All**.

If the results were sorted by the shipment status, all shipments that are within the selected status are displayed. Select a new status from the list to update the displayed results at any time.

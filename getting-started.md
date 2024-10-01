---

copyright:
  years: 2017, 2024
lastupdated: "2024-10-01"

keywords:

subcollection: DataTransferService

---

{{site.data.keyword.attribute-definition-list}}

# Getting started with Data Transfer Service
{: #gettingstarted}

The Data Transfer Service is deprecated. As of 04 November 2024, you can't create new requests for this service. Any existing requests will be serviced as per the terms of offering.
{: deprecated}

You can use {{site.data.keyword.cloud}} Data Transfer Service to send a USB 2.0 or USB 3.0 compatible device to an {{site.data.keyword.cloud_notm}} data center. The device is connected directly to your network so you can remotely control the data transfer. The device is housed in a dedicated rack that is located in your data center and mounted as an iSCSI target. The data transfer service is ideal when you need to transfer data of considerable size without using {{site.data.keyword.cloud_notm}} Private network. It's a service that is offered at no charge to all {{site.data.keyword.cloud_notm}} customers. If you’re an existing Data Transfer Serviceuser, you can continue to use the service until it is no longer supported on _DD month YYYY_.

## Accessing the Data Transfer Service screen
{: #access-dts-screen}

You can manage data transfer requests by using the {{site.data.keyword.cloud_notm}} console.

1. Log in to the [{{site.data.keyword.cloud_notm}} console](/login){: external} with your unique credentials.
2. Select **Infrastructure**  ![VPC icon](../icons/vpc.svg) > **Classic Infrastructure** > **Storage**  > **Data Migration** > **Data Transfer** from the navigation bar to access the Data Transfer Service screen.

    The Data Transfer screen is available only to the principal user of the account. To access this screen, contact the account owner.
    {: note}

## Submitting a data transfer request
{: #submit-dts-request}

Data transfer requests are designed to inform the appropriate parties in our data centers to expect a shipment from a client. Requests are submitted through the [{{site.data.keyword.cloud_notm}} console](/login){: external}.

When you create a request, keep the following guidelines in mind.

- Ensure that the device that you want to send meets all [hardware requirements](/docs/DataTransferService?topic=DataTransferService-about#hardware-requirements).
- Only one device can be associated with one request. If you want to send multiple devices, you must create a request for each device.
- If the device is to be returned, provide a pre-paid shipping label, and export documents as needed in the package so that the device can be returned after the transfer period.
- If you're shipping the device internationally, you're responsible for obtaining all licensing, shipping, and customs clearance for the Device. Your responsibilities include paying any duties, taxes, and shipping costs to and from (if applicable) the {{site.data.keyword.cloud_notm}} data center.
- You need to provide the name of the carrier and the tracking number for the shipment to the data center when you complete the request. Create the shipping label with the appropriate data center address before you submit the data transfer request.

Follow these steps to submit a data transfer request.

1. Access the **Data Transfer Service** screen in the [{{site.data.keyword.cloud_notm}} console](/login){: external}.
2. Click **Order Data Transfer Request**.
3. Complete each field in the **Device Information** section according to the following table.

   |  Field  | Device Type |
   |---------|-------------|
   | Device Type |  The type of device that is sent to the destination. If the device type is not listed, select **Other**. |
   | Serial Number| The serial number for the device.|
   | Description | A brief description of the device, such as color, labels, stickers, or other characteristics that identify the device. |
   | Note | Any additional notes about the device or the transfer. |
   | Destination| The data center that is to receive the device. |
   | Carrier| The post or express carrier that is used to ship the device to its destination. |
   | Tracking Number | The full tracking number for the shipment. |
   {: caption="Table 1 describes the fields that are required for creating a data transfer request." caption-side="bottom"}

4. Complete each field in the **Return Address** section or select the **Company Address** checkbox to automatically populate the fields with the company address on file.

   Remember to include the prepaid return label and any needed export documents in the package.
   {: note}

5. Review your order, and click the link to read the terms and conditions.
6. Click the checkbox if you agree with the terms.
7. Click **Submit Service Request**.

After you submit the request, the status for the request ticket appears as `Sent to SoftLayer`. If any import or export shipment requires a license from your local government, notify {{site.data.keyword.BluSoftlayer}} and attach licensing information in the ticket.

After the device is received, the status is updated to `Received by SoftLayer`. The ticket status is updated again to `Connected` after a data center technician connects the device to the network.

The initial data transfer period is two weeks. During this time, access to the device is granted to the account administrator only. If you need more time, you can request an extension. Also, if you want the device to be sent back sooner than two weeks, you can request the return. You must notify {{site.data.keyword.IBM}} through the [{{site.data.keyword.cloud_notm}} console](/login){: external} when transfer is complete. Then, {{site.data.keyword.cloud_notm}} detaches the device and either returns it or destroys it depending on what you requested.

## Accessing the Shipments screen
{: #access-shipments-screen}

The Shipments screen within the [{{site.data.keyword.cloud_notm}} console](/login){: external} displays all shipments that are associated with data transfer service requests. From this screen, you can view shipments and you can confirm return shipments upon receipt.

To access the Shipments screen:

1. Access the [{{site.data.keyword.cloud_notm}} console](/login){: external} with your unique credentials.
2. Select **Account** > **Manage** > **Shipments** from the Navigation Bar.

On the Shipments screen, all shipping requests within the last 30 days are displayed with their details. Shipments can be [sorted or filtered](/docs/DataTransferService?topic=DataTransferService-sort-or-filter-shipments-list) by status, age, or specific shipment details. Additionally, you can confirm the receipt of return shipments on this screen.

![Shipments Screen](/images/DTSShipmentScreen1.svg){: caption="Figure 1 shows the shipments screen." caption-side="bottom"}

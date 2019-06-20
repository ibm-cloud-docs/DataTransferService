---

copyright:
  years: 2017, 2019
lastupdated: "2019-06-20"

keywords:

subcollection: DataTransferService

---
{:new_window: target="_blank"}

# Getting started tutorial
{: #gettingstarted}

Customers can use the {{site.data.keyword.BluSoftlayer_full}} data transfer service to send a USB 2.0 or USB 3.0 compatible device to a {{site.data.keyword.BluSoftlayer}} data center. Their device is connected directly to their network so they can remotely control the data transfer. The device is housed in a dedicated rack that is located in the customers data center and mounted as an iSCSI target. The data transfer service is ideal when you need to transfer large amounts of data without using {{site.data.keyword.BluSoftlayer}}'s private network, and it's a service offered free-of-charge to all {{site.data.keyword.BluSoftlayer}} customers.

## Accessing the data transfer service screen

**Note**: this screen is only available to the master user of the account.

1. Access the [{{site.data.keyword.slportal}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){:new_window} with your unique credentials.
2. Select **Storage** > **Data Migration** > **Data Transfer** from the Navigation Bar to access the Data Transfer Service screen. <br/>

On the **Data Transfer Service** screen, users can submit a data transfer request, view details of a request, view the ticket history that is associated with the device tracking, and cancel an existing request.

## Submitting a data transfer request

Data transfer requests are designed to let the appropriate parties in our data centers know to expect a shipment from a client. Requests are submitted through the [{{site.data.keyword.slportal}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){:new_window}.

When you create a request, keep the following guidelines in mind.

- Ensure that the device you want to send meets all [hardware requirements](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html).
- Only one device can be associated with one request. If you want to send multiple devices, you must create a new request for each device.
- If the device is to be returned, provide a pre-paid shipping label and export documents as needed in the package so that the device can be returned after the transfer period.
- If you're shipping the device internationally, you're responsible to obtain all licensing, shipping, and customs clearance for the Device. Your responsibilities include paying any duties, taxes, and shipping costs to and from (if applicable) the {{site.data.keyword.BluSoftlayer}} data center.
- You need to provide the name of the carrier and the tracking number for the shipment to the data center when you complete the request.  Create the shipping label with the appropriate data center address before you submit the data transfer request.

Follow these steps to submit a data transfer request.

1. Access the **Data Transfer Service** screen in the [{{site.data.keyword.slportal}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){:new_window}.
2. Click **Order Data Transfer Request**.
3. Complete each field in the **Device Information** section according to the table 1.
<table border="1">
<caption>Table 1 lists the names of the fields in the request form on the left, and their description on the right.</caption>
 <tr><th>Field Name</th><th>Instructions</th></tr>
 <tr><td>Device Type</td><td>The type of device that is sent to the destination. If the device type is not listed, select "Other".</td></tr>
 <tr><td>Serial Number</td><td> The serial number for the device.</td></tr><tr><td>Description</td><td>A brief description of the device. Important details to include can be identifying factors such as color, labels, or stickers.</td></tr>
 <tr><td>Note</td><td>Any additional notes about the device or the transfer.</td></tr><tr><td>Destination</td><td>Data center that is to receive the device.</td></tr>
 <tr><td>Carrier</td><td>Post or express carrier that is used to ship the device to its destination.</td></tr>
 <tr><td>Tracking Number</td><td>Full tracking number for the shipment.</td></tr>
 </table>

4. Complete each field in the **Return Address** section or select the **Company Address** check box to automatically populate the fields with the company address on file. <br/> **Note**: Remember to include the prepaid return label and any needed export documents in the package.
5. After you read the service agreement, select the **I have read and agree to the Data Transfer Service Agreement and the Master Service Agreement** check box.
6. Click **Submit Service Request**.

After you submitted the request, the status for the request ticket appears as `Sent to SoftLayer`. If any import or export shipment requires a license from your local government, notify {{site.data.keyword.BluSoftlayer}} and attach licensing information in the ticket.

After the device is received, the status is updated to `Received by SoftLayer`. The ticket status is updated again to `Connected` after a data center technician connects the device to the network.

The initial data transfer period is two weeks. During this time, access to the device is granted to the account administrator only. If you need more time, you can request an extension. Also, if you want the device to be sent back sooner than two weeks, you can request the return. You must notify {{site.data.keyword.IBM}} through the [{{site.data.keyword.slportal}}](https://control.softlayer.com/) when transfer is complete. Then, {{site.data.keyword.BluSoftlayer}} detaches the Device and either returns it or destroys it depending on what you requested.


## Accessing the Shipments screen

The Shipments screen within the [{{site.data.keyword.slportal}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){:new_window} displays all shipments that are associated with data transfer service requests. From this screen, you can view shipments and you can confirm return shipments upon receipt.

To access the Shipments screen:

1. Access the [{{site.data.keyword.slportal}} ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/){:new_window} using your unique credentials.
2. Select **Account** > **Manage** > **Shipments** from the Navigation Bar.

On the Shipments screen, all shipping requests within the last 30 days are displayed with their details. Shipments can be [sorted or filtered](sort-or-filter-shipments-list.html) by status, age, or specific shipment details. Additionally, you can confirm the receipt of return shipments on this screen.
![Shipments Screen](/images/DTSShipmentScreen1.png)

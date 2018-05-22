---

copyright:
  years: 1994, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}

# Getting started with data transfer service

{{site.data.keyword.BluSoftlayer_full}} data  transfer service allows customers to send a USB 2.0 or USB 3.0 compatible device, CDs, and DVDs to a {{site.data.keyword.BluSoftlayer}} data center to be connected directly to their network to remotely control the data transfer. The device is housed in a dedicated rack located in the customers data center and mounted as an iSCSI target. Our data transfer service is ideal when you need to transfer large amounts of data without using our private network, and it's a service offered free-of-charge to all {{site.data.keyword.BluSoftlayer}} customers.

## Accessing the data transfer service screen

**Note**: this screen is currently only available to the master user of the account.

1. Access the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} using your unique credentials.
2. Select **Storage** > **Data Migration** > **Data Transfer** from the Navigation Bar to access the Data Transfer Service screen. <br/>

On the **Data Transfer Service** screen, users can submit a data transfer request, view details regarding a request, view the ticket history associated with the device tracking for a request and cancel an existing request.

## Submitting a data transfer request

Data transfer requests are designed to let the appropriate parties in our data centers know to expect a shipment from a client. Requests are submitted through the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. When you create a request, keep the following guidelines in mind:

- Ensure that the device you want to send meets all [hardware requirements](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html).
- Only one device can be associated with one requests. If you want to send multiple devices, you must create a new request for each device.
- If the device is to be returned, provide a pre-paid shipping label and export documents as needed in the package so that the device can be returned after the transfer period.
- If shipping internationally, you're responsible to obtain all licensing, shipping, and customs clearance for the Device. Your responsibilities include paying any duties, taxes, and shipping costs to and from (if applicable) the {{site.data.keyword.BluSoftlayer}} data center.
- You need to provide the name of the carrier and the tracking number for the shipment to our data center when completing the request.  Create the shipping label with the appropriate data center address before you submit the data transfer request.

Follow the steps below to submit a data transfer request.

1. Access the **Data Transfer Service** screen in the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. <br/> **Note**: This screen is only available to the master user of the account.
2. At the top of the screen, click **Order Data Transfer Request**.
3. Complete each field in the **Device Information** section according to the table below.
<table border="1">
<caption>Table one lists the names of the fields in the request form on the left, and their description on the right.</caption> 
 <tr><th>Field Name</th><th>Instructions</th></tr>
 <tr><td>Device Type</td><td>The type of device being sent to the destination. If the device type is not listed, select "Other".</td></tr>
 <tr><td>Serial Number</td><td> The serial number for the device.</td></tr><tr><td>Description</td><td>A brief description of the device. Important details to include can be identifying factors such as color, labels or stickers.</td></tr>
 <tr><td>Note</td><td>Any additional notes regarding the device or the transfer.</td></tr><tr><td>Destination</td><td>Data center that will receive the device.</td></tr>
 <tr><td>Carrier</td><td>Post or express carrier that is used to ship the device to its destination.</td></tr>
 <tr><td>Tracking Number</td><td>Full tracking number for the shipment.</td></tr>
 </table>

4. Complete each field in the **Return Address** section or select the **Company Address** check box to automatically populate the fields with the company address on file. <br/> **Note**: Remember to include the prepaid return shipping label and any needed export documents in the package so that we can return the device.
5. After you read the service agreement, select the **I have read and agree to the Data Transfer Service Agreement and the Master Service Agreement** check box .
6. Click **Submit Service Request**.

After submitting the request, the status for the request ticket appears as *Sent to SoftLayer*. If any import or export shipment requires a license from your local government, notify us and attach licensing information in the ticket.

After the device is received, the status is updated to *Received by SoftLayer* and updated again to *Connected* after a data center technician connects the device to the network. 

The initial data transfer period is to last no more than two weeks. During this time, access to the device is permitted to the account administrator only. If you need more time, you can request an extension. Also, if you want the device to be shipped sooner than two weeks, you can request the return. You must notify {{site.data.keyword.IBM}} through the [{{site.data.keyword.slportal}}](https://control.softlayer.com/) when transfer is complete. Then we will detach the Device and either return it or destroy it depending on what you requested.


## Accessing the Shipments Screen

The Shipments screen within the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} displays all shipments associated with data transfer service requests. From this screen, you can view shipments and you can confirm return shipments upon receipt. 

To access the Shipments screen:

1. Access the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} using your unique credentials.
2. Select **Account** > **Manage** > **Shipments** from the Navigation Bar.

On the Shipments screen, all shipping requests within the last 30 days are displayed in the shipments list with their details. Shipments can be [sorted or filtered](sort-or-filter-shipments-list.html) by status, age or specific shipment details. Additionally, you can confirm the receipt of return shipments on this screen.
![Shipments Screen](/images/DTSShipmentScreen1.png)

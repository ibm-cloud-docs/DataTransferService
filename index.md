---

copyright:
  years: 1994, 2017
lastupdated: "2017-12-14"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Getting Started with Data Transfer Service

{{site.data.keyword.BluSoftlayer_full}} Data Transfer Service allows customers to send a USB 2.0 or USB 3.0 compatible device and/or CDs and DVDs to a {{site.data.keyword.BluSoftlayer}} data center to be connected directly to their network to remotely control the data transfer. The device is housed in a dedicated rack located in the customers data center and will be mounted as an iSCSI target.  Our Data Transfer Service is ideal when you need to transfer large amounts of data without using our Private Network and is a service offered free-of-charge to all {{site.data.keyword.BluSoftlayer}} customers.

## Accessing the Data Transfer Service Screen

**Note**: this screen is currently only available to the master user of the account.

1. Access the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} using your unique credentials.
2. Select **Storage** > **Data Migration** > **Data Transfer** from the Navigation Bar to access the Data Transfer Service screen. <br/>

Upon accessing the Data Transfer Service screen, users may submit a data transfer request, view details regarding a request, view the ticket history associated with the device tracking for a request and cancel an existing request.

## Submitting a Data Transfer Request

Data transfer requests are designed to let the appropriate parties in our datacenters know to expect a shipment from a client. Requests are submitted through the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. When creating a request, keep the following guidelines in mind:

- Ensure that the device being sent in association with the request meets all [hardware requirements](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html).
- Only one device can be associated with each requests. If you want to send multiple devices, please create a new request for each device.
- If the device is to be returned, please provide pre-paid shipping label and export documents as needed in the package so that the device may be returned after the transfer period.
- If shipping internationally, you are responsible to obtain all licensing, shipping, and customs clearance for the Device, including paying any duties, taxes and shipping costs to and from (if applicable) the IBM data center.
- The carrier and tracking number for the shipment to our datacenter must be provided when completing the request. Ensure that the label has been created with the appropriate datacenter address prior to completing the request.

Follow the steps below to submit a data transfer request.

1. Access the **Data Transfer Service** screen in the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. <br/> **Note**: This screen is only available to the master user of the account.
2. Click **Order Data Transfer Request** at the top of the screen.
3. Complete each field in the **Device Information** section according to the table below.
<table border="1">
<tbody>
 <tr><th>Field Name</th><th>Instructions</th></tr>
 <tr><td>Device Type</td><td>The type of device being sent to the destination. If the device type is not listed, select "Other".</td></tr>
 <tr><td>Serial Number</td><td> The serial number for the device.</td></tr><tr><td>Description</td><td>A brief description of the device. Important details to include may be identifying factors such as color, labels or stickers that are attached, etc.</td></tr>
 <tr><td>Note</td><td>Any additional notes regarding the device or the transfer.</td></tr><tr><td>Destination</td><td>Datacenter that will receive the device.</td></tr>
 <tr><td>Carrier</td><td>Post or express carrier used to ship the device to its destination.</td></tr>
 <tr><td>Tracking Number</td><td>Full tracking number for the shipment.</td></tr>
 </tbody>
 </table>

4. Complete each field in the **Return Address** section or select the **Company Address** check box to automatically populate the fields with the company address on file. <br/> **Note**: Remember to include the prepaid return shipping label and export documents as needed in the package so that the device may be returned after the transfer period.
5. Select the **I have read and agree to the Data Transfer Service Agreement and the Master Service Agreement** check box after reading each service agreement provided.
6. Click **Submit Service Request** to submit the request. Click **Cancel** to cancel the action.

After submitting the request, the status for the request ticket will appear as *Sent to SoftLayer*. Please notify us, if any import or export shipment requires a license from your local government, and attach licensing information in the ticket.

After the device is received, the status is updated to *Received by SoftLayer* and updated again to *Connected* after a datacenter technician has connected the device to our network. 

The initial data transfer period is to last no more than two (2) weeks. During this time, access to the device is permitted to the account administrator only. Should additional time be necessary, an extension may be requested. Conversely, if the device should be shipped sooner than two (2) weeks, a request for return may be made. You must notify {{site.data.keyword.IBM}} via the  [{{site.data.keyword.slportal}}](https://control.softlayer.com/) once transfer is complete. We will then detach the Device and either return or destroy it depending on what you requested.


## Accessing the Shipments Screen

The Shipments screen within the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} displays all shipments associated with Data Transfer Service requests. From this screen, shipments may be viewed and return shipments may be confirmed upon receipt. Follow the steps below to access the Shipments screen.

1. Access the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} using your unique credentials.
2. Select **Account** > **Manage** > **Shipments** from the Navigation Bar to access the Shipments screen.

Upon access the Shipments screen, all shipping requests within the last 30 days are displayed in the shipments list along with details regarding each shipment. Shipments may be [sorted or filtered](sort-or-filter-shipments-list.html) by status, age or specific shipment details. Additionally, the receipt of return shipments may be confirmed from this screen.
![Shipments Screen](/images/DTSShipmentScreen1.png)

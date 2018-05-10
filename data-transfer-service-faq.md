---

copyright:
  years: 1994, 2018
lastupdated: "2018-05-02"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Data Transfer Service FAQ

## What is Data Transfer?

Data transfer allows authorized users (generally the account's administrator) to send compatible devices to one of our data centers to be connected directly to the account's network. The device is housed in a dedicated rack in the selected data center and is mounted as an iSCSI target for a two (2) week period. During that period, the administrator may access the device on the network in order to use it with other devices and/or services on the account. After the two week period, an extension may be requested to keep the device connected to the network. Otherwise, the device is returned to the party specified in the return address section when the request was created or the device is destroyed onsite if return was not requested.


## Can I Ship a Device for Data Transfer Internationally?

Hardware and disks may be shipped both domestically and internationally to any of our data centers; however you as the Client are responsible for:

- ensuring no import or export license is required to ship the Device to the {{site.data.keyword.IBM}} data center, or to return it to Client (if applicable);
- ensuring neither Client nor any Client end user whose data is included in the Content is subject to any U.S. Government order revoking or denying their U.S. export privileges. Client agrees to notify {{site.data.keyword.IBM}} immediately if Client or any such end user becomes subject to any such order;
- obtaining all licensing, shipping, and customs clearance for the Device, including paying any duties, taxes and shipping costs to and from (if applicable) the {{site.data.keyword.IBM}} data center;
- complying with all applicable laws, including privacy, import and export, associated with delivery and return of the Device, and the transfer of Content to the {{site.data.keyword.IBM}} data center; and
- having proper agreements in place, and obtaining all required permissions, with Client’s end user for any end user data Client will transfer to the Hardware.

Please include a pre-paid return shipping label and all appropriate export documents with your shipment and we will package the device(s) for return using the label and documents you provided. If return was not requested, the device will be destroyed.


## What Types of Devices Can I Send with a Data Transfer Request?
Use the following guidelines when selecting a device or disk (CD or DVD) to submit for data transfer:

- Hardware Requirements:
   - Power supply must be 208v/220v compatible.

   - Power plug must fit a standard 120v socket (NEMA 5-15P).

   - Device must be USB 2.0 or USB 3.0 compatible.

   - Provide a USB A Male connector (standard USB plug that fits most computers).

- CD/DVD Requirements:

   - Disks must be submitted in CD books, jewel cases, or similar container. If submitting multiple disks, store disks together in a single case or CD book.

   - Each disk must be clearly and uniquely labeled (i.e. Disk A, Disk B, Disk C, etc.).

## Can I Get My Device Back Sooner or Have It Stay Longer Than Two Weeks during the Data Transfer Process?

Yes, your hardware or disk(s) can be returned at any time or can stay connected longer, if necessary. In order to request a return on an extension, add a comment to the original Data Transfer Request ticket with the appropriate request. If requesting a return, we will disconnect and return the hardware or disk(s) to the return shipping address provided in the original request using the pre-paid shipping labels and packaging you provided.

If requesting an extension, the extension request will be processed as quickly as possible. It is important to note that each extension request extends the time the device is connected for one week and may be subject to an extension fee. Additional details will be included when a member of our team responds to the request in the original ticket.

## What Does Each Status on My Data Transfer Ticket Mean?

Each status on the data transfer ticket indicates the phase of the transfer process for the hardware or disk(s) submitted to the data center. Refer to the table below for specific details on each status:

|Status 	| Definition |
|---------| -----------|
|Sent To SoftLayer 	|The Data Transfer Request was submitted by the user and the hardware or disks(s) is being shipped to the selected data center.|
|Received by SoftLayer |	The shipment was received by the data center, the device was assigned a serial number and was scanned into our system.|
|Connect |	The hardware or disk has been connected to the device.|
|Connected |	An iSCSI target has been created for the device.|
|Request for Extension |	User requested an extension on the two (2) week connection time.|
|Request for Return | User requested the return of hardware or disk(s).|
|Disconnect |	Disconnection of hardware or disk(s) has been initiated.|
|Disconnected |	Target has been safely detached by Information Systems.|
|Destroyed | The device has been destroyed on site following our HDD destruction procedure.|
|Return by SoftLayer |	Hardware or disk(s) has been packaged and shipped to the return address provided in the original request.|

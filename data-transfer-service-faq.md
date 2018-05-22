---

copyright:
  years: 1994, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Frequently asked questions

## What is Data Transfer?

This service allows authorized users (generally the account's administrator) to send compatible devices to one of our data centers to be connected directly to the account's network. The device is housed in a dedicated rack and is mounted as an iSCSI target for two weeks. During that period, the administrator can access the device on the network to use it with other devices and services on the account. After the two-week period, an extension can be requested to keep the device connected to the network. Otherwise, the device is either returned to the party specified in the request; or the device is destroyed onsite.

## Can I ship a device for data transfer internationally?

Hardware and disks can be shipped both domestically and internationally to any of our data centers. However, you as the Client are responsible for:

- ensuring that no import or export license is required to ship the Device to the {{site.data.keyword.IBM}} data center, or to return it to Client (if applicable);
- ensuring that Client or any Client user whose data is included in the Content is not subject to any US Government order revoking or denying their U.S. export privileges. You must notify {{site.data.keyword.IBM}} immediately if your enterprise or any such user becomes subject to any such order;
- obtaining all licensing, shipping, and customs clearance for the Device, including paying any duties, taxes, and shipping costs to and from (if applicable) the {{site.data.keyword.IBM}} data center;
- complying with all applicable laws, including privacy, import and export, which are associated with delivery and return of the Device, and the transfer of Content to the {{site.data.keyword.IBM}} data center; and
- having proper agreements in place, and obtaining all required permissions, with Client’s user for any user data Client will transfer to the hardware.

Include a pre-paid return shipping label and all appropriate export documents with your shipment and we'll package the device for return by using the label and documents you provided. If return isn't requested, the device will be destroyed.


## What types of devices can I send with a data transfer request?
Use the following guidelines when you select a device or disk (CD or DVD) to submit for data transfer:

- Hardware Requirements:
   - Power supply must be 208v/220v compatible.

   - Power plug must fit a standard 120v socket (NEMA 5-15P).

   - Device must be USB 2.0 or USB 3.0 compatible.

   - Provide a USB A Male connector (standard USB plug that fits most computers).

- CD/DVD Requirements:

   - Disks must be submitted in CD books, jewel cases, or similar container. If you want to submit multiple disks, store disks together in a single case or CD book.

   - Each disk must be clearly and uniquely labeled (such as Disk A, Disk B, Disk C, and so on).

## Can I get my device back sooner or have it stay longer than two weeks?

Yes, your hardware or disks can be returned at any time or can stay connected longer, if necessary. To request a return on an extension, add a comment to the original data transfer request ticket with the appropriate request. If you request a return, we will disconnect and return the hardware or disks to the return shipping address provided in the original request by using the pre-paid shipping labels and packaging you provided.

If you request an extension, the extension request will be processed as quickly as possible. It's important to note that each extension request extends the time that the device is connected for one week and can be subject to an extension fee. More details will be included when a member of our team responds to the request in the original ticket.

## What does each status on my data transfer ticket mean?

Each status on the data transfer ticket indicates the phase of the transfer process for the hardware or disks submitted to the data center. Refer to the table below for specific details on each status:

|Status 	| Definition |
|---------| -----------|
|Sent To SoftLayer 	|The Data Transfer Request was submitted by the user and the hardware or disks(s) is being shipped to the selected data center.|
|Received by SoftLayer |	The shipment was received by the data center, the device was assigned a serial number and was scanned into our system.|
|Connect |	The hardware or disk is connected to the device.|
|Connected |	An iSCSI target is created for the device.|
|Request for Extension | User requested an extension on the two-week connection time.|
|Request for Return | User requested the return of hardware or disks.|
|Disconnect |	Disconnection of hardware or disks was initiated.|
|Disconnected |	Target is safely detached.|
|Destroyed | The device was destroyed on site following our HDD destruction procedure.|
|Return by SoftLayer |	Hardware or disks was packaged and shipped to the return address provided in the original request.|

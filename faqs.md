---

copyright:
  years: 2017, 2025
lastupdated: "2025-01-13"

keywords: faqs, frequently asked questions, DTS, data transfer,

subcollection: DataTransferService

---

{{site.data.keyword.attribute-definition-list}}

# FAQs
{: #faqs}

The Data Transfer Service is deprecated. As of 04 November 2024, you can't create new requests for this service. Any existing requests are serviced according to the terms of the offering.
{: deprecated}

Frequently asked questions about {{site.data.keyword.cloud}} Data Transfer Service.
{: shortdesc}

## What is the Data Transfer Service?
{: faq}
{: #DTSdefinition}

By using this service, authorized users (generally the account's administrator) can send compatible devices to one of the {{site.data.keyword.BluSoftlayer_full}} data centers to be connected directly to the account's network. The device is housed in a dedicated rack and is mounted as an iSCSI target for two weeks. During that period, the administrator can access the device on the network to use it with other devices and services on the account. After the two-week period, an extension can be requested to keep the device connected to the network. Otherwise, the device is either returned to the party specified in the request, or the device is destroyed onsite.

## Can a device for data transfer be sent internationally?
{: faq}
{: #DTSinternational}

Hardware can be sent both domestically and internationally to any of the {{site.data.keyword.BluSoftlayer}} data centers. However, you as the Client are responsible for the meeting the following requirements.

- Ensuring that no import or export license is required to ship the Device to the {{site.data.keyword.IBM}} data center, or to return it to Client (if applicable).
- Ensuring that Client or any Client user whose data is included in the Content is not subject to any US Government order that revokes or denies their US export privileges. You must notify {{site.data.keyword.IBM}} immediately if your enterprise or any such user becomes subject to any such order.
- Obtaining all licensing, shipping, and customs clearance for the Device, including paying any duties, taxes, and shipping costs to and from (if applicable) the {{site.data.keyword.IBM}} data center.
- Complying with all applicable laws, including privacy, import and export, which are associated with delivery and return of the Device, and the transfer of Content to the {{site.data.keyword.IBM}} data center.
- Having proper agreements in place, and obtaining all required permissions with Client’s user for any user data Client transfers to the hardware.

Include a pre-paid return-shipping label and all appropriate export documents with your shipment. {{site.data.keyword.BluSoftlayer}} packages the device for return by using the label and documents that you provided. If return isn't requested, the device is destroyed.


## What types of devices can be sent with a data transfer request?
{: faq}
{: #DTSdevices}

Use the following **Hardware Requirements** guidelines when you select a device to submit for data transfer.

- The power supply must be 208v/220v compatible.
- The power plug must fit a standard 120v socket (NEMA 5-15P).
- The device must be USB 2.0 or USB 3.0 compatible.
- Provide a USB A male connector (a standard USB plug that fits most computers).

    Encrypted USB devices that require support for proprietary encryption software are not supported for data transfer.
    {: note}

## Can the device be sent back sooner or can it stay longer than two weeks?
{: faq}
{: #DTSreturndate}

Yes, your hardware can be returned at any time or can stay connected longer, if necessary. To request a return on an extension, add a comment to the original data transfer request case with the appropriate request. If you request a return, {{site.data.keyword.cloud}} disconnects and returns the hardware to the return address provided in the original request by using the pre-paid shipping labels and packaging that you provided.

If you request an extension, the extension request is processed as quickly as possible. It's important to note that each extension request extends the time that the device is connected for one week and can be subject to an extension fee. More details are added when a member of the {{site.data.keyword.BluSoftlayer_full}} team responds to the request in the original ticket.

Each status on the data transfer case indicates the phase of the transfer process for the hardware that was submitted to the data center. Refer to the following table for specific details on each status.

|Status 	| Definition |
|---------| -----------|
|`Sent To SoftLayer` |The Data Transfer Request was submitted by the user and the hardware is being shipped to the selected data center.|
|`Received by SoftLayer` |	The shipment was received by the data center, the device was assigned a serial number and was scanned into the {{site.data.keyword.cloud}} system.|
|`Connect` |	The hardware is connected to the device.|
|`Connected` |	An iSCSI target is created for the device.|
|`Request for Extension` | The client requested an extension on the two-week connection time.|
|`Request for Return` | The client requested the return of the hardware.|
|`Disconnect` |	Disconnection of hardware was initiated.|
|`Disconnected` |	The target is safely detached.|
|`Destroyed` | The device was destroyed on site by following the {{site.data.keyword.cloud}} HDD destruction procedure.|
|`Return by SoftLayer` |	The hardware was packaged and shipped to the return address provided in the original request.|
{: caption="Status definitions." caption-side="bottom"}

## Can I mount DTS on VMware&reg; ESXi servers?
{: faq}
{: #DTSVMware}

{{site.data.keyword.cloud}} does not support mounting a DTS device on a VMware&reg; VCenter server. You can attach the DTS device to Linux&reg; and Windows operating systems.

## Can I access my DTS device from VPC clients?
{: faq}
{: #DTS4VPC}

No. Some Classic services are not accessible from VPC over DirectLink. If you have compute resources in Classic and VPC, you can try moving the data from your device to your Classic virtual server instance or baremetal server first. Then, copy the data from the Classic server to your VPC server.

---

copyright:
  years: 2017, 2019
lastupdated: "2019-07-01"

keywords:

subcollection: DataTransferService

---

{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:external: target="_blank" .external}
{:codeblock: .codeblock}
{:tip: .tip}
{:note: .note}
{:important: .important}

# About Data Transfer Service
{: #about}

With {{site.data.keyword.cloud}} Data Transfer Service, you can send a USB 2.0 or 3.0 compatible device to a {{site.data.keyword.cloud_notm}} data center to be connected directly to your network. The device is housed in a dedicated rack and is mounted as an iSCSI target. Advanced Format drives are now supported as well.

## Hardware requirements
{: #hardware-requirements}

- Device must have a power supply that is 208v/220v compatible
- Device must have a power plug that fits a standard 120v socket (NEMA 5-15P)
- Device must be USB 2.0 compatible (3.0 is now supported as well)
- Device must come with USB cable with USB A Male connector (standard plug that fits most computers)

  Encrypted USB devices that require support for proprietary encryption software are not supported for data transfer.
  {: note}

## Pricing
{: #pricing}

1. Initial request for service = $0
2. First two weeks of data transfer = $0
      **Note**: $25 per week is charged for extension.
3. Shipping cost to and from the {{site.data.keyword.IBM}} data center including paying any duties and taxes.

As the Client, you are responsible for:

- Ensuring no import or export license is required to send the Device to the {{site.data.keyword.IBM}} data center, or to return it to Client (if applicable).
- Ensuring that Client or any Client user whose data is included in the Content is not subject to any US Government order that revokes or denies their US export privileges. Notify {{site.data.keyword.IBM}} immediately if Client or any such user becomes subject to any such order.
- Obtaining all licensing, shipping, and customs clearance for the Device. Client responsibilities include paying any duties, taxes, and shipping costs to and from (if applicable) the {{site.data.keyword.IBM}} data center.
- Complying with all applicable laws that are associated with delivery and return of the Device, and the transfer of Content to the {{site.data.keyword.IBM}} data center. This requirement includes privacy, import, and export laws.
- Having proper agreements in place with and obtaining all required permissions from the Client???s user for any user data that the Client wants to transfer to the Hardware.

## Making a request
{: #make-request}

You can submit a request through [{{site.data.keyword.slportal}}](https://control.softlayer.com/){: external}.

1. Click **Storage** > **Data Migration** > **Data Transfer**.
2. Click **Order Data Transfer Request**.

    ![Making a Data Transfer Request](images/DTS.png)

Complete the form with the device's
1. Serial number
2. Type
3. A short description of the device
4. The data center that you want the device to go to
5. Tracking number that is used to track the shipment
6. Carrier service that is used
7. Return address of where you want the device to be sent to after data transfer is finished.

This request creates a support ticket to alert the {{site.data.keyword.cloud_notm}} technicians that the device is being shipped and allows them to track the delivery. When {{site.data.keyword.cloud_notm}} receives the device, the technicians connect it to the dedicated rack. When the device is connected, the ticket is updated to provide you a link to your logon credentials for the iSCSI target.

## Requesting a return
{: #request-return}

If you provided a return address and included the pre-paid shipping label in the packaging, you can request that the device is sent back to you any time during the two-week transfer period. You can submit the request through the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){: external}.

1. Select **Storage** > **Data Migration** > **Data Transfer**.
2. From the **Action** menu of your device, select **request return**.

This update alerts the {{site.data.keyword.cloud_notm}} technicians that you want the device to be disconnected and sent back to you.

## Requesting an extension
{: #request-extension}

After your two-week free period, if you still require use of your device you must request an extension through the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){: external}. This update alerts the {{site.data.keyword.BluSoftlayer}} technicians that you want to extend the time that the device is connected.

1. Select **Storage** > **Data Migration** > **Data Transfer**
2. In the **Action** menu for the device, select **request extension**.

Each extra week incurs a service fee of $25 that must be paid. Your extension request might be denied depending on the available space in the data center. When the request is granted, the ticket is updated.

## Disconnecting the device
{: #disconnect-device}

After the two-week period, the device is automatically be disconnected from the data center. If you requested a return, then your device is returned to you by the carrier you chose and to the return address you specified in the initial request. The ticket is updated stating that the device was disconnected. If you didn't request the return of your device, then it is destroyed onsite.

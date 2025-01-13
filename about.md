---

copyright:
  years: 2017, 2025
lastupdated: "2025-01-13"

keywords:

subcollection: DataTransferService

---

{{site.data.keyword.attribute-definition-list}}

# About Data Transfer Service
{: #about}

The Data Transfer Service is deprecated. As of 04 November 2024, you can't create new requests for this service. Any existing requests are serviced according to the terms of the offering.
{: deprecated}

With {{site.data.keyword.cloud}} Data Transfer Service, you can send a USB 2.0 or 3.0 compatible device to an {{site.data.keyword.cloud_notm}} data center to be connected directly to your network. The device is housed in a dedicated rack and is mounted as an iSCSI target. Advanced Format drives are now supported as well.

## Hardware requirements
{: #hardware-requirements}

- The device must have a power supply that is 208v/220v compatible.
- The device must have a power plug that fits a standard 120v socket (NEMA 5-15P).
- The device must be USB 2.0 compatible (3.0 is now supported as well).
- Device must come with USB cable with USB A Male connector (a standard plug that fits most computers).

   Encrypted USB devices that require support for proprietary encryption software are not supported for data transfer.
   {: note}

## Pricing
{: #pricing}

1. Initial request for service = $0
2. First two weeks of data transfer = $0

   $25 per week is charged for extension.
   {: note}

3. Shipping costs to and from the {{site.data.keyword.IBM}} data center including paying any duties and taxes.

As the Client, you are responsible for:

- Ensuring no import or export license is required to send the Device to the {{site.data.keyword.IBM}} data center, or to return it to Client (if applicable).
- Ensuring that Client or any Client user whose data is included in the Content is not subject to any US Government order that revokes or denies their US export privileges. Notify {{site.data.keyword.IBM}} immediately if Client or any such user becomes subject to any such order.
- Obtaining all licensing, shipping, and customs clearance for the Device. Client responsibilities include paying any duties, taxes, and shipping costs to and from (if applicable) the {{site.data.keyword.IBM}} data center.
- Complying with all applicable laws that are associated with delivery and return of the Device, and the transfer of Content to the {{site.data.keyword.IBM}} data center. This requirement includes privacy, import, and export laws.
- Having proper agreements in place with and obtaining all required permissions from the Client’s user for any user data that the Client wants to transfer to the Hardware.

## Requesting a return
{: #request-return}

If you provided a return address and included the pre-paid shipping label in the packaging, you can request that the device is sent back to you anytime during the two-week transfer period. You can submit the request in the [{{site.data.keyword.cloud_notm}} console](/login){: external}.

1. Select **Infrastructure** ![VPC icon](../icons/vpc.svg) > **Classic Infrastructure** > **Storage**  > **Data Migration** > **Data Transfer**.
2. From the **Action** menu of your device, select **request return**.

This update alerts the {{site.data.keyword.cloud_notm}} technicians that you want the device to be disconnected and sent back to you.

## Requesting an extension
{: #request-extension}

After your two-week no-cost period, if you still require use of your device you must request an extension in the [{{site.data.keyword.cloud_notm}} console](/login){: external}. This update alerts the technician that you want to extend the time that the device is connected.

1. Select **Infrastructure**  ![VPC icon](../icons/vpc.svg) > **Classic Infrastructure** > **Storage**  > **Data Migration** > **Data Transfer**.
2. In the **Action** menu for the device, select **request extension**.

Each added week incurs a service fee of $25 that must be paid. Your extension request might be denied depending on the available space in the data center. When the request is granted, the ticket is updated.

## Disconnecting the device
{: #disconnect-device}

After the two-week period, the device is automatically be disconnected from the data center. If you requested a return, then your device is returned to you by the carrier you chose and to the return address you specified in the initial request. The ticket is updated stating that the device was disconnected. If you didn't request the return of your device, then it is destroyed onsite.

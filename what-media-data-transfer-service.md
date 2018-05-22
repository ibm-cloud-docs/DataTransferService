---

copyright:
  years: 2017, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# What is media data transfer service?
 
The data transfer service allows you to send a USB 2.0 or 3.0 compatible device, CDs and DVDs to a {{site.data.keyword.BluSoftlayer_full}} datacenter to be connected directly to your network. The device is housed in a dedicated rack and is mounted as an iSCSI target. Advanced Format drives are now supported as well.

## Hardware Requirements
1.    Device must have a power supply that is 208v/220v compatible
2.    Device must have a power plug that fits a standard 120v socket (NEMA 5-15P)
3.    Device must be USB 2.0 compatible (3.0 is now supported as well)
4.    Device must come with USB cable with USB A Male connector (standard plug that fits most computers)
5.    CDS / DVDS
      1.    Must be in CD books, cases, jewel cases, or some of form of container and preferably all together in one container (A CD book, for example) and each disk must be labeled uniquely.
      2.    Disks will be rotated at the customer’s request via the ticket

## Cost to You
1.    Initial Request for service: $0
2.    First 2 weeks of Data Transfer: $0
      **Note**: $25 per week is charged for extension.
3.    Shipping cost to and from the {{site.data.keyword.IBM}} data center including paying any duties and taxes.

**Note**: Client is responsible for:  
- ensuring no import or export license is required to ship the Device to the {{site.data.keyword.IBM}} data center, or to return it to Client (if applicable); 
- ensuring that Client or any Client user whose data is included in the Content is not subject to any US Government order revoking or denying their US export privileges. Notify {{site.data.keyword.IBM}} immediately if Client or any such user becomes subject to any such order;  
- obtaining all licensing, shipping, and customs clearance for the Device. Client responsibilities include paying any duties, taxes, and shipping costs to and from (if applicable) the {{site.data.keyword.IBM}} data center;   
- complying with all applicable laws that are associated with delivery and return of the Device, and the transfer of Content to the {{site.data.keyword.IBM}} data center. This includes privacy, import, and export laws.
- having proper agreements in place with and obtaining all required permissions from the Client’s user for any user data that the Client wants to transfer to the Hardware.

## Making a Request
This is done through **Storage** > **Data Migration** >  **Data Transfer**, then click **Order Data Transfer Request** on the upper-right corner.

![Making a Data Transfer Request](/images/DTS.png)

Complete the form with the device's
1. Serial number
2. Type
3. A short description of the device
4. The data center you would like the device to go to
5. Tracking number that is used to track the shipment
6. Carrier service that is used
7. Return address of where you would like the device to be shipped to when finished.

This request creates a support ticket to alert our technicians that the device is being shipped to us and allows them to track the delivery. When we receive the device we connect it to our dedicated rack. After we connect the device, the ticket is updated to provide you a link to your logon credentials to the iSCSI target.

## Request Return
If you provided a return address and included the pre-paid shipping label in the packaging, you can request that the device be shipped back to you any time during the two-week transfer period. You can do this through the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. Select **Storage** > **Data Migration** > **Data Transfer** and from the **Action** menu of your device you select **request return**. This alerts our technicians that you want the device disconnected and shipped back to you.

## Request Extension
After your two-week free period, if you still require use of your device you must request an extension. This alerts our technicians that you want to extend the time that the device is connected. You can do this in the same way that you would request that your device is returned to you. Select **Storage** > **Data Migration** > **Data Transfer** and in the **Action** menu for the device select **request extension**. Each extra week incurs a service fee of $25 that must be paid. Please note that your extension request might be denied depending on the available space in the data center. When the request is granted, the ticket is updated accordingly.

## Disconnect
After the two-week period the device is automatically be disconnected from our data center. If you requested a return, then your device is returned to you by the carrier you chose and to the return address you specified in the initial request. The ticket is updated stating that the device was disconnected. If you didn't request the return of your device, then it is destroyed onsite.

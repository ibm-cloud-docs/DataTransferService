---

copyright:
  years: 2017
lastupdated: "2017-12-14"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# What is Media Data Transfer Service?
 
The Data Transfer Service is a service that allows you to send a USB 2.0 or 3.0 compatible device and/or CD's and DVD's to a {{site.data.keyword.BluSoftlayer_full}} datacenter to be connected directly to your network. The device is housed in a dedicated rack located in the datacenter of choice and will be mounted as an iSCSI target. Advanced Format drives are now supported as well.

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
      **Note**: $25 per week is charged for extension
3.    Shipping cost to and from the {{site.data.keyword.IBM}} data center including paying any duties and taxes.

**Note**: Client is responsible for:  
- ensuring no import or export license is required to ship the Device to the {{site.data.keyword.IBM}} data center, or to return it to Client (if applicable); 
- ensuring neither Client nor any Client end user whose data is included in the Content is subject to any U.S. Government order revoking or denying their U.S. export privileges. Client agrees to notify {{site.data.keyword.IBM}} immediately if Client or any such end user becomes subject to any such order;  
- obtaining all licensing, shipping, and customs clearance for the Device, including paying any duties, taxes and shipping costs to and from (if applicable) the {{site.data.keyword.IBM}} data center;   
- complying with all applicable laws, including privacy, import and export, associated with delivery and return of the Device, and the transfer of Content to the {{site.data.keyword.IBM}} data center; and 
- having proper agreements in place, and obtaining all required permissions, with Client’s end user for any end user data Client will transfer to the Hardware.

## Making a Request
This is done under **Storage** > **Data Migration** >  **Data Transfer**, then click on the **Order Data Transfer Request** link on the top right of the page.

![Making a Data Transfer Request](/images/DTS.png)
 

Fill out this form with the devices
1. Serial number
2. Type
3. A short description of the device
4. The datacenter you would like the device to go in
5. Tracking number used to track the shipment
6. Carrier service used
7. Return address of where you would like the device shipped to when finished.

Once filled out this will automatically create a support ticket to alert our technicians that the device is being shipped to us and allow them the ability to track the delivery.  Once we receive the device we will then proceed to connect it to our dedicated rack.  Once we have connected the device the ticket will be updated providing you a link to your log on credentials to the iSCSI target.

## Request Return
If you provided a return address and included the pre-paid shipping label in the packaging, you can request that the device to be shipped back to you any time during the 2 week long transfer period. You do this via the [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} by selecting **Storage** > **Data Migration** > **Data Transfer** and from the **Action** drop down of your device you select **request return**. This will alert our technicians that you would like the device disconnected and shipped back to you.

## Request Extension
After your 2 week free period if you still require use of your USB device you must request an extension which will alert our technicians that you would like to extend the time that the device is connected.  You do this in the same way that you would request your device returned to you by selecting **Storage** > **Data Migration** > **Data Transfer** and in the **Action** drop down for the device select **request extension**.  Each week longer than the two first weeks there will be a service fee of 25 dollars that must be paid.  Also depending on the available space in the datacenter for your device your request could be denied.  If the request is granted the ticket will be updated stating that you have been granted the extra week.

## Disconnect
After the two week period the device will automatically be disconnected from our datacenter and returned to you via the carrier of choice and to the return address you specified in the initial request. The ticket will be updated stating that the device has been disconnected. If you did not request the return of your device, it will be destroyed onsite.

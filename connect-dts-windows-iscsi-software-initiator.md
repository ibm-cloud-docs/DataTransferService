---

copyright:
  years: 2017, 2024
lastupdated: "2024-10-01"

keywords: connecting DTS, Map DTS Device to Windows OS, mapping DTS, attaching DTS

subcollection: DataTransferService

---

{{site.data.keyword.attribute-definition-list}}

# Connecting to DTS Device in Windows&reg;with iSCSI Software Initiator
{: #mount-dts-windows}

The Data Transfer Service is deprecated. As of 04 November 2024, you can't create new requests for this service. Any existing requests will be serviced as per the terms of offering.
{: deprecated}

To interact with an iSCSI LUN in Windows&reg;, you must connect to the storage by using the iSCSI Software Initiator, a proprietary iSCSI tool of Microsoft. 
{: shortdesc}

## Connecting to an iSCSI LUN
{: #connect-dts-iscsi}

1. From the {{site.data.keyword.slportal}}, retrieve the **iSCSI username, password, and storage address** for the storage device you want to connect.
1. Start the iSCSI Initiator. From Server Manager, click the **Tools** menu, and then choose **iSCSI Initiator**.
1. In the **Target field**, enter the hostname or IP address of the storage device, 
1. Click **Quick Connect**.
1. When the iSCSI Target is detected, click **Done**.
1. Click **Connect** to establish connection to the discovered, inactive target.
1. In the next window, select **Advanced...**.
1. In the Advanced settings, update the iSCSI logon information.
   - Click the **CHAP logon information** box to enable CHAP logon.
   - Enter the iSCSI username in the **username** field.
   - Enter the iSCSI password in the **target secret** field.
1. Verify that the new iSCSI target displays as Connected on the Targets tab.
    - If your iSCSI target displays as **Connected**, click **OK**. Your iSCSI LUN is now connected.
    - If your iSCSI target doesn't display as **Connected**, repeat all the previous steps to reset the connection.
1. To use the iSCSI Disk, turn it online and initialize it. Then, assign a drive letter to it.    

You can also use [PowerShell commands for ISCSI](https://learn.microsoft.com/en-us/powershell/module/iscsi/?view=windowsserver2022-ps){: external} to establish a connection between the local iSCSI initiator and an iSCSI target device.

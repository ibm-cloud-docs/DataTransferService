---

copyright:
  years: 2017, 2024
lastupdated: "2023-01-11"

keywords: connecting DTS, Map DTS Device to Windows OS, mapping DTS, attaching DTS

subcollection: DataTransferService

---

{{site.data.keyword.attribute-definition-list}}

# Connecting to DTS Device in Windows&reg;with iSCSI Software Initiator
{: #mount-dts-windows}

To interact with an iSCSI LUN in Windows&reg;, you must connect to the storage by using the iSCSI Software Initiator, a proprietary iSCSI tool of Microsoft. For users of Windows&reg; Server 2008, or Windows&reg; Vista or newer versions, the iSCSI Software Initiator is built into the operating system. Users of Windows&reg; Server 2003, Windows&reg; XP, and Windows&reg; 2000 must download the Initiator before they start this procedure.

## Connecting to an iSCSI LUN
{: #connect-dts-iscsi}

1. From the {{site.data.keyword.slportal}}, retrieve the **iSCSI username, password, and storage address** for the storage device you want to connect.
2. Start the iSCSI Initiator.
3. Click **Discovery**.
4. In the **Target Portals** section, click **Discover Portal...**.
5. In the **IP address or DNS name** field, enter the **iSCSI IP address**.
6. Click **Advanced**.
7. Update the iSCSI logon information.
   - Click the **CHAP logon information** box to enable CHAP logon.
   - Enter the iSCSI username in the **username** field.
   - Enter the iSCSI password in the **target secret** field.
   - Click **OK** twice.
8. Click **Targets**.
9. Select the newly added iSCSI from the **Targets** list.
10. Click **Logon**. The **Log On to Target** window appears.
11. Select **Automatically restore this connection when the system boots** to set the connection to persist between restarts.
12. Click **Advanced**.
13. Update the iSCSI logon information.
    - Select the **CHAP logon information** checkbox to enable CHAP logon.
    - Enter the iSCSI username in the **username** field.
    - Enter the iSCSI password in the **target secret** field.
    - Click **OK** twice.
14. Verify that the new iSCSI target displays as Connected on the Targets tab.
    - If your iSCSI target displays as **Connected**, click **OK**. Your iSCSI LUN is now connected.
    - If your iSCSI target doesn't display as **Connected**, repeat all the previous steps to reset the connection.

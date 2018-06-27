---

copyright:
  years: 2017, 2018
lastupdated: "2018-06-27"

---
{:new_window: target="_blank"}

# Connecting to DTS Device in Windows with iSCSI Software Initiator

To interact with an iSCSI LUN in Windows, users must connect to the storage by using the iSCSI Software Initiator, a proprietary iSCSI tool of Microsoft. For users of Windows Server 2008, or Windows Vista or newer versions, the iSCSI Software Initiator is built into the operating system. Users of Windows Server 2003, Windows XP, and Windows 2000 must download the Initiator before they start this procedure.

## Connecting to an iSCSI LUN

1. From the {{site.data.keyword.slportal}}, retrieve the **iSCSI user name, password, and storage address** for the storage device you want to connect.
2. Start the iSCSI Initiator.
3. On the **Configuration** tab, update initiator name to the IQN data in the {{site.data.keyword.slportal}}.
4. Click **Discovery**.
5. In the **Target Portals** section, click **Add**.
6. In the **IP address or DNS name** field, enter the **iSCSI IP address**.
7. Click **Advanced**.
8. Update the iSCSI logon information.
   - Select the **CHAP logon information** check box to enable CHAP logon.
   - Enter the iSCSI user name in the **user name** field.
   - Enter the iSCSI password in the **target secret** field.
   - Click **OK** twice.
9. Click **Targets**
10. Select the newly added iSCSI from the **Targets** list.
11. Click **Logon**. The **Log On to Target** window appears.
12. Select **Automatically restore this connection when the system boots** to set the connection to persist between restarts.
13. Click **Advanced**.
14. Update the iSCSI logon information.
    - Select the **CHAP logon information** check box to enable CHAP logon.
    - Enter the iSCSI user name in the **user name** field.
    - Enter the iSCSI password in the **target secret** field.
    - Click **OK** twice.
15. Verify that the new iSCSI target displays as Connected on the Targets tab.
    - If your iSCSI target displays as **Connected**, click **OK**. Your iSCSI LUN is now connected
    - If your iSCSI target doesn't display as **Connected**, repeat all the previous steps to reset the connection.

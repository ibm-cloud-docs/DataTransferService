---

copyright:
  years: 2017
lastupdated: "2017-06-27"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Connect to DTS Device in Windows with iSCSI Software Initiator

To interact with an iSCSI LUN in Windows, users must connect to the LUN using iSCSI Software Initiator, Microsoft's proprietary iSCSI tool.  For users running Windows Server 2008 or Windows Vista and above, iSCSI Software Initiator is built into the operating system.  Users running Windows Server 2003, Windows XP and Windows 2000 must download the Initiator prior to completing this procedure.  Follow the steps below to connect to an iSCSI LUN in Windows with iSCSI Software Initiator.

## Connect to an iSCSI LUN

1. Retrieve the **iSCSI User Name, Pasword and Storage Address** for the iSCSI being connected from the Customer Portal.  Refer to Access the Data Transfer Screen.
2. Launch iSCSI Initiator.
3. Update initiator name on the **Configuration** tab to the IQN data in the SoftLayer portal.
4. Click the **Discovery** tab.
5. Click the **Add** button in the **Target Portals** section of the screen.
6. Enter the **iSCSI IP Address** in the **IP address or DNS name** field.
7. Click the **Advanced** tab.
8. Update the iSCSI logon information.
   - Select the **CHAP logon information** check box to enable CHAP logon.
   - Enter the **iSCSI Username** in the **User name** field.
   - Enter the **iSCSI Password** in the **Target secret** field.
   - Click the **OK** button twice.
9. Click the **Targets** tab.
10. Select the newly added iSCSI from the **Targets** list.
11. Click the **Logon** button. The **Log On to Target** pop up menu will appear.
12. Select the **Automatically restore this connection when the system boots** check box to set the connection to persist between reboots.
13. Click **the Advanced** button.
14. Update the iSCSI logon information.
    - Select the **CHAP logon information** check box to enable CHAP logon.
    - Enter the **iSCSI Username** in the **User name** field.
    - Enter the **iSCSI Password** in the **Target secret** field.
    - Click the **OK** button twice.
15. Verify that the new iSCSI target displays as Connected on the Targets tab.

<table>
<tbody>
<tr>
<th>If the iSCSI target…</th><th>Then...</th></tr>
<tr><td>Displays as Connected</td><td>Click the <strong>OK</strong> button. Your iSCSI LUN is now connected.</td></tr>
<tr><td>Does not display as Connected</td><td>Repeat the steps above to reset the connection.</td></tr></tbody></table>

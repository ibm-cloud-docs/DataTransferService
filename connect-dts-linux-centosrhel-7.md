---

copyright:
  years: 2017, 2023
lastupdated: "2023-01-11"

keywords: connecting DTS device, hook up, link up, mount DTS device, DTS

subcollection: DataTransferService

---

{{site.data.keyword.attribute-definition-list}}

# Connecting to DTS Device in Linux&reg;for CentOS/RHEL 7
{: #mount-dts-linux}

To interact with an iSCSI LUN in Linux-based operating systems, you must connect to the LUN by entering a series of commands in the terminal. The tool that is used to interact with an iSCSI LUN in a Linux&reg;-based OS is dependent upon the type and version of the OS that is installed on the device.

Before you begin, retrieve the iSCSI username, password, and storage address for the storage volume that you want to connect from the [{{site.data.keyword.cloud_notm}} console](/login){: external}.

## Configuring connection in CentOS 7 and RHEL 7
{: #configure-connection-linux}

1. Install iSCSI initiator and multipath mapper utilities for Linux&reg;.
   ```zsh
   yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath
   ```
   {: pre}

2. Create the `iscsid.conf` configuration file.

3. Back up the original configuration.
   ```zsh
   cp /etc/iscsi/iscsid.conf{,.save}
   ```
   {: pre}

4. Open `/etc/iscsi/iscsid.conf` with your favorite text editor and replace the contents with the following code:
   ```zsh
   node.startup = automatic
   node.session.auth.username = ISCSI_USER
   node.session.auth.password = ISCSI_PASS
   discovery.sendtargets.auth.username = ISCSI_USER
   discovery.sendtargets.auth.password = ISCSI_PASS
   node.session.timeo.replacement_timeout = 120
   node.conn[0].timeo.login_timeout = 15
   node.conn[0].timeo.logout_timeout = 15
   node.conn[0].timeo.noop_out_interval = 10
   node.conn[0].timeo.noop_out_timeout = 15
   node.session.iscsi.InitialR2T = No
   node.session.iscsi.ImmediateData = Yes
   node.session.iscsi.FirstBurstLength = 262144
   node.session.iscsi.MaxBurstLength = 16776192
   node.conn[0].iscsi.MaxRecvDataSegmentLength = 65536
   ```
   {: pre}

5. Start iSCSI.
   ```zsh
   systemctl start iscsi.service
   ```
   {: pre}

6. Run a discovery against the iscsi target host.
   ```zsh
   iscsiadm -m discovery -t sendtargets -p [IP address in StorageLayer]
   ```
   {: pre}

7. Connect to the iscsi target host.
   ```zsh
   iscsiadm -m node -T [output from previous command, starting with IQN.] -p [IP address in StorageLayer] -l
   ```
   {: pre}

8. Restart the iSCSI service. Because `node.startup` is set to automatic in `iscsid.conf`, it automatically logs in to the target host.
   ```zsh
   systemctl restart iscsi.service
   ```
   {: pre}

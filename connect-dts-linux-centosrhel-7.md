---

copyright:
  years: 2017
lastupdated: "2017-11-13"-

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Connecting to DTS Device in Linux for CentOS/RHEL 7

To interact with an iSCSI LUN in Linux-based operating systems, users must connect to the LUN by entering a series of commands in the terminal based on the operating system being used to perform the interactions.  The tool used to interact with an iSCSI LUN in a Linux-based OS is dependent upon the type and version of the OS installed on the device.

## Instructions for CentOS 7 and RHEL 7

1. Install iscsi-initiator and multipath mapper for Linux <br/>
   ``yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath`` 
2. Create the iscsid.conf configuration file <br/>
3. Backup the original configuration: <br/>
   ``cp /etc/iscsi/iscsid.conf{,.save}`` 
4. Open /etc/iscsi/iscsid.conf with your favorite text editor and replace the contents with the following: <br/>
   ``node.startup = automatic ``<br/>
   ``node.session.auth.username = ISCSI_USER ``<br/>
   ``node.session.auth.password = ISCSI_PASS ``<br/>
   ``discovery.sendtargets.auth.username = ISCSI_USER ``<br/>
   ``discovery.sendtargets.auth.password = ISCSI_PASS ``<br/>
   ``node.session.timeo.replacement_timeout = 120 ``<br/>
   ``node.conn[0].timeo.login_timeout = 15 ``<br/>
   ``node.conn[0].timeo.logout_timeout = 15 ``<br/>
   ``node.conn[0].timeo.noop_out_interval = 10 ``<br/>
   ``node.conn[0].timeo.noop_out_timeout = 15 ``<br/>
   ``node.session.iscsi.InitialR2T = No ``<br/>
   ``node.session.iscsi.ImmediateData = Yes ``<br/>
   ``node.session.iscsi.FirstBurstLength = 262144 ``<br/>
   ``node.session.iscsi.MaxBurstLength = 16776192 ``<br/>
   ``node.conn[0].iscsi.MaxRecvDataSegmentLength = 65536 ``<br/>
5. Start iscsid:<br/>
   ``/etc/init.d/iscsi start``
6. Run a discovery against the iscsi target host:<br/>
   ``iscsiadm -m discovery -t sendtargets -p [IP Address in StorageLayer]``
7. Connect to the iscsi target host:<br/>
   ``iscsiadm -m node -T [output from above starting with iqn.] -p [IP Address in storagelayer] -l``
8. Restart the iscsi service (Since node.startup was set to automatic in iscsid.conf it will automatically login to the target host).<br/>
   ``/etc/init.d/iscsi restart``

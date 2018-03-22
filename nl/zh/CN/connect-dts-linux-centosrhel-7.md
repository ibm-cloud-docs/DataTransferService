---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# 连接到 Linux for CentOS/RHEL 7 中的 DTS 设备

要与基于 Linux 的操作系统中的 iSCSI LUN 进行交互，用户必须通过在终端（基于要用于执行交互的操作系统）中输入一系列命令来连接到该 LUN。用于与基于 Linux 的操作系统中的 iSCSI LUN 进行交互的工具取决于设备上安装的操作系统的类型和版本。

## CentOS 7 和 RHEL 7 的指示信息

1. 安装 Linux 的 iSCSI 启动器和多路径映射器<br/>
   ``yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath`` 
2. 创建 iscsid.conf 配置文件<br/>
3. 备份原始配置：<br/>
   ``cp /etc/iscsi/iscsid.conf{,.save}`` 
4. 使用偏好的文本编辑器打开 /etc/iscsi/iscsid.conf，并替换为以下内容：<br/>
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
5. 启动 iscsid：<br/>
   ``/etc/init.d/iscsi start``
6. 对 iSCSI 目标主机运行发现：<br/>
   ``iscsiadm -m discovery -t sendtargets -p [IP Address in StorageLayer]``
7. 连接到 iSCSI 目标主机：<br/>
   ``iscsiadm -m node -T [output from above starting with iqn.] -p [IP Address in storagelayer] -l``
8. 重新启动 iSCSI 服务（由于 iscsid.conf 中的 node.startup 设置为 automatic，因此它将自动登录到目标主机）。<br/>
   ``/etc/init.d/iscsi restart``

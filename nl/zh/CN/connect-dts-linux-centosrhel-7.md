---

copyright:
  years: 2017, 2018
lastupdated: "2017-05-22"

---
{:pre: .pre}

# 连接到 Linux for CentOS/RHEL 7 中的 DTS 设备

 要与基于 Linux 的操作系统中的 iSCSI LUN 进行交互，用户必须通过在终端中输入一系列命令来连接到该 LUN。用于与基于 Linux 的操作系统中的 iSCSI LUN 进行交互的工具取决于设备上安装的操作系统的类型和版本。

## 针对 CentOS 7 和 RHEL 7 的指示信息

1. 针对 Linux 安装 iSCSI 启动器和多路径映射器。
   ```
   yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath
   ``` 
   {: pre}
   
2. 创建 iscsid.conf 配置文件。

3. 备份原始配置：
   ```
   cp /etc/iscsi/iscsid.conf{,.save}
   ``` 
   {: pre}
   
4. 使用最喜欢的文本编辑器打开 /etc/iscsi/iscsid.conf，并将内容替换为以下代码： 
   ```
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

5. 启动 iSCSI：<br/>
   ```
   /etc/init.d/iscsi start
   ```
   {: pre}
   
6. 对 iSCSI 目标主机运行发现：<br/>
   ```
   iscsiadm -m discovery -t sendtargets -p [IP address in StorageLayer]
   ```
   {: pre}
   
7. 连接到 iSCSI 目标主机：<br/>
   ```
   iscsiadm -m node -T [output from previous command, starting with IQN.] -p [IP address in StorageLayer] -l
   ```
   {: pre}
   
8. 重新启动 iSCSI 服务（由于在 iscsid.conf 中 node.startup 设置为 automatic，因此它自动登录到目标主机）。<br/>
   ```
   /etc/init.d/iscsi restart
   ```
   {: pre}

---

copyright:
  years: 2017, 2018
lastupdated: "2018-05-22"

---
{:pre: .pre}

# 在 Linux for CentOS/RHEL 7 中連接至 DTS 裝置

若要與 Linux 型作業系統中的 iSCSI LUN 互動，使用者必須在終端機中輸入一系列指令來連接至 LUN。用來在 Linux 型作業系統中與 iSCSI LUN 互動的工具，取決於裝置上安裝的作業系統類型及版本。

## CentOS 7 及 RHEL 7 的指示

1. 安裝適用於 Linux 的 iSCSI 啟動器及多路徑對映程式。
   ```
   yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath
   ```
   {: pre}

2. 建立 iscsid.conf 配置檔。

3. 備份原始配置：
   ```
   cp /etc/iscsi/iscsid.conf{,.save}
   ```
   {: pre}

4. 使用您偏好的文字編輯器開啟 /etc/iscsi/iscsid.conf，將內容取代為下列程式碼：
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

5. 啟動 iSCSI：<br/>
   ```
   /etc/init.d/iscsi start
   ```
   {: pre}

6. 針對 iSCSI 目標主機執行探索：<br/>
   ```
   iscsiadm -m discovery -t sendtargets -p [IP address in StorageLayer]
   ```
   {: pre}

7. 連接至 iSCSI 目標主機：<br/>
   ```
   iscsiadm -m node -T [output from previous command, starting with IQN.] -p [IP address in StorageLayer] -l
   ```
   {: pre}

8. 重新啟動 iSCSI 服務（因為 node.startup 在 iscsid.conf 中已設為自動，所以它會自動登入目標主機）。<br/>
   ```
   /etc/init.d/iscsi restart
   ```
   {: pre}

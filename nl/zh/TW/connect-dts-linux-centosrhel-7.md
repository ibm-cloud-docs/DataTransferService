---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# 在 Linux for CentOS/RHEL 7 中連接至 DTS 裝置

若要與 Linux 型作業系統中的 iSCSI LUN 互動，使用者必須根據用來執行互動的作業系統在終端機中輸入一系列指令來連接至 LUN。用來在 Linux 型 OS 中與 iSCSI LUN 互動的工具，取決於裝置上安裝的 OS 類型及版本。

## CentOS 7 及 RHEL 7 的指示

1. 安裝適用於 Linux 的 iSCSI 啟動器及多路徑對映程式<br/>
   ``yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath`` 
2. 建立 iscsid.conf 配置檔<br/>
3. 備份原始配置：<br/>
   ``cp /etc/iscsi/iscsid.conf{,.save}`` 
4. 使用您偏好的文字編輯器開啟 /etc/iscsi/iscsid.conf，將內容取代為：<br/>
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
5. 啟動 iscsid：<br/>
   ``/etc/init.d/iscsi start``
6. 針對 iSCSI 目標主機執行探索：<br/>
   ``iscsiadm -m discovery -t sendtargets -p [IP Address in StorageLayer]``
7. 連接至 iSCSI 目標主機：<br/>
   ``iscsiadm -m node -T [output from above starting with iqn.] -p [IP Address in storagelayer] -l``
8. 重新啟動 iSCSI 服務（由於 node.startup 在 iscsid.conf 中已設為自動，所以它會自動登入目標主機）。<br/>
   ``/etc/init.d/iscsi restart``

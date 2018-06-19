---

copyright:
  years: 2017, 2018
lastupdated: "2018-05-22"

---
{:pre: .pre}

# CentOS/RHEL 7 対応の Linux での DTS デバイスへの接続

Linux ベースのオペレーティング・システムで iSCSI LUN を操作するには、端末で一連のコマンドを入力して LUN に接続する必要があります。Linux ベースの OS で iSCSI LUN を操作するために使用するツールは、デバイスにインストールされている OS のタイプとバージョンによって異なります。

## CentOS 7 と RHEL 7 に関する指示

1. Linux の iSCSI イニシエーターとマルチパス・マッパーをインストールします。
   ```
   yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath
   ```
   {: pre}

2. iscsid.conf 構成ファイルを作成します。

3. 以下のようにして元の構成をバックアップします。
   ```
   cp /etc/iscsi/iscsid.conf{,.save}
   ```
   {: pre}

4. 任意のテキスト・エディターで /etc/iscsi/iscsid.conf を開き、その内容を以下のコードに置き換えます。
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

5. iSCSI を開始します。<br/>
   ```
   /etc/init.d/iscsi start
   ```
   {: pre}

6. 以下のように、iscsi ターゲット・ホストに対してディスカバリーを実行します。<br/>
   ```
   iscsiadm -m discovery -t sendtargets -p [IP address in StorageLayer]
   ```
   {: pre}

7. 以下のように iscsi ターゲット・ホストに接続します。<br/>
   ```
   iscsiadm -m node -T [output from previous command, starting with IQN.] -p [IP address in StorageLayer] -l
   ```
   {: pre}

8. iSCSI サービスを再始動します (iscsid.conf で node.startup が automatic に設定されているため、ターゲット・ホストに自動的にログインします)。<br/>
   ```
   /etc/init.d/iscsi restart
   ```
   {: pre}

---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# CentOS/RHEL 7 対応の Linux での DTS デバイスへの接続

Linux ベースのオペレーティング・システムの iSCSI LUN と対話するには、対話を実行するために使用されているオペレーティング・システムをベースとした端末で、ユーザーが一連のコマンドを入力して LUN に接続する必要があります。Linux ベースの OS の iSCSI LUN との対話に使用されるツールは、デバイスにインストールされている OS のタイプとバージョンに依存します。

## CentOS 7 と RHEL 7 に関する指示

1. Linux の iSCSI イニシエーターとマルチパス・マッパーをインストールします。<br/>
   ``yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath`` 
2. iscsid.conf 構成ファイルを作成します。<br/>
3. 以下のように、元の構成をバックアップします。<br/>
   ``cp /etc/iscsi/iscsid.conf{,.save}`` 
4. 任意のテキスト・エディターで /etc/iscsi/iscsid.conf を開き、その内容を以下に置き換えます。<br/>
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
5. 以下のように iscsid を開始します。<br/>
   ``/etc/init.d/iscsi start``
6. 以下のように、iscsi ターゲット・ホストに対してディスカバリーを実行します。<br/>
   ``iscsiadm -m discovery -t sendtargets -p [IP Address in StorageLayer]``
7. 以下のように iscsi ターゲット・ホストに接続します。<br/>
   ``iscsiadm -m node -T [output from above starting with iqn.] -p [IP Address in storagelayer] -l``
8. iscsi サービスを再始動します (iscsid.conf で node.startup が automatic に設定されたため、ターゲット・ホストに自動ログインします)。<br/>
   ``/etc/init.d/iscsi restart``

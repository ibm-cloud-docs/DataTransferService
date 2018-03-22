---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Linux에서 CentOS/RHEL 7에 대한 DTS 디바이스에 연결

Linux 기반 운영 체제에서 iSCSI LUN과 상호작용하려면 상호작용을 수행하는 데 사용할 운영 체제에 기반하는 터미널에서 일련의 명령을 입력하여 LUN에 연결해야 합니다. Linux 기반 OS에서 iSCSI LUN과 상호작용하는 데 사용하는 도구는 디바이스에 설치된 OS의 유형 및 버전에 따라 달라집니다. 

## CentOS 7 및 RHEL 7에 대한 지시사항

1. Linux에 대한 iscsi-initiator 및 다중 경로 맵퍼를 설치하십시오. <br/>
   ``yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath`` 
2. iscsid.conf 구성 파일을 작성하십시오. <br/>
3. 원래 구성을 백업하십시오. <br/>
   ``cp /etc/iscsi/iscsid.conf{,.save}`` 
4. 자주 사용하는 문서 편집기에서 /etc/iscsi/iscsid.conf를 열고 컨텐츠를 다음으로 대체하십시오. <br/>
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
5. iscsid를 시작하십시오. <br/>
   ``/etc/init.d/iscsi start``
6. iscsi 대상 호스트에서 discovery를 실행하십시오. <br/>
   ``iscsiadm -m discovery -t sendtargets -p [IP Address in StorageLayer]``
7. iscsi 대상 호스트에서 연결하십시오. <br/>
   ``iscsiadm -m node -T [output from above starting with iqn.] -p [IP Address in storagelayer] -l``
8. iscsi 서비스를 다시 시작하십시오(node.startup은 iscsid.conf에서 자동으로 설정되므로 대상 호스트에 자동으로 로그인됨). <br/>
   ``/etc/init.d/iscsi restart``

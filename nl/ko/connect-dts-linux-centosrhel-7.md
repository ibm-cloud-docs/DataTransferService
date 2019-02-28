---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:pre: .pre}

# CentOS/RHEL 7용 Linux에서 DTS 디바이스에 연결
{: #mountingDTSlinux}

Linux 기반 운영 체제에서 iSCSI LUN과 상호작용하려면 사용자가 터미널에서 일련의 명령을 입력하여 LUN에 연결해야 합니다. Linux 기반 OS에서 iSCSI LUN과의 상호작용에 사용되는 도구는 디바이스에 설치된 OS의 유형과 버전에 따라 다릅니다.

## CentOS 7 및 RHEL 7에서 연결 구성

1. Linux용 다중 경로 맵퍼 유틸리티와 ISCSI Initiator를 설치하십시오.
   ```
   yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath
   ```
   {: pre}

2. `iscsid.conf` 구성 파일을 작성하십시오.

3. 원래 구성을 백업하십시오.
   ```
   cp /etc/iscsi/iscsid.conf{,.save}
   ```
   {: pre}

4. 선호하는 텍스트 편집기에서 `/etc/iscsi/iscsid.conf`를 열고 컨텐츠를 다음 코드로 대체하십시오.
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

5. iSCSI를 시작하십시오.<br/>
   ```
   systemctl start iscsi.service
   ```
   {: pre}

6. iscsi 대상 호스트에 대해 discovery를 실행하십시오.<br/>
   ```
   iscsiadm -m discovery -t sendtargets -p [IP address in StorageLayer]
   ```
   {: pre}

7. iscsi 대상 호스트에 연결하십시오.<br/>
   ```
   iscsiadm -m node -T [output from previous command, starting with IQN.] -p [IP address in StorageLayer] -l
   ```
   {: pre}

8. iSCSI 서비스를 다시 시작하십시오. `node.startup`이 `iscsid.conf`에서 자동으로 설정되어 있으므로 대상 호스트에 자동으로 로그인됩니다.<br/>
   ```
   systemctl restart iscsi.service
   ```
   {: pre}

---

copyright:
  years: 2017, 2018
lastupdated: "2018-06-27"

---
{:new_window: target="_blank"}

# Windows에서 iSCSI Software Initiator를 사용하여 DTS 디바이스에 연결

Windows에서 iSCSI LUN과 상호작용하려면 사용자가 Microsoft의 전용 iSCSI 도구인 iSCSI Software Initiator를 사용하여 스토리지에 연결해야 합니다. Windows Server 2008 또는 Windows Vista 이상 버전의 사용자의 경우, iSCSI Software Initiator가 운영 체제에 내장되어 있습니다. Windows Server 2003, Windows XP 및 Windows 2000의 사용자는 이 프로시저를 시작하기 전에 Initiator를 다운로드해야 합니다.

## iSCSI LUN에 연결

1. {{site.data.keyword.slportal}}에서 연결하고자 하는 스토리지 디바이스의 **iSCSI 사용자 이름, 비밀번호 및 스토리지 주소**를 검색하십시오.
2. iSCSI Initiator를 시작하십시오.
3. **구성** 탭에서 {{site.data.keyword.slportal}}의 IQN 데이터로 초기자 이름을 업데이트하십시오.
4. **검색**을 클릭하십시오.
5. **대상 포털** 섹션에서 **추가**를 클릭하십시오.
6. **IP 주소 또는 DNS 이름** 필드에 **iSCSI IP 주소**를 입력하십시오.
7. **고급**을 클릭하십시오.
8. iSCSI 로그온 정보를 업데이트하십시오.
   - **CHAP 로그온 정보 사용** 선택란을 선택하여 CHAP 로그온을 사용하십시오.
   - **사용자 이름** 필드에 iSCSI 사용자 이름을 입력하십시오.
   - **대상 암호** 필드에 iSCSI 비밀번호를 입력하십시오.
   - **확인**을 두 번 클릭하십시오.
9. **대상**을 클릭하십시오.
10. **대상** 목록에서 새로 추가된 iSCSI를 선택하십시오.
11. **로그온**을 클릭하십시오. **대상에 로그온** 창이 나타납니다.
12. **시스템 부팅 시 이 연결 자동 복원**을 선택하여 다시 시작하는 동안 연결이 유지되도록 설정하십시오.
13. **고급**을 클릭하십시오.
14. iSCSI 로그온 정보를 업데이트하십시오.
    - **CHAP 로그온 정보 사용** 선택란을 선택하여 CHAP 로그온을 사용하십시오.
    - **사용자 이름** 필드에 iSCSI 사용자 이름을 입력하십시오.
    - **대상 암호** 필드에 iSCSI 비밀번호를 입력하십시오.
    - **확인**을 두 번 클릭하십시오.
15. 새 iSCSI 대상이 대상 탭에 연결됨으로 표시되는지 확인하십시오.
    - iSCSI 대상이 **연결됨**으로 표시되면 **확인**을 클릭하십시오. iSCSI LUN이 이제 연결되었습니다.
    - iSCSI 대상이 **연결됨**으로 표시되지 않으면 모든 이전 단계를 반복하여 연결을 재설정하십시오.

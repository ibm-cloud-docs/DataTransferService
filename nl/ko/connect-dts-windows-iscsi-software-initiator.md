---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Windows에서 iSCSI Software Initiator를 사용하여 DTS 디바이스에 연결

Windows에서 iSCSI LUN과 상호작용하려면 Microsoft 독점 iSCSI 도구, iSCSI Software Initiator를 사용하여 LUN에 연결해야 합니다. Windows Server 2008 또는 Windows Vista 이상을 실행하는 사용자의 경우 iSCSI Software Initiator는 운영 체제에 빌드되어 있습니다. Windows Server 2003, Windows XP, Windows 2000을 실행하는 사용자는 이 프로시저를 완료하기 전에 Initiator를 다운로드해야 합니다. 아래 단계를 수행하여 Windows에서 iSCSI Software Initiator를 사용하여 iSCSI LUN에 연결합니다. 

## iSCSI LUN에 연결

1. 고객 포털에서 연결하는 iSCSI에 대한 **iSCSI 사용자 이름, 비밀번호, 스토리지 주소**를 검색하십시오. 데이터 전송 화면에 액세스를 참조하십시오. 
2. iSCSI Initiator를 실행하십시오. 
3. **구성** 탭에서 Initiator 이름을 SoftLayer 포털의 IQN 데이터로 업데이트하십시오. 
4. **발견** 탭을 클릭하십시오. 
5. 화면의 **대상 포털** 섹션에서 **추가** 단추를 클릭하십시오. 
6. **IP 주소 또는 DNS 이름** 필드에 **iSCSI IP 주소**를 입력하십시오. 
7. **고급** 탭을 클릭하십시오. 
8. iSCSI 로그온 정보를 업데이트하십시오. 
   - **CHAP 로그온 정보** 선택란을 선택하여 CHAP 로그온을 사용하십시오. 
   - **사용자 이름** 필드에 **iSCSI 사용자 이름**을 입력하십시오. 
   - **대상 시크릿** 필드에 **iSCSI 비밀번호**를 입력하십시오. 
   - **확인** 단추를 두 번 클릭하십시오. 
9. **대상** 탭을 클릭하십시오. 
10. **대상** 목록에서 새로 추가된 iSCSI를 선택하십시오. 
11. **로그온** 버튼을 클릭하십시오. **대상에 로그온** 팝업 메뉴가 나타납니다. 
12. **시스템 부팅 시 이 연결 자동 복원** 확인란을 선택하여 재부팅 사이에 연결을 지속하도록 설정하십시오. 
13. **고급** 단추를 클릭하십시오. 
14. iSCSI 로그온 정보를 업데이트하십시오. 
    - **CHAP 로그온 정보** 선택란을 선택하여 CHAP 로그온을 사용하십시오. 
    - **사용자 이름** 필드에 **iSCSI 사용자 이름**을 입력하십시오. 
    - **대상 시크릿** 필드에 **iSCSI 비밀번호**를 입력하십시오. 
    - **확인** 단추를 두 번 클릭하십시오. 
15. 새 iSCSI 대상이 대상 탭에 연결됨으로 표시되는지 확인하십시오. 

<table>
<tbody>
<tr>
<th>iSCSI 대상의 상태...</th><th>수행 작업...</th></tr>
<tr><td>연결됨으로 표시됨</td><td><strong>확인</strong> 단추를 클릭하십시오. 이제 iSCSI LUN이 연결됩니다. </td></tr>
<tr><td>연결됨으로 표시되지 않음</td><td>위 단계를 반복하여 연결을 재설정하십시오. </td></tr></tbody></table>

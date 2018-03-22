---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Windows での iSCSI ソフトウェア・イニシエーターを使用した DTS デバイスへの接続

Windows の iSCSI LUN と対話するには、ユーザーが Microsoft 専有の iSCSI ツールである iSCSI ソフトウェア・イニシエーターを使用して LUN に接続する必要があります。Windows Server 2008 または Windows Vista 以上を実行しているユーザーの場合、iSCSI ソフトウェア・イニシエーターはオペレーティング・システムに組み込まれています。Windows Server 2003、Windows XP、Windows 2000 を実行しているユーザーは、まずこのイニシエーターをダウンロードしてからこの手順を実行する必要があります。以下のステップに従って、Windows で iSCSI ソフトウェア・イニシエーターを使用して iSCSI LUN に接続します。

## iSCSI LUN への接続

1. カスタマー・ポータルから、接続しようとしている iSCSI に関する **iSCSI ユーザー名、パスワード、ストレージのアドレス**を取得します。「Access the Data Transfer Screen」を参照してください。
2. iSCSI イニシエーターを起動します。
3. **「構成」**タブ上のイニシエーター名を、SoftLayer ポータル内の IQN データに更新します。
4. **「ディスカバリー」**タブをクリックします。
5. 画面の**「ターゲット・ポータル (Target Portals)」**セクション内の**「追加」**ボタンをクリックします。
6. **「IP アドレスまたは DNS 名 (IP address or DNS name)」**フィールドで **iSCSI の IP アドレス**を入力します。
7. **「詳細」**タブをクリックします。
8. iSCSI ログオン情報を更新します。
   - **「CHAP ログオン情報 (CHAP logon information)」**チェック・ボックスを選択して、CHAP ログオンを有効にします。
   - **「ユーザー名」**フィールドで **iSCSI ユーザー名**を入力します。
   - **「ターゲットの機密事項 (Target secret)」**フィールドで **iSCSI パスワード**を入力します。
   - **「OK」**ボタンを 2 回クリックします。
9. **「ターゲット」**タブをクリックします。
10. **「ターゲット」**リストから新しく追加した iSCSI を選択します。
11. **「ログオン (Logon)」**ボタンをクリックします。**「ターゲットにログオン (Log On to Target)」**ポップ・アップ・メニューが表示されます。
12. **「システムのブート時にこの接続を自動的に復元する (Automatically restore this connection when the system boots)」**チェック・ボックスを選択して、リブートの合間に接続が持続するように設定します。
13. **「詳細」**ボタンをクリックします。
14. iSCSI ログオン情報を更新します。
    - **「CHAP ログオン情報 (CHAP logon information)」**チェック・ボックスを選択して、CHAP ログオンを有効にします。
    - **「ユーザー名」**フィールドで **iSCSI ユーザー名**を入力します。
    - **「ターゲットの機密事項 (Target secret)」**フィールドで **iSCSI パスワード**を入力します。
    - **「OK」**ボタンを 2 回クリックします。
15. 「ターゲット」タブで新しい iSCSI ターゲットが「接続済み」と表示されていることを確認します。

<table>
<tbody>
<tr>
<th>iSCSI ターゲットの状況</th><th>対応策</th></tr>
<tr><td>「接続済み」と表示される</td><td><strong>「OK」</strong>ボタンをクリックします。これで iSCSI LUN に接続されます。</td></tr>
<tr><td>「接続済み」と表示されない</td><td>上記のステップを繰り返して、接続をリセットします。</td></tr></tbody></table>

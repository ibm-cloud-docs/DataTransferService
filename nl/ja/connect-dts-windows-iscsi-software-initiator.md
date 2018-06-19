---

copyright:
  years: 2017, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Windows での iSCSI ソフトウェア・イニシエーターを使用した DTS デバイスへの接続

Windows で iSCSI LUN を操作するには、Microsoft 専有の iSCSI ツールである iSCSI ソフトウェア・イニシエーターを使用してストレージに接続する必要があります。Windows Server 2008 または Windows Vista 以上のユーザーの場合、iSCSI ソフトウェア・イニシエーターはオペレーティング・システムに組み込まれています。Windows Server 2003、Windows XP、Windows 2000 のユーザーは、まずこのイニシエーターをダウンロードしてからこの手順を開始する必要があります。

## iSCSI LUN への接続

1. {{site.data.keyword.slportal}}から、接続するストレージ・デバイスの **iSCSI ユーザー名、パスワード、ストレージ・アドレス**を取得します。
2. iSCSI イニシエーターを開始します。
3. **「構成」**タブでイニシエーター名を {{site.data.keyword.slportal}}の IQN データに更新します。
4. **「ディスカバリー」**をクリックします。
5. **「ターゲット・ポータル (Target Portals)」**セクションで**「追加 (Add)」**をクリックします。
6. **「IP アドレスまたは DNS 名 (IP address or DNS name)」**フィールドに **iSCSI の IP アドレス**を入力します。
7. **「詳細 (Advanced)」**をクリックします。
8. iSCSI ログオン情報を更新します。
   - **「CHAP ログオン情報 (CHAP logon information)」**チェック・ボックスを選択して、CHAP ログオンを有効にします。
   - **「ユーザー名」**フィールドに iSCSI ユーザー名を入力します。
   - **「ターゲット・シークレット (target secret)」**フィールドに iSCSI パスワードを入力します。
   - **「OK」**を 2 回クリックします。
9. **「ターゲット」**をクリックします。
10. **「ターゲット」**リストから新しく追加した iSCSI を選択します。
11. **「ログオン」**をクリックします。**「ターゲットにログオン (Log On to Target)」**ウィンドウが表示されます。
12. **「システムのブート時にこの接続を自動的に復元する (Automatically restore this connection when the system boots)」**チェック・ボックスを選択して、再始動しても接続が持続するように設定します。
13. **「詳細 (Advanced)」**をクリックします。
14. iSCSI ログオン情報を更新します。
    - **「CHAP ログオン情報 (CHAP logon information)」**チェック・ボックスを選択して、CHAP ログオンを有効にします。
    - **「ユーザー名」**フィールドに iSCSI ユーザー名を入力します。
    - **「ターゲット・シークレット (target secret)」**フィールドに iSCSI パスワードを入力します。
    - **「OK」**を 2 回クリックします。
15. 「ターゲット」タブで新しい iSCSI ターゲットが「接続済み」と表示されていることを確認します。
    - iSCSI ターゲットが**「接続済み」**と表示されたら、**「OK」**をクリックします。これで iSCSI LUN に接続されました。
    - iSCSI ターゲットが**「接続済み」**と表示されない場合は、上記のすべての手順をもう一度実行して接続を再設定します。

---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# 在 Windows 中使用 iSCSI Software Initiator 連接至 DTS 裝置

若要與 Windows 中的 iSCSI LUN 互動，使用者必須使用 iSCSI Software Initiator（Microsoft 專有的 iSCSI 工具）來連接至 LUN。對於執行 Windows Server 2008 或 Windows Vista 及更高版本的使用者，iSCSI Software Initiator 內建在作業系統中。執行 Windows Server 2003、Windows XP 及 Windows 2000 的使用者，則必須在完成此程序之前先下載啟動器。遵循下面的步驟，在 Windows 中使用 iSCSI Software Initiator 連接至 iSCSI LUN。

## 連接至 iSCSI LUN

1. 擷取 **iSCSI 使用者名稱、密碼及儲存空間位址**，用於從「客戶入口網站」連接的 iSCSI。請參閱「存取資料傳送畫面」。
2. 啟動「iSCSI 啟動器」。
3. 將**配置**標籤上的啟動器名稱更新為 SoftLayer 入口網站中的 IQN 資料。
4. 按一下**探索**標籤。
5. 按一下畫面的**目標入口網站**區段中的**新增**按鈕。
6. 在 **IP 位址或 DNS 名稱**欄位中，輸入 **iSCSI IP 位址**。
7. 按一下**進階**標籤。
8. 更新 iSCSI 登入資訊。
   - 選取 **CHAP 登入資訊**勾選框，以啟用 CHAP 登入。
   - 在**使用者名稱**欄位中，輸入 **iSCSI 使用者名稱**。
   - 在**目標密碼**欄位中，輸入 **iSCSI 密碼**。
   - 按兩次**確定**按鈕。
9. 按一下**目標**標籤。
10. 從**目標**清單中，選取最近新增的 iSCSI。
11. 按一下**登入**按鈕。即會出現**登入目標**蹦現功能表。
12. 選取**系統啟動時自動還原此連線**勾選框，以設定在重新開機之間持續保持連線。
13. 按一下**進階**按鈕。
14. 更新 iSCSI 登入資訊。
    - 選取 **CHAP 登入資訊**勾選框，以啟用 CHAP 登入。
    - 在**使用者名稱**欄位中，輸入 **iSCSI 使用者名稱**。
    - 在**目標密碼**欄位中，輸入 **iSCSI 密碼**。
    - 按兩次**確定**按鈕。
15. 驗證在「目標」標籤上新的 iSCSI 目標顯示為「已連接」。

<table>
<tbody>
<tr>
<th>如果 iSCSI 目標…</th><th>則...</th></tr>
<tr><td>顯示為「已連接」</td><td>按一下<strong>確定</strong>按鈕。您的 iSCSI LUN 現在已連接。</td></tr>
<tr><td>未顯示為「已連接」</td><td>重複上述步驟，以重設連線。</td></tr></tbody></table>

---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:new_window: target="_blank"}

# 開始使用資料傳送服務
{: #gettingstarted}

客戶可以使用 {{site.data.keyword.BluSoftlayer_full}} 資料傳送服務，將 USB 2.0 或 3.0 相容裝置、CD 和 DVD 傳送至 {{site.data.keyword.BluSoftlayer}} 資料中心。他們的裝置會直接連接至網路，以便遠端控制資料傳送。此裝置安裝在位於客戶資料中心內的專用機架中，並作為 iSCSI 目標裝載。當您需要在不使用 {{site.data.keyword.BluSoftlayer}} 專用網路的情況下傳送大量資料時，資料傳送服務非常理想，而且這個服務免費提供給所有 {{site.data.keyword.BluSoftlayer}} 客戶。

## 存取資料傳送服務畫面

**附註**：只有帳戶的主要使用者才能使用此畫面。

1. 用您的唯一認證存取 [{{site.data.keyword.slportal}} ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){:new_window}。
2. 從「導覽列」中，選取**儲存空間** > **資料移轉** > **資料傳送**，以存取「資料傳送服務」畫面。<br/>

在**資料傳送服務**畫面上，使用者可提交資料傳送要求、檢視要求的詳細資料、檢視與裝置追蹤相關聯的問題單歷程，以及取消現有的要求。

## 提交資料傳送要求

資料傳送要求旨在讓資料中心內的相關方知道期望來自用戶端的出貨。要求是透過 [{{site.data.keyword.slportal}} ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){:new_window} 提出。

建立要求時，請牢記下列準則。

- 確保您要傳送的裝置符合所有[硬體需求](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html)。
- 一個要求只能有一台相關聯的裝置。如果您要傳送多台裝置，則必須為每一台裝置建立一個新要求。
- 如果要運回裝置，請在包裝中提供已預付款的運送標籤，並視需要提供出口文件，讓裝置可以在傳送期限後運回。
- 如果在國際間運送裝置，您要負責取得「裝置」的所有授權、出貨及清關。您負責的部分包括支付任何關稅、稅款及 {{site.data.keyword.BluSoftlayer}} 資料中心的進出貨成本（適用時）。
- 在完成要求時，您需要提供運送到資料中心之貨物的承運人名稱以及追蹤號碼。在提交資料傳送要求之前，請先建立含有適當資料中心地址的出貨標籤。

請遵循這些步驟，以提交資料傳送要求。

1. 存取 [{{site.data.keyword.slportal}} ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){:new_window} 中的**資料傳送服務**畫面。
2. 按一下**訂購資料傳送要求**。
3. 根據表 1，完成**裝置資訊**區段中的每一個欄位。
<table border="1">
<caption>表 1 在左側列出要求表單中的欄位名稱，並在右側列出其說明。</caption>
 <tr><th>欄位名稱</th><th>指示</th></tr>
 <tr><td>裝置類型</td><td>傳送至目的地的裝置類型。如果裝置類型未列出，請選取「其他」。</td></tr>
 <tr><td>序號</td><td> 裝置的序號。</td></tr><tr><td>說明</td><td>裝置的簡要說明。要包括的重要詳細資料可為識別因素，例如顏色、標籤或貼紙。</td></tr>
 <tr><td>附註</td><td>任何關於裝置或傳送的其他附註。</td></tr><tr><td>目的地</td><td>將接收裝置的資料中心。</td></tr>
 <tr><td>承運人</td><td>用來將裝置運送到目的地的郵政或快遞公司。</td></tr>
 <tr><td>追蹤號碼</td><td>出貨的完整追蹤號碼。</td></tr>
 </table>

4. 完成**運回地址**區段中的每一個欄位，或選取**公司地址**勾選框，自動將檔案中的公司地址移入欄位中。<br/> **附註**：請記得在包裝中包含預付運回標籤及任何所需的出口文件。
5. 閱讀完服務合約之後，請選取**我已閱讀並同意「資料傳送服務合約」及「主要服務合約」**勾選框。
6. 按一下**提交服務要求**。

在提交要求之後，要求問題單的狀態會呈現為`傳送至 SoftLayer`。如果任何進出口貨物需要當地政府的授權，請通知 {{site.data.keyword.BluSoftlayer}}，並在問題單上附加授權資訊。

收到裝置之後，狀態會更新為`由 SoftLayer 接收`。在資料中心技術人員將裝置連接至網路之後，問題單狀態會再次更新為`已連接`。

起始資料傳送期間為兩週。在此期間，只授權帳戶管理者存取裝置。如果您需要更多時間，可以要求延長。同樣地，如果您想要裝置在兩週之內運回，也可以要求運回。在傳送已完成時，您必須透過 [{{site.data.keyword.slportal}}](https://control.softlayer.com/) 通知 {{site.data.keyword.IBM}}。然後，{{site.data.keyword.BluSoftlayer}} 會拆卸「裝置」，並根據您的要求將它運回或銷毀。


## 存取出貨畫面

[{{site.data.keyword.slportal}} ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){:new_window} 內的「出貨」畫面會顯示所有與資料傳送服務要求相關聯的出貨。從這個畫面中，您可以檢視出貨，並且可以確認收到運回的貨物。

若要存取「出貨」畫面，請執行下列動作：

1. 用您的唯一認證存取 [{{site.data.keyword.slportal}} ![外部鏈結圖示](../../icons/launch-glyph.svg "外部鏈結圖示")](https://control.softlayer.com/){:new_window}。
2. 從「導覽列」中，選取**帳戶** > **管理** > **出貨**。

在「出貨」畫面上，會顯示過去 30 天內的所有出貨要求及其詳細資料。出貨可依狀態、經歷時間或特定出貨詳細資料進行[排序或過濾](sort-or-filter-shipments-list.html)。此外，您也可以在此畫面上確認收到運回的貨物。
![出貨畫面](/images/DTSShipmentScreen1.png)
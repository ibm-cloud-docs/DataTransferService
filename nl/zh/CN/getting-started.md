---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:new_window: target="_blank"}

# 开始使用数据传输服务
{: #gettingstarted}

客户可以使用 {{site.data.keyword.BluSoftlayer_full}} 数据传输服务将 USB 2.0 或 USB 3.0 兼容设备、CD 和 DVD 发往 {{site.data.keyword.BluSoftlayer}} 数据中心。这样，客户的设备可直接连接到其网络，从而可远程控制数据传输。设备将安装在客户数据中心的专用机架中，并作为 iSCSI 目标安装。当您需要传输大量数据但不使用 {{site.data.keyword.BluSoftlayer}} 的专用网络时，数据传输服务是您理想的选择，且该服务对所有 {{site.data.keyword.BluSoftlayer}} 客户免费提供。

## 访问数据传输服务屏幕

**注**：此屏幕仅供帐户的主用户使用。

1. 使用您的唯一凭证来访问 [{{site.data.keyword.slportal}} ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/){:new_window}。
2. 从导航栏中选择**存储** > **数据迁移** > **数据传输**，以访问“数据传输服务”屏幕。<br/>

在**数据传输服务**屏幕上，用户可以提交数据传输请求，查看请求的详细信息，查看与设备跟踪关联的凭单历史记录以及取消现有请求。

## 提交数据传输请求

数据传输请求旨在让我们数据中心的相应当事方了解有客户发来的设备。请求会通过 [{{site.data.keyword.slportal}} ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/){:new_window} 进行提交。

创建请求时，请记住以下准则。

- 确保要发送的设备满足所有[硬件需求](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html)。
- 一个请求只能与一个设备相关联。如果要发送多个设备，必须为每个设备创建一个新请求。
- 如果要退回设备，请根据需要在包裹中提供预付的装运标签和出口单据，以使设备可在传输周期结束后退回。
- 如果是国际发运设备，您负责获取设备的所有许可、装运和清关。您的责任包括支付任何关税、税费以及运送到 {{site.data.keyword.BluSoftlayer}} 数据中心和从数据中心运回（如果适用）的运输成本。
- 填写请求时，您需要提供发往数据中心的货物承运方的名称和跟踪号。在提交数据传输请求之前，创建包含相应的数据中心地址的装运标签。

执行以下步骤来提交数据传输请求。

1. 访问 [{{site.data.keyword.slportal}} ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/){:new_window} 中的**数据传输服务**屏幕。
2. 单击**订购数据传输请求**。
3. 根据表 1 填写**设备信息**部分中的每个字段。
<table border="1">
<caption>表 1 左侧列出请求表单上的字段名称，右侧列出其描述。</caption>
 <tr><th>字段名称</th><th>指示信息</th></tr>
 <tr><td>设备类型</td><td>要发往目的地的设备类型。如果未列出设备类型，请选择“其他”。</td></tr>
 <tr><td>序列号</td><td> 设备的序列号。</td></tr><tr><td>描述</td><td>设备的简短描述。包含的重要详细信息可以是识别因素，如颜色、标签或标贴。</td></tr>
 <tr><td>注释</td><td>有关设备或运输的其他任何注释。</td></tr><tr><td>目的地</td><td>要接收设备的数据中心。</td></tr>
 <tr><td>承运方</td><td>用于将设备运输到其目的地的邮政或快递承运方。</td></tr>
 <tr><td>跟踪号</td><td>货物的完整跟踪号。</td></tr>
 </table>

4. 填写**退回地址**部分中的每个字段，或选中**公司地址**复选框以使用存档的公司地址自动填充各字段。<br/> **注**：请记住在包裹中包含预付的退回标签和任何所需的出口单据。
5. 阅读服务协议后，选中**我已阅读并同意数据传输服务协议和主服务协议**复选框。
6. 单击**提交服务请求**。

提交请求后，请求凭单的状态将显示为`已发往 SoftLayer`。如果任何进口或出口装运需要当地政府的许可，请通知 {{site.data.keyword.BluSoftlayer}}，并在凭单中附加许可信息。

在收到设备后，状态将更新为 `SoftLayer 已接收`。在数据中心技术人员将设备连接到网络后，凭单状态将再次更新为`已连接`。

初始数据传输周期为 2 周。在此期间，仅帐户管理员有权访问该设备。如果需要更多时间，您可以请求延期。另外，如果想要在两周内就发回设备，可请求退回。传输完成后，您必须通过 [{{site.data.keyword.slportal}}](https://control.softlayer.com/) 通知 {{site.data.keyword.IBM}}。然后，{{site.data.keyword.BluSoftlayer}} 会断开设备的连接，并根据您的请求将其退回或销毁。


## 访问装运屏幕

[{{site.data.keyword.slportal}} ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/){:new_window} 中的“装运”屏幕会显示与数据传输服务请求相关联的所有装运。您可以从此屏幕查看装运并且可在回执上确认退货装运。

要访问“装运”屏幕：

1. 使用您的唯一凭证来访问 [{{site.data.keyword.slportal}} ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](https://control.softlayer.com/){:new_window}。
2. 从导航栏中选择**帐户** > **管理** > **装运**。

在“装运”屏幕上，会显示过去 30 天内的所有装运请求及其详细信息。您可按状态、时限或特定装运详细信息对装运进行[排序或过滤](sort-or-filter-shipments-list.html)。此外，您可以在此屏幕中确认已收到退回的装运。![“装运”屏幕](/images/DTSShipmentScreen1.png)

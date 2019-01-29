---

copyright:
  years: 1994, 2018
lastupdated: "2018-11-05"

---
{:faq: data-hd-content-type='faq'}

# 常见问题

## 什么是数据传输？
{: faq}

此服务允许授权用户（通常是帐户的管理员）将兼容设备发往其中一个 {{site.data.keyword.BluSoftlayer_full}} 数据中心，以使其直接与帐户网络连接。设备将安装在专用机架中，并作为 iSCSI 目标安装两周。在此期间，管理员可以在网络上访问该设备，以与帐户上的其他设备和服务一起使用。两周后，可能需要请求延期，才能使该设备保持与网络的连接。否则，我们会将设备退回至请求中指定的当事方；或者就地销毁设备。

## 用于数据传输的设备可国际运送吗？
{: faq}

硬件和光盘均可国内或国际运送到任一 {{site.data.keyword.BluSoftlayer}} 数据中心。但是您作为客户需要负责：

- 确保无需进口或出口许可即可将设备运输到 {{site.data.keyword.IBM}} 数据中心，否则设备会退回给客户（如果适用）；
- 确保内容中包含其数据的客户或任何客户用户，均不受美国政府的撤销或拒绝其美国出口特权的任何命令的限制。如果贵企业或任何此类用户受任何此类命令的限制，您必须立即通知 {{site.data.keyword.IBM}}；
- 获取设备的所有许可、装运和清关，包括支付任何关税、税费以及运送到 {{site.data.keyword.IBM}} 数据中心和从数据中心运回（如果适用）的运输成本；
- 遵守所有适用法律，包括隐私法、与交付和退回设备关联的进出口法，以及将内容传输到 {{site.data.keyword.IBM}} 数据中心的相关法律；以及
- 与客户的用户就客户传输到硬件的任何用户数据签订相应协议，并获取所有必需许可权。

请在装运中包含预付的退回装运标签和所有相应的出口单据。{{site.data.keyword.BluSoftlayer}} 将使用您提供的标签和单据来包装设备进行退回。如果未请求退回，将销毁设备。


## 可以利用数据传输请求发送哪些类型的设备？
{: faq}

选择数据传输所需提交的设备或光盘（CD 或 DVD）时，请使用以下准则：

- **硬件需求**

   - 电源必须兼容 208 伏/220 伏。

   - 电源插头必须匹配标准 120 伏插座 (NEMA 5-15P)。

   - 设备必须兼容 USB 2.0 或 USB 3.0。

   - 提供 USB A 公头接口（匹配大部分计算机的标准 USB 插头）。

- **CD/DVD 需求**

   - 光盘必须装在 CD 包、包装盒或类似容器中进行提交。如果要提交多张光盘，请将所有光盘存放在一个包装盒或 CD 包中。

   - 必须清晰且唯一标记每张光盘。

## 能否更快地退回设备或者保留超过 2 周？
{: faq}

可以，如果需要，您的硬件或光盘可随时退回，也可以保持连接更长时间。要请求延期退回，请在原始数据传输请求凭单上添加注释，在其中包含相应的请求。如果请求退回，{{site.data.keyword.BluSoftlayer}} 将断开硬件或光盘的连接，并使用您提供的预付装运标签和包装将硬件或光盘退回到在原始请求中提供的退回地址。

如果请求延期，我们将尽快处理延期请求。请务必注意，每次延期请求可使设备连接时间延长一周，且可能会产生延期费用。{{site.data.keyword.BluSoftlayer_full}} 团队成员答复原始凭单中的请求时，会包含更多详细信息。

数据传输凭单上的各个状态指示提交到数据中心的硬件或光盘的传输过程中的各阶段。请参阅下表以获取有关每个状态的特定详细信息：

|状态|定义
|
|---------| -----------|
|`已发往 SoftLayer`|用户提交了数据传输请求，硬件或光盘正在运往所选数据中心。|
|`SoftLayer 已接收`|	数据中心已收到货，为设备分配了序列号，并已扫描进 {{site.data.keyword.BluSoftlayer}} 系统。|
|`连接`|	硬件或光盘与设备连接。|
|`已连接` |	为设备创建 iSCSI 目标。|
|`请求延期`| 客户已请求在两周连接时间的基础上延期。|
|`请求退回`| 客户已请求退回硬件或光盘。|
|`断开连接`|	已启动断开硬件或光盘的连接。|
|`已断开连接`|	已安全拆离目标。|
|`已销毁`| 设备已根据 {{site.data.keyword.BluSoftlayer}} HDD 销毁过程就地销毁。|
|`SoftLayer 退回`|	硬件或光盘已打包，并运往原始请求中提供的退回地址。|
---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# 使用 iSCSI Software Initiator 连接到 Windows 中的 DTS 设备

要与 Windows 中的 iSCSI LUN 进行交互，用户必须使用 iSCSI Software Initiator（Microsoft 的专有 iSCSI 工具）来连接到该 LUN。对于运行 Windows Server 2008 或 Windows Vista 及更高版本的用户，iSCSI Software Initiator 构建于操作系统内。运行 Windows Server 2003、Windows XP 和 Windows 2000 的用户必须先下载该 Initiator，然后再完成此过程。执行以下步骤来使用 iSCSI Software Initiator 连接到 Windows 中的 iSCSI LUN。

## 连接到 iSCSI LUN

1. 检索从客户门户网站连接的 iSCSI 的 **iSCSI 用户名、密码和存储地址**。请参阅“访问数据传输屏幕”。
2. 启动 iSCSI 启动器。
3. 将**配置**选项卡上的启动器名称更新为 SoftLayer 门户网站中的 IQN 数据。
4. 单击**发现**选项卡。
5. 单击屏幕上**目标门户网站**部分中的**添加**按钮。
6. 在 **IP 地址或 DNS 名称**字段中，输入 **iSCSI IP 地址**。
7. 单击**高级**选项卡。
8. 更新 iSCSI 登录信息。
   - 选中 **CHAP 登录信息**复选框以启用 CHAP 登录。
   - 在**用户名**字段中输入 **iSCSI 用户名**。
   - 在**目标私钥**字段中输入 **iSCSI 密码**。
   - 单击**确定**按钮两次。
9. 单击**目标**选项卡。
10. 从**目标**列表中选择新添加的 iSCSI。
11. 单击**登录**按钮。此时将显示**登录到目标**弹出菜单。
12. 选中**系统启动时自动还原此连接**复选框，以设置在重新启动时保持连接。
13. 单击**高级**按钮。
14. 更新 iSCSI 登录信息。
    - 选中 **CHAP 登录信息**复选框以启用 CHAP 登录。
    - 在**用户名**字段中输入 **iSCSI 用户名**。
    - 在**目标私钥**字段中输入 **iSCSI 密码**。
    - 单击**确定**按钮两次。
15. 验证“目标”选项卡上新的 iSCSI 目标显示为“已连接”。

<table>
<tbody>
<tr>
<th>如果 iSCSI 目标...</th><th>那么...</th></tr>
<tr><td>显示为“已连接”</td><td>单击<strong>确定</strong>按钮。现在，已连接您的 iSCSI LUN。</td></tr>
<tr><td>未显示为“已连接”</td><td>重复上述步骤以重置连接。</td></tr></tbody></table>

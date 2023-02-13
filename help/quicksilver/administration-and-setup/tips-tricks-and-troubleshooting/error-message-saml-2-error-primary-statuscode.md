---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: “错误消息：SAML 2.0错误：Primary StatusCode'
description: 无法成功建立与ADFS的连接。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# 错误消息：SAML 2.0错误：主状态代码

## 问题

无法成功建立与ADFS的连接。

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>如果您成功建立了测试连接，但仍然遇到问题，则可能存在不正确的属性映射或联合ID问题。 如有问题，请联系客户支持。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 原因1:安全哈希算法设置为SHA-256

### 解决方案

1. 在Windows中，单击 **[!UICONTROL 开始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**.\
   将显示ADFS 2.0管理对话框。

1. 选择 **[!UICONTROL 信任关系]** > **[!UICONTROL 信赖方信托]** 在左窗格中。

1. 右键单击与 [!DNL Adobe Workfront]，然后选择 **[!UICONTROL 属性]**.
1. 单击 **[!UICONTROL 高级]** 选项卡，然后选择 **[!UICONTROL SHA-1]** 从 **[!UICONTROL 安全哈希算法]** 下拉菜单。\
   ![](assets/1-350x287.png)

## 原因2:ADFS签名证书即将过期，并已替换为日期重叠的新证书

### 解决方案

的 [!DNL Workfront] “SSO设置”页列出证书过期日期。 如果证书即将过期，您需要从ADFS服务器中手动提取新签名证书：

1. 在Windows中，单击 **[!UICONTROL 开始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**.\
   将显示ADFS 2.0管理对话框。

1. 选择 **[!UICONTROL 信任关系]** > **[!UICONTROL 信赖方信托]** 在左窗格中。

1. 右键单击与 [!DNL Workfront]，然后选择 **[!UICONTROL 属性]**.
1. 单击 **[!UICONTROL 签名]** 选项卡。
1. 单击签名证书的名称，然后单击 **[!UICONTROL 查看]**.
1. 单击复制到 **[!UICONTROL 文件]**...，然后选择 **[!UICONTROL 下一个]**.

1. 选择 **[!UICONTROL Base-64编码x.509(CER)]**，然后单击 **[!UICONTROL 下一个]**.

1. 指定文件名，然后单击 **[!UICONTROL 下一个]**.
1. 单击 **[!UICONTROL 完成]**.
1. 在 [!DNL Workfront]，导航到 **[!UICONTROL 设置]** > **[!UICONTROL 系统]** > **[!UICONTROL 单点登录(SSO)]** 和手动上传签名证书。

## 原因3:证书吊销检查失败

解决方案取决于 [!DNL Microsoft] 您使用的ADFS。 咨询 [!DNL Microsoft]的文档，以获取适合您版本的相应命令。

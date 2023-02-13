---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: “错误消息：无法验证XML数字签名”
description: 无法成功建立与ADFS的连接。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# 错误消息：无法验证XML数字签名

## 问题

无法成功建立与ADFS的连接。

![error_message.png](assets/error-message.png)

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

## 原因1:证书不正确

### 解决方案

从ADFS服务器手动检索签名证书：

1. 在 [!DNL Windows]，单击 **[!UICONTROL 开始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**.\
   将显示ADFS 2.0管理对话框。

1. 选择 **[!UICONTROL 信任关系]** > **[!UICONTROL 信赖方信托]** 在左窗格中。

1. 右键单击 **[!UICONTROL 信赖方信任]**，然后选择 **[!UICONTROL 属性]**.

1. 单击 **[!UICONTROL 签名]** 选项卡。
1. 单击签名证书的名称，然后单击 **[!UICONTROL 查看]**.
1. 单击复制到 **[!UICONTROL 文件]**...，然后选择 **[!UICONTROL 下一个]**.

1. 选择 **[!UICONTROL Base-64编码x.509(CER)]**，然后单击 **[!UICONTROL 下一个]**.

1. 指定文件名，然后单击 **[!UICONTROL 下一个]**.
1. 单击 **[!UICONTROL 完成]**.
1. 在 [!DNL Adobe Workfront]，导航到 **[!UICONTROL 设置]** > **[!UICONTROL 系统]** > **[!UICONTROL 单点登录(SSO)]** 和手动上传签名证书。

## 原因2:当 [!DNL Workfront] 需要RSA签名

### 解决方案

重新创建证书并使用RSA签名而不是DSA。

## 原因3:XML数据不正确

### 解决方案

从ADFS管理系统中重新导出和重新导入XML元数据。

## 原因4:由于SAML端出错，无法执行请求

### 解决方案

联系您的SAML提供程序。

---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: “错误消息：无法验证XML数字签名”
description: 无法成功建立与ADFS的连接。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 1%

---

# 错误消息：无法验证XML数字签名

## 问题

无法成功建立与ADFS的连接。

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>如果成功建立了测试连接，但仍遇到问题，则属性映射可能不正确，或者联合ID出现问题。 如有疑问，请联系客户支持。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>
   <p>新增：标准</p>
   <p>或</p>
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>您必须是[!DNL Workfront]管理员。 </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 原因1：证书不正确

### 解决方案

从ADFS服务器手动检索签名证书：

1. 在[!DNL Windows]中，单击&#x200B;**[!UICONTROL 开始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**。\
   将显示“ADFS 2.0管理”对话框。

1. 在左侧窗格中选择&#x200B;**[!UICONTROL 信任关系]** > **[!UICONTROL 信赖方信任]**。

1. 右键单击&#x200B;**[!UICONTROL 信赖方信任]**，然后选择&#x200B;**[!UICONTROL 属性]**。

1. 单击&#x200B;**[!UICONTROL 签名]**&#x200B;选项卡。
1. 单击签名证书的名称，然后单击&#x200B;**[!UICONTROL 查看]**。
1. 单击“复制到&#x200B;**[!UICONTROL 文件]**...”，然后选择&#x200B;**[!UICONTROL 下一步]**。

1. 选择&#x200B;**[!UICONTROL Base-64编码的x.509 (CER)]**，然后单击&#x200B;**[!UICONTROL 下一步]**。

1. 指定文件名，然后单击&#x200B;**[!UICONTROL 下一步]**。
1. 单击&#x200B;**[!UICONTROL 完成]**。
1. 在[!DNL Adobe Workfront]中，导航到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 系统]** > **[!UICONTROL 单点登录(SSO)]**&#x200B;并手动上传签名证书。

## 原因2：当[!DNL Workfront]需要RSA签名时，使用DSA对证书签名

### 解决方案

重新创建证书并使用RSA签名而不是DSA。

## 原因3： XML数据不正确

### 解决方案

从ADFS管理系统重新导出和重新导入XML元数据。

## 原因4：由于SAML端出错，无法执行请求

### 解决方案

请联系您的SAML提供商。

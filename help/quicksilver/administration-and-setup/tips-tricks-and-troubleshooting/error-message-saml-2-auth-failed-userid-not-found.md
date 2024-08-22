---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: “错误消息： SAML 2.0身份验证失败：未找到用户标识符”
description: 使用SAML 2.0时，出现“SAML 2.0身份验证失败 — 用户标识符未找到”错误，表示未从ADFS声明规则传递UID或名称ID。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 错误消息： SAML 2.0身份验证失败：未找到用户标识符

## 问题

我在使用SAML 2.0时收到此错误：“SAML 2.0身份验证失败：未找到用户标识符。”

## 原因

当未从&#x200B;**ADFS声明规则**&#x200B;传递&#x200B;**UID**&#x200B;或&#x200B;**名称ID**&#x200B;时，会发生这种情况。

在ADFS中，**信赖方信任**&#x200B;需要有一个传递&#x200B;**UID**&#x200B;或&#x200B;**名称ID**&#x200B;值的&#x200B;**声明规则**。 当您运行&#x200B;**[!DNL Workfront]测试连接**&#x200B;时，如果成功，它将显示此连接。

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

## 解决方案

1. 编辑&#x200B;**[!UICONTROL ADFS信息]**&#x200B;时，在&#x200B;**[!UICONTROL 信赖方信任]** >选择对象>**[!UICONTROL 编辑声明规则]**&#x200B;中。

1. **[!UICONTROL LDAP属性]** （左列）应具有&#x200B;**[!UICONTROL 电子邮件地址]** （或任何唯一标识符）。

1. **[!UICONTROL 传出声明类型]** （右列）应为&#x200B;**[!UICONTROL 名称ID]**。

   >[!NOTE]
   >
   >它不必具有LDAP属性电子邮件地址。 可以使用任何标识用户的唯一标识符，但必须将其作为&#x200B;**NAME ID**&#x200B;传递到[!DNL Adobe Workfront]。

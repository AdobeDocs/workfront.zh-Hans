---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 访问级别中缺少外部用户许可证类型
description: 我在“设置”中的访问级别下无法再看到外部用户许可证类型。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: fcc876d9-0512-424a-a731-6bbacd55af3f
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 1%

---

# 访问级别中缺少外部用户许可证类型

## 问题

我在“设置”中的访问级别下无法再看到外部用户许可证类型。

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

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 系统]** > **[!UICONTROL 首选项]**。

1. 在&#x200B;**[!UICONTROL 安全性]**&#x200B;部分中，确保启用了选项&#x200B;**[!UICONTROL 通过使用没有Workfront帐户的人员的电子邮件地址与其协作]**。

   如果未启用此选项，则外部用户不会出现在访问级别设置中。

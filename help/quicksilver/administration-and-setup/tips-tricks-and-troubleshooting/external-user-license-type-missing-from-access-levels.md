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
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 2%

---

# 访问级别中缺少外部用户许可证类型

## 问题

我在“设置”中的访问级别下无法再看到外部用户许可证类型。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>[!UICONTROL 系统管理员]</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 解决方案

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 系统]** > **[!UICONTROL 首选项]**。

1. 在&#x200B;**[!UICONTROL 安全性]**&#x200B;部分中，确保启用了选项&#x200B;**[!UICONTROL 通过使用没有Workfront帐户的人员的电子邮件地址与其协作]**。

   如果未启用此选项，则外部用户不会出现在访问级别设置中。

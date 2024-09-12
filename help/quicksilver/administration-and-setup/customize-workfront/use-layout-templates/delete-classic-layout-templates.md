---
title: 删除经典布局模板
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: 经典 Workfront 体验中的布局模板在 Workfront 界面中不再可用，但仍可能会影响 Workfront 数据。这可能会导致报告或仪表板上受布局模板影响的字段（如“共享对象”）中出现不一致。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c6d33d5d-da93-4aba-8897-f177c1171595
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 51%

---

# 授予对布局模板的管理访问权限

经典 Workfront 体验中的布局模板在 Workfront 界面中不再可用，但仍可能会影响 Workfront 数据。这可能会导致报告或仪表板上受布局模板影响的字段（如“共享对象”）中出现不一致。

您可以通过删除传统布局模板来解决这些不一致问题。 由于它们在Workfront界面中不可用，因此使用必须使用Workfront API来删除它们。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td><p>新增：标准</p>
  <p> 当前：计划</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。
要为组执行这些操作，您必须是该组的经理。</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用API调用删除经典布局模板

您可以在浏览器的URL栏中输入API调用，然后按Enter。 API响应会显示在您的浏览器中。

>[!NOTE]
>
>无法删除全局和系统布局模板。

1. 登录到Workfront。
1. 使用以下 API 调用找到要删除的布局模板：
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. 记下要删除的布局模板的 ID。
1. 使用以下 API 调用找到您的会话 ID：
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >请勿与任何人分享您的会话 ID。

1. 将布局模板 ID 和会话 ID 插入到以下 API 调用中：
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. 将第 4 步中的 API 调用粘贴到浏览器的 URL 栏中，然后按 Enter。

   这样将删除该布局模板。

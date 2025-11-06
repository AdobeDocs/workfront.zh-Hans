---
title: 重置用户的首选项
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作为Adobe Workfront管理员，您可以重置或删除Workfront系统中任何用户的用户首选项设置。 个人用户也可以重置自己的用户首选项设置。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: f1fe1a2fe6e123d8a039e8d7e3547c0b0a8141df
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 3%

---

# 重置用户的首选项

<!-- Audited: 12/2023 -->

作为Adobe Workfront管理员，您可以重置或删除Workfront系统中任何用户的用户首选项设置。

个人用户也可以重置自己的用户首选项设置。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>系统管理员</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 关于受影响的设置

重置用户首选项时，某些首选项将恢复为系统默认值，而其他首选项将清除或删除：

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preference</strong> </th> 
   <th><strong>Status after the reset</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Views</td> 
   <td> <p> Reverted to the system default</p> <p>Existing views are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Reverted to the system default</p> <p>Existing filters are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupings</td> 
   <td> <p>Reverted to the system default</p> <p>Existing groupings are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Recent Items list</td> 
   <td>Cleared</td> 
  </tr> 
  <tr> 
   <td>Favorites list</td> 
   <td>Unaffected</td> 
  </tr> 
  <tr> 
   <td>User Preferences</td> 
   <td> <p>Reverted to the system default</p> <p>Email notifications revert to the system defaults. The default notifications are listed in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Event notifications available in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User-Defined Custom Tabs</td> 
   <td>Removed</td> 
  </tr> 
  <tr> 
   <td>User-Defined Global Navigation Options</td> 
   <td>Set back to layout template definition, or system default if no layout template is assigned.</td> 
  </tr> 
 </tbody> 
</table>
-->

<!--Display this table and hide the HTML table above, when the unshim is released.-->

| 首选项 | 重置后的状态 |
| --- | --- |
| 视图 | 已还原为系统默认值 <p>不会删除现有视图。 您可以再次选择它们。</p> |
| 过滤器 | 已还原为系统默认值 <p>不会删除现有筛选器。 您可以再次选择它们。</p> |
| 分组 | 已还原为系统默认值 <p>现有分组不会被删除。 您可以再次选择它们。</p> |
| 最新项目列表 | 已清除 |
| 收藏夹列表 | 未受影响 |
| 用户首选项 | 已还原为系统默认值 <p>电子邮件通知将还原为系统默认值。 默认通知列在Adobe Workfront[中可用的](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)事件通知中。</p> |

## 重置用户首选项

{{step-1-to-setup}}

1. 选择&#x200B;**登录身份**。
1. 开始键入要重置其首选项的用户名，然后在名称出现在下拉列表中时单击该名称。
1. 选择&#x200B;**登录**。
1. 如果贵组织尚未载入Adobe Unified Experience，请按照以下步骤操作：

   * 在Web浏览器顶部的URL字段中，在`/resetUser`之后添加`workfront.com`。

     >[!NOTE]
     >
     >这区分大小写。 U必须大写，其余字符必须为小写。 例如：
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. 如果您的组织已载入到Adobe Unified Experience，请按照以下步骤操作：

   * 在Web浏览器顶部的URL字段中，在`/resetUser`之后添加`workfront`。

     >[!NOTE]
     >
     >这区分大小写。 U必须大写，其余字符必须为小写。 例如：
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. 按&#x200B;**Enter**。

1. 要重置所有用户首选项，请单击&#x200B;**重置**。

   或

   要将用户的左侧导航重置为原始布局模板配置，请单击&#x200B;**重置左侧导航**。

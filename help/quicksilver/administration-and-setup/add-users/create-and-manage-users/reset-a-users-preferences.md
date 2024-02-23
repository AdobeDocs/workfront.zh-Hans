---
title: 重置用户的首选项
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作为Adobe Workfront管理员，您可以重置或删除Workfront系统中任何用户的用户首选项设置。 个人用户也可以重置自己的用户首选项设置。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: c3cb97a36c29b90bbc9d8438d8811cc23266d894
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 2%

---

# 重置用户的首选项

<!-- Audited: 12/2023 -->

作为Adobe Workfront管理员，您可以重置或删除Workfront系统中任何用户的用户首选项设置。

个人用户也可以重置自己的用户首选项设置。

## 访问要求

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
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 关于受影响的设置

重置用户首选项时，某些首选项将恢复为系统默认值，而其他首选项将清除或删除：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>首选项</strong> </th> 
   <th><strong>重置后的状态</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>视图</td> 
   <td> <p> 已还原为系统默认值</p> <p>不会删除现有视图。 您可以再次选择它们。</p> </td> 
  </tr> 
  <tr> 
   <td>过滤器</td> 
   <td> <p>已还原为系统默认值</p> <p>不会删除现有筛选器。 您可以再次选择它们。</p> </td> 
  </tr> 
  <tr> 
   <td>分组</td> 
   <td> <p>已还原为系统默认值</p> <p>现有分组不会被删除。 您可以再次选择它们。</p> </td> 
  </tr> 
  <tr> 
   <td>最新项目列表</td> 
   <td>已清除</td> 
  </tr> 
  <tr> 
   <td>收藏夹列表</td> 
   <td>未受影响</td> 
  </tr> 
  <tr> 
   <td>用户首选项</td> 
   <td> <p>已还原为系统默认值</p> <p>电子邮件通知将还原为系统默认值。 默认通知列在 <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Adobe Workfront中可用的事件通知</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>用户定义的自定义选项卡</td> 
   <td>已删除</td> 
  </tr> 
  <tr> 
   <td>用户定义的全局导航选项</td> 
   <td>设置为布局模板定义，如果未分配布局模板，则设置为系统默认值。</td> 
  </tr> 
 </tbody> 
</table>

## 重置用户首选项

{{step-1-to-setup}}

1. 选择 **登录身份**.
1. 开始键入要重置其首选项的用户名，然后在名称出现在下拉列表中时单击该名称。
1. 选择  **登录**.
1. 在Web浏览器顶部的URL字段中添加 `/resetUser` 之后 `workfront.com`.

   >[!NOTE]
   >
   >这区分大小写。 U必须大写，其余字符必须为小写。 例如：
   >
   >`https://company_domain.my.workfront.com/resetUser`

1. 按 **输入**.
1. 要重置所有用户首选项，请选择 **重置**.

   或

   要仅重置自定义选项卡，请选择 **重置选项卡**.

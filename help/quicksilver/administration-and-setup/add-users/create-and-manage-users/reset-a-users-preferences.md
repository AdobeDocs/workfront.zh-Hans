---
title: 重置用户首选项
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 作为Adobe Workfront管理员，您可以重置或删除Workfront系统中任何用户的用户首选项设置。 个人用户还可以重置自己的用户首选项设置。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 2%

---

# 重置用户首选项

作为Adobe Workfront管理员，您可以重置或删除Workfront系统中任何用户的用户首选项设置。

个人用户还可以重置自己的用户首选项设置。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 关于受影响的设置

重置用户首选项时，某些首选项会还原为系统默认设置，而其他首选项会被清除或删除：

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
   <td> <p> 还原到系统默认值</p> <p>不会删除现有视图。 您可以再次选择它们。</p> </td> 
  </tr> 
  <tr> 
   <td>过滤器</td> 
   <td> <p>还原到系统默认值</p> <p>不会删除现有过滤器。 您可以再次选择它们。</p> </td> 
  </tr> 
  <tr> 
   <td>分组</td> 
   <td> <p>还原到系统默认值</p> <p>不会删除现有分组。 您可以再次选择它们。</p> </td> 
  </tr> 
  <tr> 
   <td>最近项目列表</td> 
   <td>已清除</td> 
  </tr> 
  <tr> 
   <td>收藏夹列表</td> 
   <td>未受影响</td> 
  </tr> 
  <tr> 
   <td>用户首选项</td> 
   <td> <p>还原到系统默认值</p> <p>电子邮件通知还原为系统默认值</p> </td> 
  </tr> 
  <tr> 
   <td>用户定义的自定义选项卡</td> 
   <td>已删除</td> 
  </tr> 
  <tr> 
   <td>用户定义的全局导航选项</td> 
   <td>如果未分配布局模板，则设置回布局模板定义或系统默认值。</td> 
  </tr> 
 </tbody> 
</table>

## 重置用户首选项

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 选择 **登录方式**.
1. 开始键入要重置其首选项的用户名称，然后在下拉列表中显示该名称时单击。
1. 选择  **登录**.
1. 在Web浏览器顶部的URL字段中，添加 `/resetUser` after `workfront.com`.

   >[!NOTE]
   >
   >这区分大小写。 U必须大写，其余字符必须小写。 例如：
   >
   >
   ```
   >https://company_domain.my.workfront.com/resetUser
   >```

1. 按 **输入**.
1. 要重置所有用户首选项，请选择 **重置**.

   或

   要仅重置自定义选项卡，请选择 **重置选项卡**.

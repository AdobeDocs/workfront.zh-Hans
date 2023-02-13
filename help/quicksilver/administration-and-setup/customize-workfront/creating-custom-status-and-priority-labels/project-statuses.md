---
title: 访问系统项目状态列表
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 用户可以指定项目的状态，以便其他用户能够在给定的时间查看项目的当前开发阶段。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# 访问系统项目状态列表

用户可以指定项目的状态，以便其他用户能够在给定的时间查看项目的当前开发阶段。

Workfront具有9个系统项目状态。 您可以更改这些状态的名称，但无法删除它们。

您还可以添加自定义项目状态以满足您组织中的需求。

作为Workfront管理员，您可以为系统中的所有新项目配置默认状态。 有关说明，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

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

## 访问项目状态

作为Workfront管理员，您可以访问系统级别项目状态列表。

有关编辑系统状态和创建自定义状态的信息，请参阅 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **项目首选项** > **状态**.

1. 单击 **项目** 选项卡。

   此选项卡上列出了Workfront中可用的项目状态。

   ![](assets/project-status.png)

   有关每个内置系统项目状态的详细信息，请参阅 [系统项目状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

## 创建自定义项目状态和自定义系统状态

作为Workfront管理员，您可以将系统项目状态添加到Workfront。 作为群组所有者，您可以添加特定于一个群组的自定义状态。 有关创建自定义状态或编辑系统状态的更多信息，请参阅 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

创建自定义项目状态时，必须始终将新状态与现有系统状态等同起来。 您必须了解系统状态的行为，才能知道哪个状态适合将自定义状态等同起来。 选择等于状态后，无法更改此选择。 有关系统项目状态的详细信息，请参阅 [系统项目状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

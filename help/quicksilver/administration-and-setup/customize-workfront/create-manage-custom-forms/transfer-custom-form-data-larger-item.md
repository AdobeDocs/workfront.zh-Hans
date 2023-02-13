---
title: 转换对象时传输自定义表单数据
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 当工作项中定义的工作变得过大时，您可以将其转换为较大的工作项。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 转换对象时传输自定义表单数据

根据贵组织的业务需求，任务或问题中定义的工作可能会变得过大，无法在任务或问题中管理它。 在这种情况下，您可以将它们转换为较大的工作项：

* 您可以将问题转换为任务或项目
* 您可以将任务转换为项目

要将自定义表单数据从问题传输到任务或项目，您必须按照以下顺序完成本文中的两个任务。

有关更多信息，请参阅 [转换Adobe Workfront中的问题概述](../../../manage-work/issues/convert-issues/convert-issues.md) 或 [转换Adobe Workfront中的问题概述](../../../manage-work/issues/convert-issues/convert-issues.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>计划</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对自定义表单的管理访问权限</p> <p>有关Workfront管理员如何授予此访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请联系您的Workfront管理员。

## 第一：复制自定义表单 {#first-copy-the-custom-form}

首先，您需要确保保留任何要转换的任务或问题的自定义表单数据。 由于自定义表单数据必须与转换后的项目完全匹配，因此最佳做法是复制表单，以便将其附加到新对象。

>[!TIP]
>
>在这种情况下，保留自定义表单数据的另一种方法是将较大的对象类型添加到自定义表单。 有关说明，请参阅 [开始编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) 在文章中 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms**.
1. 选择任务类型或问题类型自定义表单，然后单击 **复制**.
1. 在 **自定义表单** 对话框，为新表单指定名称。

1. 从 **表单类型** 下拉菜单中，选择要为其创建新自定义表单的对象类型

   **示例：** 如果要将自定义表单数据传输到项目，请选择项目。

1. 单击 **复制表单**.

   现在，可以将此复制的自定义表单附加到任务或项目。

1. 继续 [第二：转换问题或任务并传输自定义表单数据](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## 第二：转换问题或任务并传输自定义表单数据 {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. 复制您要转换的问题或任务的自定义表单，如部分所述 [第一：复制自定义表单](#first-copy-the-custom-form) 在本文中。
1. 使用 **自定义Forms** 选项来选择您复制的自定义表单。 有关说明，请参阅以下文章：

   * [在Adobe Workfront中将问题转换为项目](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [在Adobe Workfront中将问题转换为任务](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [将任务转换为项目](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. 在 **转换为（对象类型）** 对话框，单击 **添加Forms** 下拉菜单，然后选择您在上一部分中复制的表单。

   现在，在问题的自定义字段中捕获的信息将传输到任务上的自定义表单。


---
title: 列出并编辑添加到自定义表单的自定义表单和小部件
description: 当您查看组织的自定义表单以及已添加到其中的自定义字段和小部件的列表时，您可以使用工具栏中的选项编辑其属性、限制共享对象、复制它们以及删除它们。 您还可以在显示的列中查看其他信息，例如每个自定义表单与哪些对象类型相关联。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---


# 列出并编辑添加到自定义表单的自定义表单和小部件

当您查看组织的自定义表单以及已添加到其中的自定义字段和小部件的列表时，您可以使用工具栏中的选项编辑其属性、限制共享对象、复制它们以及删除它们。 您还可以在显示的列中查看其他信息，例如每个自定义表单与哪些对象类型相关联。

有关自定义表单中的自定义字段和小部件的信息，请参阅 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [在自定义表单中添加或编辑资源小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>任何</td> 
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

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请与Workfront管理员联系。

## 列出并编辑自定义表单以及添加到自定义表单的项目

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms**.

   使用 **Forms** 选项卡选定后，将列出贵组织的所有自定义表单及其说明、与其关联的对象类型、创建这些表单的用户的名称以及它们在系统中是否处于活动状态。

   有关在列表中选择自定义表单时可执行的操作的信息，请参阅以下文章：

   * [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [共享自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)
   * [复制自定义表单以创建新表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md)
   * [删除或停用自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md)

1. 单击 **字段** 选项卡。

   此选项卡列出了系统中用户添加到自定义表单的自定义字段和小部件，以及有关每个项目的类型的信息、有关该项目的说明和详细信息，以及包含该项目的自定义表单列表。

   此列表仅包含至少满足以下条件之一的自定义表单项目：

   * 可编辑系统范围
   * 在系统范围内可见
   * 由您创建
   * 已与您共享，具有查看或管理权限

   >[!NOTE]
   >
   >分节符未显示在字段选项卡上。

   有关在列表中选择项目时可执行的操作的信息，请参阅以下文章：

   * [编辑自定义表单中自定义字段、分区界限或小部件的属性](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/edit-a-custom-field.md)
   * [配置自定义字段和小部件的共享](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md)
   * [从系统中删除自定义字段或构件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md)

1. 选择 **区域** 选项卡，然后确保 **参数组** 已选为 **视图** 对于列表……

   此视图中将显示所有分节符，以及包含每个分节符的自定义表单列表。

   有关编辑您在列表中选择的自定义部分的信息，请参见 [向自定义表单添加分区界限](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).


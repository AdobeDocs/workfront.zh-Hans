---
title: 列出并编辑添加到自定义表单的自定义表单和小组件
description: 当您查看组织的自定义表单列表以及已添加到这些表单的自定义字段和小组件时，可以使用工具栏中的选项编辑其属性、限制与谁共享、复制和删除这些属性。 您还可以在显示的列中查看其他信息，例如每个自定义表单与哪些对象类型关联。
author: Caroline
source-git-commit: 49d4de3455fc1156efc8a88e8d2bee329c375279
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# 列出并编辑添加到自定义表单的自定义表单和小组件

当您查看组织的自定义表单列表以及已添加到这些表单的自定义字段和小组件时，可以使用工具栏中的选项编辑其属性、限制与谁共享、复制和删除这些属性。 您还可以在显示的列中查看其他信息，例如每个自定义表单与哪些对象类型关联。

有关自定义表单中的自定义字段和小组件的信息，请参阅 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [在自定义表单中添加或编辑资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## 列出并编辑添加到自定义表单的自定义表单和项目

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms**.

   使用 **Forms** 选项卡，将列出贵组织的所有自定义表单及其说明、与其关联的对象类型、创建这些表单的用户名以及他们在系统中是否处于活动状态。

   有关在列表中选择自定义表单时可以执行的操作信息，请参阅以下文章：

   * [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [共享自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)
   * [复制自定义表单以创建新表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md)
   * [删除或停用自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md)

1. 单击 **字段** 选项卡。

   此选项卡列出了系统中用户添加到自定义表单的自定义字段和小组件，以及有关每个项目类型、说明和详细信息以及包含该项目的自定义表单列表的信息。

   此列表仅包含至少满足以下条件之一的自定义表单项目：

   * 可编辑的系统范围
   * 可见系统范围
   * 由您创建
   * 与您共享，具有“查看”或“管理”访问权限

   >[!NOTE]
   >
   >“字段”选项卡上不显示分区符。

   有关在列表中选择项目时可以执行的操作的信息，请参阅以下文章：

   * [在自定义表单中编辑自定义字段、区域分时或小组件的属性](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/edit-a-custom-field.md)
   * [配置自定义字段和小组件的共享](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md)
   * [从系统中删除自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md)


1. 选择 **部分** 选项卡，然后确保 **参数组** 作为 **查看** 列表……

   所有部分都会中断在此视图中显示，同时还有包含每个部分中断的自定义表单列表。

   有关编辑您在列表中选择的自定义部分的信息，请参阅 [向自定义表单中添加节分符](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).


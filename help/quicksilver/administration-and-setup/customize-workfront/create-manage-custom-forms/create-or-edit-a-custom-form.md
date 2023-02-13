---
title: 创建或编辑自定义表单
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以创建或编辑新的自定义表单。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# 创建或编辑自定义表单

您可以创建或编辑新的自定义表单。 本文对这两项任务进行了说明。

有关从现有表单创建新自定义表单的信息，请参阅 [复制自定义表单以创建新表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

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

## 开始创建自定义表单

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms** 中。

   在显示的视图中，您可以查看为贵组织创建的所有自定义表单和自定义字段。 您还可以查看创建每个表单的人员以及与其关联的字段。

1. 单击 **新的自定义表单。**
1. 至少选择要与自定义表单关联的对象类型，然后单击 **继续**.

   ![](assets/choose-object-type.jpg)

1. 在 **表单设置** ，键入 **表单标题** 和可选 **描述** （自定义表单）。

1. （可选）如果要向表单中添加更多对象类型，以使其能够附加到更多对象，请在对象类型后单击加号，然后在显示的菜单中选择所需的对象类型。

   您可以重复此操作以添加所需数量的对象类型。您还可以单击对象类型上的X以从表单中删除它。

   有关从已保存的自定义表单中删除对象类型的信息，请参阅 [删除自定义表单中的对象类型](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. 单击 **完成**.

   >[!TIP]
   >
   >您可以单击 **应用** 创建自定义表单以保存所做更改并保持表单打开时，随时可以执行此操作。

1. 如果要向表单中添加新的自定义字段，请继续 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 或 [在自定义表单中重复使用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   或

   如果您希望以其他方式继续构建自定义表单，请继续阅读以下文章之一：

   * [在自定义表单中添加或编辑资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [在自定义表单中放置自定义字段和小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [向自定义表单中添加节分符](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自定义表单中重复使用现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [向自定义表单添加显示逻辑和跳过逻辑](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## 开始编辑自定义表单

您可以在自定义表单创建后随时对其进行编辑。

>[!CAUTION]
>
>有关在不丢失用户在自定义表单中输入的数据的情况下删除这些字段的信息，请参阅部分 [删除自定义字段，同时不会丢失用户输入的数据](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) 在文章中 [从系统中删除自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>通常，我们建议最大限度地减少您编辑已在使用的自定义表单的次数。 没有通知系统可提醒使用自定义表单的人员您所做的更改。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms** 中。

   在显示的视图中，您可以查看为贵组织创建的所有自定义表单。 您还可以查看谁创建了每个表单、它与哪种对象类型一起使用，以及它是否处于活动状态。

1. 选择要编辑的自定义表单，然后单击 **编辑**.
1. （可选）要更改自定义表单的标题和描述，请单击 **表单设置** 选项卡，然后键入 **表单标题** 和 **描述**.

1. （可选）如果要向表单中添加更多对象类型，以便能够将其附加到更多对象，请单击后面的加号+ **对象类型**，然后在显示的菜单中选择所需的类型。

   ![](assets/add-object-type-existing-form.png)

   您可以重复此操作以添加所需数量的对象类型。

   您还可以单击对象类型上的X，以将其从表单中删除。 当您要从已保存的自定义表单中删除对象类型时，应谨慎执行此操作。 有关更多信息，请参阅 [删除自定义表单中的对象类型](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. 单击 **完成**.

   >[!TIP]
   >
   >您可以单击 **应用** 创建自定义表单以保存所做更改并保持表单打开时，随时可以执行此操作。

1. 如果要向表单中添加新的自定义字段，请继续 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 或 [在自定义表单中重复使用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   或

   如果您希望以其他方式继续构建自定义表单，请继续阅读以下文章之一：

   * [在自定义表单中添加或编辑资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [在自定义表单中放置自定义字段和小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [向自定义表单中添加节分符](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自定义表单中重复使用现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [向自定义表单添加显示逻辑和跳过逻辑](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

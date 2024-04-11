---
title: 使用旧版表单生成器创建或编辑自定义表单
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以创建或编辑新的自定义表单。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# 使用旧版表单生成器创建或编辑自定义表单

<!--Audited: 01/2024-->

您可以创建新的自定义表单或编辑现有表单。 本文解释了这两项任务。

有关从现有自定义表单创建新自定义表单的信息，请参阅 [复制自定义表单以使用旧版表单生成器创建新表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

本文介绍了如何使用旧版表单生成器创建自定义表单。 有关使用表单设计器创建自定义表单的信息，请参阅 [使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront计划</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
   <p>或</p>
   <p>当前：计划</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>对自定义表单的管理访问权限</p> </td> 
  </tr>  
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 开始创建自定义表单

{{step-1-to-setup}}

1. 单击 **自定义Forms** 在左侧面板中。

   自定义表单显示在列表中。 您可以查看为您的组织创建的所有自定义表单和自定义字段。 您还可以查看创建每个表单的人员、与其关联的对象以及表单是否处于活动状态。

1. 单击 **新建自定义表单。**
1. 选择至少一个要与自定义表单关联的对象类型，然后单击 **继续**.

   ![](assets/choose-object-type.jpg)

1. 在 **表单设置** 打开选项卡，键入 **表单标题** 和可选 **描述** 用于自定义表单。

1. （可选）如果要向表单中添加更多对象类型，以便将其附加到更多对象，请单击 **加** 签名晚于 **对象类型**，然后在显示的菜单中选择所需的对象类型。

   您可以重复此操作，以添加所需数量的对象类型。

1. （可选）单击 **X** 对象类型，以将其从表单中删除。

   有关从已保存的自定义表单中删除对象类型的信息，请参阅 [删除自定义表单上的对象类型](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. 单击 **完成** 屏幕左下角的。

   >[!TIP]
   >
   >您可以单击 **应用** 在创建自定义表单时，可随时保存更改并保持表单打开。

1. 如果要向表单中添加新的自定义字段，请继续 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 或 [在自定义表单中重用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   或

   如果要继续以其他方式构建自定义表单，请继续阅读以下文章之一：

   * [在自定义表单中添加或编辑资源小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [在自定义表单中放置自定义字段和小部件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [向自定义表单添加分区界限](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自定义表单中重用现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [向自定义表单添加显示逻辑和跳过逻辑](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## 开始编辑自定义表单

您可以在创建自定义表单后随时对其进行编辑。

>[!CAUTION]
>
>有关从自定义表单中删除字段而不丢失用户在这些字段中输入的数据的信息，请参阅部分 [删除自定义字段而不丢失用户输入的数据](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) 在文章中 [从系统中删除自定义字段或构件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>通常，我们建议最大限度地减少编辑已使用的自定义表单的次数。 没有通知系统来提醒使用自定义表单的人员您的更改。

{{step-1-to-setup}}

1. 单击 **自定义Forms** 在左侧面板中。

   自定义表单显示在列表中。 您可以查看为您的组织创建的所有自定义表单和自定义字段。 您还可以查看创建每个表单的人员、与其关联的对象以及表单是否处于活动状态。

1. 选择要编辑的自定义表单，然后单击 ![“编辑”图标](assets/edit-icon.png).
1. （可选）要更改自定义表单的标题和描述，请单击 **表单设置** 选项卡，然后键入 **表单标题** 和 **描述**.

1. （可选）如果要向表单中添加更多对象类型，以便将其附加到更多对象，请单击后面的加号+ **对象类型**，然后在显示的菜单中选择所需的类型。

   ![](assets/add-object-type-existing-form.png)

   您可以重复此操作，以添加所需数量的对象类型。

   也可以单击对象类型上的X将其从表单中删除。 当您想要从已保存的自定义表单中删除对象类型时，应谨慎执行此操作。 有关更多信息，请参阅 [删除自定义表单上的对象类型](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. 单击 **完成**.

   >[!TIP]
   >
   >您可以单击 **应用** 在创建自定义表单时，可随时保存更改并保持表单打开。

1. 如果要向表单中添加新的自定义字段，请继续 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 或 [在自定义表单中重用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   或

   如果要继续以其他方式构建自定义表单，请继续阅读以下文章之一：

   * [在自定义表单中添加或编辑资源小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [在自定义表单中放置自定义字段和小部件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [向自定义表单添加分区界限](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自定义表单中重用现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [向自定义表单添加显示逻辑和跳过逻辑](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

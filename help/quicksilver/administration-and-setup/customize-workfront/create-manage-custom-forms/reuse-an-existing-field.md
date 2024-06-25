---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 使用旧版表单生成器重新使用自定义表单中的自定义字段或资产小组件
description: 创建或编辑自定义表单时，您可以添加已添加到其他自定义表单的自定义字段或小组件。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2c617909-48cb-4ee1-b0e8-002f2e57b0f0
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# 使用旧版表单生成器重新使用自定义表单中的自定义字段或资产小组件

{{form-designer-default}}

创建或编辑自定义表单时，您可以添加已添加到其他自定义表单的自定义字段或资源小部件。

您还可以在自定义表单中重用现有的计算自定义字段。 有关说明，请参阅 [在自定义表单中重用现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md).

有关自定义表单中的自定义字段和资产小部件的信息，请参阅 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [在自定义表单中添加或编辑资源小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## 重复使用已在其他自定义表单中使用的自定义字段或小组件

1. 开始创建或编辑自定义表单，如中所述 [使用旧版表单生成器创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 替换为 **添加字段** 选中，单击 **字段库**.

1. 将您希望在自定义表单中显示的字段或构件拖动到此处。
1. （可选）重复前两个步骤以添加任何其他字段或小组件。

   >[!NOTE]
   >
   >您最多可以在单个自定义表单上添加500个字段和小部件。 但是，当表单中存在超过100个时，可能会发生性能下降，具体取决于表单的复杂性。
   >
   >
   >复杂表单的示例包括带有层叠参数的表单、计算的自定义数据字段以及单个字段中的多个值选项。

1. 如果要继续以其他方式构建自定义表单，请继续阅读以下文章之一：

   * [使用旧版表单生成器将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [使用旧版表单生成器向自定义表单添加分区界限](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [使用旧版表单生成器添加或编辑自定义表单中的资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [使用旧版表单生成器将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [使用旧版表单生成器将自定义字段和小组件放置在自定义表单中](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [使用旧版表单生成器向自定义表单添加显示逻辑和跳过逻辑](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [使用旧版表单生成器预览并完成自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

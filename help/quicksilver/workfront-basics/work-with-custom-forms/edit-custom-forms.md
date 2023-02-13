---
product-area: projects;user-management
keywords: 编辑，表单，富文本，特殊，格式，字段，自定义，信息，自定义，对象
navigation-topic: work-with-custom-forms
title: 编辑自定义表单字段中的信息
description: 在表单附加到对象后，您可以编辑自定义表单上的信息。 有关将自定义表单添加到对象的信息，请参阅将自定义表单添加到对象。
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 6580fec18982215dbc2535d5f2ab159fc32ac3f5
workflow-type: tm+mt
source-wordcount: '982'
ht-degree: 0%

---

# 编辑自定义表单字段中的信息

在表单附加到对象后，您可以编辑自定义表单上的信息。 有关将自定义表单添加到对象的信息，请参阅 [将自定义表单添加到对象](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>团队或更高级别</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront许可证*</p> </td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对要编辑其自定义表单的对象的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>对象权限</p> </td> 
   <td> 
    <ul> 
     <li> <p>对要编辑其自定义表单的对象拥有更高权限</p> </li> 
     <li>查看要编辑的字段的权限。 有关共享自定义字段权限的信息，请参阅 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定义字段和小组件的共享</a>.</li> 
     <li> <p>要编辑的字段所在的表单部分的编辑权限</p> </li> 
    </ul> <p>有关请求对象的附加访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

* 您的Workfront管理员或对自定义表单具有管理访问权限的计划用户必须在您的环境中创建自定义表单。 有关更多信息，请参阅 [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* 必须将自定义表单附加到对象。

   有关如何将自定义表单应用到对象的信息，请参阅 [将自定义表单添加到对象](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 编辑自定义表单上的信息

对于所有对象，对附加到对象的自定义表单的编辑信息都是相同的。 有关哪些对象可以具有自定义表单的信息，请参阅 [自定义表单概述](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. 转到要编辑其自定义表单信息的对象。
1. 单击 **`<Object type>`详细信息** 中。

   例如，在编辑关于项目自定义表单的信息时，单击 **项目详细信息**.

1. 滚动到自定义表单。 当对象附加了自定义表单时，表单的名称将在“详细信息”部分显示为一个区域。
1. 如有必要，请单击箭头 ![](assets/expand-arrow-right.png) 来展开自定义表单名称的左侧。
1. 在页面的右上角附近，单击编辑图标 ![](assets/edit-icon.png).
1. 开始在您有权访问的任何字段中输入信息。

   ![](assets/click-in-field-to-edit-info-350x132.png)

   或

   如果尚未在表单上输入任何信息，请单击 **添加+** 对于您有权访问的任何字段，请开始输入信息。

   ![](assets/plus-add-to-edit-info-350x180.png)

   如果将多个自定义表单附加到对象，则可以对每个表单执行此操作。

   根据您所在字段的类型，请考虑以下事项：

   * 您只能为单选按钮字段选择一个选项。
   * 您可以在复选框字段中选择一个或多个选项，具体取决于表单创建者配置字段的方式。
   * 您可以在多选下拉字段中选择一个或多个选项，具体取决于表单创建者配置字段的方式。
   * 仅当创建表单的用户将文本字段设置为具有格式字段类型的文本字段时，才能设置文本字段的格式（粗体、斜体或下划线）。 单行文本字段和段落文本字段的格式不能。
   * 仅当创建表单的用户在创建字段时包含了日期字段类型时，才能在日期字段类型中更新一天中的时间。

   有关所有字段类型的信息，请参阅 [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 单击 **保存** 更改。

   >[!IMPORTANT]
   >
   >
   >
   ><!--   >
   ><p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This is true in "Edit custom forms" but not in "Add a custom form to an object." This snippet is used in both articles. The whole snippet is conditioned for classic only in "Add" but not in "Edit." Don't remove the NWE conditioning in the snippet because it is needed in "Edit."</p>   >
   >-->   >
   >
   >在保存表单之前，必须填写表单上的所有必填字段。 必填字段的名称后跟一个星号。
   ![](assets/nwe-required-custom-field.png)   >

   当某人更改了对象中由计算的自定义字段引用的另一个对象中的数据时，这些更改不会自动反映在您的对象中。 有关手动更新对象中所有计算的自定义字段的信息，请参阅 [为对象重新计算所有计算的自定义字段](#recalculate-all-calculated-custom-fields-for-an-object) 在本文中。

   当您批量编辑某个对象以及列表中的其他对象时，您还可以手动更新该对象的所有计算自定义字段。 有关说明，请参阅 [编辑对象时，重新计算列表中多个对象的所有计算自定义字段](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) 在本文中。

## 为对象重新计算所有计算的自定义字段  {#recalculate-all-calculated-custom-fields-for-an-object}

1. 转到要重新计算其自定义字段的对象的主页。
1. 单击 **更多** 菜单 ![](assets/more-icon.png) 在对象名称的右侧，单击 **重新计算表达式**.

   这会重新计算对象表单上的所有自定义字段。

## 编辑对象时，重新计算列表中多个对象的所有计算自定义字段 {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

您可以通过从列表或报表批量编辑多个对象的自定义字段来手动重新计算这些对象的自定义字段。

1. 转到包含具有计算字段的自定义表单的对象列表。
1. 选择要更新其计算自定义字段的对象。
1. 单击 **“编辑”图标**.
1. 单击 **自定义Forms** 在左侧菜单中，选择 **重新计算自定义表达式**.
1. 单击 **保存** **更改**.

   Workfront会计算所有选定对象的所有自定义字段。

>[!TIP]
根据项目的复杂性，我们建议在批量重新计算计算的自定义字段时不要选择大量项目，以确保获得最佳性能。 某些可能导致项目过于复杂的因素可能是多个依赖关系或分配或大量自定义字段。
要从项目列表批量重新计算自定义表达式，请执行以下操作：
1. 转到项目列表或报表，然后选择一个或多个项目。
1. 单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **重新计算自定义表达式**.
![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
Workfront会计算所有选定项目的所有自定义字段。

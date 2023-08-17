---
product-area: projects;user-management
keywords: 编辑，表单，富文本，特殊，格式，字段，自定义，信息，自定义，对象
navigation-topic: work-with-custom-forms
title: 编辑自定义表单字段中的信息
description: 将自定义表单附加到对象后，您可以编辑该表单上的信息。 有关将自定义表单添加到对象的信息，请参阅将自定义表单添加到对象。
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 7cc8c27848082c0547440ae98e4c4ec62809f5bd
workflow-type: tm+mt
source-wordcount: '1025'
ht-degree: 0%

---

# 编辑自定义表单字段中的信息

{{preview-and-fast-release}}

将自定义表单附加到对象后，您可以编辑该表单上的信息。 有关将自定义表单添加到对象的信息，请参阅 [向对象添加自定义表单](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>团队或更高</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront许可证*</p> </td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对要编辑其自定义表单的对象的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>对象权限</p> </td> 
   <td> 
    <ul> 
     <li> <p>要编辑自定义表单的对象的Contribute或更高权限</p> </li> 
     <li>查看要编辑的字段的权限。 有关共享自定义字段权限的信息，请参阅 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">配置自定义字段和小部件的共享</a>.</li> 
     <li> <p>编辑表单上要编辑的字段所在区域的权限</p> </li> 
    </ul> <p>有关请求对象的其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

* 您的Workfront管理员或对自定义表单具有管理访问权限的计划用户必须在您的环境中创建自定义表单。 有关更多信息，请参阅 [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* 您必须将自定义表单附加到对象。

  有关如何将自定义表单应用于对象的信息，请参阅 [向对象添加自定义表单](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 编辑自定义表单上的信息

对于所有对象，编辑附加到对象的自定义表单上的信息都是相同的。 有关哪些对象可以具有自定义表单的信息，请参见 [自定义表单概述](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. 转到要编辑其自定义表单信息的对象。
1. 单击 **`<Object type>`详细信息** 在左侧面板中。

   例如，在编辑项目自定义表单的信息时，单击 **项目详细信息**.

1. 滚动到自定义表单。 当有自定义表单附加到对象时，表单的名称在详细信息部分显示为区域。
1. 如有必要，单击箭头 ![](assets/expand-arrow-right.png) 以展开自定义表单名称的左侧。
1. 在页面的右上角附近，单击编辑图标 ![](assets/edit-icon.png).
1. 开始在您有权访问的任何字段中输入信息。

   ![](assets/click-in-field-to-edit-info-350x132.png)

   或

   如果尚未在表单上输入信息，请单击 **添加+** 对于您有权访问的任何字段，开始输入信息。

   ![](assets/plus-add-to-edit-info-350x180.png)

   如果将多个自定义表单附加到对象，您可以对每个表单执行此操作。

   根据您使用的字段类型，请考虑以下事项：

   * 您只能为单选按钮字段选择一个选项。
   * 您可以在复选框字段中选择一个或多个选项，具体取决于表单创建者如何配置该字段。
   * 您可以在多选下拉字段中选择一个或多个选项，具体取决于表单创建者如何配置该字段。
   * 仅当创建表单的用户将文本字段（粗体、斜体或下划线）设置为具有格式字段类型的文本字段时，您才可以设置文本字段的格式。 单行文本字段和段落文本字段无法格式化。
   * 仅当创建表单的用户在创建日期字段时包含该时间时，您才可以更新日期字段类型中的时间。

   有关所有字段类型的信息，请参见 [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 单击 **保存更改**.

   >[!IMPORTANT]
   >
   >在保存表单之前，必须填写表单上的所有必填字段。 必填字段的名称后跟一个星号。
   >
   >![](assets/nwe-required-custom-field.png)

   当有人更改对象中计算自定义字段引用的其他对象中的数据时，更改不会自动反映在对象中。 有关手动更新对象中所有已计算的自定义字段的信息，请参阅 [重新计算对象的所有已计算自定义字段](#recalculate-all-calculated-custom-fields-for-an-object) 本文章中。

   <span class="preview">修改页面上的依赖字段时，自定义表单上的计算字段会实时动态重新计算。 您无需保存表单即可查看更新后的结果。 这适用于默认表单以及自定义表单中的计算字段。</span>

   当您与列表中的其他对象一起批量编辑对象时，也可以手动更新该对象的所有计算自定义字段。 有关说明，请参阅 [编辑对象时，重新计算列表中多个对象的所有计算自定义字段](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) 本文章中。

## 重新计算对象的所有已计算自定义字段  {#recalculate-all-calculated-custom-fields-for-an-object}

1. 转到要重新计算其自定义字段的对象的主页。
1. 单击 **更多** 菜单 ![](assets/more-icon.png) 对象名称的右侧，然后单击 **重新计算表达式**.

   这会重新计算对象表单上的所有自定义字段。

## 编辑对象时，重新计算列表中多个对象的所有计算自定义字段 {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

您可以通过从列表或报表中批量编辑多个对象的自定义字段来手动重新计算它们。

1. 转到包含带有计算字段的自定义表单的对象列表。
1. 选择要更新其计算自定义字段的对象。
1. 单击 **“编辑”图标**.
1. 单击 **自定义Forms** 在左侧菜单中，然后选择 **重新计算自定义表达式**.
1. 单击 **保存** **更改**.

   Workfront会为所有选定对象计算所有自定义字段。

>[!TIP]
>
>根据项目的复杂性，我们建议不要在批量重新计算已计算的自定义字段时选择大量项目以确保最佳性能。 某些因素可能会使项目过于复杂，例如多个依赖项或分配或者大量自定义字段。
>
>要从项目列表中批量重新计算自定义表达式，请执行以下操作：
>
>1. 转到项目列表或报告，然后选择一个或多个项目。
>1. 单击 **更多** 菜单 ![](assets/more-icon.png)，然后单击 **重新计算自定义表达式**.
>
>![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
>
>Workfront会为所有选定项目计算所有自定义字段。

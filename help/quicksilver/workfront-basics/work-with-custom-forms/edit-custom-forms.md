---
product-area: projects;user-management
keywords: 编辑，表单，富文本，特殊，格式，字段，自定义，信息，自定义，对象
navigation-topic: work-with-custom-forms
title: 编辑自定义表单字段中的信息
description: 将自定义表单附加到对象后，您可以编辑该表单上的信息。 有关将自定义表单添加到对象的信息，请参阅将自定义表单添加到对象。
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 0%

---

# 编辑自定义表单字段中的信息

将自定义表单附加到对象后，您可以编辑该表单上的信息。 有关将自定义表单添加到对象的信息，请参阅[将自定义表单添加到对象](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

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
   <td> <p>编辑对要编辑其自定义表单的对象的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>对象权限</p> </td> 
   <td> 
    <ul> 
     <li> <p>要编辑自定义表单的对象的Contribute或更高权限</p> </li> 
     <li>查看要编辑的字段的权限。 有关共享自定义字段权限的信息，请参阅<a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md" class="MCXref xref">配置自定义字段和小部件的共享</a>。</li> 
     <li> <p>编辑表单上要编辑的字段所在区域的权限</p> </li> 
    </ul> <p>有关请求对象的其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 先决条件

* 您的Workfront管理员或对自定义表单具有管理访问权限的计划用户必须在您的环境中创建自定义表单。 有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
* 您必须将自定义表单附加到对象。

  有关如何将自定义表单应用于对象的信息，请参阅[将自定义表单添加到对象](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

## 编辑自定义表单上的信息

对于所有对象，编辑附加到对象的自定义表单上的信息都是相同的。 有关哪些对象可以具有自定义表单的信息，请参阅[自定义表单概述](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md)。

1. 转到要编辑其自定义表单信息的对象。
1. 单击左侧面板中的&#x200B;**`<Object type>`详细信息**。

   例如，在编辑项目自定义表单上的信息时，单击&#x200B;**项目详细信息**。

1. 滚动到自定义表单。 当有自定义表单附加到对象时，表单的名称在详细信息部分显示为区域。
1. 如有必要，请单击自定义表单名称左侧的箭头![](assets/expand-arrow-right.png)以展开该表单。
1. 在页面的右上角附近，单击编辑图标![](assets/edit-icon.png)。
1. 开始在您有权访问的任何字段中输入信息。

   ![](assets/click-in-field-to-edit-info-350x132.png)

   或

   如果尚未在表单上输入任何信息，请单击您有权访问的任何字段的&#x200B;**添加+**&#x200B;并开始输入信息。

   ![](assets/plus-add-to-edit-info-350x180.png)

   如果将多个自定义表单附加到对象，您可以对每个表单执行此操作。

   根据您使用的字段类型，请考虑以下事项：

   * 您只能为单选按钮字段选择一个选项。
   * 您可以在复选框字段中选择一个或多个选项，具体取决于表单创建者如何配置该字段。
   * 您可以在多选下拉字段中选择一个或多个选项，具体取决于表单创建者如何配置该字段。
   * 仅当创建表单的用户将文本字段（粗体、斜体或下划线）设置为具有格式字段类型的文本字段时，您才可以设置文本字段的格式。 单行文本字段和段落文本字段无法格式化。
   * 仅当创建表单的用户在创建日期字段时包含该时间时，您才可以更新日期字段类型中的时间。

   有关所有字段类型的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. 单击&#x200B;**保存更改**。

   >[!IMPORTANT]
   >
   >在保存表单之前，必须填写表单上的所有必填字段。 必填字段的名称后跟一个星号。
   >
   >![](assets/nwe-required-custom-field.png)

   当有人更改对象中计算自定义字段引用的其他对象中的数据时，更改不会自动反映在对象中。 有关手动更新对象中所有计算自定义字段的信息，请参阅本文中的[重新计算对象的所有计算自定义字段](#recalculate-all-calculated-custom-fields-for-an-object)。

   修改页面上的依赖字段时，自定义表单上的计算字段会实时动态重新计算。 您可以在不保存表单的情况下查看新的计算字段值，但在保存更改之前，该值不会实际应用于表单和对象。 这适用于默认表单以及自定义表单中的计算字段。

   当您与列表中的其他对象一起批量编辑对象时，也可以手动更新该对象的所有计算自定义字段。 有关说明，请参阅在编辑本文中的对象](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects)时，重新计算列表中多个对象的所有计算自定义字段[。

## 重新计算对象的所有已计算自定义字段  {#recalculate-all-calculated-custom-fields-for-an-object}

1. 转到要重新计算其自定义字段的对象的主页。
1. 单击对象名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-icon.png)，然后单击&#x200B;**重新计算表达式**。

   这会重新计算对象表单上的所有自定义字段。

## 编辑对象时，重新计算列表中多个对象的所有计算自定义字段 {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

您可以通过从列表或报表中批量编辑多个对象的自定义字段来手动重新计算它们。

1. 转到包含带有计算字段的自定义表单的对象列表。
1. 选择要更新其计算自定义字段的对象。
1. 单击&#x200B;**编辑图标**。
1. 单击左侧菜单中的&#x200B;**自定义Forms**，然后选择&#x200B;**重新计算自定义表达式**。
1. 单击&#x200B;**保存** **更改**。

   Workfront会为所有选定对象计算所有自定义字段。

>[!TIP]
>
>根据项目的复杂性，我们建议不要在批量重新计算已计算的自定义字段时选择大量项目以确保最佳性能。 某些因素可能会使项目过于复杂，例如多个依赖项或分配或者大量自定义字段。
>
>要从项目列表中批量重新计算自定义表达式，请执行以下操作：
>
>1. 转到项目列表或报告，然后选择一个或多个项目。
>1. 单击&#x200B;**更多**&#x200B;菜单![](assets/more-icon.png)，然后单击&#x200B;**重新计算自定义表达式**。
>
>![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
>
>Workfront会为所有选定项目计算所有自定义字段。

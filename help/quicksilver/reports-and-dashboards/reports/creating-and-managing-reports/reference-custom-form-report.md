---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 在报表中引用自定义表单
description: 您可以在该对象的报表的视图、过滤器和分组中引用对象的自定义形式。
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 2%

---

# 在报表中引用自定义表单

您可以在该对象的报表的视图、过滤器和分组中引用对象的自定义形式。

您可以引用要包含在报表中的自定义表单内容，也可以引用有关要包含在报表中的自定义表单本身的信息。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

自定义表单必须存在，然后才能在报表中引用。

有关创建自定义表单的更多信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 引用自定义表单的内容

您可以引用自定义表单中的字段。 将自定义表单应用于对象后，与该自定义表单关联的所有字段都可在报表中引用，就像对象上的任何其他字段一样。

>[!NOTE]
>
>对于具有多个选项的字段，报表的过滤器和提示中提供了所有选项，包括隐藏的选项。\
>有关在具有多个选项的自定义字段中隐藏选项的更多信息，请参阅文章 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

创建报告时，只需使用表单的对象类型作为字段源，并使用自定义字段的名称作为字段名称即可。

例如，您可能有一个自定义表单应用于包含该自定义字段的所有项目 **顾问**. 要创建列出Olivia Kim担任顾问的所有项目的报表，请使用 **项目** 对象类型作为字段源，并使用 **顾问** 作为字段名称。 将过滤器限定符设置为 **等于**&#x200B;然后输入奥利维亚·金。

![](assets/qs-consultant-filter-example-350x126.png)

有关创建报表的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## 有关自定义表单的参考信息

您可以引用有关自定义表单的信息，例如与对象关联的任何自定义表单的名称。

根&#x200B;据元素（“查看”、“过滤器”或“分组”），可以引用以下任一项：

* 应用于对象的主自定义表单：

   这是首先在对象的“详细信息”(Details)页面上显示的表单。

* 所有自定义表单（如果对象应用了多个自定义表单）

您可以根据视图、过滤器和分组引用自定义表单：

* [在报表视图（列）中引用自定义表单](#reference-custom-forms-in-a-report-view-column)
* [在报表过滤器中引用自定义表单](#reference-custom-forms-in-a-report-filter)
* [在报表分组中引用自定义表单](#reference-custom-forms-in-a-report-grouping)

### 在报表视图（列）中引用自定义表单 {#reference-custom-forms-in-a-report-view-column}

要显示与对象关联的所有自定义表单，请执行以下操作：

1. 按照文章中所述开始创建报告 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 在 **列** 选项卡，展开要引用的自定义表单所应用的对象类型，然后单击 **类别名称**.\
   例如，要显示与任务关联的所有自定义表单，请展开 **任务** 字段源，然后单击 **类别名称** 字段名称。\
   ![](assets/qs-category-name-column-350x267.png)

要仅显示与对象关联的主自定义表单，请执行以下操作：

1. 按照文章中所述开始创建报告 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 在 **列** 选项卡，展开 **类别** 字段源，然后单击 **名称** 字段名称。\
   ![](assets/qs-category-name-column-2-350x248.png)

### 在报表过滤器中引用自定义表单 {#reference-custom-forms-in-a-report-filter}

要过滤与对象类型关联的所有自定义表单，请执行以下操作：

1. 按照文章中所述开始创建报告 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 在 **过滤器** 选项卡，展开 **类别**，然后单击 **名称**.\
   ![](assets/qs-categories-name-filter-350x311.png)

1. 选择要使用的条件限定符：

   * 空白
   * 不为空白
   * 包含
   * 不包含
   * 等于 (区分大小写)
   * 不等于

   有关每个限定符的更多信息，请参阅文章 [过滤器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >如果要筛选的字段具有多个选项，并且您使用 **不等于** 或 **不包含** 限定符，则会过滤出仅包含您指定选择的结果。 如果字段包含其他选项（包括指定的选项），则不会从报表中过滤这些结果。 这包括过滤多个自定义Forms（如果它们附加到同一对象）。

1. 开始键入要过滤的自定义表单的名称，然后在下拉列表中显示该名称时单击该名称。
1. （可选）单击 **添加其他过滤器规则**，然后重复步骤2-4以创建其他过滤器规则。
1. 单击 **保存并关闭**.

要仅对与对象类型关联的主自定义表单进行过滤，请执行以下操作：

1. 按照文章中所述开始创建报告 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 在 **过滤器** 选项卡，展开 **类别** 字段源，然后单击 **名称** 字段名称。\
   ![](assets/qs-category-name-filter-350x437.png)

1. 选择要使用的条件限定符：

   * 空白
   * 不为空白
   * 包含
   * 不包含
   * 等于 (区分大小写)
   * 不等于

   有关每个限定符的更多信息，请参阅文章 [过滤器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. 开始键入要过滤的自定义表单的名称，然后在下拉列表中显示该名称时单击该名称。
1. （可选）单击 **添加其他过滤器规则**，然后重复步骤2-4以创建其他过滤器规则。
1. 单击 **保存并关闭**.

### 在报表分组中引用自定义表单 {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>您只能按与对象关联的主要自定义表单对项目进行分组；不能按与对象关联的所有表单对项目进行分组。

1. 按照文章中所述开始创建报告 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. 在 **分组** 选项卡，展开 **类别**，然后单击 **名称**.\
   ![](assets/qs-category-name-grouping-350x373.png)

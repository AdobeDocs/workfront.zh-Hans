---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 在报表中引用自定义表单
description: 您可以在报表的视图、筛选器和分组中引用该对象的自定义表单。
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '998'
ht-degree: 2%

---

# 在报表中引用自定义表单

您可以在报表的视图、筛选器和分组中引用该对象的自定义表单。

您可以引用要包含在报表中的自定义表单的内容，也可以引用要包含在报表中的自定义表单本身的相关信息。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 先决条件

自定义表单必须存在，您才能在报表中引用它。

有关创建自定义表单的详细信息，请参阅[创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)。

## 引用自定义表单的内容

您可以在自定义表单中引用字段。 将自定义表单应用于对象后，与该自定义表单关联的所有字段均可在报表中引用，就像该对象上的任何其他字段一样。

>[!NOTE]
>
>对于具有多个选项的字段，报表的过滤器和提示中会提供所有选项，包括隐藏的选项。\
>有关从具有多个选项的自定义字段中隐藏选项的更多信息，请参阅文章[创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)。

创建报告时，只需使用表单的对象类型作为字段源，并使用自定义字段的名称作为字段名称即可。

例如，您可能将自定义表单应用于包含自定义字段&#x200B;**顾问**&#x200B;的所有项目。 若要创建列出所有项目（Olivia Kim是其中的顾问）的报告，请使用&#x200B;**Project**&#x200B;对象类型作为字段源，并使用&#x200B;**Consultant**&#x200B;作为字段名称。 将筛选器限定符设置为&#x200B;**等于**，然后键入Olivia Kim。

![](assets/qs-consultant-filter-example-350x126.png)

有关创建报告的详细信息，请参阅文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 有关自定义表单的参考信息

您可以引用有关自定义表单的信息，例如与对象关联的任何自定义表单的名称。

根据&#x200B;元素（视图、过滤器或分组），您可以引用以下任一元素：

* 应用于对象的主要自定义表单：

  此表单首先显示在对象的“详细信息”页面上。

* 所有自定义表单（如果对对象应用了多个自定义表单）

您可以引用视图、筛选器和分组的自定义表单：

* [在报表视图（列）中引用自定义表单](#reference-custom-forms-in-a-report-view-column)
* [在报表筛选器中引用自定义表单](#reference-custom-forms-in-a-report-filter)
* [在报表分组中引用自定义表单](#reference-custom-forms-in-a-report-grouping)

### 在报表视图中引用自定义表单（列） {#reference-custom-forms-in-a-report-view-column}

要显示与对象关联的所有自定义表单，请执行以下操作：

1. 按照文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中的说明开始创建报告。
1. 在&#x200B;**列**&#x200B;选项卡上，展开要引用自定义表单的对象类型，然后单击&#x200B;**类别名称**。\
   例如，要显示与任务关联的所有自定义表单，请展开&#x200B;**任务**&#x200B;字段源，然后单击&#x200B;**类别名称**&#x200B;字段名称。\
   ![](assets/qs-category-name-column-350x267.png)

要仅显示与对象关联的主要自定义表单，请执行以下操作：

1. 按照文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中的说明开始创建报告。
1. 在&#x200B;**列**&#x200B;选项卡上，展开&#x200B;**类别**&#x200B;字段源，然后单击&#x200B;**名称**&#x200B;字段名称。\
   ![](assets/qs-category-name-column-2-350x248.png)

### 在报表过滤器中引用自定义表单 {#reference-custom-forms-in-a-report-filter}

要筛选与对象类型关联的所有自定义表单，请执行以下操作：

1. 按照文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中的说明开始创建报告。
1. 在&#x200B;**筛选器**&#x200B;选项卡上，展开&#x200B;**类别**，然后单击&#x200B;**名称**。\
   ![](assets/qs-categories-name-filter-350x311.png)

1. 选择要使用的条件限定符：

   * 空白
   * 不为空白
   * 包含
   * 不包含
   * 等于
   * 不等于

   有关每个限定符的详细信息，请参阅文章[筛选器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   >[!NOTE]
   >
   >如果您要过滤的字段有多个选项，并且您使用&#x200B;**不等于**&#x200B;或&#x200B;**不包含**&#x200B;限定符，这将过滤掉仅包含您指定选项的结果。 如果字段包含其他选项（包括指定的选项），则不会从报表中筛选这些结果。 这包括筛选附加到同一对象的多个自定义Forms。

1. 开始键入要过滤的自定义表单的名称，然后在该名称出现在下拉列表中时单击该名称。
1. （可选）单击&#x200B;**添加其他筛选器规则**，然后重复步骤2-4以创建其他筛选器规则。
1. 单击&#x200B;**保存+关闭**。

要仅筛选与对象类型关联的主要自定义表单，请执行以下操作：

1. 按照文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中的说明开始创建报告。
1. 在&#x200B;**筛选器**&#x200B;选项卡上，展开&#x200B;**类别**&#x200B;字段源，然后单击&#x200B;**名称**&#x200B;字段名称。\
   ![](assets/qs-category-name-filter-350x437.png)

1. 选择要使用的条件限定符：

   * 空白
   * 不为空白
   * 包含
   * 不包含
   * 等于
   * 不等于

   有关每个限定符的详细信息，请参阅文章[筛选器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

1. 开始键入要过滤的自定义表单的名称，然后在该名称出现在下拉列表中时单击该名称。
1. （可选）单击&#x200B;**添加其他筛选器规则**，然后重复步骤2-4以创建其他筛选器规则。
1. 单击&#x200B;**保存+关闭**。

### 在报表分组中引用自定义表单 {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>只能按与对象关联的主要自定义表单对项目进行分组；不能按与对象关联的所有表单对项目进行分组。

1. 按照文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中的说明开始创建报告。
1. 在&#x200B;**分组**&#x200B;选项卡上，展开&#x200B;**类别**，然后单击&#x200B;**名称**。\
   ![](assets/qs-category-name-grouping-350x373.png)

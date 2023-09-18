---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 按多选自定义字段绘制报表图表
description: 只有在您创建捕获多选自定义字段中选定选项的附加计算字段后，才能按多选自定义字段绘制报表的图表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: a2f0ef565b0f0dbcfec7f3f5b5fece4c7b4b1ec6
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 0%

---

# 按多选自定义字段绘制报表图表

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

我们建议您不要使用多选自定义字段构建图表，而是为多选自定义字段的每个选项创建单独的字段。

多选自定义字段的示例包括：

* 复选框
* 多选下拉菜单

有关使用文本模式的信息，请参阅文章 [文本模式概述](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

但是，如果无法为多选字段的每个选项设置单独的字段，则可以通过使用计算的自定义字段将多选字段中的选项首先分组，按多选自定义字段绘制报表图表。 之后，您可以按计算字段绘制报表图表。

>[!NOTE]
>
>具有任何选定选项的项目仅被计数一次。
>
>例如，如果您有一个复选框自定义字段，其中选项1和选项2为选项，并且您将表单附加到任务，则同时具有选项1和选项2的任务将显示在一个单独的图表元素中，而不是仅显示仅选定选项1或选项2的任务。
>
>已选择选项1的任务与已选择选项1和选项2的任务不会显示在相同的图表元素中。

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
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须创建一个计算自定义字段，以显示从多选自定义字段中选择的值。 有关信息，请参见 [构建引用多选自定义字段的计算自定义字段](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) 部分。

## 按多选自定义字段绘制报表图表

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

无法通过引用多选自定义字段在报表中构建图表。 您可以改为创建一个计算字段，以记录给定对象上的多选自定义字段的值，并按计算字段进行分组。 

* [构建引用多选自定义字段的计算自定义字段](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [构建引用计算自定义字段的图表](#build-a-chart-that-references-a-calculated-custom-field)

### 构建引用多选自定义字段的计算自定义字段 {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

要生成引用多选自定义字段的计算字段，您必须满足以下先决条件：

* 自定义表单中的多选自定义字段。\
  有关构建自定义表单以及向其中添加自定义字段的信息，请参阅文章 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* 带有附加到对象的多选自定义字段的自定义表单。
* 每个对象的多选自定义字段的值。

要构建引用多选自定义字段的计算自定义字段，请执行以下操作：

1. 创建自定义表单或编辑现有表单。

   有关创建自定义表单的信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 选择您计划用于自定义表单的一个或多个对象。
1. 单击 **添加字段**，则 **已计算** 以将多选自定义字段添加到表单。

1. 在 **标签** 框中，命名新的计算字段以指示它引用了多选自定义字段。

   例如：“计算的多选字段。”

1. 在 **计算** 框中，输入以下代码：

   `{DE:Multi-select Custom Field}`

   这会将多选自定义字段中选定的选项添加到计算的自定义字段中。 例如，如果表单附加到任务并从多选自定义字段中选择了选项1，则计算自定义字段显示值“选项1”。 如果为其他任务选择了选项1和选项2，则计算的自定义字段显示值“选项1，选项2”。

1. 将“多选自定义字段”替换为您在Workfront中显示的多选自定义字段的实际名称。

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. （可选）如果多选自定义字段已存在于此表单上，且此表单已附加到对象，请启用 **更新以前的计算（在后台）** 选项。

   这可确保使用多选自定义字段中的值自动填充新的计算字段，因为该字段已添加到已附加到对象的表单中。

1. 单击 **完成**.
1. 单击 **保存+关闭**.

   计算的自定义字段将添加到自定义表单，如果表单当前附加到对象，则使用多选自定义字段中的信息填充该字段。

### 构建引用计算自定义字段的图表 {#build-a-chart-that-references-a-calculated-custom-field}

1. （可选）要确保要按其绘制图表的所有计算字段均填充了值，请从报表的详细信息选项卡中选择包含具有多选自定义字段和计算自定义字段的自定义表单的所有对象，然后单击 **编辑**.
1. （可选且视情况而定）选择 **重新计算自定义表达式** 字段，然后单击 **保存更改**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   >此选项已从批量编辑项目中消除。  您仍然可以通过单击 **更多** 图标 ![](assets/more-icon-45x33.png) 在项目列表的顶部，然后 **重新计算表达式**.

1. 转到要在其中添加引用多选自定义字段的计算字段的图表的报表。
1. 单击 **报表操作**，则 **编辑**.

1. 选择 <strong>分组</strong> 选项卡，然后单击 <strong>添加分组</strong>.
1. 添加 <strong>计算的多选字段</strong> 您已创建作为您的分组。
1. 选择 <strong>图表</strong> 制表符，并将图表添加到报表中。

   例如，选择 **列** 图表。
   <br>有关将图表添加到报表的信息，请参阅部分 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">向报表中添加图表</a> 在文章中 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报表</a>.
1. 在 **底部(X)轴** 字段中，选择 <strong>计算的多选字段</strong> 以显示在图表中。
1. 单击 <strong>保存+关闭</strong>.

   该报告在图表中显示按计算的多选字段分组的结果。

   ![](assets/chart-multi-select-field-column-chart-example.png)
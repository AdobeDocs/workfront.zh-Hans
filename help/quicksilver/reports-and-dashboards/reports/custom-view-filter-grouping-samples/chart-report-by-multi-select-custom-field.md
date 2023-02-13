---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 按多选自定义字段绘制报表图表
description: 无法通过多选自定义字段来绘制报表图表。 您需要创建一个引用多选自定义字段的附加计算字段，以便还按多选自定义字段的值来图表报表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 按多选自定义字段绘制报表图表

无法通过多选自定义字段来绘制报表图表。 您需要创建一个引用多选自定义字段的附加计算字段，以便还按多选自定义字段的值来图表报表。

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

在开始之前，必须创建一个计算的自定义字段，以显示从多选自定义字段中选择的值。 有关信息，请参阅 [构建引用多选自定义字段的计算自定义字段](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) 章节。

## 按多选自定义字段绘制报表图表

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

不能通过引用多选自定义字段在报表中构建图表。 您而是可以创建一个计算字段，用于记录给定对象上的多选自定义字段的值，并按计算字段进行分组。 

* [构建引用多选自定义字段的计算自定义字段](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [构建引用计算自定义字段的图表](#build-a-chart-that-references-a-calculated-custom-field)

### 构建引用多选自定义字段的计算自定义字段 {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

要能够生成引用多选自定义字段的计算字段，您必须具备以下先决条件：

* 在自定义表单中构建多选自定义字段。\
   有关构建自定义表单以及向其添加自定义字段的信息，请参阅文章 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* 将自定义表单附加到对象。
* 在多选自定义字段中填充每个对象的值。

要生成引用多选自定义字段的计算自定义字段，请执行以下操作：

1. 创建自定义表单，或编辑现有表单。\
   有关创建自定义表单的信息，请参阅文章 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 选择您计划与自定义表单一起使用的一个或多个对象。
1. 单击&#x200B;**添加字段**，则 **已计算** 向表单中添加多选自定义字段。

1. 在 **标签** 框中，将新的计算字段命名为，以指示它引用了多选自定义字段。\
   例如：&quot;Calculated Multi-select Field（计算的多选字段）&quot;

1. 在 **计算** 框中，输入以下代码：

   ```
   {DE:Multi-select Custom Field}
   ```

1. 将“多选自定义字段”替换为多选自定义字段的实际名称，如在Workfront中所示。

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. （可选）如果此表单上已存在多选自定义字段，并且此表单已附加到对象，请启用 **更新以前的计算** 选项。\
   这可确保在新字段添加到附加到对象的表单时，自动使用多选自定义字段中的值填充该字段。

1. 单击 **完成**.
1. 单击 **保存+关闭**.

### 构建引用计算自定义字段的图表 {#build-a-chart-that-references-a-calculated-custom-field}

1. （可选）要确保要按图表显示的所有计算字段都填充了值，请选择报表中包含自定义表单（包含多选自定义字段和计算量度自定义字段）的所有对象，然后单击 **编辑**.
1. （可选和视情况而定）启用 **重新计算自定义表达式** 字段，然后单击 **保存更改**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

1. 转到要为引用多选自定义字段的计算字段添加图表的报表。
1. 单击 **报表操作**，则 **编辑**.

1. 选择 <strong>分组</strong> ，然后单击 <strong>添加分组</strong>.
1. 添加<strong>计算的多选字段</strong> 创建为组。
1. 选择 <strong>图表</strong> 选项卡，并向报表中添加图表。<br>有关将图表添加到报表的信息，请参阅部分 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">将图表添加到报表</a> 在文章中 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报表</a>.
1. 选择 <strong>计算的多选字段</strong> 作为图表中显示的字段之一。
1. 单击 <strong>保存并关闭</strong>.<br>报表在图表中显示按计算的多选字段分组的结果。

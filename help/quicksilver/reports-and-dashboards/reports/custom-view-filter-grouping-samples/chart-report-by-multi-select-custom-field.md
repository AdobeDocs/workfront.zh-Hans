---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 按多选自定义字段绘制报表图表
description: 不能通过多选自定义字段绘制报表图表。 您需要创建一个引用多选自定义字段的附加计算字段，以便按照多选自定义字段的值绘制报表图表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 23257f11b0795aa1f1e422923f6d596017c58126
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# 按多选自定义字段绘制报表图表

<span class="preview">此页面上高亮显示的信息是指尚未公开发布的功能。 它仅在“预览”环境中可用。</span>

不能通过多选自定义字段绘制报表图表。 您需要创建一个引用多选自定义字段的附加计算字段，以便按照多选自定义字段的值绘制报表图表。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须创建一个计算自定义字段，以显示从多选自定义字段中选择的值。 欲了解相关信息，请参见 [构建引用多选自定义字段的计算自定义字段](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) 章节。

## 按多选自定义字段绘制报表图表

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

无法通过引用多选自定义字段在报告中构建图表。 相反，您可以创建一个计算字段，以记录给定对象上的多选自定义字段的值，并按计算字段进行分组。 

* [构建引用多选自定义字段的计算自定义字段](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [构建引用计算自定义字段的图表](#build-a-chart-that-references-a-calculated-custom-field)

### 构建引用多选自定义字段的计算自定义字段 {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

要生成引用多选自定义字段的计算字段，您必须满足以下先决条件：

* 在自定义表单中构建多选自定义字段。\
   有关构建自定义表单和向其中添加自定义字段的信息，请参阅文章 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* 将自定义表单附加到对象。
* 在每个对象上使用值填充多选自定义字段。

要构建引用多选自定义字段的计算自定义字段，请执行以下操作：

1. 创建自定义表单或编辑现有表单。\
   有关创建自定义表单的信息，请参阅文章 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 选择您计划在自定义表单中使用的一个或多个对象。
1. 单击&#x200B;**添加字段**，则 **已计算** 以将多选自定义字段添加到表单。

1. 在 **标签** 框中，命名新的计算字段以指示它引用了多选自定义字段。\
   例如：“计算的多选字段”。

1. 在 **计算** 框中，输入以下代码：

   ```
   {DE:Multi-select Custom Field}
   ```

1. 将“多选自定义字段”替换为多选自定义字段的实际名称，该名称显示在Workfront中。

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. （可选）如果此表单上已有多选自定义字段，并且此表单已附加到对象，请启用 **更新以前的计算** 选项。\
   这可确保使用多选自定义字段中的值自动填充新字段，因为该字段已添加到附加到对象的表单中。

1. 单击 **完成**.
1. 单击 **保存+关闭**.

### 构建引用计算自定义字段的图表 {#build-a-chart-that-references-a-calculated-custom-field}

1. （可选）要确保要按其绘制图表的所有计算字段均填充了值，请选择报表中包含自定义表单的所有对象，其中具有多选自定义字段和计算自定义字段，然后单击 **编辑**.
1. （可选和条件）启用 **重新计算自定义表达式** 字段，然后单击 **保存更改**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   ><span class="preview">在“预览”环境中批量编辑项目时，已取消使用此选项。  您仍然可以通过单击批量重新计算项目的表达式 **更多** ![](assets/more-icon-45x33.png) 在项目列表顶部，然后 **重新计算表达式**. </span>


1. 转到要在其中添加引用多选自定义字段的计算字段的图表的报表。
1. 单击 **报表操作**，则 **编辑**.

1. 选择 <strong>分组</strong> 选项卡，然后单击 <strong>添加分组</strong>.
1. 添加<strong>计算的多选字段</strong> 您已创建作为您的分组。
1. 选择 <strong>图表</strong> 选项卡，并向报表中添加图表。<br>有关将图表添加到报表的信息，请参阅小节 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">向报告添加图表</a> 在文章中 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">创建自定义报表</a>.
1. 选择 <strong>计算的多选字段</strong> 作为要在图表中显示的字段之一。
1. 单击 <strong>保存+关闭</strong>.<br>该报告在图表中显示按计算的多选字段分组的结果。

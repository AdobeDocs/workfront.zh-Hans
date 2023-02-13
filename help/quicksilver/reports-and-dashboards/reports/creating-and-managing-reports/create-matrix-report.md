---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 创建矩阵报表
description: 矩阵报表以汇总表格式显示摘要信息，与在传统报表等列表中显示相比，这样更便于查看。
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 0%

---

# 创建矩阵报表

矩阵报表以汇总表格式显示摘要信息，与在传统报表等列表中显示相比，这样更便于查看。

## 何时使用矩阵报表

您可以为包含2个或更多分组的任何报表创建矩阵报表。 传统报表最多可包含3个分组，而矩阵报表最多可包含4个分组。

例如，您要创建一个显示3个月期间记录的小时数的小时报表，并希望报表按照输入小时数的人以及按月和按周进行组织。

![](assets/report-matrix-overview-350x123.png)

## 数据在矩阵报表中的显示方式

矩阵报表中的信息始终显示为数值。 在大多数情况下，包含数值的列最适合在矩阵报表中显示（如记录的小时数和实际成本）。

但是，其他列（如状态）仍可以在矩阵报表中显示，如下图所示：\
![](assets/report-matrix-status-350x73.png)

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

## 设置矩阵报表

1. 创建在报表输出中包含数值数据的传统报表。\
   有关如何创建报表的信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 转到在步骤1中创建的报表，单击 **报表操作**，然后选择 **编辑**.

1. （视情况而定）如果您已经创建了一个视图，并且希望将其应用于此报表，请单击 **应用现有视图**，然后从下拉列表中选择视图。
1. （视情况而定）如果要为报表创建新视图，请完成以下步骤：

   1. 单击 **列（视图）** 选项卡，然后选择要在矩阵报表中汇总的列。
   1. 在 **列设置** 区域，单击 **按以下方式汇总此列** 下拉列表中，然后选择用于汇总信息的可用选项之一。

      >[!IMPORTANT]
      >
      >如果未选择此选项，则列中的信息无法在矩阵报表中正确显示。

      ![](assets/qs-report-matrix-summarized-350x392.png)

   1. 在“列（视图）”选项卡中对每列重复此过程，然后单击 **完成**.

1. 单击 **分组** 选项卡。
1. （视情况而定）如果您已创建分组并且希望将其应用于此报表，请单击 **应用现有分组**，然后从下拉列表中选择分组。
1. （视情况而定）如果要为报表创建新矩阵分组，请完成以下步骤：

   1. 选择 **切换到矩阵分组** 中。
   1. 在 **行分组** 部分，确定行分组，该分组建立表的水平分组。
   1. （可选）要添加附加行分组，请单击 **添加辅助行分组**.
   1. 在 **列分组** 部分，确定列分组，以建立表的垂直分组。
   1. （可选）要添加附加列分组，请单击 **添加次列分组**.
   1. （视情况而定）如果您按日期添加分组，还应指定结果是按日、周、月、季度还是年进行分组。\
      ![](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)

   1. （视情况而定）如果您选择按日期分组并按季度显示结果，例如，通过选择 **显示没有结果的季度** 复选框。\
      ![](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >的 **显示没有结果的季度** 字段仅可用于矩阵分组，而不适用于标准分组。\
      >只有没有数据的季度（具有有效数据的季度介于两个季度之间）才会在矩阵选项卡中为数据值显示零。 没有数据的季度（位于过滤器选择的时间范围的开始和结束）根本不会显示在矩阵分组中。 没有结果的季度将不会显示在报表详细信息选项卡的分组中。

1. （可选和视情况而定）单击 **矩阵设置**，然后从以下选项中选择：\
   **显示记录计数：** 选择此选项可显示给定字段的条目总数为的行。\
   **显示值列：** 选择此选项可在矩阵中显示以下信息：

   * 记录计数
   * 值列

      >[!NOTE]
      >
      >此列包含描述每行数据表示内容的信息。\
      >在分组中聚合以下字段的值时，父对象（例如，父任务）会出现以下例外：
      >
      >   
      >   
      >   * 除“实际工时”(例如“计划/实际人工成本”、“计划/实际费用成本”、“计划/实际成本”、“计划/实际工时”之外的所有“数字”和“币种”字段仅汇总子任务和独立任务的值。 它们不会聚合父任务或父代父代的值。
      >   * 实际小时数汇总主要父任务和独立任务的值；它们不会聚合父任务或子任务的父任务的数字。
      >   * 数字和货币值的自定义数据字段聚合所有任务：父母、子女、父母的父母和独立任务。 如果您创建矩阵报表以在 **值** 列中，请注意，任何父对象（如父任务）的小时数或成本信息未显示在矩阵报表中。 要查看父对象的小时数，您必须查看 **详细信息** 选项卡。

   **条件规则：** 为汇总的值设置任何格式规则。\
   添加规则后，您可以定义字段和文本样式，以了解匹配该规则的字段的显示方式。 单击 **添加规则** 定义完规则后， **完成** 来保存规则。

1. 单击 **过滤器** 选项卡来定义将在报表中显示的信息。
1. （视情况而定）如果您已创建过滤器，并且希望将其应用于此报表，请单击 **应用现有过滤器**，然后从下拉列表中选择过滤器。
1. （视情况而定）如果要为此报表创建新过滤器，请参阅 [过滤器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   有关构建过滤器时可使用的各种限定符的信息。

1. 单击 **保存并关闭** 以保存和查看矩阵报表。

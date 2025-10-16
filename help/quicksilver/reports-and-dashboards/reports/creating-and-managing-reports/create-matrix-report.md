---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 创建矩阵报告
description: 矩阵报表以汇总表的格式显示摘要信息，因此与传统报表中的列表相比，更容易查看这些信息。
author: Nolan
feature: Reports and Dashboards
exl-id: 714f2802-089f-4a41-8205-f397cf474a24
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1083'
ht-degree: 0%

---

# 创建矩阵报告

矩阵报表以汇总表的格式显示摘要信息，因此与传统报表中的列表相比，更容易查看这些信息。

## 何时使用Matrix报告

可以为包含2个或更多分组的任何报表创建矩阵报表。 传统报表最多可包含3个分组，而矩阵报表最多可包含4个分组。

例如，要创建显示3个月期间记录的小时数的小时报告，并希望根据输入小时数的人员以及按月和按周组织报告。

![报告矩阵概述](assets/report-matrix-overview-350x123.png)

## 数据如何在矩阵报表中显示

矩阵报告中的信息始终显示为数值。 在大多数情况下，包含数值的列最适合在矩阵报表中显示（例如记录的小时数和实际成本）。

但是，其他列（如“状态”）仍可显示在矩阵报表中，如下图所示：\
![矩阵状态](assets/report-matrix-status-350x73.png)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
      <p>标准</p>
      <p>规划</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
 <td> <p>管理报表的权限</p></td>  
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 设置矩阵报表

1. 创建包含报表输出中数值数据的传统报表。\
   有关如何创建报告的信息，请参阅[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

1. 转到您在步骤1中创建的报告，单击&#x200B;**报告操作**，然后选择&#x200B;**编辑**。

1. （视情况而定）如果您已创建视图，并且要将其应用于此报表，请单击&#x200B;**应用现有视图**，然后从下拉列表中选择该视图。
1. （视情况而定）如果要为报表创建新的视图，请完成以下步骤：

   1. 单击&#x200B;**列（视图）**&#x200B;选项卡，然后选择要汇总到矩阵报表中的列。
   1. 在&#x200B;**列设置**&#x200B;区域中，单击&#x200B;**汇总此列**&#x200B;下拉列表，然后选择用于汇总信息的可用选项之一。

      >[!IMPORTANT]
      >
      >如果未选择此选项，则列中的信息在矩阵报表中无法正确显示。

      ![汇总的矩阵](assets/qs-report-matrix-summarized-350x392.png)

   1. 对“列（视图）”选项卡中的每一列重复此过程，然后单击&#x200B;**完成**。

1. 单击&#x200B;**分组**&#x200B;选项卡。
1. （视情况而定）如果已创建分组并且要将其应用于此报表，请单击&#x200B;**应用现有分组**，然后从下拉列表中选择分组。
1. （视情况而定）如果要为报告创建新的矩阵分组，请完成以下步骤：

   1. 选择生成器界面右上角的&#x200B;**切换到矩阵分组**。
   1. 在&#x200B;**行分组**&#x200B;部分中，标识用于建立表的水平分组的行分组。
   1. （可选）要添加额外的行分组，请单击&#x200B;**添加辅助行分组**。
   1. 在&#x200B;**列分组**&#x200B;部分中，标识用于建立表的垂直分组的列分组。
   1. （可选）要添加额外的列分组，请单击&#x200B;**添加辅助列分组**。
   1. （视情况而定）如果按日期添加分组，还应指定是否按天、周、月、季度或年对结果进行分组。\
      ![按日期分组选项](assets/qs-grouping-by-date-options-for-matrix-report-350x450.png)

   1. （视情况而定）如果您选择按日期分组并按季度显示结果，例如，通过选中&#x200B;**显示没有结果的季度**&#x200B;复选框，指定是否要显示没有数据的季度。\
      ![显示没有结果的季度](assets/qs-show-quarters-with-no-results-on-matrix-report-350x175.png)

      >[!NOTE]
      >
      >**显示没有结果的季度**&#x200B;字段仅适用于矩阵分组，不适用于标准分组。\
      >只有位于具有有效数据的两个季度之间的季度中没有数据，才会在matrix选项卡中显示数据值为零。 没有数据且位于过滤器选择的时间范围开始和结束的季度完全不出现在矩阵分组中。 没有结果的季度将不会在报告的“详细信息”选项卡上的分组中显示。

1. （可选且有条件）单击&#x200B;**矩阵设置**，然后从以下选项中进行选择：\
   **显示记录计数：**&#x200B;选择此选项可显示包含给定字段条目总数的行。\
   **显示值列：**&#x200B;选择此选项可在矩阵中显示以下信息：

   * 记录计数
   * “值”列

     >[!NOTE]
     >
     >此列包含的信息描述每行中的数据表示的内容。\
     >在分组中聚合以下字段的值时，以下例外适用于父对象（例如，父任务）：
     >
     >   
     >   
     >   * 除“实际小时数”（例如，“计划/实际劳力成本”、“计划/实际费用成本”、“计划/实际成本”、“计划小时数”）之外的所有数字和货币字段仅汇总子任务和独立任务的值。 它们不会聚合父任务的值或父任务的父值。
     >   * 实际小时数聚合主父级任务和独立任务的值；它们不会聚合父级任务或子级任务的父级任务的数量。
     >   * 数字和货币值的自定义数据字段汇总所有任务：父任务、子任务、父任务的父任务和独立任务。 如果您创建了矩阵报表，以在&#x200B;**值**&#x200B;列中显示计划小时数或实际小时数，请注意，任何父对象（如父任务）的小时数或成本信息都不会显示在矩阵报表中。 要查看父对象的小时数，必须查看&#x200B;**详细信息**&#x200B;选项卡。
     >   
     >   
     >

   **条件规则：**&#x200B;为聚合的值设置任何格式规则。\
   添加规则后，您可以定义字段和文本样式，以显示与该规则匹配的字段。 完成规则定义后，单击&#x200B;**添加规则**，然后单击&#x200B;**完成**&#x200B;以保存规则。

1. 单击&#x200B;**筛选器**&#x200B;选项卡以定义将在报告中显示的信息。
1. （视情况而定）如果已创建筛选器且要将其应用于此报表，请单击&#x200B;**应用现有筛选器**，然后从下拉列表中选择该筛选器。
1. （视情况而定）如果要为此报告创建新的筛选器，请参阅[筛选器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   and
   <a href="../../../reports-and-dashboards/reports/reporting-elements/advanced-filter-condition-qualifiers.md" class="MCXref xref">Advanced Filter and condition qualifiers </a>
   </MadCap:conditionalText>
   -->

   有关可在构建过滤器时使用的各种限定符的信息。

1. 单击&#x200B;**保存+关闭**&#x200B;以保存并查看矩阵报告。

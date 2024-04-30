---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: 查看图表以了解Adobe Workfront目标中的目标进度趋势
description: 您可以在Adobe Workfront目标的“图形”部分中查看目标的总体运行状况及其及时进度趋势。 此部分中的图表不会细分每个目标的进度，而是为您提供指定时间段内所有目标进度状态及其时间进度趋势的整体快照。
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 0%

---

# 查看图表以了解Adobe Workfront目标中的目标进度趋势

<!-- drafted mostly for P&P release-->

您可以在Adobe Workfront目标的“图形”部分中查看目标的总体运行状况及其及时进度趋势。 此部分中的图表不会细分每个目标的进度，而是为您提供指定时间段内所有目标进度状态及其时间进度趋势的整体快照。

>[!IMPORTANT]
>
>您可以在图形部分中，查看选定时间段内的目标总数。 但是，在计算整体目标进度状态和完成百分比时，Workfront目标只考虑状态为“活动”和“已关闭”的目标。

## 访问要求

您必须具有以下权限才能执行本文中所述的操作：

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> 
   <p>对于新计划和许可证结构：
  <ul><li>最终计划 </li>
  或
  <li>适用于Prime或Select Adobe Workfront计划的Adobe Workfront目标的附加许可证。 </li></ul> </p>
<p>对于当前计划和许可证结构： 
<ul><li> Pro或更高版本 </li>
  <li>除了Adobe Workfront许可证之外，还提供了Workfront目标许可证。</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront许可证*</td>
 <td>
 <p>新许可证：参与者或更高版本</p>
 或
 <p>当前许可证：请求或更高版本</p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">产品*</td>
 <td>
 <p> 新产品要求，为以下项之一： </p>
<ul>
<li>Select或Prime Adobe Workfront计划和其他Adobe Workfront Goals许可证。</li>
<li>默认包含Workfront目标的Ultimate Workfront计划。 </li></ul>
 <p>或</p>
 <p>当前产品要求： Workfront计划和Adobe Workfront Goals的附加许可证。 </p> <p>有关信息，请参阅 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront Goals的要求</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>访问级别</p></td>
 <td> <p>编辑对目标的访问权限</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">对象权限</td>
 <td>
  <div>
  <p>查看目标的权限或更高以查看目标</p>
  <p>管理目标的权限以编辑它</p>
  <p>有关共享目标的信息，请参阅 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目标中共享目标</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>必须为包括Workfront管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的目标区域。 </p>  
</td>
  </tr>
</tbody>
</table>

*有关详细信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Workfront目标中的图形类型

以下图表位于“图形”部分或Workfront目标中：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">目标运行状况图表</td> 
   <td> <p>显示以下内容的仪表图表：</p> 
    <ul> 
     <li>选定时间段的目标总数。 具有任何状态的目标都会被考虑。 </li> 
     <li>状态为“活动”和“已关闭”的目标进度状态。</li> 
    </ul> <p>有关Workfront Goals如何计算进度状态的信息，请参阅 <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Adobe Workfront目标中的目标进度和条件概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">目标进度图</td> 
   <td> <p>折线图可显示目标持续时间内，以每周增量为目标进行的更新。 目标进度图显示以下内容：</p> 
    <ul> 
     <li>选定时段内所有活动和已关闭目标的平均预期完成百分比和实际完成百分比。 完成百分比进度将划分为按节点标记的每周增量。 </li> 
     <li>自上周以来，活跃目标和已关闭目标的总体平均进度百分比。 </li> 
    </ul> <p>提示：当在所选时段以外对目标进行更新时，目标进度图可能不显示任何信息。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 在图形中查看目标进度

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) > **目标** 在右上角。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   这将打开Workfront目标区域。

1. 单击 **图形** 在左侧面板中。

   ![](assets/graphs-in-left-panel.png)

   此时将显示“图形”部分。

   默认情况下，“图形”部分中显示的目标受以下条件的限制：

   * 应用于“图形”区域的过滤器。
   * 处于“活动”和“草稿”状态的目标。

1. （可选）通过更新“图形”部分右上角的过滤器，选择要显示的信息类型。

   有关筛选目标的更多信息，请参阅 [在Adobe Workfront目标中过滤信息](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   >
   >如果选择显示多个时间段，则会显示每个时间段的运行状况图表（量规）以及进度图表（折线）。

1. 查看目标运行状况图表时，请查看下表中的信息。

   ![](assets/gauge-graph-wf-align-350x230.png)

   | 目标总数 | 图表底部的数字表示选定时段内所有目标的数量，以及所有选定状态中的目标数量。 |
   |---|---|
   | 平均完成百分比 | 在图表顶部，此数字表示在所选时段内活动目标和已关闭目标的平均完成百分比。 |
   | 目标及其进展 | 当您将鼠标悬停在图表的区段上时，每个进度状态区段的目标数。 只有状态为“活动”或“已关闭”的目标才会被计入区段中。 |


1. 查看目标进度表时，请查看下表中的信息。

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>基线进度</td> 
      <td>绿色斜线表示选定时间段内活动和已关闭目标的预期总体完成百分比平均值。 一个时期内的所有目标都预计会完成，因此基线进展在时期结束时始终是100%。 </td> 
     </tr> 
     <tr> 
      <td>实际进度</td> 
      <td> <p>蓝线表示选定时间段内活动目标和已关闭目标的实际总体完成百分比平均值（以周为增量）。 目标持续时间内的每一周均由行中的节点进行标记。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 将鼠标悬停在目标进度图中的周节点上，并查看以下内容：

   * **周日期**：所选周的月、日和年。
   * **进度**：选定周内所有目标的平均实际完成百分比。
   * **基线**：选定周内所有目标的预期完成百分比平均值。

1. （可选）单击 **进度** 在进度图底部删除实际总体进度线

   或

   单击 **基线** 在进度图底部删除预期进度。

 

---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: 在Adobe Workfront目标的目标列表中管理目标
description: 在您或其他用户创建目标后，可以在“目标列表”中查看其进度和信息。 有关创建目标的信息，请参阅在Adobe Workfront目标中创建目标。
author: Alina
feature: Workfront Goals
exl-id: 2a2c1240-f796-4cb8-b8a6-2ad5853916b9
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 2%

---

# 在Adobe Workfront目标的目标列表中管理目标

<!-- printing or exporting goals is no longer possible, but see if they add it later-->

在您或其他用户创建目标后，可以在“目标列表”中查看其进度和信息。 有关创建目标的信息，请参阅 [在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md).

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
 <td role="rowheader">访问级别</td>
 <td> <p>编辑对目标的访问权限</p>  </td>
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

## 管理目标列表中的目标

您可以在Workfront目标的以下部分中查看和管理目标：

* 目标列表
* 目标对齐方式

每个部分以略微不同的格式显示目标。 使用哪个部分取决于您在使用目标时想要达到的目的。

有关更多信息，请参阅 [Adobe Workfront目标部分概述](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

本文介绍了如何查看目标列表中的目标。

查看目标列表时，请考虑以下事项：

* 您可以查看自己或组织中的任何其他人在目标列表中创建的目标。 您必须具有目标的管理权限才能编辑目标。

<!--

### Manage the Goal List in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner, then click **Goals**.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List section displays by default. You can view goals regardless of their status, period, or owner, by default.

   The list of goals contains the following columns with information about each goal, result, or activity: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> 
       <div> 
        <p role="rowheader">Name </p> 
       </div> </td> 
      <td>The name of the goal, result, or activity.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Owner</td> 
      <td>The name of the goal, result, or activity owner. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Period</td> 
      <td>The time period for which the goal is scheduled.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress </td> 
      <td> <p>The progress indicator for the goal includes the following:</p> 
       <ul> 
      <li> <p>The progress label. </p> <p>For information, see <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Overview of goal progress and condition in Adobe Workfront Goals</a>. </p> </li> 
      <li> <p>The percent complete of the goal, activity, or result. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Status (includes alignment icon)</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
      <td> <p>The status of the goal which can be one of the following:</p> 
       <ul> 
        <li>Active</li> 
        <li>Draft</li> 
        <li>Inactive</li> 
        <li>Closed</li> 
       </ul> <p>For information about goal status, see <a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">Goal status overview in Adobe Workfront Goals</a>. </p> <p>The alignment icon appears on goals that are aligned to other goals. For information about aligning goals, see <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">Align goals by connecting them in Adobe Workfront Goals</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Use the filters in the upper-right corner of the goal list to select only goals that are important to you. For information about using filters in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md)
1. Click any of the fields in the column headers to sort it by that field.

   An arrow displays to the right of the field by which the list is sorted.

   ![](assets/goal-list-with-goal-expanded-+-result-+-activity-350x117.png)

1. (Optional) Click the field in the column again to sort the same column in a descending order. 
1. Click the right-pointing arrow to the left of the goal name to expand a goal

   Or

   Click the right-pointing arrow ![](assets/right-pointing-arrow.png) in the header of the list to expand all the goals in the list and view additional information about each goal, including any of the following:

   * Results names, owners, and progress

     For information about results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   
   * Activity names, owners, and progress

     For information about activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

1. Click the name of a goal to open the **Goal Details** panel on the right and review more information about the goal as well as manage it. For information about reviewing individual goals, see [Update goals in the Goal details section in Adobe Workfront Goals](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. (Optional) Expand the **Goals per page** drop-down menu and select from the following options to display additional goals:

   * 20  
      
      This is the default selection. 
   * 50
   * 100

1. Click **Print** to export a list of goals, results, and activities to a .pdf file.

   >[!TIP]
   >
   >* When printing a list of goals, the file produced contains only the information displayed on the screen. Items eliminated by filtering a list of goals do not display in the .pdf file.
   >* When you do not expand the goals in the list before printing the list, the .pdf file displays only goals without their results and activities.

   For more information, see [Print the Goal List in Adobe Workfront Goals](../../workfront-goals/goal-management/print-the-goal-list.md). 

1. Click the **Alignment icon** ![](assets/align-icon.png) next to an aligned to open the goal's card in the Goal Alignment section. For more information, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).
-->

要管理“目标列表”中的目标，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png)  图标，然后单击 **目标**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   默认情况下，将显示“目标列表”部分。 默认情况下，您可以查看目标，而不考虑其状态、时段或所有者。

   目标列表包含以下字段，其中包含有关每个目标的信息：

   * **名称**：目标的名称。
   * **所有者**：目标所有者的名称。
   * **期间**：计划目标的时间段。
   * **状态**：目标的状态可以是以下状态之一：
      * 活动
      * 草稿
      * 非活动
      * 已关闭

     有关目标状态的信息，请参阅 [Adobe Workfront目标中的目标状态概述](../goal-management/goal-status-overview.md).

     对齐图标显示在与其他目标对齐的目标上。 有关对齐目标的信息，请参阅 [通过在Adobe Workfront目标中连接目标来调整目标](../goal-alignment/align-goals-by-connecting-them.md).

   * **条件**：目标在为目标分配完成的时段内进度的可视化表示形式。

     目标的条件可以是以下任一条件：

      * 新建
      * 准时
      * 处于风险中
      * 存在问题

     有关目标条件的信息，请参阅 [Adobe Workfront目标中的目标进度和条件概述](../goal-management/calculate-goal-progress.md).

   * **进度**：目标的进度指示器，以百分比值表示。 进度指示器的颜色与目标条件的颜色相匹配。

     有关信息，请参阅 [在Adobe Workfront目标中计算目标进度](../goal-management/calculate-goal-progress.md).

1. 单击过滤器图标 ![](assets/filter-icon.png) 位置设置筛选条件，以仅显示对您而言重要的目标。

   有关在Workfront目标中使用过滤器的信息，请参阅 [在Adobe Workfront目标中过滤信息](../goal-management/filter-information-wf-goals.md).

1. 单击列标题中的任何字段，以按该字段对列表进行排序。
字段右侧显示一个箭头，按此箭头对列表进行排序。

1. （可选）再次单击列中的字段以对同一列进行降序排序。
1. 单击目标的名称以打开目标的页面。
1. 在列表中选择一个目标，然后单击列表顶部的以下选项之一：
   * **编辑** 图标 ![](assets/edit-icon.png) 以编辑有关目标的信息。 有关信息，请参阅 [在Adobe Workfront目标中编辑目标](../goal-management/edit-goals.md).
   * **共享** 图标 ![](assets/share-icon.png) 与其他人共享目标。 有关信息，请参阅 [在Adobe Workfront目标中共享目标](../workfront-goals-settings/share-a-goal.md).
   * **打开对齐方式** 图标 ![](assets/align-icon-unshimmed.png) 以打开“目标对齐方式”区域。 仅当所选目标与其他目标对齐时，才会显示此选项。
   * **删除** 图标 ![](assets/delete-icon.png) 要删除目标，请单击 **删除** 以确认。  有关信息，请参阅 [删除和停用Adobe Workfront目标中的目标](../goal-management/delete-and-deactivate-goals.md).






---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: 查看图表以了解Adobe Workfront目标中的目标进度趋势
description: 您可以在Adobe Workfront目标的图形部分中及时查看目标的整体运行状况及其进度趋势。 本节中的图表不会划分每个目标的进度，而是会为您提供所有目标的进度状态及其在指定时间段内的进度趋势的整体快照。
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 3989903687f2ea64ebd5ad754119ce1a9d70b9f3
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# 查看图表以了解Adobe Workfront目标中的目标进度趋势

<!-- drafted mostly for P&P release-->

您可以在Adobe Workfront目标的图形部分中及时查看目标的整体运行状况及其进度趋势。 本节中的图表不会划分每个目标的进度，而是会为您提供所有目标的进度状态及其在指定时间段内的进度趋势的整体快照。

>[!IMPORTANT]
>
>您可以在图形部分查看选定时间段内目标的总计数。 但是，在计算总体目标进度状态和完成百分比时，Workfront目标仅考虑状态为“活动”和“已关闭”的目标。

## 访问要求

<!--drafted for P&P release: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>

-->

您必须具有以下访问权限才能执行本文中描述的操作：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求或更高版本</p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td> <p>您必须为Adobe Workfront目标购买额外的许可证才能访问本文所述的功能。 </p> <p>有关信息，请参阅 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目标的要求</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>查看或更高权限访问目标</p> <p><b>注释</b><p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅：</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">授予对Adobe Workfront目标的访问权限</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象权限</td> 
   <td> 
    <div> 
     <p>查看或更高权限</p> 
     <p>有关共享目标的信息，请参阅 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目标中共享目标</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须具备以下条件：

* 包含主菜单中“目标”区域的布局模板。

## Workfront目标中的图表类型

图形部分或Workfront目标中提供了以下图表：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">目标运行状况图</td> 
   <td> <p>一个量规图，显示以下内容：</p> 
    <ul> 
     <li>选定时间段内的目标总数。 考虑任何状态的目标。 </li> 
     <li>状态为“活动”和“已关闭”的目标的进度状态。</li> 
    </ul> <p>有关Workfront Target如何计算进度状态的信息，请参阅 <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Adobe Workfront目标中的目标进度和条件概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">目标进度图</td> 
   <td> <p>一个折线图，用于在目标持续期间以每周增量显示对目标所做的更新。 目标进度图显示以下内容：</p> 
    <ul> 
     <li>选定时段内所有活动目标和已结束目标的平均预期和实际完成百分比。 完成进度百分比按节点标记的每周增量进行划分。 </li> 
     <li>自上一周以来，活动目标和已结束目标的总体平均进度百分比。 </li> 
    </ul> <p>提示：当在选定的时间段以外对目标进行更新时，目标进度图可能不会显示任何信息。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 查看图形中的目标进度

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) > **目标** 中。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   这将打开Workfront目标区域。

1. 单击 **图形** 中。

   ![](assets/graphs-in-left-panel.png)

   此时将显示图形部分。

   默认情况下，图形部分中显示的目标受以下条件的限制：

   * 应用于图形区域的过滤器。
   * 处于“活动”和“草稿”状态的目标。

1. （可选）通过更新图表部分右上角的过滤器，选择要显示的信息类型。

   有关筛选目标的更多信息，请参阅 [在Adobe Workfront目标中筛选信息](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   如果选择显示多个时间段，则将显示每个时间段的运行状况图（量规）和进度图（折线）。

1. 查看目标运行状况图时，请查看下表中的信息。

   ![](assets/gauge-graph-wf-align-350x230.png)

   | 目标总数 | 图表底部的数字表示选定时段内所有目标（处于您选择的所有状态）的数量。 |
   |---|---|
   | 平均完成百分比 | 在图表顶部，此数字表示选定时间段内活动目标和已结束目标的平均完成百分比。 |
   | 目标及其进展 | 将鼠标悬停在图表的区段上时，每个进度状态区段的目标数。 只有处于“活动”或“已关闭”状态的目标才会计入区段。 |


1. 查看目标进度图时，请查看下表中的信息。

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>基线进度</td> 
      <td>绿色斜率线表示选定时间段内活动目标和已结束目标的预期总体完成百分比平均值。 预期一个时段内的所有目标都将完成，因此基准进度在时段结束时始终为100%。 </td> 
     </tr> 
     <tr> 
      <td>实际进度</td> 
      <td> <p>蓝线以每周增量指示选定时间段内活动目标和已结束目标的实际总体完成百分比平均值。 目标持续期间的每周都由行中的节点进行标记。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在目标进度图中将鼠标悬停在周节点上，并查看以下内容：

   * **周日期**:选定周的月、日和年。
   * **进度**:选定周内所有目标实际完成百分比的平均值。
   * **基线**:选定周内所有目标的预期完成百分比平均值。

1. （可选）单击 **进度** 在进度图的底部，以删除实际的整体进度线

   或

   单击 **基线** ，以从图表中删除预期进度。

 

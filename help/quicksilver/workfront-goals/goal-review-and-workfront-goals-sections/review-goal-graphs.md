---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: 查看图形以了解Adobe Workfront目标中的目标进度趋势
description: 您可以在Adobe Workfront目标的“图形”部分中查看目标的总体运行状况及其及时进度趋势。 此部分中的图表不会细分每个目标的进度，而是为您提供指定时间段内所有目标进度状态及其时间进度趋势的整体快照。
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 0%

---

# 查看图表以了解Adobe Workfront目标中的目标进度趋势

<!--Audited for P&P only: 4/2025-->

您可以在Adobe Workfront目标的“图形”部分中查看目标的总体运行状况及其及时进度趋势。 此部分中的图表不会细分每个目标的进度，而是为您提供指定时间段内所有目标进度状态及其时间进度趋势的整体快照。

>[!IMPORTANT]
>
>您可以在图形部分中，查看选定时间段内的目标总数。 但是，在计算整体目标进度状态和完成百分比时，Workfront目标只考虑状态为“活动”和“已关闭”的目标。

## 访问要求

>[!NOTE]
>
>如果您的公司以前购买过此包，则可能会选择继续使用Adobe Workfront Goals。 有关详细信息，请与您的客户代表联系。
>
>Adobe Workfront目标不再可供购买。

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront包</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront许可证</td>
 <td>
 <p>参与者或更高版本</p>
<p>请求或更高版本</p></td>
 </tr>
  <tr>
 <td role="rowheader">访问级别配置</td>
 <td> <p>编辑对目标的访问权限</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">对象权限</td>
 <td>
  <div>
  <p>查看目标的权限或更高以查看目标</p>
  <p>管理目标的权限以编辑它</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>版面模板</p></td>
   <td> <p>必须为包括系统管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的目标区域。 </p>  
</td>
  </tr>
</tbody>
</table>

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
    <p> New product requirement: Workfront</p>
    Or
    <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p> </td>
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
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

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
    </ul> <p>有关Workfront目标如何计算进度状态的信息，请参阅<a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Adobe Workfront目标中的目标进度和条件概述</a>。</p> </td> 
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

1. 单击右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png) > **目标**。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   这将打开Workfront目标区域。

1. 单击左侧面板中的&#x200B;**图形**。

   左侧面板中的![图形](assets/graphs-in-left-panel.png)

   此时将显示“图形”部分。

   默认情况下，“图形”部分中显示的目标受以下条件的限制：

   * 应用于“图形”区域的过滤器。
   * 处于“活动”和“草稿”状态的目标。

1. （可选）通过更新“图形”部分右上角的过滤器，选择要显示的信息类型。

   有关筛选目标的更多信息，请参阅[在Adobe Workfront目标中筛选信息](../../workfront-goals/goal-management/filter-information-wf-goals.md)。

   >[!TIP]
   >
   >如果选择显示多个时间段，则会显示每个时间段的运行状况图表（量规）以及进度图表（折线）。

1. 查看目标运行状况图表时，请查看下表中的信息。

   ![量规图](assets/gauge-graph-wf-align-350x230.png)

   | 目标总数 | 图表底部的数字表示选定时段内所有目标的数量，以及所有选定状态中的目标数量。 |
   |---|---|
   | 平均完成百分比 | 在图表顶部，此数字表示在所选时段内活动目标和已关闭目标的平均完成百分比。 |
   | 目标及其进展 | 当您将鼠标悬停在图表的区段上时，每个进度状态区段的目标数。 只有状态为“活动”或“已关闭”的目标才会被计入区段中。 |


1. 查看目标进度表时，请查看下表中的信息。

   ![折线图](assets/line-graph-wf-align-350x161.png)

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

   * **周日期**：选定周的月、日和年。
   * **进度**：所选周所有目标的实际完成百分比的平均值。
   * **基线**：选定周内所有目标的预期完成百分比的平均值。

1. （可选）单击进度图底部的&#x200B;**进度**&#x200B;以删除实际的总体进度线

   或

   单击进度图底部的&#x200B;**基线**&#x200B;以从图表中删除预期的进度。

 

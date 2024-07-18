---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 在Adobe Workfront目标中的目标对齐部分中进行导航
description: 使用“目标对齐方式”部分可在流程图中显示整个组织的目标对齐方式的整体视图。 对齐的目标显示在分层树中互连的卡上。
author: Alina
feature: Workfront Goals
exl-id: e79ced31-4680-4af7-b083-3d615c747af8
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 1%

---

# 在Adobe Workfront目标中的目标对齐部分中进行导航

使用“目标对齐方式”部分可在流程图中显示整个组织的目标对齐方式的整体视图。 对齐的目标显示在分层树中互连的卡上。

有关目标对齐以及如何实现目标对齐的信息，另请参阅以下文章：

* Adobe Workfront目标中的[目标对齐概述](../../workfront-goals/goal-alignment/goal-alignment-overview.md)
* [通过在Adobe Workfront目标中连接目标来调整目标](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)

## 访问要求

您必须具备以下条件才能执行本文中所述的活动：

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront计划</td>
<td>
<p>任何</p>

</td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront许可证*</td>
<td>
<p>新许可证：参与者或更高版本</p>
或
<p>当前许可证：请求或更高版本</p>  </td>
</tr>
<tr>
<td role="rowheader">产品*</td>
<td>
<p> 新产品要求，为以下项之一： </p>
<ul>
<li>Select或Prime Adobe Workfront计划和其他Adobe Workfront Goals许可证。</li>
<li>默认包含Workfront目标的Ultimate Workfront计划。 </li></ul>
<p>或</p>
<p>当前产品要求： Workfront计划和Adobe Workfront Goals的附加许可证。 </p> <p>有关信息，请参阅<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目标的要求</a>。 </p> </td>
</tr>
<tr>
<td role="rowheader">访问级别</td>
<td> <p>编辑对目标的访问权限</p> </td>
</tr>
<tr data-mc-conditions="">
<td role="rowheader">对象权限</td>
<td>
<div>
<p>查看目标的权限或更高以查看目标</p>
<p>管理目标的权限以编辑它</p>
<p>有关共享目标的信息，请参阅<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目标中共享目标</a>。 </p>
</div> </td>
</tr>
<tr>
<td role="rowheader"><p>布局模板</p></td>
<td> <p>必须为包括Workfront管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的目标区域。 </p>  
</td>
</tr>
</tbody>
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 导航到目标对齐方式部分

1. 单击屏幕右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](../goal-alignment/assets/dots-main-menu-icon.png)，然后单击&#x200B;**目标**。
   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-alignment/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. 单击左侧面板中的&#x200B;**目标对齐方式**。
1. 使用对齐图表右上角的过滤器，仅选择对您很重要的目标。 有关在Workfront目标中使用过滤器的信息，请参阅[Adobe Workfront目标中的过滤信息](../../workfront-goals/goal-management/filter-information-wf-goals.md)。

   与筛选器匹配的目标会在卡片上的对齐图表中显示。

   目标信息卡上会显示以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">时间段日期 </td> 
      <td> <p>这是打开目标的时段。 目标必须在期间的结束日期之前实现。 Workfront目标根据目标期间的持续时间和当前日期计算目标进度。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">进度指示器</td> 
      <td>目标的进度指示器的数量。 进度指标可以是一致的目标、结果或活动。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有者名称</td> 
      <td>指定为目标所有者的用户、团队、组或组织的名称。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">目标名称</td> 
      <td>目标的名称。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">目标进度条<span>和进度</span></td> 
      <td> <p>目标进度指示当前已实现目标的程度。 这是根据自目标时间段开始以来经过的时间，自动计算所有瞄准的目标、结果和目标活动的平均进度。 有关计算目标进度的信息，请参阅<a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Adobe Workfront目标中的目标进度和条件概述</a>。 </p> 
       <div> 
        <p>到当前日期的目标实际进度。 以下进度值和颜色指示按时实现目标的可能性： </p> 
        <ul> 
         <li><span>准时</span>（绿色指示器）：目标准时，将准时实现。</li> 
         <li> <span>处于风险中</span>（黄色指示器）：目标进度落后，可能无法按时实现。</li> 
         <li> <span>存在问题</span> （红色指示器）：目标有无法按时实现的危险。 </li> 
        </ul> 
       </div> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Updated on date </td> 
       <td> <p>The date when the goal was last updated</p> <p>(NOTE: drafted because I think this was removed with the alignment chart redesign - 21.1) </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">状态</td> 
      <td><span>所有状态下的目标都会显示在“目标对齐方式”部分中。</span> </td> 
     </tr> 
    </tbody> 
   </table>

   与其他目标一致的目标会在目标卡下显示一致的目标数。

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

1. 单击目标下方的&#x200B;**向下箭头**&#x200B;图标可进一步展开并查看子目标。

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

   >[!TIP]
   >
   >将儿童目标与其对齐的目标会在各自的卡片下显示对齐的目标数。

1. （视情况而定）如果当前过滤器不包括参与对齐的某些目标，则会显示一条警告消息，指示并非所有目标都会显示。

   ![](assets/parent-goal-excluded-by-filter-alignment-section-350x230.png)

1. 单击&#x200B;**显示它们**&#x200B;以显示筛选器当前消除的目标。

   请注意对齐图中的以下更改：

   * 以前通过过滤器消除的已连接目标现在显示在对齐图表中。
   * 右上角的过滤器以黄色列出，表示当前未应用该过滤器。

     ![](assets/reapply-filter-link-and-yellow-filter-highlight-350x120.png)

     重新应用过滤器链接显示在过滤器名称的左侧。

1. （可选）单击&#x200B;**重新应用筛选器**&#x200B;以返回原始结果并显示目标层次结构。
1. （可选）将鼠标悬停在进度指示器上以了解当天的目标进度在哪里。

   ![](assets/progress-mouse-over-alignment-chart-350x163.png)

   将显示以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">截至今天</td> 
      <td>进度状态始终为最新状态。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>实际</span> </td> 
      <td>按当前日期计算的目标实际进度（百分比），计算方法是考虑目标上的所有进度指标。 目标进度指标是相一致的目标、活动和结果。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">预期</td> 
      <td> <p>当前日期之前目标的预期进度（百分比），假设您将按时实现目标。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击目标卡以打开目标页面。 有关编辑现有目标的信息，请参阅[在Adobe Workfront目标中编辑目标](../../workfront-goals/goal-management/edit-goals.md)。 有关更新目标进度的信息，请参阅[在Adobe Workfront目标中更新目标进度](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md)。

1. 单击当前级别目标的向上箭头，以返回到图表层次结构中的上一级别。

   或

   （可选）单击&#x200B;**退出目标层次结构**&#x200B;以显示与当前筛选器匹配的所有目标的卡片，而不显示它们彼此的连接。



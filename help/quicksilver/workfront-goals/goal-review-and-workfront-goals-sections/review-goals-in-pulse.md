---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: 查看Adobe Workfront目标脉冲部分中的目标
description: 无论所有者是谁，您都可以查看组织中的所有目标。 有关创建目标的信息，请参阅在Adobe Workfront目标中创建目标。
author: Alina
feature: Workfront Goals
exl-id: 33873797-183d-4efc-9099-26eb907ca799
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 1%

---

# 查看Adobe Workfront目标脉冲部分中的目标

>[!IMPORTANT]
> 
>从23.1版本开始，本文中描述的功能已从Workfront中删除。\
>2023年初23.1版发布后不久，也将删除本文。 此时，我们建议您相应地更新任何书签。


无论所有者是谁，您都可以查看组织中的所有目标。 有关创建目标的信息，请参阅 [在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md).

您可以将Adobe Workfront目标的“脉冲”部分用作协作工具，在该工具中，您可以查看并参与属于您、您的团队、组或组织的有关当前目标的一系列更新，并确保目标保持为最新。 Workfront目标在“脉冲”部分按目标对进度更新、评论和编辑历史记录进行分组。

## 访问要求

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
   <td> <p>查看或更高权限访问目标</p> <p>注释:  <p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅：</p> 
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

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须具备以下条件：

* 包含主菜单中“目标”区域的布局模板。

## 在Pulse部分中管理目标更新和注释 

>[!TIP]
>
>只有至少已签入一次的目标才会显示在“脉冲”部分中。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) > **目标** 的位置。

   这将打开Workfront目标区域。

   默认情况下，将显示所有目标。

1. 单击 **脉冲** 中。

   <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      (NOTE: see the numbering in the procedure)
      </MadCap:conditionalText>
      -->

   随即会显示目标列表。 该列表包含以下列，其中包含有关每个目标的信息：

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">目标</td> 
         <td>目标名称。</td> 
      </tr> 
      <tr> 
         <td role="rowheader">所有者</td> 
         <td>目标所有者的名称。</td> 
      </tr> 
      <tr> 
         <td role="rowheader">期间</td> 
         <td>计划目标的时间段。</td> 
      </tr> 
      <tr> 
         <td role="rowheader">进度</td> 
         <td>目标的进度指示器，通常为百分比值。</td> 
      </tr> 
      <tr> 
         <td role="rowheader"> <p>状态（包括对齐图标）</p> <p> <img src="assets/alignment-icon-large.png"> </p> </td> 
         <td> <p>目标的状态，可以是以下任一状态：</p> 
         <ul> 
         <li>活动</li> 
         <li>草稿</li> 
         <li>非活动</li> 
         <li>已关闭</li> 
         </ul> <p>对齐图标显示在与其他目标对齐的目标上。 有关协调目标的信息，请参阅 <a href="../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md" class="MCXref xref">在Adobe Workfront目标中通过将目标连接起来来调整目标</a>.</p>

   <p>“状态”列还包含对每个结果或活动进行的增量更新，以及对目标进行的每次签入。</p>

   例如，如果目标有一个手动进度条活动，并且您登入该目标并将活动更新为50%，则“状态”列会为该目标的活动显示50%。 稍后，您可以将同一活动更新为60%。 在这种情况下，同一活动的同一目标下会显示一行新的10% — 因为您刚刚为活动进度添加了10%。
   </td>
   </tr> 
      </tbody> 
      </table>

1. （可选）通过更新Pulse部分右上角的过滤器，选择要显示的信息类型。

   “脉冲”(Pulse)列表显示符合选定过滤器标准的目标及其更新历史记录。

   有关筛选目标的更多信息，请参阅 [在Adobe Workfront目标中筛选信息](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. 单击目标名称左侧的向右箭头可展开目标并查看有关每个目标更新的其他信息。

   以下信息显示在每个目标下的“脉冲”部分：

   * 结果名称和所有者。 有关结果的信息，请参阅 [将结果添加到Adobe Workfront目标中的目标](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   * 活动名称和所有者。 有关活动的信息，请参阅 [将活动添加到Adobe Workfront目标中的目标](../../workfront-goals/results-and-activities/add-activities-to-goals.md).
   * 结果和活动进度栏和进度状态。 有关Workfront Target如何计算目标进度的信息，请参阅 [Adobe Workfront目标中的目标进度和条件概述](../../workfront-goals/goal-management/calculate-goal-progress.md).

1. 单击 **添加评论** 要为目标添加评论，请单击 **帖子**. 注释显示在签入区域，以及“目标详细信息”面板的“更新”选项卡中。 我们建议您使用“脉冲”部分对一段时间内未更新的目标进行评论，并请求目标所有者进行更新。

1. （可选）单击 **显示所有更新** 以显示所有目标更新。 此操作将打开右侧目标详细信息面板中的更新选项卡。
1. 单击目标的名称以打开 **目标详细信息** 右侧面板，查看有关目标的更多信息，以及管理目标及其结果和活动。 有关审核单个目标的信息，请参阅 [更新Adobe Workfront目标中“目标详细信息”部分中的目标](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
1. （可选和视情况而定）单击 **对齐图标** ![](assets/align-icon.png) ，以在“目标对齐”部分中打开目标（如果目标与其他目标一致）。

1. （可选）将 **每页目标数** 下拉菜单，然后从以下选项中选择以显示其他目标：

   * 20. 这是默认选项。
   * 50
   * 100



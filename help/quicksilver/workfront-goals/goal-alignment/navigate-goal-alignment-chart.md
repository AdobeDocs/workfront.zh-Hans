---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: 导航Adobe Workfront Target中的“目标对齐”部分
description: 使用“目标对齐”部分在流程图中显示整个组织的目标对齐的整体视图。 对齐目标显示在分层树中互连的卡上。
author: Alina
feature: Workfront Goals
exl-id: e79ced31-4680-4af7-b083-3d615c747af8
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '933'
ht-degree: 1%

---

# 导航Adobe Workfront Target中的“目标对齐”部分

使用“目标对齐”部分在流程图中显示整个组织的目标对齐的整体视图。 对齐目标显示在分层树中互连的卡上。

有关目标一致性以及如何实现目标的信息，另请参阅以下文章：

* [Adobe Workfront目标中的目标协调概述](../../workfront-goals/goal-alignment/goal-alignment-overview.md)
* [在Adobe Workfront目标中通过将目标连接起来来调整目标](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)

## 访问要求

<!-- drafted for P&P release: 

You must have the following to perform the activities described in this article:

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

您必须具备以下条件才能执行本文中描述的活动：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">AdobeWorkfrontlicense*</td> 
   <td> <p>请求或更高版本</p> <p>有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td> <p>您必须为Adobe Workfront目标购买额外的许可证才能访问本文所述的功能。 </p> <p>有关信息，请参阅 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目标的要求</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对目标的访问权限</p> <p><b>注释</b><p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅：</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">授予对Adobe Workfront目标的访问权限</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象权限</td> 
   <td> 
    <div> 
     <p>查看或更高对目标的权限</p> 
     <p>有关共享目标的信息，请参阅 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目标中共享目标</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须具备以下条件：

* 包含主菜单中“目标”区域的布局模板。

## 导航目标对齐部分

1. 单击 **主菜单** 图标 ![主菜单图标](../goal-alignment/assets/dots-main-menu-icon.png) ，然后单击 **目标**.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-alignment/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. 单击 **目标对齐** 中。
1. 使用对齐图表右上角的过滤器，只选择对您而言重要的目标。 有关在Workfront目标中使用过滤器的信息，请参阅 [在Adobe Workfront目标中筛选信息](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   与过滤器匹配的目标将显示在卡片上的对齐图表中。

   目标卡片上会显示以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">时间段日期 </td> 
      <td> <p>这是目标打开的时段。 该目标必须在期终日之前实现。 Workfront目标根据目标期间的持续时间和当前日期计算目标的进度。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">进度指示器</td> 
      <td>目标的进度指标数。 进度指标可以是目标、结果或活动的一致。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有者姓名</td> 
      <td>指定为目标所有者的用户、团队、组或组织的名称。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">目标名称</td> 
      <td>目标的名称。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">目标进度栏 <span>和进度</span></td> 
      <td> <p>目标进展表明目前已实现多少目标。 这是根据自目标时间段开始以来经过的时间自动计算目标所有已协调目标、结果和活动的平均进度。 有关计算目标进度的信息，请参阅 <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Adobe Workfront目标中的目标进度和条件概述</a>. </p> 
       <div> 
        <p>按当前日期确定目标的实际进度。 以下进度值和颜色指示目标按时实现的可能性： </p> 
        <ul> 
         <li><span>On Target</span> （绿色指示器）：目标按时完成，并将按时完成。</li> 
         <li> <span>面临风险</span> （黄色指示器）：目标落后，可能无法按时实现。</li> 
         <li> <span>遇到麻烦</span> （红色指示器）：这个目标有可能不能按时实现。 </li> 
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
      <td><span>处于所有状态的目标都会显示在“目标对齐”部分中。</span> </td> 
     </tr> 
    </tbody> 
   </table>

   与其他目标一致的目标在目标卡下显示一致目标的数量。

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

1. 单击 **向下箭头** 图标，以进一步展开和查看子项目标。

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

   >[!TIP]
   >
   >将子目标与子目标一致的目标在各自卡片下显示一致目标的数量。

1. （视情况而定）如果当前过滤器排除了参与对齐的某些目标，则会显示一条警告消息，指明并非所有目标都会显示。

   ![](assets/parent-goal-excluded-by-filter-alignment-section-350x230.png)

1. 单击 **给他们看** 以显示过滤器当前消除的目标。

   请注意对齐图表中的以下更改：

   * 过滤器之前消除的连接目标现在显示在对齐图表中。
   * 右上角的过滤器以黄色列出，表示当前未应用。

      ![](assets/reapply-filter-link-and-yellow-filter-highlight-350x120.png)

      过滤器名称的左侧会显示“重新应用”过滤器链接。

1. （可选）单击 **重新应用过滤器** 返回到原始结果并显示目标层次结构。
1. （可选）将鼠标悬停在进度指示器上，可了解当天的目标进度应在何处。

   ![](assets/progress-mouse-over-alignment-chart-350x163.png)

   将显示以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">截至今天</td> 
      <td>进度状态始终为最新。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>实际</span> </td> 
      <td>按当前日期计算的目标实际进度（百分比），其中考虑了目标的所有进度指标。 目标进度指标是目标、活动和结果的一致。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">预期</td> 
      <td> <p>目标的预期进度（百分比），按当前日期确定，假定您将按时实现目标。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击目标卡片以打开目标页面。 有关编辑现有目标的信息，请参阅 [在Adobe Workfront目标中编辑目标](../../workfront-goals/goal-management/edit-goals.md). 有关更新目标进度的信息，请参阅 [更新Adobe Workfront目标中的目标进度](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

1. 单击当前级别目标的向上箭头可返回到图表层次结构中的上一级别。

   或

   （可选）单击 **退出目标层次结构** 以显示与当前过滤器匹配的所有目标的卡片，而不显示它们彼此的连接。



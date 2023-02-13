---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目标中关闭并重新打开目标
description: 当您想要指示您已完成目标，或者由于目标已过时而不再使用该目标时，可以关闭目标。
author: Alina
feature: Workfront Goals
exl-id: bbb549c1-aea6-4f5e-8a6b-01fc04cf06ef
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# 在Adobe Workfront目标中关闭并重新打开目标

如果要指示以下内容，您可以关闭目标：

* 目标完成，原因可能是您实现了目标，或者是时间段过去了。
* 你不再在做这件事，也不打算在不久的将来做。

您可以重新打开已关闭的目标，以便它们重新变得相关。

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

您必须具备以下条件：

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
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对目标或更高版本的访问权限</p> <p><b>注释</b><p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅：</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">授予对Adobe Workfront目标的访问权限</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象权限</td> 
   <td> 
    <div> 
     <p>管理目标的权限</p> 
     <p>有关共享目标的信息，请参阅 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">在Workfront目标中共享目标</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须具备以下条件：

* 包含主菜单中“目标”区域的布局模板。

## 关闭或重新打开目标时的注意事项

* 您必须在访问级别拥有编辑目标的访问权限，然后才能关闭并重新打开目标。 有关授予对Goals的访问权限的信息，请参阅 [授予对Adobe Workfront目标的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).
* 您只能关闭活动目标。 无法关闭处于“草稿”状态的目标。

   有关目标状态的信息，请参阅 [Adobe Workfront目标中的目标状态概述](../../workfront-goals/goal-management/goal-status-overview.md).

* 关闭目标会锁定其进度，并允许您评估在完成目标方面做得如何。

   >[!CAUTION]
   >
   >在结束具有积极贡献目标的目标时，其进度在结束后会发生变化，以指示积极贡献目标的进度。 有关协调目标的信息，请参阅 [在Adobe Workfront目标中通过将目标连接起来来调整目标](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* 在您关闭目标之前，请更新目标的进度指标，以确保目标以准确的进度值结束。 如果已经实现了所有进展指标，则完成目标百分比应为100%，而您的目标已经实现。 有关更新目标的信息，请参阅 [更新Adobe Workfront目标中的目标进度](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).
* 请保留任何最终评论，以作为您关闭的目标的更新。 有关向目标添加评论的信息，请参阅 [在Adobe Workfront目标中管理目标注释](../../workfront-goals/goal-management/manage-goal-comments.md).
* 您无法再更新结束目标上的结果和活动进度。
* 如果要继续处理已关闭的目标，可以重新打开该目标。
* 如果目标尚未实现，请考虑将其大部分信息复制到下一个时间段（季度或年）。 对于从一个时间段到下一个时间段相同的目标或您可能需要努力在下一个时间段内实现的目标，这是一个很好的选项。 有关复制目标的信息，请参阅 [复制Adobe Workfront目标中的目标](../../workfront-goals/goal-management/copy-goals.md). 您还可以更新目标上的时间段，而不是将其复制到其他时间段。
* Workfront会在您重新打开已关闭的目标时删除该目标的注释。 如果必须保留注释，我们建议复制已关闭的目标，包括与其关联的任何结果，而不是将其重新打开。


## 关闭目标

<!--
Closing goals differs depending on what environment you use. 

### Close goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are active.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md). 

1. Click an active goal.

   The Goal Details panel displays on the right. 

1. (Optional and recommended) Click the **Updates** tab and add an update in the **Comment here** field about the reason you are closing the goal, then click **Post**. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Close** > **Close Goal**.

   This closes the goal and saves the current progress on the goal and its results and activities.

   >[!IMPORTANT]
   >
   >If the goal has contributing goals that are still active, the progress of the goal continues to update based on the progress of the aligned goals.
   >
   >
   >![](assets/closing-goals-with-active-aligned-goals-warning-350x71.png)   >
   >

1. (Optional) Modify your filters again to display only closed goals. The goals you closed display on the screen.
-->

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) > **目标** 中。

   随即会打开目标列表。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. （可选）修改过滤器，以仅显示处于活动状态的目标。

   有关在Workfront目标中过滤信息的信息，请参阅 [在Adobe Workfront目标中筛选信息](../goal-management/filter-information-wf-goals.md).
1. 单击活动目标。

   随即会打开目标页面。

   ![](assets/goal-page-unshimmed.png)
1. 单击 **更多** 菜单 ![](assets/more-icon.png) 在目标名称的右侧，单击 **关闭**.

   目标将关闭，此时您将在屏幕的右上角收到确认消息。

   ![](assets/goal-close-confirmation-with-add-closing-notes-link.png)

1. （可选）在确认框中，单击 **添加结束说明** 添加对此目标的评论以及您需要关闭此目标的原因。
1. 添加结束注释，然后单击 **添加注释**.

   ![](assets/add-closing-notes-box-unshimmed.png)

   注释显示在目标页面的“目标详细信息”部分的“结束注释”区域。

   >[!NOTE]
   >
   >如果您稍后重新打开已关闭的目标，Workfront将删除结束注释。


## 重新打开目标

如果您确定已关闭的目标已重新变得相关，并且您需要继续更新其进度，则可以重新打开这些目标。

<!--
Reopening goals differs depending on what environment you use.

### Reopen goals in the Production environment

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List opens. 

1. (Optional) Modify your filters to display only goals that are closed.

   For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).


1. Click a closed goal.

   This opens the Goal Details panel on the right. 

1. Click the **More icon** ![](assets/more-icon.png) to the right of the goal name, then click **Reopen** > **Reopen**.

   This reopens the goal and places it in a status of Active. The progress of the goal is recalculated starting with the current date. 

1. (Optional) Modify your filters again to display only active goals. The goals you opened display on the screen.

-->

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png)> **目标** 中。

   随即会打开目标列表。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. （可选）修改您的过滤器以仅显示已关闭的目标。

   有关在Workfront目标中过滤信息的信息，请参阅 [在Adobe Workfront目标中筛选信息](../goal-management/filter-information-wf-goals.md).
1. 单击已关闭目标的名称。

   随即会打开目标页面。
1. 单击 **更多** 菜单 ![](assets/more-icon.png) 目标名称的右侧， **重新打开** > **重新打开**.

   发生以下情况：
   * 目标现已打开，状态为“活动”。
   * 从当前日期开始，将重新计算目标进度。
   * 所有结束注释都将从“目标详细信息”页面中删除。 删除的结案笔记无法恢复。

1. （可选）再次修改过滤器，以仅显示活动目标。

   您打开的目标将显示在屏幕上。


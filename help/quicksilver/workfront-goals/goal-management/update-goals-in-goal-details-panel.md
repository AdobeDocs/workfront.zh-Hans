---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目标的“目标详细信息”部分中更新目标
description: 您可以通过访问目标详细信息面板来更新各个目标的信息。
author: Alina
feature: Workfront Goals
exl-id: e9df0d98-05a1-4977-b7f1-426b8f5b3eae
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 1%

---

# 在Adobe Workfront目标的“目标详细信息”部分中更新目标

<!--Audited for P&P only: 4/2025-->

您可以通过访问目标详细信息面板来更新各个目标的信息。

>[!NOTE]
>
>您无法更新状态为“已关闭”的目标。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

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
  <ul><li>Ultimate计划 </li></ul>
   </p>
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
 <p>当前许可证：请求或更高版本</p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>。</p> </td>
 </tr>
 <tr>
 <td role="rowheader">产品*</td>
 <td>
  <p> 新产品要求：Workfront</p>
  或
  <p>当前产品要求：除了Workfront许可证之外，您必须为Adobe Workfront Goals购买许可证。 </p> <p>有关信息，请参阅<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目标的要求</a>。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">访问级别*</td>
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
   <td role="rowheader"><p>版面模板</p></td>
   <td> <p>必须为包括Workfront管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的目标区域。 </p>  
</td>
  </tr>
</tbody>
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 更新目标详细信息部分中的目标

您可以从目标列表中访问单个目标。

<!--

Updating goals in the Goal Details panel differs depending on where you access the goal from. 

### Update goals in the Goal Details panel in the Production environment

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Goals area in Workfront. 

1. Click the name of a goal in the Goal List, then click the name of a goal.

   This opens the Goal Details panel on the right.
   ![Goal details summary](assets/goal-details-summary-tab-350x294.png)

   >[!TIP]
   >
   >You can also click the name of a goal in the Goal Alignment, Check-in, or Pulse sections. 
   >
   ><!-- drafted for goal redesign:
   >Add this to the TIP above with goal redesign: 
   >
   >The Check-in and Pulse sections have been removed from the Preview environment.
   >

1. On the Summary tab, click the **More icon** ![More icon](assets/more-icon.png), then click any of the following options:

   1. **Edit**. For information about editing goals, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
   1. **Copy**. For information about copying goals, see [Copy goals in Adobe Workfront Goals](../../workfront-goals/goal-management/copy-goals.md).
   1. **Activate**. This option is available only for drafted and inactive goals.

      For information about activating goals, see [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md). 
   
   1. **Close**, then click**Close Goal**. This option is available only for active goals.

      For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. **Deactivate**. This option is available only for active goals. This deactivates the goal immediately.

      For information about deactivating goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).
   
   1. **Delete**, then click **Yes, Delete**.

      For information about deleting goals, see [Delete and deactivate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/delete-and-deactivate-goals.md).

      >[!NOTE]
      >
      >Deleted goals cannot be recovered.

   1. **Reopen**, then click **Reopen**. This option is available only for closed goals that are from a current time period.

      For information about reopening goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   
   1. (Conditional) If you clicked any of the options between steps a-i above except Delete or Reopen, click **Save**.    
   
      (!--ensure this is accurate)--)

1. Click **Align to another goal** in the upper-right of the Summary tab, then specify the name of a goal in the **Align to** **another goal** field that you want to align the current goal to. The current goal becomes the child of the goal you align it to. For information about child and parent goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md). 
1. Click **Add results**. Results drive the progress of your goal. For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).

1. Click **Add activities**. Activities drive the progress of your goal. For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 

1. Click the **Updates** tab. Here, you can view goal comments and review the entire editing history of the goal, activities, and results, to understand who changed what and when.

   ![Goal details updates](assets/goal-details-updates-tab-350x280.png)

1. (Optional) Deselect any of the following options if you want to not display them in the Updates tab.&nbsp;They are selected by default: 

   | Option |Description  |
   |---|---|
   | Progress Updates |Displays information about the history of progress updates on results and activities.  |
   | Comments |Displays comments made by users on the goal.  |
   | Editing History |Displays information about creating and updating the goal, results, and activities.  |

1. (Optional) Click **Details** under a progress or an editing history update to display additional information about the update.

   ![Details in update tab](assets/update-details-in-updates-tab-expanded-highlighted-350x139.png)

-->



1. 单击目标列表中目标的名称，然后单击目标的名称。

   这将打开左侧的&#x200B;**目标详细信息**&#x200B;部分。

   ![目标页面](assets/goal-page-unshimmed.png)

1. 单击右上角的&#x200B;**编辑图标** ![编辑图标](assets/edit-icon.png)，然后单击&#x200B;**全部编辑**&#x200B;或&#x200B;**概述**

   或

   开始在“目标详细信息”部分的其中一个可编辑字段中键入信息。 该部分将变为可编辑。

   >[!IMPORTANT]
   >
   >并非所有显示在目标详细信息部分中的字段都可以编辑。 Workfront会计算某些字段，这些字段为只读。

1. 更新或查看以下字段：

   * **描述**：添加或更新有关目标的信息。
   * **进度**：指示到目前为止已完成目标的百分比。 您无法手动更新目标的进度。 目标进度是计算所有进度指标。
   * **条件**：指示目标是新目标且尚未更新、目标是按时完成还是延迟。 您无法更新目标的条件。 目标条件由Workfront自动计算。\
     有关目标条件和进度的更多信息，请参阅
     [Adobe Workfront目标中的目标进度和条件概述](../goal-management/calculate-goal-progress.md)。
   * **状态**：无法手动更新目标的状态。 有关详细信息，请参阅Adobe Workfront目标中的[目标状态概述](../goal-management/goal-status-overview.md)。
   * **目标所有者**：单击可更新目标所有者的名称。 开始键入用户、团队、组的名称或您的组织的名称，然后当它显示在列表中时将其选定。 一个目标只能有一个所有者。
   * **父目标**：开始键入要设置为所选目标的父目标的名称。 所选目标的进度将自动更新父目标的进度。

     >[!TIP]
     >
     >您无法更新以下有关父目标的信息：
     >    * 父目标期间
     >    * 父目标进度
     >    * 父目标所有者。
     >      
     >您必须更新有关父目标本身的此信息。

   * **时段**：单击以更新目标的时段\
     或\
     选择&#x200B;**启用自定义日期**&#x200B;以指定目标的&#x200B;**开始**&#x200B;和&#x200B;**结束日期**&#x200B;的日期。
   * **关闭注释**：此字段仅对状态为“已关闭”的目标可见。 无法编辑已关闭的目标。 重新打开已关闭的目标会永久删除关闭注释。



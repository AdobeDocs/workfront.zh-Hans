---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: 删除和停用Adobe Workfront目标中的目标
description: 当您开始处理某个目标时，如果它在您的组织中变得无关紧要，我们建议您停用它，而不是删除它。 停用目标会保留其历史信息，并让您有机会稍后重新激活它。 但是，有时删除目标可能比较合理，这样可以保持目标列表的准确性。
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# 删除和停用Adobe Workfront目标中的目标

当您开始处理某个目标时，如果它在您的组织中变得无关紧要，我们建议您停用它，而不是删除它。 停用目标会保留其历史信息，并让您有机会稍后重新激活它。 但是，有时删除目标可能比较合理，这样可以保持目标列表的准确性。

## 访问要求

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
 <p>当前许可证：请求或更高版本</p> </td>
 </tr>
 <tr>
 <td role="rowheader">产品*</td>
 <td>
 <p> 新产品要求，为以下项之一： </p>
<ul>
<li>Select或Prime Adobe Workfront计划和附加Adobe Workfront Goals许可证。</li>
<li>Ultimate Workfront计划，默认情况下包括Workfront目标。 </li></ul>
 <p>或</p>
 <p>当前产品要求： Workfront计划和Adobe Workfront Goals的附加许可证。 </p> <p>有关信息，请参阅<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目标的要求</a>。 </p> </td>
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

## 取消激活目标

您可以停用不再相关并且将来可能想要重新激活的目标。

* [停用目标时的注意事项](#considerations-when-deactivating-goals)
* [取消激活目标](#deactivate-goals)

### 停用目标时的注意事项

停用目标时，请记住以下事项：

* 您只能停用处于活动状态的目标。 有关激活目标的信息，请参阅[在Adobe Workfront目标中激活目标](../../workfront-goals/goal-management/activate-goals.md)。

  >[!TIP]
  >
  >您无法取消激活处于草稿状态的目标。

* Workfront停止计算已停用目标的进度。
* 非活动目标不再显示于Workfront目标上，或者在“图形”部分中将考虑这些目标。 有关Workfront目标图形的信息，请参阅[查看图形以了解Adobe Workfront目标中的目标进度趋势](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md)。

  <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* 您无法再对已停用的目标进行更新。
* 您可以编辑有关目标及其对齐方式的信息。
* 您可以重新激活之前已停用的目标。

### 取消激活目标

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Deactivate**.

   ![Deactivate goal](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

1. 单击右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**目标**。

   此时将显示目标列表。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

1. （可选）修改筛选器以仅显示处于活动状态的目标。

   有关在Workfront目标中过滤信息的信息，请参阅[在Adobe Workfront目标中过滤信息](../goal-management/filter-information-wf-goals.md)。

1. 单击活动目标。

   此时将打开目标页面。

   ![目标页面](assets/goal-page-unshimmed.png)

1. 单击目标名称右侧的&#x200B;**更多**&#x200B;菜单![更多图标](assets/more-icon.png)，然后单击&#x200B;**停用**。

1. 目标已停用，其状态变为不活动。

## 删除目标

您可以删除不再相关或可能不再相关的目标。

* [删除目标时的注意事项](#considerations-when-deleting-goals)
* [删除目标](#delete-goals)

### 删除目标时的注意事项 {#considerations-when-deleting-goals}

* 您可以删除任何状态下的目标，包括已关闭的目标。
* 无法恢复已删除的目标。
* 附加到目标的结果和手动进度条活动也会被删除。
* 不会删除与目标关联的项目，但会删除它们与目标的关联。

### 删除目标

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Delete**.

   ![Delete goal](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

1. 单击右上角的主菜单图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**目标**。

   此时将显示目标列表。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. 单击目标的名称。 这将打开目标页面。
1. 单击目标名称右侧的&#x200B;**更多**&#x200B;菜单![更多图标](assets/more-icon.png)，然后单击&#x200B;**删除目标**，然后单击&#x200B;**删除**。

   目标及其活动和结果也会被删除并且无法恢复。 不会删除与一个或多个子目标关联的项目。



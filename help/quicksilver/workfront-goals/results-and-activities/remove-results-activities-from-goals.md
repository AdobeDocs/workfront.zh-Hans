---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: 从Adobe Workfront目标中的目标删除进度指示器
description: 如果不再相关，您可以从Adobe Workfront目标中的目标删除结果、活动和项目。
author: Alina
feature: Workfront Goals
exl-id: 0e064dbd-6168-47b4-98ab-b5c0481e839e
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 0%

---

# 从Adobe Workfront目标中的目标删除进度指示器

<!-- for goal redesign PRODUCTION RELEASE: Should this article be called "Remove or disconnect progress indicators from goals" when this is available to ALL progress indicators (including "disconnect goals")-- if yes, updte the title everywhere else where this is linked?
-->

如果结果、活动和项目不再相关，您可以从目标中删除它们。

有关创建目标以及将结果和活动添加到目标的信息，请参阅以下文章：

* [在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md)
* [将活动添加到Adobe Workfront目标中的目标](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
* [将结果添加到Adobe Workfront目标中的目标](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [在Adobe Workfront目标中编辑结果和活动](../../workfront-goals/results-and-activities/edit-results-and-activities.md)

目标也可以与父目标一致，成为子目标。 子目标也是父目标的进度指示器。

您可以通过删除目标之间的连接来删除目标之间的对齐方式。 有关信息，请参阅[在Adobe Workfront目标中移除目标对齐方式](../goal-alignment/remove-goal-alignment.md)。

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
 <p>当前许可证：请求或更高版本</p> <p>有关详细信息，请参阅<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>。</p> </td>
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

## 先决条件

您必须有一个与结果、活动或项目关联的目标。

## 有关移除结果、活动以及从目标断开项目的注意事项

* 您只能从活动目标中删除结果和活动。
* 您可以通过删除结果和活动来从目标中删除它们。 无法恢复已删除的结果和活动。
* 从目标中删除结果或活动时，删除的结果或活动的进度会影响目标的整体进度。
* 您无法从目标中删除项目，但可以断开其与目标的连接。 通过将项目与目标断开连接，项目的完成百分比不再影响目标的进度。

  有关项目如何影响目标进度的信息，请参阅[在Adobe Workfront目标中添加项目](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md)。

* 您不能从目标中删除结果或活动，也不能断开子目标或项目的连接（如果它们是该目标的最后一个进度指示器）。
* 如果从项目区域删除了某个项目，并且该项目是目标的最后一个进度指示器，则该目标将变为非活动。

## 从目标中删除结果和活动

您可以通过删除结果和活动来从目标中删除它们。 从目标中删除结果和活动是相同的。

<!--
How you delete results and activities differs depending on the environment you use.

### Delete results and activities in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click **Results** to remove results or **Activities** to remove activities. 

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name, then click **Delete** > **Yes, delete**.

   ![](assets/delete-result-goal-details-350x108.png)

   The result or activity is deleted and cannot be recovered. The percent complete of the goal updates to exclude the deleted activity or result.

-->

1. 单击右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**目标**。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
   这将打开Workfront目标区域，默认情况下将显示目标列表。

1. 单击要从其中移除结果和活动的目标的名称。

   这将打开目标页面。

1. 单击左侧面板中的&#x200B;**进度指示器**。

1. 选择结果或活动，然后单击列表顶部的&#x200B;**删除**&#x200B;图标![](assets/delete-icon.png)。

1. 单击&#x200B;**删除**&#x200B;以确认删除。 结果或活动被删除，无法恢复。 目标的完成百分比将更新，以排除已删除的活动或结果。


## 从目标中删除项目

<!--
Dsconnecting projects from goals differs depending on the environment you use.

### Disconnect projects from goals in the Production environment


1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   (!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   This opens the Workfront Goals area and the Goal List displays by default. 

1. Click the name of a goal you want to remove results and activities from.

   This opens the Goal Details panel on the right.

1. Click the **right-pointing arrow** to the left of the Activities sections to expand it. 
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the project name, then click **Disconnect**.

   ![](assets/disconnect-project-goal-details-350x94.png)

   The project is disconnected from the goal. The percent complete of the goal updates to exclude the percent complete of the disconnected project.
-->


1. 单击右上角的&#x200B;**主菜单**&#x200B;图标，然后单击&#x200B;**目标**。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../results-and-activities/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   这将打开Workfront目标区域，默认情况下将显示目标列表。

1. 单击要从其中移除结果和活动的目标的名称。

   这将打开目标页面。
1. 单击左侧面板中的&#x200B;**进度指示器**。
1. 选择一个项目，然后单击列表顶部的&#x200B;**断开连接**&#x200B;图标![](assets/disconnect-icon.png)。
1. 单击&#x200B;**断开连接**&#x200B;以确认。

   项目不再连接到目标。 目标更新的完成百分比，用于排除断开连接的项目。


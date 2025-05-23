---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目标中访问和打开目标
description: 本文介绍了如何在Adobe Workfront中找到和管理目标。
author: Alina
feature: Workfront Goals
exl-id: a729f334-6ca4-4cf5-a3ef-01a7effb7153
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 1%

---

# 在Adobe Workfront目标中访问和打开目标

<!--Audited P&P only: 4/2025-->

本文介绍了如何在Adobe Workfront中找到和管理战略目标。


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
<p>或</p>
 <p>当前产品要求：除了Workfront许可证之外，您必须为Adobe Workfront Goals购买许可证。 </p> <p>有关信息，请参阅<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">使用Workfront目标的要求</a>。 </p> </td>
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
   <td role="rowheader"><p>版面模板</p></td>
   <td> <p>必须为包括Workfront管理员在内的所有用户分配一个布局模板，该模板应包括主菜单中的目标区域。 </p>  
</td>
  </tr>
 </tbody> 
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 访问Workfront目标

1. 单击右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**目标**。

   <!-- drafted for Shell release: Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   此时将显示“目标列表”。


   >[!IMPORTANT]
   >
   >   正确访问Workfront目标后，您可以查看自己或任何其他人在目标列表中创建的目标（默认情况下）。

   <!--   
   (NOTE: This might change when sharing is in place; right now, with sharing in place, they can VIEW all goals in the system but they cannot EDIT the ones others created!)
   -->

1. （可选）单击目标的名称以将其打开或编辑。

   或

   单击&#x200B;**新建目标**&#x200B;以添加新目标。

   有关创建目标的信息，请参阅[在Adobe Workfront目标中创建目标](../../workfront-goals/goal-management/create-goals.md)。

## 打开和管理各个目标

在管理目标时，必须访问单个目标才能执行以下操作：

* 编辑它
* 向其添加结果或活动
* 编辑与其关联的结果和活动
* 激活它
* 取消激活它
* 删除它
* 使其与另一个目标保持一致
* 将结果或活动转换为其他目标
* 更新它
<!--
Accessing goals differs depending on what environment you use.

To access an individual goal in the Production environment:

1. Click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Goals** .

     (!--drafted for Shell release: Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   --)

   The Goal List displays by default. 

1. Click the name of a goal in the list 

   Or

   Click one of the options below in the left panel, then click the name of a goal to access it:

   * Goal Alignment
   * Check-in 
   * Pulse 

   >[!NOTE]
   >
   >Depending on what action you want to perform on the individual goal, you might choose to select different sections every time. For information about the differences between the Workfront Goals sections, see [Overview of the Adobe Workfront Goals sections](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

   The Goal Details panel displays on the right. You can update the goal, its results, and activities in the Goal Details panel when you have access to manage it. For information about updating goals using the Goal Details panel, see [Update goals in the Goal details section in Adobe Workfront Goals](../../workfront-goals/goal-management/update-goals-in-goal-details-panel.md).
-->

要访问单个目标，请执行以下操作：

1. 单击Workfront右上角的&#x200B;**主菜单**&#x200B;图标，然后单击&#x200B;**目标** 。
默认情况下，将显示“目标列表”。
   ![目标列表](assets/goal-list-unshimmed.png)
1. 单击列表中目标的名称。
此时将显示目标的页面。
   ![目标页面](assets/goal-page-unshimmed.png)
1. 单击目标名称右侧的&#x200B;**更多**&#x200B;菜单![更多图标](assets/more-icon.png)以进一步编辑或共享目标。
1. 单击左侧面板中的&#x200B;**目标详细信息**&#x200B;以编辑有关目标的信息。 有关详细信息，请参阅Adobe Workfront目标[&#128279;](../goal-management/update-goals-in-goal-details-panel.md)的“目标详细信息”部分中的更新目标。



---
product-previous: workfront-goals
navigation-topic: goal-management
title: 查看Adobe Workfront目标中的有问题的目标
description: 在“Adobe Workfront目标”中，拥有进度条的Oals存在无法实现的危险，其代表为红色进度条。 您应该经常审查目标并了解进度滞后的原因。
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: 01e53bbc10573950d08f2df63fc742e6b9771e77
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# 查看Adobe Workfront目标中的有问题的目标

<!--Audited: 4/2025-->

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

“进展存在问题”的目标有无法实现的危险，在“Adobe Workfront目标”中有红色进度条表示。 您应该经常审查目标并了解进度滞后的原因。 有关目标进度的信息，请参阅[Adobe Workfront目标中的目标进度和条件概述](../../workfront-goals/goal-management/calculate-goal-progress.md)。

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
 <td role="rowheader">访问级别</td>
 <td> <p>编辑对目标的访问权限</p></td>
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

## 防止目标取得有问题的进展的建议

在目标达到“存在问题”的进度之前，您可以经常监控这些目标，并在目标达到“有风险”的进度时调整其进度。 有风险的目标有陷入麻烦的危险。 有关目标进度的更多信息，请参阅[Adobe Workfront目标中的目标进度和条件概述](../../workfront-goals/goal-management/calculate-goal-progress.md)

在您的目标达到“存在问题”进度之前，我们建议执行以下操作：

* 审核经常处于风险状态的分配给您的目标，以及分配给您的团队、组或受目标进度影响的组织的组织目标。 面临风险的目标有成为麻烦目标的危险。 处于风险中的目标用黄色进度条标记。 使用目标列表查看属于您、您的团队、组或您的组织的目标。


## 查看目标列表中的存在问题的目标

您可以在Workfront目标的任何部分中查看目标。 有关Workfront目标部分的信息，请参阅[Adobe Workfront目标概述部分](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md)。

本文介绍了如何查看目标列表中的目标。

1. 单击右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png) > **目标**。

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   这将打开Workfront目标区域，默认情况下将显示目标列表部分。

1. （推荐）为“目标列表”区域调整以下过滤器，以查看风险目标：

   * 依次单击&#x200B;**公司**、**我的团队**、**我的群组**&#x200B;和&#x200B;**个人**&#x200B;目标，以查看属于您的组织、团队、群组的目标，以及您自己的目标。

     >[!TIP]
     >
     >在Adobe Workfront目标中，公司过滤器显示您的组织被选为所有者的目标。
     >
     >
     >您无法使用此字段搜索公司。 默认情况下，仅选择您拥有Workfront实例的组织。

   * 对于以上选择的每个组织单位，单击&#x200B;**新建筛选器** > **进度** > **存在问题** >**应用。**
   * （可选）选择要查看其目标的时间段。

     目标列表中每个目标的进度条指示器均以红色显示。

     有关在右侧面板中使用所有其他标准筛选目标的更多信息，请参阅[在Adobe Workfront目标中筛选信息](../../workfront-goals/goal-management/filter-information-wf-goals.md)。

1. 将鼠标悬停在进度条指示器上可查看实际的进度百分比以及当天的预期值。

   ![GOal进度悬停详细信息](assets/goal-progress-hover-over-detail-unshimmed.png)

1. （可选）使用过滤器查找属于特定所有者的目标。

   选定用户的有问题的目标会显示在目标列表中。

1. 单击目标名称以打开目标页面，然后单击左侧面板中的&#x200B;**进度指示器**。 查看哪个进度指示器导致目标落后，并在进度指示器列表的&#x200B;**实际进度**&#x200B;列中更新内联指示器的进度。

   有关更新结果和活动的信息，请参阅[在Adobe Workfront目标中更新目标进度](../goal-review-and-workfront-goals-sections/check-in-goals.md)

   ![实际进度](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >您只能更新进度指示器列表中的结果和活动。 您必须通过访问目标来更新子目标的进度指示器，并且您必须更新已连接项目上的任务以更新项目进度。



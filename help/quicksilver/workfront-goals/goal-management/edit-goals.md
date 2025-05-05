---
product-previous: workfront-goals
navigation-topic: goal-management
title: 在Adobe Workfront目标中编辑目标
description: 您可以从任何时段和任何状态编辑现有目标。
author: Alina
feature: Workfront Goals
exl-id: 74db534c-6897-40c2-bea9-a9d30a40f61c
source-git-commit: 4e1558b47f6041501aa4e4fbfa6317dec8aee571
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 1%

---

# 在Adobe Workfront目标中编辑目标

<!--Audited for P&P only: 4/2025-->

您可以从任何时段和任何状态编辑现有目标。

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

## 有关编辑目标的注意事项

* 您无法编辑状态为“已关闭”的目标。
* 您可以编辑任何时间段的目标。

  您可以编辑过去目标的以下信息：

   * 名称
   * 时间段
   * 状态

     >[!TIP]
     >
     >如果目标为“已关闭”，则重新打开它将会重新计算进度完成百分比。 您无法编辑已关闭的目标。

   * 描述
   * 结果和活动

## 编辑目标

<!--
Editing goals differs depending on what environment you use.

### Edit goals in the Production environment

1. Go to a goal that you want to edit and click the goal name to open the **Goal Details** panel. 
1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Edit**.

   ![Edit goal](assets/edit-goal-highlighted.png)

1. Update the name of the goal in the **Goal** field. 
1. Select a time period when the goal should be completed.

   Select from the following predefined options:

   * The current year
   * The quarters of the current year
   * The next two years
   * The quarters of the next two years

   Or

   Click **Define custom dates** to select a custom time frame. 

1. (Conditional) Select a start and an end date for your goal, if you clicked **Define custom dates**.

   
   <p>(NOTE: these fields don't yet have a name) </p>
   

   >[!CAUTION]
   >
   >You cannot create a goal with custom dates in the past.

1. (Optional) Click **Reset custom dates** to return to the predefined options.

   >[!TIP]
   >
   >We recommend that everyone in your organization selects the same time frames for similar goals or goals that are aligned. This provides better alignment between goals and ensures that everyone's work supports your larger organization-wide strategy.

1. Click the **Owner** field and select a new owner for the goal, if you want to indicate someone else as the owner of the goal. 
1. (Conditional) Start typing the name of a user, team, group, or the name of your organization in the **Owner** field, then select it when it displays in the list. You can have only one owner for a goal. 
1. Update the **Description** of the goal, then click **Save**.

-->

1. 单击&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**目标**。\
   随即会显示目标列表。
1. 单击目标。\
   此时将显示目标页面。

   ![目标页面](assets/goal-page-unshimmed.png)

1. 执行以下操作之一以编辑目标的信息：
   * 单击目标标题中显示的字段以更新它们。 标头中的所有字段并非都可以编辑。
   * 单击目标名称右侧的&#x200B;**更多图标** ![更多图标](assets/more-icon.png)，然后单击&#x200B;**编辑**。
   * 单击左面板中的&#x200B;**目标详细信息**，然后单击右上角的&#x200B;**编辑图标**![编辑图标](assets/edit-icon.png)，然后单击&#x200B;**全部编辑**。 开始更新目标详细信息部分中的字段。

     >[!IMPORTANT]
     >
     >并非上述区域显示的所有字段都可以编辑。 Workfront会计算某些字段，这些字段为只读。

1. （视情况而定）根据您在上一步中选择的内容，更新以下有关目标的信息：

   * 更新目标标题中的以下信息，然后按Enter保存更改：
      * **目标名称**：单击目标的名称并开始键入新名称。
      * **所有者**：单击所有者的名称，然后开始键入用户、团队、群组或公司的名称，然后在列表显示该名称时将其选定。 一个目标只能有一个所有者。
   * 在“编辑目标”框中更新以下信息，然后单击&#x200B;**保存**：
      * **目标名称**
      * **时段**：单击以更新目标的时段\
        或\
        选择&#x200B;**启用自定义日期**&#x200B;以指定目标的&#x200B;**开始**&#x200B;和&#x200B;**结束日期**&#x200B;的日期。

        >[!TIP]
        >
        >取消选择&#x200B;**启用自定义日期**&#x200B;以返回到目标的原始时间段。

      * **目标所有者**
      * **描述**：添加或更新有关目标的信息。
   * 更新或查看“目标详细信息”部分中的信息。 有关详细信息，请参阅Adobe Workfront目标[&#128279;](../goal-management/update-goals-in-goal-details-panel.md)的“目标详细信息”部分中的更新目标。

   <!-- (should you update the title here after changing it at production??? - change it to Update goals in the goal Details section)-->

1. （可选）单击左侧面板中的&#x200B;**进度指示器**&#x200B;以将结果、活动或项目添加到目标。 通过添加进度指示器，您可以确保可以跟踪目标的进度。
有关更多信息，请参阅以下文章：
   * [将活动添加到Adobe Workfront目标中的目标](../results-and-activities/add-activities-to-goals.md)
   * [将结果添加到Adobe Workfront目标中的目标](../results-and-activities/add-results-to-goals.md)。
   * [在Adobe Workfront目标中添加项目](../results-and-activities/connect-projects-to-goals-overview.md)。

</div>

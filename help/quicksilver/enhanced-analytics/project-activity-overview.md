---
title: 在增强型分析中查看项目活动可视化
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 项目活动可视化图表显示在特定时间范围内发生的项目级别活动的汇总视图，即分配给项目的每个人的活动。 您可以集中精力了解项目中的活动，也可以将项目活动与Adobe Workfront中的其他项目进行比较。
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 8%

---

# 在增强型分析中查看项目活动可视化

<!-- Audited: 12/2023 -->

项目活动可视化图表显示在特定时间范围内发生的项目级别活动的汇总视图，即分配给项目的每个人的活动。 您可以集中精力了解项目中的活动，也可以将项目活动与Adobe Workfront中的其他项目进行比较。

>[!NOTE]
>
>“按团队分类的活动”可视化图表的行为与此可视化图表类似，但“按团队分类的活动”可视化图表显示所有项目的主团队活动。\
>有关按团队分类的活动可视化图表的信息，请参阅[在增强型分析中查看按团队分类的活动](../enhanced-analytics/activity-by-team-overview.md)。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront计划</a></td> 
   <td> <p>业务或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a></td> 
   <td>   <p>新增：</p> 
   <ul><li>浅色或更高</li></ul>
   <p>当前：</p>
   <ul><li>审阅或更高</li></ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看对项目的访问权限</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 先决条件

有关使用增强型分析的先决条件，请参阅[增强型分析概述](../enhanced-analytics/enhanced-analytics-overview.md)中的“先决条件”部分。

## 了解项目活动可视化图表

项目活动以不同的颜色显示，以总结一段时间内项目中的特定事件：

* **用户登录**：紫色框显示分配给项目的人员在当天登录。 颜色越深表示登录人数越多。

  ![](assets/project-activity-users-logged-in.png)

* **任务状态更改**：粉色框显示人员在该日更改了项目的任务状态。 阴影颜色越深表示任务状态变化的数量越多。

  ![](assets/project-activity-task-status-changes.png)

* **已完成任务**：蓝色框显示人员已完成项目的任务。 阴影颜色越深表示完成的任务数量越多。

  ![](assets/project-activity-tasks-completed.png)

将鼠标悬停在框上会显示该操作在指定日期内完成的准确次数。 您可以选择项目来按项目中的每个参与者查看这些活动的细分。

查看此信息可以帮助您确定：

* 针对特定项目的活动。
* 与其他项目相比，一个项目的活动情况。
* 哪些用户正在处理一个项目，频率是多少。

要了解如何为此可视化获取最佳数据，请参阅[增强分析概述](../enhanced-analytics/enhanced-analytics-overview.md)。

## 查看项目活动可视化图表

1. 单击主菜单图标![](assets/main-menu-icon-16x12.png)，然后选择&#x200B;**Analytics**。
1. （可选）要使用不同的日期范围，请从日期范围过滤器中选择新的开始日期和结束日期。

   ![](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅[在增强型分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

   >[!NOTE]
   >
   >如果您选择的日期范围超过3个月，则项目活动可视化图表不会显示任何数据。

1. （视情况而定）如果您需要限制项目数据集，请选择并应用要使用的过滤器。

   有关在增强分析中添加筛选器的详细信息，请参阅[在增强分析中应用筛选器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

   添加过滤器后，会显示最多50个项目的数据，即使您离开页面或退出Workfront，过滤器也会保持活动状态。

1. （可选）要放大日期范围，请在可视化图表上选择一个点作为日期范围的起点，然后拖动到日期范围的终点。

   所有其他可视化都会更新到相同的日期范围，并创建一个时间范围过滤器。

   ![](assets/timeframe-filter-350x220.png)

1. （可选）要更改项目的排序方式，请单击&#x200B;**排序依据**&#x200B;菜单，然后选择新的排序选项：

   * **A - Z**
   * **Z - A**
   * **计划完成日期**
   * **计划开始日期**

   页面上的所有其他可视化图表将更新以匹配您的排序选择。

1. （视情况而定）如果数据集中有超过50个项目，请使用可视化图表左下角的箭头，从包含50个项目的组导航到下一个项目。

   页面上的所有其他可视化图表将更新以匹配您选择的页面。

   ![](assets/pagination-350x118.png)

1. 单击可视化图表中的项目可查看该项目的更多详细信息。

   该列表将展开以显示项目中每个投稿人的活动。

1. 将鼠标悬停在框上可查看用户完成某项操作的日期以及该日操作的完成次数。

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. （可选）要导出可视化数据，请单击可视化右上角的&#x200B;**导出图标** ![](assets/export.png)，然后选择导出格式：

   * **图表(PNG)**
   * **数据表(XSLX)**


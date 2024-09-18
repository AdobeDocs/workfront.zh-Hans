---
title: 在增强型分析中查看按团队分类的活动可视化图表
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: “按团队分类的活动”可视化图表显示在特定时间范围内为主团队发生的活动，使您能够了解不同主团队在Adobe Workfront中花费时间的情况。 根据您的主团队在Workfront中的设置方式，此可视化图表可为您提供不同的见解并回答不同的问题。
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 364b668f23f5437e5cca0c4cc4793b17d444fb56
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 7%

---

# 在增强型分析中查看按团队分类的活动可视化图表

<!-- Audited: 12/2023 -->

“按团队分类的活动”可视化图表显示在特定时间范围内为主团队发生的活动，使您能够了解不同主团队在Adobe Workfront中花费时间的情况。 根据您的主团队在Workfront中的设置方式，此可视化图表可为您提供不同的见解并回答不同的问题。

>[!NOTE]
>
>项目活动可视化图表与此可视化图表类似，但它根据分配给项目的人员而不是分配给主团队的人员来显示活动。\
>有关项目活动可视化的信息，请参阅[在增强型分析中查看项目活动可视化图表](../enhanced-analytics/project-activity-overview.md)。

![](assets/activity-by-team-350x113.png){width="700"}

## 访问要求

+++ 展开以查看访问要求。

您必须具有以下权限才能执行本文中的步骤：

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
   <td>
      <p>新增：</p> 
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

+++

## 先决条件

有关使用增强型分析的先决条件，请参阅[增强型分析概述](../enhanced-analytics/enhanced-analytics-overview.md)中的“先决条件”部分。

## 按团队了解“活动”可视化图表

不同的活动会以不同的颜色显示，以总结在过滤的时间段内发生的特定事件：

* **用户登录**：紫色框显示主团队中的人员已在当天登录。 颜色越深表示登录人数越多。

  ![](assets/project-activity-users-logged-in.png)

* **任务状态更改**：粉色框显示主团队的人员在当天更改了任务的状态。 阴影颜色越深表示任务状态变化的数量越多。

  ![](assets/project-activity-task-status-changes.png)

* **已完成任务**：蓝色框显示主团队中的人员已在当天完成任务。 阴影颜色越深表示完成的任务数量越多。

  ![](assets/project-activity-tasks-completed.png)

将鼠标悬停在框上会显示该操作在指定日期内完成的准确次数。 您可以选择团队来查看按主团队中的每个人划分的这些活动的细目。

查看此信息可以帮助您确定：

* 主团队中正在进行哪些活动以及以什么速率进行。
* 哪些主场团队工作过度，或者更多地使用系统。
* 工作分配是否适合主团队。

要了解如何为此可视化获取最佳数据，请参阅[增强分析概述](../enhanced-analytics/enhanced-analytics-overview.md)。

## 查看“按团队列出的活动”可视化图表

1. 单击主菜单图标![](assets/main-menu-icon-16x12.png)，然后选择&#x200B;**Analytics**。
1. 在左侧面板中，选择&#x200B;**人员**。

   ![](assets/people-area-cropped-qs-350x276.png)

1. （可选）要使用不同的日期范围，请从日期范围过滤器中选择新的开始日期和结束日期。

   ![](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅[在增强型分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

1. （视情况而定）如果尚未设置团队筛选器，请添加团队筛选器并选择要查看其数据的每个团队。

   有关在增强分析中添加筛选器的详细信息，请参阅[在增强分析中应用筛选器](../enhanced-analytics/use-enhanced-analytics-filters.md)。

   添加过滤器后，会显示最多50个项目的数据，即使您离开页面或退出Workfront，过滤器也会保持活动状态。

1. （可选）要放大日期范围，请在可视化图表上选择一个点作为日期范围的起点，然后拖动到日期范围的终点。

   所有其他可视化都会更新到相同的日期范围，并创建一个时间范围过滤器。

   ![](assets/timeframe-filter-350x220.png)

1. 单击团队名称

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   查看主团队完成活动的更多详细信息。

   该列表将展开以显示分配给主团队的每个人的活动。

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. 将鼠标悬停在彩色框上可查看用户完成操作的日期以及操作在当天完成的次数。

   较暗的颜色表示较高的活动。

   ![](assets/activity-by-team-activity-pop-up-350x155.png)

1. （可选）要导出可视化数据，请单击可视化右上角的导出图标![](assets/export.png)，然后选择导出格式：

   * **图表(PNG)**
   * **数据表(XSLX)**


---
title: 在增强型分析中按团队查看活动可视化图表
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: “按团队划分的活动”可视化图表显示在家庭团队的特定时间段内发生的活动，从而让您了解不同的家庭团队在Adobe Workfront的逗留时间。 根据您的家庭团队在Workfront中的设置方式，此可视化图表可以为您提供不同的洞察和回答不同的问题。
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# 在增强型分析中按团队查看活动可视化图表

“按团队划分的活动”可视化图表显示在家庭团队的特定时间段内发生的活动，从而让您了解不同的家庭团队在Adobe Workfront的逗留时间。 根据您的家庭团队在Workfront中的设置方式，此可视化图表可以为您提供不同的洞察和回答不同的问题。

>[!NOTE]
>
>项目活动可视化与此可视化类似，只是它根据分配给项目的人员而不是分配给家庭团队的人员来显示活动。\
>有关项目活动可视化的信息，请参阅 [在Enhanced Analytics中查看项目活动可视化](../enhanced-analytics/project-activity-overview.md).

![](assets/activity-by-team-350x113.png)

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront计划</a>*</td> 
   <td> <p>业务或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront许可证概述</a>*</td> 
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看项目访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。<br>有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

有关使用Enhanced Analytics的先决条件，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 了解“按团队划分的活动”可视化图表

不同的活动以不同的颜色显示，以汇总过滤时间段内的特定事件：

* **已登录的用户**:紫色的框显示当天主队的用户登录。 较深的阴影表示登录的人数较高。

   ![](assets/project-activity-users-logged-in.png)

* **任务状态更改**:粉红色框显示当天，主团队中的人员更改了某项任务的状态。 颜色较深表示任务状态发生更多更改。

   ![](assets/project-activity-task-status-changes.png)

* **任务已完成**:蓝框显示主队的人员当天完成了一项任务。 颜色较深表示已完成的任务数较多。

   ![](assets/project-activity-tasks-completed.png)

将鼠标悬停在框上可显示在给定日期内完成操作的确切次数。 您可以选择一个团队，以查看按主团队中每个人划分的这些活动细目。

查看此信息可帮助您确定：

* 在主团队中进行的活动以及发生的频率。
* 哪些主团队工作过度，或者正在更多地使用系统。
* 如果工作分配适合本队。

要了解如何获取此可视化图表的最佳数据，请参阅 [增强的分析概述](../enhanced-analytics/enhanced-analytics-overview.md).

## 按团队查看活动可视化图表

1. 单击主菜单图标 ![](assets/main-menu-icon-16x12.png)，然后选择 **Analytics**.
1. 在左侧面板中，选择 **人员**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. （可选）要使用其他日期范围，请从日期范围筛选器中选择新的开始日期和结束日期。

   ![](assets/filters-select-date-range-350x344.png)

   有关使用日期范围过滤器的信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. （视情况而定）如果您未设置团队过滤器，请添加团队过滤器，然后选择要查看其数据的每个团队。

   有关在Enhanced Analytics中添加过滤器的更多信息，请参阅 [在增强的分析中应用过滤器](../enhanced-analytics/use-enhanced-analytics-filters.md).

   添加过滤器后，最多会显示50个项目的数据，并且即使您离开页面或注销Workfront后，这些过滤器仍保持活动状态。

1. （可选）要放大日期范围，请在可视化中选择一个点以表示日期范围的开始日期，然后拖到日期范围的结束日期。

   所有其他可视化图表将更新至同一日期范围，并创建时间范围过滤器。

   ![](assets/timeframe-filter-350x220.png)

1. 单击团队名称

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   查看主团队完成的活动的更多详细信息。

   此列表将展开，以显示分配给主团队的每个人员的活动。

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. 将鼠标悬停在彩色框上可查看用户完成操作的日期以及该操作在该天的完成次数。

   颜色较深表示活动较高。

   ![](assets/activity-by-team-activity-pop-up-350x155.png)

1. （可选）要导出可视化数据，请单击导出图标 ![](assets/export.png) 在可视化的右上角，选择导出格式：

   * **图表 (PNG)**
   * **数据表(XSLX)**


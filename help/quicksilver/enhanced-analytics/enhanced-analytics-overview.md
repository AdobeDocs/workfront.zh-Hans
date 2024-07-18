---
title: 增强的分析概述
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 增强型分析是Adobe Workfront中一款具有预建可视化图表的强大工具，允许您查看项目数据并识别计划和完成趋势。 对您项目的这种深入了解有助于您管理当前的工作，使您能够更准确地规划未来的工作。
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 3%

---

# 增强的分析概述

增强型分析是Adobe Workfront中一款具有预建可视化图表的强大工具，允许您查看项目数据并识别计划和完成趋势。 对您项目的这种深入了解有助于您管理当前的工作，使您能够更准确地规划未来的工作。

增强的分析功能可以帮助您识别：

* 计划项目的方式
* 当工作被添加到项目时
* 不同项目正在完成的工作量
* 与计划主团队的小时或天数相比，完成项目所需的小时或天数
* 用户在项目期间完成特定操作的频率
* 项目进度以及项目中的各个任务

![](assets/nwe-full-screen-analytics-350x222.png)

要查看用例或了解有关管理当前工作和规划增强分析未来工作的更多信息，请参阅[增强分析学习路径](https://one.workfront.com/s/enhanced-analytics-program)。

## 先决条件

要访问增强的分析区域，您必须：

* 拥有业务或企业计划。

  有关详细信息，请参阅[Workfront计划](https://www.workfront.com/plans)。

* 让您的Workfront管理员将增强型分析添加到您的布局模板。

  有关详细信息，请参阅[增强型分析：将分析添加到布局模板](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE)。

要查看有关项目和任务的信息，您必须：

* 拥有访问级别中“项目”和“任务”区域的查看权限。

  有关Workfront管理员如何修改您的访问级别的信息，请参阅[创建或修改自定义访问级别](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* 具有特定任务和/或项目的查看权限。

  有关请求其他访问权限的信息，请参阅[请求访问对象](../workfront-basics/grant-and-request-access-to-objects/request-access.md)。

## 增强分析的最佳实践

要获得项目的最佳数据，请使用具有准确计划小时数和持续时间天的模板。 您还需要确保用户尽可能准确地输入和更新以下字段。

>[!NOTE]
>
>以下某些字段是Workfront根据用户输入的信息执行的计算。 您无法手动更新这些字段。

* 规划小时数

  这是需要填写的最重要的字段。

  >[!NOTE]
  >
  >如果您的团队不使用计划小时数，您仍然可以看到一些基于项目持续时间的数据。\
  >有关详细信息，请参阅本文中的[持续时间视图](#duration-view)部分。

* 项目名称

  名称应为项目的描述性名称。

* 项目完成情况
* 项目状态
* 项目规划开始日期
* 规划完成日期
* 项目实际开始日期
* 项目实际结束日期
* 项目持续时间小时数
* 项目实际小时数
* 任务状态（包括将任务标记为“已完成”。）
* 任务名称
* 任务完成百分比
* 任务规划开始日期
* 任务规划完成日期

>[!IMPORTANT]
>
>对任务和项目所做的更改最多可能需要24小时才能反映在增强的分析中。

## 持续时间视图 {#duration-view}

默认情况下，“燃尽”和“项目”树形图可视化基于计划小时数。 如果您的团队不使用计划小时数，您可以根据项目持续时间查看这些可视化图表。

在Enhanced Analytics中，项目持续时间按以下公式计算：

* 计划时间范围：

  ```
  Planned Completion Date of the project - Start Date of the project
  ```

* 工作天数：

  ```
  Planned Duration for tasks completed in the selected date range / Typical hours per work day
  ```

  >[!NOTE]
  >
  >8小时是&#x200B;**每个工作日的典型小时数**&#x200B;的默认小时数。 Adobe Workfront管理员可以在&#x200B;**设置** > **项目偏好设置** > **项目** > **时间表**&#x200B;下更新&#x200B;**每个工作日的典型小时数**&#x200B;设置。\
  >若要了解详细信息，请参阅[配置系统范围的项目首选项](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

有关计划持续时间的信息，请参阅[项目持续时间概述](../manage-work/projects/planning-a-project/project-duration.md)。

## 键盘快捷键

您可以在键盘上使用以下键，导航或完成增强型分析区域中的特定操作：

| 键 | 操作 |
|---|---|
| **选项卡** | 导航到页面上的每个元素，以及包含未在页面上显示的每个可视化图表信息的表 |
| **进入** | 打开日历构件，删除现有筛选器，打开添加筛选器选项，选择/取消选择筛选器值，应用已创建的筛选器，打开每个可视化图表的导出选项，打开“燃尽”、“外部测试版任务”和“项目树状图”可视化图表的下拉菜单 |
| **箭头键** | 通过日历小组件上的日期、添加过滤器时的过滤器选项以及可视化图表上所有下拉菜单中的选项，进行导航 |
| **空格键** | 在日历小组件中选择日期，在添加过滤器时选择过滤器类型，从每个可视化图表的下拉菜单中选择导出选项，并从燃尽、外部测试版中的任务和项目树状图可视化图表的下拉菜单中选择选项 |

{style="table-layout:auto"}

如果使用屏幕阅读软件或插件，屏幕阅读器会大声阅读屏幕上的信息，并描述在使用上面列出的键时您正在完成的操作。

## 增强的分析视图和功能

要详细了解Enhanced Analytics中特定功能的详细信息、可完成哪些操作以获得进一步的见解，以及可从该数据中学到什么，请参阅以下文章：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>文章</th> 
   <th>说明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">在增强型分析中应用筛选器</a> </td> 
   <td> <p>您可以应用自定义筛选器、项目字段筛选器或团队筛选器以仅查看符合特定条件的项目。 添加过滤器时，项目数量会相应地更新。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">了解增强的分析KPI</a> </td> 
   <td> <p>屏幕顶部显示特定时间范围内所有项目的关键绩效指标(KPI)。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">在增强型分析中查看外部测试版计划可视化图表</a> </p> </td> 
   <td> <p><b>外部测试版计划</b>可视化图表显示项目生命周期中的状况已更改。 与可视化图表交互可为您提供有关特定日期的更多详细信息。 选择项目会打开外部测试版中的燃尽和任务可视化图表。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">在增强型分析中查看燃尽可视化图表</a> </td> 
   <td> <p><b>燃尽</b>可视化图表显示项目的计划速度与项目实际花费小时数的对比。 与可视化交互可让您了解有关特定日期项目状况的更多详细信息。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">在Enhanced Analytics中查看外部测试版中的任务可视化图表</a> </td> 
   <td> <p>外部测试版中的<b>任务</b>可视化图表显示项目中每个任务的状态。 与可视化交互允许您快速轻松地更改任务。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">在增强型分析中查看项目活动可视化图表</a> </td> 
   <td> <p><b>项目活动</b>可视化图表显示了一个热图，其中显示了分配给某个项目的用户登录Workfront、更改了该项目中任务的状态以及该项目中已完成任务的时间。 与可视化交互允许您查看每个用户的这些详细信息。 您还可以查看这些操作的特定日期以及完成每个操作的次数。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">在增强型分析中查看项目树状图可视化图表</a> </td> 
   <td> <p><b>项目树状图</b>可视化图表显示一些项目与其他项目相比所花费的时间。 与可视化交互可为您提供有关项目完成情况、计划项目完成和实际项目完成的详细信息。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">在增强型分析中查看按团队分类的活动可视化图表</a> </td> 
   <td> <p><b>按团队分类的活动</b>可视化图表显示主团队用户登录Workfront、更改任务状态以及完成任务的时间热图。 与可视化交互允许您查看每个用户的这些详细信息。 您还可以查看这些操作的特定日期以及完成每个操作的次数。</p> </td> 
  </tr> 
  <!-- Features permanently removed from Workfront
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">View the Resource capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Resource capacity</b> visualization shows you which home teams have the capacity to take on more work and which home teams have more work assigned to them than they can complete. Interacting with the visualization allows you to see more details about work completed and available hours for more work.&nbsp;Selecting a team opens the Team capacity visualization.</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">View the Team capacity visualization in Enhanced analytics</a> </td> 
   <td> <p>The <b>Team capacity</b> visualization shows you a percentage of the amount of work a home team has completed out of the amount of work assigned to them. Interacting with the visualization allows you to see scheduled hours and planned hours for a specific date, as well as the capacity percentage and whether the home team was over, under, or at capacity on that day.</p> </td> 
  </tr>--> 
 </tbody> 
</table>

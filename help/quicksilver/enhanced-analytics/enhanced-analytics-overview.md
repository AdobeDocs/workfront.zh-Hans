---
title: 增强的分析概述
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: 增强型分析是Adobe Workfront中一款功能强大的工具，带有预建的可视化图表，允许您查看项目数据并通过规划和完成来识别趋势。 这种对项目的洞察有助于您管理当前的工作，并使您能够更准确地规划未来的工作。
author: Nolan
feature: Reports and Dashboards
exl-id: a14ad57c-859b-43df-84c0-575ccda86e50
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 2%

---

# 增强的分析概述

增强型分析是Adobe Workfront中一款功能强大的工具，带有预建的可视化图表，允许您查看项目数据并通过规划和完成来识别趋势。 这种对项目的洞察有助于您管理当前的工作，并使您能够更准确地规划未来的工作。

增强的分析可以帮助您识别：

* 项目规划的方式
* 将工作添加到项目时
* 不同项目正在完成的工作量
* 完成项目所需的小时数或天数，与家庭团队计划完成项目的小时数或天数相比
* 用户在项目期间完成特定操作的频率
* 项目进度以及项目中的各个任务

![](assets/nwe-full-screen-analytics-350x222.png)

要查看用例或了解有关使用Enhanced Analytics管理当前工作和规划未来工作的更多信息，请参阅 [增强的Analytics学习路径](https://one.workfront.com/s/enhanced-analytics-program).

## 先决条件

要访问“增强的分析”区域，您必须：

* 制定业务或企业计划。

   有关更多信息，请参阅 [Workfront计划](https://www.workfront.com/plans).

* 让您的Workfront管理员将Enhanced Analytics添加到布局模板。

   有关更多信息，请参阅 [增强的Analytics:将分析添加到布局模板](https://one.workfront.com/s/managed-content-videos/enhanced-analytics-adding-analytics-to-layout-templates-MCH7URDSIXRREHHHF7TRTYYP2LTE).

要查看项目和任务的信息，您必须：

* 拥有访问级别中项目和任务区域的查看权限。

   有关Workfront管理员如何修改访问级别的信息，请参阅 [创建或修改自定义访问级别](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 具有特定任务和/或项目的“查看”权限。

   有关请求其他访问权限的信息，请参阅 [请求对对象的访问](../workfront-basics/grant-and-request-access-to-objects/request-access.md).

## 增强分析的最佳实践

为了获得项目的最佳数据，请使用具有准确计划小时数和持续时间天数的模板。 您还需要确保用户尽可能准确地输入和更新下面的字段。

>[!NOTE]
>
>以下一些字段是Workfront根据用户输入的信息执行的计算。 您无法手动更新这些字段。

* 计划小时

   这是需要填写的最重要字段。

   >[!NOTE]
   >
   >如果您的团队不使用计划时间，您仍可以根据项目持续时间查看一些数据。\
   >有关更多信息，请参阅 [持续时间视图](#duration-view) 在本文中。

* 项目名称

   该名称应当对项目进行描述。

* 项目完成情况
* 项目状态
* 项目计划起始日期
* 计划完成日期
* 项目实际开始日期
* 项目实际结束日期
* 项目持续时间
* 项目实际小时数
* 任务状态（这包括标记任务已完成。）
* 任务名称
* 任务完成百分比
* 任务计划的开始日期
* 任务计划完成日期

>[!IMPORTANT]
>
>对任务和项目所做的更改最长可能需要24小时才能在Enhanced Analytics中反映出来。

## 持续时间视图 {#duration-view}

默认情况下，“燃耗图”和“项目树图”可视化图表基于计划时间。 如果您的团队不使用计划时间，则可以根据项目持续时间查看这些可视化图表。

在Enhanced Analytics中，项目的持续时间由以下公式计算：

* 已计划时间框架:

   ```
   Planned Completion Date of the project - Start Date of the project
   ```

* 已工作天数:

   ```
   Planned Duration for tasks completed in the selected date range / Typical hours per work day
   ```

   >[!NOTE]
   >
   >8小时是 **每个工作日的典型小时数**. Adobe Workfront管理员可以更新 **每个工作日的典型小时数** 设置 **设置** > **项目首选项** > **项目** > **时间轴**.\
   >要了解更多信息，请参阅 [配置系统范围的项目首选项](../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

有关计划持续时间的信息，请参阅 [项目持续时间概述](../manage-work/projects/planning-a-project/project-duration.md).

## 键盘快捷键

您可以在键盘上使用以下键来导航或完成增强分析区域中的特定操作：

| 密钥 | 操作 |
|---|---|
| **选项卡** | 导航到页面上的每个元素，以及一个表格，其中包含的每个可视化图表的信息不会显示在页面上 |
| **输入** | 打开日历小组件、删除现有过滤器、打开添加过滤器选项、选择/取消选择过滤器值、应用您创建的过滤器、打开每个可视化上的导出选项、打开“燃耗”、“正在执行的任务”和“项目树状图”可视化上的下拉菜单 |
| **箭头键** | 导航到日历小组件上的日期、通过添加过滤器时的过滤器选项，以及通过可视化图表上所有下拉菜单中的选项 |
| **空格键** | 在日历小组件中选择日期，在添加过滤器时选择过滤器类型，从每个可视化的下拉菜单中选择导出选项，然后从“燃耗”、“飞行中的任务”和“项目树状图”可视化的下拉菜单中选择选项 |

{style=&quot;table-layout:auto&quot;}

如果您使用屏幕阅读软件或插件，屏幕阅读器将朗读屏幕上的信息，并描述您使用上面列出的键时正在完成的操作。

## 增强的Analytics视图和功能

要详细了解Enhanced Analytics中特定功能的详细信息、为获得进一步洞察而可完成的操作，以及可从此数据中了解的内容，请参阅以下文章：

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
   <td><a href="../enhanced-analytics/use-enhanced-analytics-filters.md" class="MCXref xref">在增强的分析中应用过滤器</a> </td> 
   <td> <p>您可以应用自定义过滤器、项目字段过滤器或团队过滤器，以仅查看符合特定条件的项目。 添加过滤器时，项目数量会相应地发生更新。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/understand-enhanced-analytics-kpis.md" class="MCXref xref">了解增强的分析KPI</a> </td> 
   <td> <p>特定时间范围内所有项目的关键绩效指标(KPI)位于屏幕顶部。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../enhanced-analytics/flight-plan-overview.md" class="MCXref xref">在Enhanced Analytics中查看飞行计划可视化</a> </p> </td> 
   <td> <p>的 <b>飞行计划</b> 可视化图表显示在项目生命周期中条件发生了更改。 与可视化交互会为您提供有关特定日期的更多详细信息。 选择项目会打开“燃尽”和“飞行任务”可视化图表。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/burndown-overview.md" class="MCXref xref">在Enhanced Analytics中查看燃耗可视化</a> </td> 
   <td> <p>的 <b>燃耗</b> 可视化图表显示项目的计划速度与项目花费的实际小时数之比。 与可视化交互会为您提供有关特定日期项目条件的更多详细信息。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/tasks-in-flight-overview.md" class="MCXref xref">在增强分析中查看“飞行”可视化中的任务</a> </td> 
   <td> <p>的 <b>正在飞行的任务</b> 可视化图表显示项目中每项任务的状态。 通过与可视化图表交互，您可以快速轻松地更改任务。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-activity-overview.md" class="MCXref xref">在Enhanced Analytics中查看项目活动可视化</a> </td> 
   <td> <p>的 <b>项目活动</b> 可视化图表显示了以下时间的热图：分配给登录到Workfront的项目的用户、更改了该项目中任务的状态以及完成了该项目中的任务。 与可视化交互允许您查看每个用户的这些详细信息。 您还可以查看这些操作的特定日期以及每个操作完成的次数。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/project-treemap-overview.md" class="MCXref xref">在增强型分析中查看项目树状图可视化</a> </td> 
   <td> <p>的 <b>项目树图</b> 可视化图表显示某些项目与其他项目相比已花费的时间。 与可视化交互会为您提供有关项目条件、计划项目完成情况和实际项目完成情况的详细信息。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/activity-by-team-overview.md" class="MCXref xref">在增强型分析中按团队查看活动可视化图表</a> </td> 
   <td> <p>的 <b>按团队划分的活动</b> 可视化图表显示了一个热图，其中显示了家庭团队的用户登录到Workfront、更改了任务状态以及完成了任务的时间。 与可视化交互允许您查看每个用户的这些详细信息。 您还可以查看这些操作的特定日期以及每个操作完成的次数。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/resource-capacity-overview.md" class="MCXref xref">在Enhanced Analytics中查看资源容量可视化</a> </td> 
   <td> <p>的 <b>资源能力</b> 可视化图表显示了哪些主团队有能力承担更多工作，以及哪些主团队的工作分配量多于他们完成的工作量。 与可视化图表交互允许您查看有关已完成工作的更多详细信息以及可供更多工作使用的小时数。 选择团队会打开“团队能力”可视化。</p> </td> 
  </tr> 
  <tr> 
   <td><a href="../enhanced-analytics/team-capacity-overview.md" class="MCXref xref">在Enhanced Analytics中查看“团队容量”可视化</a> </td> 
   <td> <p>的 <b>团队能力</b> 可视化图表显示家庭团队完成的工作量占分配给他们的工作量的百分比。 通过与可视化图表交互，您可以查看特定日期的计划小时数和计划小时数，以及容量百分比，以及主团队是否在当天结束、不足，还是处于容量状态。</p> </td> 
  </tr> 
 </tbody> 
</table>

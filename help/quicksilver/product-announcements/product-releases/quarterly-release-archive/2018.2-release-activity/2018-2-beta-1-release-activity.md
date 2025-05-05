---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 1发行版活动
description: 本页介绍了2018.2 Beta 1版本在“预览”环境中最近提供的所有更改。 2018年3月22日，该功能在预览环境中提供。 该版本将于2018年6月在生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: cbe98ee2-f155-4d31-88c4-7f41b6f91eb2
source-git-commit: 51b8e474cefe63b4db8c42e480990ca0ba431a4d
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 0%

---

# 2018.2 Beta 1发行版活动

本页介绍了2018.2 Beta 1版本在“预览”环境中最近提供的所有更改。 2018年3月22日，该功能在预览环境中提供。 该版本将于2018年6月在生产环境中提供。

>[!IMPORTANT]
>
>此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2018.2版中所做所有更改的列表，请参阅[2018.2版活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md)。

2018.2 Beta 1版本包含以下增强功能：

* [在甘特图中修改任务日期](#modify-task-dates-in-the-gantt-chart)
* [从“更新”选项卡](#access-the-project-gantt-chart-from-the-updates-tab)访问项目甘特图（暂时删除）

* [重新引入文档列表](#various-links-re-introduced-to-documents-on-the-document-list)上的文档的各种链接
* 资源规划者中的[用户视图改进](#user-view-improvements-in-the-resource-planner)
* [新项目列表体验](#new-project-list-experience)
* [更新选项卡的新外观](#new-look-for-updates-tab)
* [移动改进](#mobile-improvements)

## 在甘特图中修改任务日期 {#modify-task-dates-in-the-gantt-chart}

您现在可以拖动任务气泡以更改甘特图中的规划开始日期和规划完成日期。 借助这项更改，您可以将假设情景应用于您的项目而不会影响时间线。

在此更改之前，您只能在任务列表或任务级别更改任务日期。

有关详细信息，请参阅任务列表甘特图[&#128279;](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)中的更新信息。

## 从更新选项卡访问项目甘特图 {#access-the-project-gantt-chart-from-the-updates-tab}

>[!NOTE]
>
>此功能已从“预览”环境中暂时删除。

您现在可以从更新选项卡访问新项目甘特图。 当用户以影响项目时间线的方式更改任务的提交日期时，您可以在项目甘特图中查看影响。

在此更改之前，项目时间线链接会打开旧版甘特图。

有关详细信息，请参阅[提交日期概述](../../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)。

有关详细信息，请参阅[Portfolio优化程序概述](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)。

## 重新引入到“文档列表”中文档的各种链接 {#various-links-re-introduced-to-documents-on-the-document-list}

在18.1版本中，从文档列表上的文档中删除了各种链接，并将其移至界面的其他区域（其中一些链接作为文档名称旁边的按钮，另一些链接则作为按钮上的下拉菜单中的按钮）。 在此版本中，文档名称下方将重新引入以下链接，这些链接现在可以在文档列表中的各个文档中找到：

* 生成校对（在尚未生成校对时可用）
* 打开验证（在生成验证时可用）
* 文档详细信息（在尚未生成验证时可用）
* 校对详细信息（生成校对时可用）
* 打印摘要

在文档列表中，以下操作不会作为文档上的链接重新引入：

* 共享（仍作为菜单中的按钮提供）
* 签出/签入（仍可在菜单的“更多”下拉菜单中找到）

有关更多信息，请参阅以下部分：

*  在 

## 资源规划者中的用户视图改进 {#user-view-improvements-in-the-resource-planner}

资源规划者的“用户视图”现在包含下列改进：

* “用户视图”现在为默认视图，取代了“项目视图”。
* 改进了从整个数据库提取信息（而不仅仅是屏幕上的信息）的过滤器。
* 全屏模式。
* 性能现在更快、更有效。

   * 可显示的用户、项目、角色和任务数的新限制。
   * 延迟加载，可加快用户加载速度。

已在资源规划程序中临时禁用以下功能：

* 使用用户视图时从资源规划者导出数据。

在这些改进之前，您已经报告资源规划者加载缓慢，并且您已经注意到显示的数据中存在不一致的情况。 有了这些改进，这些应该取消。

有关资源规划者的区域的详细信息，请参阅[资源规划者导航概述](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)。

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a></p>
-->

## 新建项目列表体验 {#new-project-list-experience}

现在，查看项目列表时会有新体验可用。 该体验包括提高性能以及更顺畅、更快的列表导航。 此新Experience仅更新了Workfront的“项目”区域的“项目”选项卡中的列表。

大多数情况下，更改在于列表的速度和效率。 还引入了以下可见更改：

* 默认情况下，该列表最多显示2,000个项目。

  在此增强功能之前，列表显示100个项目。

* 默认情况下，将折叠分组。

  在此更改之前，默认情况下展开分组。

* 用于选择行的区域已展开到整行。

在指定的项目列表中已暂时禁用以下功能：

* 调整列大小(此功能在2018.2 Beta 5版本中重新引入)
* 列重新排序
* 状态图标字段显示为空白(2018.2 Beta 5版本中重新引入了此功能)
* 甘特图无法访问(此功能在2018.2 Beta 3版本中重新引入。)

有关在列表中工作的更多信息，请参阅[Adobe Workfront中的列表入门](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)。

## “更新新外观”选项卡 {#new-look-for-updates-tab}

>[!NOTE]
>
>对于某些用户，新的更新选项卡可能不会显示在预览环境中。 我们的开发团队目前正在排查问题，并努力尽快解决问题。

“更新”选项卡的外观已更改为与界面其他区域更加一致。 此更改适用于项目、任务、问题和文档。

下表显示了对“更新”选项卡所做的更新：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>任务</strong> </p> </th> 
   <th> <p><strong>上一个用户操作</strong> </p> </th> 
   <th> <p><strong>新用户操作</strong> </p> </th> 
   <th> <p><strong>有关详细信息，请参阅……</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>在时间表上记录时间</p> </td> 
   <td> <p>单击日志时间链接</p> </td> 
   <td> <p>单击“记录时间”按钮</p> </td> 
   <td> <p><a href="../../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">记录时间</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>在“更新”选项卡上过滤掉系统更新</p> </td> 
   <td> <p>单击过滤器系统更新链接</p> </td> 
   <td> <p>禁用“显示活动日志”切换</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>在“更新”选项卡上查看系统更新</p> </td> 
   <td> <p>单击显示所有更新</p> </td> 
   <td> <p>启用“显示活动日志”切换功能</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>在更新或评论中标记其他用户</p> </td> 
   <td> <p>单击将其他人包含在此更新图标</p> </td> 
   <td> <p>在通知字段中添加用户和团队</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>仅允许公司内的用户查看对象</p> </td> 
   <td> <p>单击锁定图标</p> </td> 
   <td> <p>启用“我的公司私有”切换开关</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">标记其他人的更新</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>允许公司外部的用户查看对象</p> </td> 
   <td> <p>单击锁定图标</p> </td> 
   <td> <p>禁用“我的公司私有”切换开关</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">标记其他人的更新</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>向评论或更新中添加回复或更新</p> </td> 
   <td> <p>单击“注释”按钮</p> </td> 
   <td> <p>单击回复或更新按钮</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">更新工作</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">更新任务状态</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">更新任务和问题的条件</a> </p> <p> </p> <p><a href="../../../../documents/managing-documents/add-update-documents.md" class="MCXref xref">向文档添加更新</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 移动改进 {#mobile-improvements}

移动设备应用程序包含以下增强功能：

* 现在，在其他移动设备应用程序中与您共享的链接会在Workfront移动设备应用程序中打开。

  有关共享链接的更多信息，请参阅。

  此更新有时会在本周发布到iOS，Android更新将在不久之后发布。

* 我们更新了对iOS平台的支持要求以支持iPhone X。

  有关支持的移动设备和操作系统的更多信息，请参阅。

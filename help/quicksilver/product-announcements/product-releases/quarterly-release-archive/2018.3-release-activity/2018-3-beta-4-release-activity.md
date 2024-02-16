---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.3 Beta 4发布活动
description: 本页介绍了2018.3 Beta 4版本预览环境中最近提供的所有更改。 该功能将于2018年8月30日在预览环境中可用。 该版本将于2018年11月在生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b40eda2c-8ad4-4945-a7e3-cb28ed8a14db
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 0%

---

# 2018.3 Beta 4发布活动

本页介绍了2018.3 Beta 4版本预览环境中最近提供的所有更改。 该功能将于2018年8月30日在预览环境中可用。 该版本将于2018年11月在生产环境中提供。

有关2018.3版中所做所有更改的列表，请参阅  [2018.3发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md).

2018.3 Beta 4版本包含面向Workfront管理员和其他用户的增强功能：

**适用于管理员**

* [以组管理员身份更新用户配置文件中的报告结构](#update-reporting-structure-in-the-user-profile-as-a-group-administrator) 

**适用于所有用户**

* [从资源规划者导出更多信息](#export-more-information-from-the-resource-planner)
* [任务列表改进](#task-list-improvements) 已从版本中删除
* [项目列表改进](#project-list-improvements)
* [在甘特图编辑模式下编辑任务列表](#editing-the-task-list-in-gantt-chart-edit-mode) 已从版本中删除
* [测量工具颜色](#measurement-tool-colors)
* [在新选项卡中打开的验证](#proofs-open-in-a-new-tab)  已从版本中删除

* [打印摘要增强功能](#print-summary-enhancements)
* [在Workfront移动设备应用程序中记录时间（以天为单位）](#log-time-in-days-in-the-workfront-mobile-app)

## 以组管理员身份更新用户配置文件中的报告结构 {#update-reporting-structure-in-the-user-profile-as-a-group-administrator}

组管理员现在可以编辑其管理的组中的用户的“直接下属”和“收件人”字段。

以前，只有Workfront管理员和具有用户管理访问权限的用户才有此功能。

有关组管理员的信息，请参见 [组管理员](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

## 从资源规划者导出更多信息 {#export-more-information-from-the-resource-planner}

您现在可以在资源规划程序中导出长达52周、36个月或12个季度的信息。 如果导出的信息量太大，您将收到一封电子邮件，其中附有导出的文件。 自开始下载起，您最多可以下载该文件一周。

以前，一次最多只能导出4周、月或季度。

欲了解更多信息，请参见 [从资源规划者导出信息](../../../../resource-mgmt/resource-planning/export-resource-planner.md).

## 任务列表改进 {#task-list-improvements}

>[!NOTE]
>
>* 此功能已从“预览”环境中删除，将不会包含在2018.3版本中。 它将在晚些时候发布。

现在，查看任务列表时会有新体验可用。 这种体验包括更高的性能，以及更顺畅、更快的列表导航。

以下可见更改也可用：

* 默认情况下，将折叠分组。\
  在此更改之前，默认情况下展开分组。
* 快速筛选器已添加到任务列表。
* 向下滚动任务列表时，项目标题保持可见。
* 新状态图标可用。

任务列表中的以下功能已更改：

* 右键单击功能和它提供的上下文菜单。\
  您可以执行以下操作，而不是右键单击任务来编辑它们：

   * 现在，当您选择单个任务时，可以使用与上一个右键单击菜单选项相同的“更多”菜单。
   * 选择多个任务时，可以使用列表顶部的图标来执行上一个右键单击菜单中包含的任何操作。

     所有更改在项目内的任务列表中可见，并在任务下的子任务选项卡中可见。

有关在列表中工作的详细信息，请参阅 [开始使用Adobe Workfront中的列表](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

有关在甘特图中链接任务的详细信息，请参阅 [通过链接任务创建前置任务关系](../../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).

## 项目列表改进 {#project-list-improvements}

重新排序列的功能已添加回以下子选项卡中的项目列表：

* 我拥有的项目
* 我在处理的项目
* 所有项目

2018.2版本中删除了此功能。

有关在列表中工作的详细信息，请参阅 [开始使用Adobe Workfront中的列表](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## 在甘特图编辑模式下编辑任务列表 {#editing-the-task-list-in-gantt-chart-edit-mode}

>[!NOTE]
>
>* 此功能已从“预览”环境中删除，将不会包含在2018.3版本中。 它将在晚些时候发布。

当项目中的任务以甘特图的编辑模式显示时，您现在可以对它们执行以下操作：

* 添加任务
* 删除任务
* 内联编辑任务

虽然您可以看到所做的更改如何影响项目的时间表，但不会立即进行更改。 您可以保存它们以更新项目时间线，也可以取消它们。

以前，当任务以甘特图的编辑模式显示时，您无法在任务上执行这些操作。 您可以在甘特图中未显示的任务列表中进行这些更改，但这些更改是立即进行的。

有关在甘特图中编辑任务的信息，请参阅 [更新任务列表甘特图中的信息](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## 测量工具颜色 {#measurement-tool-colors}

当使用测量工具测量校样上的区域时，现在可以更改工具颜色和不透明度。 Workfront会记住您打开的所有验证中的这些设置，直到您清空浏览器缓存为止。

默认颜色现在为红色。

以前，测量工具仅以蓝色显示，这使得在包含类似蓝色阴影的验证内容上难以查看。

## 在新选项卡中打开的验证 {#proofs-open-in-a-new-tab}

>[!NOTE]
>
>* 此功能已从预览环境中删除，将不再包含在2018.3版本中。

现在，当您在Workfront或Workfront Proof的任何位置打开验证时，验证查看器会在新的浏览器选项卡中启动，并且焦点将切换到该选项卡。 您可以在多个浏览器选项卡中工作，查看验证并继续在Workfront或Workfront Proof中处理项目、任务和问题。

以前，验证查看器在当前Workfront或Workfront Proof浏览器选项卡上方的框架中启动，导致该选项卡在关闭验证查看器之前无法访问。

有关更多信息，请参阅。

## 打印摘要增强功能 {#print-summary-enhancements}

现在，当您打印校样或将其另存为PDF或XLS文件时，打印摘要页面上提供了以下增强功能：

* 您可以按创建者对校样的注释进行排序。

  以前，您可以按照创建注释的顺序或注释在每个页面中的出现顺序对注释进行排序。

* 您可以按“作者”、“操作”和“未解决”状态筛选校对的评论。

  以前，在打印摘要页面上无法使用评论过滤。

* 现在包括阶段以及有关每个阶段的详细信息。

  以前，不包含阶段。

有关更多信息，请参阅 [在Adobe Workfront中打印验证摘要](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

## 在Workfront移动设备应用程序中记录时间（以天为单位） {#log-time-in-days-in-the-workfront-mobile-app}

您现在可以在Workfront移动设备应用程序中记录时间（以天为单位）。 

以前，即使您的配置文件首选项设置为以天为单位记录时间，您也只能在移动应用程序中使用小时记录时间。

有关在移动设备应用程序中记录时间的更多信息，请参阅。 

此功能可立即在Android Beta版应用程序中测试。 

---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 2发行版活动
description: 本页介绍了2018.1 Beta 2版本在“预览”环境中最近提供的所有更改。 2017年12月14日，预览环境中提供了此页面上的功能。 该版本将于2018年3月在生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 22e3836c-c41e-48a6-9926-e832af91e616
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 2%

---

# 2018.1 Beta 2发行版活动

本页介绍了2018.1 Beta 2版本在“预览”环境中最近提供的所有更改。 2017年12月14日，预览环境中提供了此页面上的功能。 该版本将于2018年3月在生产环境中提供。

>[!IMPORTANT]
>
> 此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2018.1版中所做所有更改的列表，请参阅  [2018.1版本活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md)。

2018.1 Beta 2版本包含面向Workfront管理员和其他用户的增强功能：

管理员的&#x200B;****

* [用户和布局模板的组管理](#group-administration-for-users-and-layout-templates)

所有用户&#x200B;****

* [系统范围宽屏显示器](#system-wide-widescreen-display)
* [在甘特图上调整时间线快照的大小](#resize-timeline-snapshot-on-the-gantt-chart)
* 业务案例中的[交互式资源规划者](#interactive-resource-planner-in-the-business-case)
* 资源规划者中的[可视化图表 — 用户分配图表](#visualization-in-the-resource-planner-user-allocation-chart)
* 主页区域中的[改进功能](#improvements-in-the-home-area)
* [新验证查看器改进](#new-proofing-viewer-improvements) 

## 用户和布局模板的组管理 {#group-administration-for-users-and-layout-templates}

现在，您可以在Workfront中指定组管理员。 “组所有者”字段已重命名为“组管理员”，被指定为“组管理员”的用户具有管理其管理的组的用户和布局模板的附加权限。

* [组管理员的用户管理](#user-management-by-group-administrator)
* [组管理员的布局模板管理](#layout-template-management-by-group-administrators)

### 由组管理员管理的用户管理 {#user-management-by-group-administrator}

我们正在介绍&#x200B;**组管理员**&#x200B;的新概念。 为了支持此功能，**组所有者**&#x200B;字段已重命名为&#x200B;**组管理员**，被指定为组管理员的用户具有管理用户和组的附加权限。

除了组所有者以前管理用户所拥有的权限之外，组管理员现在还可在将用户设置为组管理员的组内管理用户时获得以下附加访问权限：

* 以属于他们管理的组的另一个用户身份登录。
* 重置属于他们管理的组的其他用户的密码。
* 创建由其组管理的布局模板。 

在此更改之前，只有Workfront管理员可以执行这些功能。

有关组管理员的详细信息，请参阅[创建组](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的“了解组管理员”部分。

### 组管理员的布局模板管理 {#layout-template-management-by-group-administrators}

我们正在引入具有管理访问权限的&#x200B;**组**&#x200B;的新概念，您可以将其与布局模板关联。

指定为此组的组管理员的用户有权管理该布局模板和创建新布局模板，其中他们管理的组是模板的管理组。 

在此更改之前，只有Workfront管理员可以创建布局模板。

有关创建布局模板的更多信息，请参阅创建和管理布局模板。

## 系统范围宽屏显示器 {#system-wide-widescreen-display}

在Workfront中显示任何页面时，现在会自动填充整个浏览器窗口，并会根据屏幕大小进行调整。

在此更改之前，仅与以下对象关联的页面以宽屏显示：

* 项目
* 任务
* 问题
* 报告
* 仪表板
* 日程表

## 在甘特图上调整时间线快照的大小 {#resize-timeline-snapshot-on-the-gantt-chart}

您现在可以展开时间线快照以在甘特图中显示整个项目。

在此增强功能之前，您可以选择时间线快照上的特定点，以便在甘特图中导航到该点。

有关配置信息在甘特图上的显示方式的详细信息，请参阅[配置信息在甘特图上的显示方式](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)。

## 业务案例中的交互式资源规划者 {#interactive-resource-planner-in-the-business-case}

作为资源管理器，您现在可以在业务案例的资源预算部分添加资源池。 您还可以使用项目层资源规划程序来预算项目资源。 对项目资源进行预算可生成项目的预算劳力成本。

在此更改之前，如果项目已为全局资源规划者中的资源编列预算，则您可以在业务案例中查看资源预算信息。

有关在Business Case中完成预算项目资源的详细信息，请参阅Business Case中的[预算资源](../../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

## 资源规划者 — 用户分配图中的可视化 {#visualization-in-the-resource-planner-user-allocation-chart}

您现在可以在资源规划者图表中显示所有用户相对于其可用性的总计划分配。 在资源规划者中选择&#x200B;**按用户查看**&#x200B;时，图表可用。

图表显示以下信息：

* 所有用户都没有过度分配的可用性百分比
* 所有用户的过度分配百分比
* 所有用户的低利用率百分比
* 在此期间，至少过度分配了一个用户

在此更改之前，您只能以表格式查看单个用户的分配和可用性。

有关资源规划者中用户分配图表的详细信息，请参阅[资源规划者概述](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

## 主页区域的改进 {#improvements-in-the-home-area}

主页区域现在提供了各种改进功能，包括：

* 外观和感觉改进

   * 右侧面板现在更大了，为任务和问题信息提供了更多空间。
   * 现在，在左侧面板中选择过期项目时，将以较浅的红色阴影显示。
   * 现在，您可以更轻松地查看左面板和右面板之间的关系。 左侧面板中选定的文档指向右侧面板。

* 显示选定项目的默认字段。 

  有关默认字段的更多信息，请参阅创建和管理布局模板。

* 在请求中单击“处理它”后，与问题关联的字段将显示在右侧面板中。

  有关处理主页区域中的请求的更多信息，请参阅[管理主页区域中的工作和团队请求](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md)中的[管理主页区域中的工作和团队请求](../../../../workfront-basics/using-home/using-the-home-area/manage-work-and-team-requests-home.md)。

* 指向左侧面板中工作项上的用户头像，以查看用户的名称。
* 展开左侧面板中的“延迟”区域以查看所有延迟的项目（当此区域折叠时，仅显示前5项）。
* 将某个项目标记为“完成”后，该项目将保留在左侧面板中，直到您选择另一个项目为止。\
  有关显示已完成项的信息，请参阅[主页的工作列表显示项](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)中的[主页的工作列表显示项](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)。

有关使用新“主页”区域的详细信息，以及描述“我的工作”和“主页”之间功能差异的信息，请参阅[使用主页区域](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)。

## 新的校对查看器改进  {#new-proofing-viewer-improvements}

* [布局和设计已改进](#improved-layout-and-design)
* [按评论编号搜索评论](#search-comments-by-comment-number)
* [用于编辑标记指示器旁的评论的选项](#option-to-edit-comment-next-to-the-markup-indicator)
* [将所有评论标记为已读](#mark-all-comments-as-read)
* [左侧菜单改进](#left-menu-improvements)

### 改进了布局和设计 {#improved-layout-and-design}

校对查看器的外观和感觉已更新。 此  已更新验证查看器的以下区域：

* 缩略图区域

  有关使用缩略图的更多信息，请参阅中的。

* 评论区域\
  有关注释区域的更多信息，请参阅。
* 左侧菜单区域

### 按评论编号搜索评论 {#search-comments-by-comment-number}

现在，当您在验证查看器中搜索评论列表时，可以在搜索字段中输入评论的编号。 然后，筛选注释列表以显示您搜索的注释。 

有关更多信息，请参阅中的。

### 用于编辑标记指示器旁的注释的选项 {#option-to-edit-comment-next-to-the-markup-indicator}

您现在可以更轻松地编辑现有评论。 单击校样上的注释指示器后，球标旁边会显示编辑图标。 

在此更改之前，您必须单击“注释”区域中的编辑图标。  

有关更多信息，请参阅。

### 将所有评论标记为已读 {#mark-all-comments-as-read}

在校对查看器中查看文档时，您现在可以将所有注释标记为“已读”。

### 左侧菜单改进 {#left-menu-improvements}

验证查看器左侧的菜单包含以下改进：

* 更新外观
* 菜单顶部的图标，用于显示或隐藏菜单

  ![proof_viewer_menu_hide.png](assets/proof-viewer-menu-hide.png)

* 将鼠标悬停在菜单上可自动展开菜单以查看图标以及标签。 （或者启用选项以将菜单始终保留在折叠视图中。）

---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta 4发行版活动
description: 本页介绍了2018.2 Beta 4版本在“预览”环境中最近提供的所有更改。 该功能将于2018年5月17日在预览环境中可用。 该版本将于2018年7月在生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4b54b9e6-d1bf-4802-9d6c-9c3d3b6a6583
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 0%

---

# 2018.2 Beta 4发行版活动

本页介绍了2018.2 Beta 4版本在“预览”环境中最近提供的所有更改。 该功能将于2018年5月17日在预览环境中可用。 该版本将于2018年7月在生产环境中提供。

>[!IMPORTANT]
>
> 此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2018.2版中所做所有更改的列表，请参阅  [2018.2发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md)。

2018.2 Beta 4版本包含适用于Workfront管理员和其他用户的增强功能：

管理员的&#x200B;**&#x200B;**

* [系统设置：外部页面中的会话信息](#system-setting-session-information-in-external-pages)

所有用户&#x200B;**&#x200B;**

* Kanban展示板上的[正在工作(WIP)限制增强功能](#work-in-progress-wip-limit-enhancements-on-the-kanban-board)
* [改进了配置Agile团队状态的界面](#improved-interface-for-configuring-statuses-for-an-agile-team)
* [主页区域已更新工作列表（左面板）](#updated-work-list-left-panel-in-the-home-area)
* [新桌面验证查看者用于验证交互式（富媒体）内容](#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content) 
* [导出资源规划者中的用户视图](#export-the-user-view-in-the-resource-planner)
* [支持Google团队驱动器](#support-for-google-team-drives)
* [甘特图的新导出限制](#new-export-limit-for-the-gantt-chart)
* 使用Internet Explorer或Safari时，[从剪贴板粘贴选项现在显示为灰色](#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari)
* [适用于Android的新Beta环境以及新功能](#new-beta-environment-for-android-along-with-new-features)
* [事件订阅消息的过滤器示例](#examples-of-filters-for-event-subscriptions-messages)

## Kanban展示板上的正在进行的工作(WIP)限制增强功能 {#work-in-progress-wip-limit-enhancements-on-the-kanban-board}

### 为Kanban展示板上的每个列配置正在进行的工作(WIP)限制

现在，您可以为Kanban展示板上的每个列配置正在进行的工作(WIP)限制。 

在此更改之前，您只能配置一个应用于Kanban展示板上所有列的WIP限制。 

有关更多信息，请参阅部分  在文章中[配置正在进行的工作(WIP)限制](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4)  [配置Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)。

### 直接从Kanban展示板更新正在进行的工作(WIP)限制

现在，拥有团队编辑权限的团队成员可以直接从Kanban展示板更新WIP限制。

在此更改之前，只能从“团队设置”区域更新WIP限制。

有关更多信息，请参阅  在文章中。

## 改进了用于为Agile团队配置状态的界面 {#improved-interface-for-configuring-statuses-for-an-agile-team}

更新了配置Agile团队状态的界面，改进如下：

* 新外观
* 通过拖放操作对状态列重新排序 

有关更多信息，请参阅以下文章：

* [配置Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
* [配置Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## 主页区域已更新工作列表（左侧面板） {#updated-work-list-left-panel-in-the-home-area}

主页区域的工作列表包含以下改进：

* 未读项目现在以粗体和蓝点突出显示。

  在“主页”区域之外查看的项目在“主页”区域仍显示为“未读”。

  有关详细信息，请参阅[在主页区域的工作列表中显示项目](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)。

* 现在，通过问题旁边显示的问题图标来区分问题。
* 现在按审批类型区分审批，并显示审批类型。 可能的审批类型包括任务、项目、问题、访问、文档、时间表和验证。

  在此更改之前，仅通过“批准”一词区分批准。

* 现在，可通过项目是否准备好启动来区分这些项目。 可能的选项包括“准备开始”、“未就绪”或“正在处理”。

  此信息不显示以供审批，因为审批始终可以开始。

* 每次将文档附加到项目时，项目名称下方都会显示文档图标。
* 您现在可以折叠和展开工作列表内的分组，以便更好地控制显示哪些信息。 分组包括延迟、项目、日期和已完成。

  默认情况下，“本周”部分处于展开状态，而所有其他分组则处于折叠状态。

* 选择是按计划完成日期还是提交日期对物料排序。
* 现在，每个分组中的项目数都显示在分组标题旁边的括号中。

  此数字不可用于“已完成”分组。

  有关详细信息，请参阅[在主页区域的工作列表中显示项目](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)。

* 通过拖放调整工作列表的大小。 您可以调整工作列表的大小，使其最多占用一半屏幕。 您设置的大小将在下次访问Home时保留。

  在此更改之前，无法更改工作列表的大小。

* 对于请求，现在会显示发出请求的用户的用户头像，其中显示文本“[Approver_name]”表示希望您审批。
* 创建新的个人任务时，“待办事项”按钮现在标记为“个人”。

  有关详细信息，请参阅文章[从主页区域创建工作项](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)中的[从主页区域创建工作项](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)。

* 仅在计划完成日期后一小时内，延迟物料才会显示为“延迟”。

有关主页区域的详细信息，请参阅[使用主页区域](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)。

## 用于对交互式（富媒体）内容进行校对的新桌面校对查看器 {#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content}

新的桌面校对查看器允许您校对交互式内容。 与现有的旧版验证查看器和在浏览器中运行的新验证查看器不同，桌面验证查看器是在您的工作站上运行的应用程序。

在新的桌面校对查看器之前，您只能在旧版校对查看器中校对交互式内容。 

与传统校对查看器相比，桌面校对查看器包括对交互式内容进行校对的以下增强功能：

* 审查不安全(HTTP)站点

  旧版验证查看器允许您仅查看安全(HTTPS)站点

* 查看受iframe保护的网站（受保护的网站，以免在iframe内查看）。

  旧版验证查看器不支持审核在iframe中无法查看的网站。

* 查看各种设备具有预配置分辨率的内容。 例如，您可以看到内容在各种标准桌面分辨率上或iPhone 8等单个设备上的显示方式。 

有关下载、安装和使用桌面校对查看器的更多信息，请参阅。

有关桌面验证查看器和基于浏览器的验证查看器之间的功能差异的信息，请参阅[Web验证查看器和桌面验证查看器之间的差异概述](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)。

## 导出资源规划者中的用户视图 {#export-the-user-view-in-the-resource-planner}

为了解决一些性能问题，我们在用户视图中显示数据时暂时禁止从资源规划者导出数据。 在此版本中，我们在用户视图中显示资源规划者时重新启用数据导出。

有关将资源规划者数据导出到Excel的更多信息，请参阅[资源规划者导航概述](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)中的“导出选项”部分。

要参与我们当前针对资源规划者的测试版计划，请参阅[资源规划者绩效Beta。](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront)

## 系统设置：外部页面中的会话信息 {#system-setting-session-information-in-external-pages}

在创建外部页面时，Workfront管理员现在可以限制使用会话信息（例如，会话ID）。

在此更改之前，可创建外部页面的用户在将其他网站嵌入到Workfront仪表板中时，可以使用任何会话信息。 

有关在Workfront中配置系统首选项的详细信息，请参阅[配置系统安全首选项](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

## 支持Google团队驱动器 {#support-for-google-team-drives}

您现在可以从Workfront链接位于Google团队驱动器上的文档或文件夹。

在此增强功能之前，您可以链接仅位于Google我的驱动器上的文档或文件夹。

有关将文档和文件夹从各种应用程序链接到Workfront的更多信息，请参阅[链接来自外部应用程序的文档](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

## 甘特图的新导出限制 {#new-export-limit-for-the-gantt-chart}

您现在最多可以在甘特图中导出500个任务。

以前，最多只能导出250个任务。

有关详细信息，请参阅[将甘特图导出到PDF](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)。

## 使用Internet Explorer或Safari时，“从剪贴板粘贴”选项现在显示为灰色 {#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari}

现在，使用Internet Explorer或Safari浏览器时，“从剪贴板粘贴”选项显示为灰色，并带有工具提示来说明此功能仅支持Chrome和Firefox浏览器。

在此更改之前，使用Internet Explorer或Safari时不显示此选项。 

有关从剪贴板粘贴图像的详细信息，请参阅[从剪贴板粘贴图像](../../../../documents/managing-documents/paste-image-clipboard.md)。

## 适用于Android的新Beta环境以及新增功能 {#new-beta-environment-for-android-along-with-new-features}

现在，您可以通过注册成为测试版测试员，在面向公众发布移动应用程序的最新功能之前，体验我们的团队正在努力处理的最新功能。 目前，Workfront移动设备应用程序仅支持Android手机使用此环境。

有关如何注册成为Workfront移动设备应用程序的测试版测试者的更多信息，请参阅。

移动应用程序的测试版现在提供以下改进：

* 新建帐户页面

  您现在可以查看帐户信息，并管理移动设置、提交反馈或从新的帐户页面注销。

  在此改进之前，您无法在移动应用程序上查看您的帐户信息，并且可以从Workfront主菜单访问设置、提交反馈和注销。

* 新建导航底部面板

  屏幕底部现在有一个更突出的导航栏，可启动移动设备应用程序的所有区域。

  在此改进之前，Workfront主菜单上列出了功能领域。 Workfront主菜单已被删除，并已被新的底部导航栏取代。

  有关配置新导航栏的更多信息，请参阅中的“配置您的移动设备应用程序”部分。

* 新建通知列表视图

  改进了“通知”列表的外观，使您可以根据通知的类型和是否阅读过这些通知，轻松区分列表中的通知。

* 搜索框已移至更显眼的位置。

* 新登录体验更精简的新登录体验。

* 新的教程体验

  现在提供了新的教程，可在用户首次登录时对其在应用程序中的操作进行简要指导。 在此体验之前，教程仅在用户访问特定功能区域时启动。

## 事件订阅消息的过滤器示例 {#examples-of-filters-for-event-subscriptions-messages}

为了演示如何过滤事件订阅以仅接收与您的组织相关的消息，现在提供了示例代码片段来过滤到达您端点的事件流。 若要了解有关查看筛选示例的详细信息，请参阅[筛选事件订阅消息](../../../../wf-api/api/filter-event-sub-messages.md)。

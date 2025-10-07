---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 Beta最终发行版活动
description: 本页介绍了2017.3 Beta Final版本在“预览”环境中最近提供的所有更改。 此页面上的功能已于2017年9月12日在预览环境中提供。 该版本将于2017年11月初在“生产”环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
source-git-commit: f5044d457ebf203269e8007075e98ba4c136660f
workflow-type: tm+mt
source-wordcount: '3791'
ht-degree: 0%

---

# 2017.3 Beta最终发行版活动

本页介绍了2017.3 Beta Final版本在“预览”环境中最近提供的所有更改。 此页面上的功能已于2017年9月12日在预览环境中提供。 该版本将于2017年11月初在“生产”环境中提供。

>[!IMPORTANT]
>
> 此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2017.3版中所做所有更改的列表，请参阅  [2017.3发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md)。

2017.3 Beta最终版本包含面向Workfront管理员和其他用户的增强功能：

管理员的&#x200B;****

* [在审批设置区域重新调用请求的新配置](#new-configuration-for-recalling-requests-in-the-approval-settings-area)
* [配置默认验证角色](#configure-default-proof-roles)

所有用户&#x200B;****

* [主页区域（已更新我的工作区）](#home-area-updated-my-work-area)

* [已更新布局模板以支持主区域](#updated-layout-template-to-support-the-home-area)

* 适用于Agile的[Kanban](#kanban-for-agile)
* [Agile团队的Scrum积压中包括问题](#include-issues-on-the-scrum-backlog-for-an-agile-team)
* [在Scrum敏捷故事板上包含问题](#include-issues-on-the-scrum-agile-story-board)
* [将分组和筛选器应用于Agile团队的积压工作](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [在预览环境中返回增强的@Tagging功能](#enhanced-tagging-functionality-returns-in-the-preview-environment)
* 更新流中的[筛选器系统更新现在跨对象持续存在](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [在利用率报告中可视化数据](#visualize-data-in-the-utilization-report)
* [利用率报告性能改进](#utilization-report-performance-improvement)
* [文档增强：精简的界面](#document-enhancements-streamlined-interface)
* Workfront中的[校对增强功能](#proofing-enhancements-within-workfront)
* Workfront Proof和Workfront中的[校对增强功能](#proofing-enhancements-within-both-workfront-proof-and-workfront)
* 更新和电子邮件的[富文本格式](#rich-text-formatting-for-updates-and-emails)
* [新甘特图重新设计](#new-gantt-chart-redesign)
* [内置报告包含更新的描述](#built-in-reports-contain-updated-descriptions)
* [在导出的报告、列表和功能板中品牌化](#branding-in-exported-reports-lists-and-dashboards)
* [复制任务和移动任务或问题时的改进](#improvements-when-copying-tasks-and-moving-tasks-or-issues)
* [资源预算小时报告的新分组：分配日期](#new-grouping-for-resource-budgeted-hour-reports-allocation-date)
* [资源规划者改进](#resource-planner-improvements)
* [移动改进](#mobile-improvements)
* [Workfront与Slack的集成](#workfront-integration-with-slack)
* [Outlook 365改进](#outlook-365-improvements)
* [API更改](#api-changes)

## 主页区域（已更新我的工作区） {#home-area-updated-my-work-area}

>[!NOTE]
>
>此功能将不会在17.3版本中发布到“生产”环境；在2018年初之前，它将一直保留在“预览”中。

新的“主页”区域为当前在“我的工作”区域中可用的相同数据提供另一个增强视图。 与“我的工作”区域相比，“主页”区域具有以下优点：

* 更加精简和直观的界面
* 增强的性能

以下功能在“我的工作”区域中可用，但尚未在“主页”区域中实施：

* 查看您的个人日历
* 更新富文本格式的任务和问题
* 批准验证
* 查看您提交以供审批的工作列表
* 在项目中创建临时问题
* 仅查看那些委托给您的审批

有关使用新主页区域的详细信息，请参阅[使用主页区域](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)。

## 更新了布局模板以支持主页区域 {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>此功能将不会在17.3版本中发布到“生产”环境；在2018年初之前，它将一直保留在“预览”中。

作为Workfront管理员，您可以通过配置用户所分配的布局模板来确定组织中的用户是否具有主页区域的访问权限。 未分配布局模板的用户始终可以访问“主页”区域。

有关更多信息，请参阅创建和管理布局模板中的“自定义主页”。

## 适用于敏捷的Kanban  {#kanban-for-agile}

除了已支持的Scrum敏捷方法之外，Agile团队现在还可以在Workfront中使用Kanban方法。

Workfront中的Scrum和Kanban敏捷方法在以下方面有所不同：

**在Workfront中使用Kanban的好处**

* 在Kanban敏捷故事板上显示积压。

  有关更多信息，请参阅中的。

* 配置积压中的物料，当其他物料移至等同于“完成”的状态时，这些物料自动添加到Kanban敏捷故事板。

  有关详细信息，请参阅[配置Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5)中的[配置要自动从积压工作中添加的故事](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)。

* 配置要在Kanban敏捷故事板上显示的进行中的工作(WIP)限制。

  有关详细信息，请参阅[配置Kanban](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4)中的[配置正在进行的工作(WIP)限制](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)。

**在Workfront中使用Scrum的好处**

* 将一组故事添加到敏捷开发周期中，并为该开发周期创建一个故事板。
* 将问题包含在Scrum故事板上。
* 包括Agile团队积压的问题。

  有关详细信息，请参阅[配置Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)中的[配置将工作项添加到开发周期](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)时如何应用日期。

* 子任务可以显示在Scrum故事板上。
* 查看燃尽图以查看迭代期间历程的进度。

  有关详细信息，请参阅[敏捷燃尽图概述](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md)。

有关为Agile团队启用和配置Kanban的更多信息，请参阅[创建Agile团队](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding)中的[确定Agile方法](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md)。

## 包括有关Agile团队的Scrum积压的问题 {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>此功能已于2017年11月14日从生产环境中删除。 计划于2018年初将其重新引入预览环境，并增强设计和稳定性。 它将在2018.1版本的生产环境中可用。

使用Scrum敏捷方法时，您现在可以在敏捷团队的积压中包括问题（使用Kanban方法时，问题未显示在敏捷团队的积压中）。 现有的Scrum Agile团队必须启用此功能才能包含问题。 在2017.3版本之后创建的Scrum敏捷团队的积压中自动包含问题。

在此更改之前，只能将任务添加到积压。 如果要添加问题，必须先将问题转化为任务，然后才能添加问题。

由于您现在不仅可以访问积压中的任务，因此积压中之前可用的任何自定义任务视图都会复制并作为自定义积压工作项目视图添加到积压中。

有关在积压中使用问题的信息，请参阅  [管理Agile积压](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)。

有关启用问题在Agile Scrum团队的积压中可用的信息，请参阅  [在](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)配置Scrum[中配置将工作项添加到迭代](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)时如何应用日期。

## 包含有关Scrum敏捷故事板的问题 {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>此功能已于2017年11月14日从生产环境中删除。 计划于2018年初将其重新引入预览环境，并增强设计和稳定性。 它将在2018.1版本的生产环境中可用。

在使用Scrum敏捷方法时，您现在可以在故事板上包含问题。

有关详细信息，请参阅[配置Scrum](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2)中的[在Agile故事板](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)上配置状态列。

## 将分组和筛选器应用于Agile团队的积压 {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>此功能已于2017年11月14日从生产环境中删除。 计划于2018年初将其重新引入预览环境，并增强设计和稳定性。 它将在2018.1版本的生产环境中可用。

分组和筛选选项现在适用于Agile积压，允许您按分组组织积压，并筛选特定任务和问题。

在此更改之前，您可以将视图应用于Agile积压。

有关更多信息，请参阅  [管理Agile积压工作](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)，位于  [管理Agile积压](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)。

## 更新和电子邮件的富文本格式 {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>您在预览环境中所做的格式更改可能会恢复为未格式化的状态。

现在，您可以通过设置对Workfront对象所做的注释和更新的格式来强调重要信息。 

使用富文本工具，您可以将格式属性应用于文本，生成项目符号和编号列表，以及向其他资源添加超链接。

应用于更新流中评论的格式也会显示在更新电子邮件通知中。 若要了解有关设置评论格式的详细信息，请参阅[更新工作](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

## 预览环境中返回的@Tagging增强功能 {#enhanced-tagging-functionality-returns-in-the-preview-environment}

可以再次使用@符号在“预览”环境中所有对象的更新流中标记其他用户。 过去，@tagging将已标记用户的名字和姓氏放置在更新流中。 现在，增强的@tagging功能仅显示用户的名字。 若要了解有关在更新中标记用户的更多信息，请参阅[在更新中标记其他用户](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)。

## 更新流中的过滤器系统更新现在可以跨对象持续进行 {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

过滤器系统更新选项现在可以跨整个Workfront站点的对象持续使用。 这允许您隐藏系统更新并仅查看某个对象更新流中的用户注释，并在浏览到其他对象时保留该设置。

在此更改之前，您必须选择在浏览Workfront站点时筛选掉每个对象的系统更新。

有关详细信息，请参阅[更新工作](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

## 在利用率报告中可视化数据 {#visualize-data-in-the-utilization-report}

 您现在可以在图表视图中查看利用率信息。 

有关详细信息，请参阅[资源利用率报告概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)中的[资源利用率报告概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 利用率报告性能改进 {#utilization-report-performance-improvement}

>[!NOTE]
>
>此功能在Beta最终版本发布后的修补程序中发布。

现在，当运行利用率报告时，系统会提示您先应用过滤器，然后再运行报告。 此更改可确保尽快在利用率报告中生成最相关的信息。

有关运行利用率报告的详细信息，请参阅[资源利用率报告概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)中的[资源利用率报告概览](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)。

## 文档增强：简化的界面 {#document-enhancements-streamlined-interface}

现在，向Workfront添加文档的用户体验更加简洁直观。 现在，您可以通过简单的下拉菜单从文件系统上传文档、请求文档或从第三方应用程序(如Google或Dropbox)链接文件。 

以前，通过启动“添加文档”对话框可以使用这些选项。 

有关更多信息，请参阅以下信息：

* [将文档从您的文件系统添加到Adobe Workfront](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)
* [请求文档](../../../../documents/adding-documents-to-workfront/request-a-document.md)
* [链接来自外部应用程序的文档](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) 

>[!NOTE]
>
>进行此更改后，从剪贴板粘贴图像或文档的选项不再可用。

## Workfront中的校对增强功能 {#proofing-enhancements-within-workfront}

* [已改进的用户体验和附加功能](#improved-user-experience-and-additional-functionality)
* [直接从验证查看者共享](#share-directly-from-the-proofing-viewer)
* [配置默认验证角色](#configure-default-proof-roles)

### 改进了用户体验和其他功能 {#improved-user-experience-and-additional-functionality}

除了在Workfront中创建验证时改进的用户体验之外，现在还提供以下附加功能：

* 将多个图像合并到单个验证中。
* 多个分辨率的验证网站（多个分辨率可以作为单个验证创建，或者可以组合到单个验证中）。
* 在上载过程中编辑文件名。
* 在验证创建表单中包含自定义字段。
* 添加自定义消息以验证电子邮件通知。
* 其他校对设置 
* 验证URL时的实时错误验证（以前，显示错误之前必须等待几分钟）

有关更多信息，请参阅。

>[!NOTE]
>
> 使用自动化工作流创建新验证时，不支持使用拖放操作将用户从一个阶段移动到另一个阶段。 取而代之的是，从一个步骤中删除用户，然后将其添加到另一个步骤。

*2018.1版本将重新引入使用拖放功能将用户从一个步骤移动到另一个步骤的选项。*

### 直接从验证查看器共享 {#share-directly-from-the-proofing-viewer}

现在，您可以直接从验证查看器与特定Workfront用户共享。

>[!NOTE]
>
>此功能仅适用于新验证（2017.3版本之后创建的验证），并且仅适用于与Workfront Proof Premium帐户集成的Workfront实例。

在此更改之前，您只能通过创建链接并与用户共享该链接来进行共享。 

有关详细信息，请参阅[在Adobe Workfront中共享验证](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)中的[在Adobe Workfront中共享验证](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)。

### 配置默认验证角色 {#configure-default-proof-roles}

您现在可以配置默认验证角色，以便新用户和访客用户在Workfront系统中具有新验证的功能。 

这是与用户共享验证时，用户在验证中分配的默认角色。 

## Workfront Proof和Workfront中的校对增强功能 {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [在HTML5视频校对查看器中重新启动并跳过（键盘快捷键）](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts)
* [HTML5验证查看器更新](#html5-proofing-viewer-updates)

### 在HTML5视频校对查看器中重新启动和跳过（键盘快捷键） {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

现在，在HTML5视频验证查看器中提供了键盘快捷键，可让您从头开始重新启动视频并跳到视频结尾。

有关可用键盘快捷键的更多信息，请参阅Workfront Proof验证查看器中的[键盘快捷键](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md)。

### HTML5验证查看器更新 {#html5-proofing-viewer-updates}

HTML5查看器现在支持静态校样。

在此更改之前，HTML5查看器仅支持视频校样。 

在校对静态内容时，HTML查看器包括以下新功能：

* 在单个视图中时，在多个页面上添加带标记的单个注释

  以前，只有在“连续视图”或“磁带盒”视图中才能执行此操作

* 通过验证缩略图导航验证

   * 轻松识别正在审阅的证明部分。 这一点很重要，尤其是当用户使用格式更大的验证和较长的网页时，或者在任何时候  需要更大的缩放级别才能查看详细信息。
   * 更改缩放级别
   * 平移内容

* 在测量工具中指定自定义值
* 在Workfront Proof的验证查看器中为验证中的文本添加注释时，您可以包含用于指示文本应该加粗、斜体和下划线的选项。

HTML5查看器尚不支持现有Flash查看器当前提供的所有功能。 以下功能目前不可用，但将包含在未来版本中：

* 富媒体文件支持
* 比较模式（视频和静态）
* 过滤注释（视频和静态）
* 查看文档中的超链接（静态）
* 翻译（视频和静态）
* 显示当前正在处理验证的用户的存在标识符
* 共享校样

有关在HTML5查看器中校对静态校样的更多信息，请参阅。

作为Workfront Proof中的Workfront管理员，您可以确定贵组织中的用户是否有权访问新的HTML5验证查看器以查看视频验证。

## 新的甘特图重新设计 {#new-gantt-chart-redesign}

新的甘特图包括以下改进：

* 新图标和标记
* 用于放大和缩小特定时间范围的新选项
* 图表列表部分中的较小任务单元格
* 重新设计了设置、打印和切换到预计日期的选项。

有关配置甘特图中的选项的详细信息，请参阅[配置信息在甘特图上的显示方式](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)。 

## 内置报告包含更新的描述 {#built-in-reports-contain-updated-descriptions}

我们更新了Workfront中系统报表的描述，以包括关于报表类型和所包含字段的信息。  

在此更改之前，我们的大多数内置报告没有描述，或者描述非常有限。

有关内置报告的详细信息，请参阅[使用Adobe Workfront内置报告](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)。

## 导出的报告、列表和功能板中的品牌化 {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>此功能当前在预览环境中的所有群集上不可用。

如果您利用Workfront中的品牌策略，则全局导航栏中使用的徽标现在包含在从Workfront导出的.pdf文件中。

以下.pdf文件将在导出的文档中包含您组织的徽标：

* 导出的列表
* 导出和传递的报表
* 打印的功能板

有关从Workfront导出数据的详细信息，请参阅[导出数据](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)。

## 复制任务和移动任务或问题时的改进 {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

我们改进了您复制任务或移动任务或问题的方式，使其更易于为复制或移动的任务或问题选择父级。 例如，在复制任务时选择父项时，您现在可以看到任务的层次结构及其父 — 子关系，以及在具有大量任务的项目中搜索父项。

在此更改之前，**选择父项**&#x200B;步骤中没有搜索字段，任务列表中的任务层次结构不可见。

有关复制任务的详细信息，请参阅[复制和复制任务](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)。

有关移动问题的详细信息，请参阅[移动问题](../../../../manage-work/issues/manage-issues/move-issues.md)。

## 用于在“审批设置”区域中撤消请求的新配置 {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

我们已在系统级别的批准设置区域引入新设置，以允许Workfront管理员决定他们是否应允许用户撤消其第一个状态为未决批准的问题或请求。 如果允许撤消，则问题将被删除；如果不允许撤消，则当问题的第一个状态为未决批准时，用户无法看到“撤消”按钮。

在此更改之前，始终允许召回问题。 撤回批准后，批准被完全绕过，将问题置于其第一状态，不附批准。

有关审批设置的详细信息，请参阅[配置全局审批设置](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)。 

>[!NOTE]
>
>此功能发布时，默认情况下将禁用此选项。 默认情况下，所有组织都启用当前回调问题。 发布此功能时，Workfront管理员必须手动启用此设置，以便保持该功能在Workfront中的原样。

## 资源预算小时报表的新分组：分配日期 {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

我们添加了当您构建资源预算小时数报告时按分配日期对您的结果进行分组的功能。

在此更改之前，您可以在报表视图中显示分配日期，并在筛选器中使用它，但不能在分组中使用此字段。

有关分配日期的详细信息，请参阅[Adobe Workfront术语词汇表](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

有关生成报告的详细信息，请参阅[创建自定义报告](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

## 资源规划者改进 {#resource-planner-improvements}

* [资源规划者：按FTE显示数据](#resource-planner-show-data-by-fte)
* [资源规划者：按周和季度显示数据](#resource-planner-show-data-by-week-and-quarter)
* [资源规划者：按用户查看](#resource-planner-view-by-user)
* [资源规划者：拖放项目以建立优先级](#resource-planner-drag-and-drop-projects-to-establish-priority)
* [资源规划者：将资源规划者中的数据导出到Excel](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### 资源规划者：按FTE显示数据 {#resource-planner-show-data-by-fte}

您现在可以在资源规划程序中按FTE显示资源的分配和可用性。 在此更改之前，您只能以小时为单位显示值。

有关使用资源规划者的详细信息，请参阅[资源规划者概述](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

### 资源规划者：按周和季度显示数据 {#resource-planner-show-data-by-week-and-quarter}

您现在可以更改资源规划者的时间范围间隔，以按周或季度查看。 在此更改之前，您可以查看资源的分配和可用性，并仅按月份对其进行预算。

有关使用资源规划者的详细信息，请参阅[资源规划者概述](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

### 资源规划者：按用户查看 {#resource-planner-view-by-user}

现在，您可以在资源规划程序中按用户、先按项目、角色和任务显示信息。 您还可以为用户显示计划小时数和可用小时数或FTE之间的差异。 在此更改之前，您可以按项目和角色在资源规划者中显示信息。

有关使用资源规划者的详细信息，请参阅[资源规划者概述](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

### 资源规划者：拖放项目以建立优先级 {#resource-planner-drag-and-drop-projects-to-establish-priority}

您现在可以根据所需的优先级顺序拖放项目。 在此更改之前，您只能通过手动为项目分配一个编号来建立项目的优先级。

有关使用资源规划者的详细信息，请参阅[资源规划者概述](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

### 资源规划者：将资源规划者中的数据导出到Excel {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

您现在可以将资源规划者中的信息导出到Excel文件。

有关使用资源规划者的详细信息，请参阅[资源规划者概述](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)。

## 移动改进 {#mobile-improvements}

我们添加了从Workfront移动设备应用程序访问和管理项目的功能。 现在，您可以使用Workfront移动设备应用程序执行以下操作：

* 访问项目列表
* 访问项目中的任务和子任务的列表
* 访问项目的问题列表
* 在项目上记录新问题

您可以在更新Workfront移动应用程序时安装此功能。 此更新将于2017年11月在Apple和Android移动商店中提供。

## Workfront与Slack集成 {#workfront-integration-with-slack}

>[!NOTE]
>
>Slack集成当前不可用。 它将于2017年11月可用于您的生产环境。

我们正在启动Workfront与Slack之间的新集成。 如果贵组织已经在使用Slack进行通信，则您现在可以将其与Workfront集成并执行常见的Workfront操作，而无需在Slack中离开通信渠道。 您现在可以通过Slack帐户执行以下操作：

* 在Workfront中搜索项目
* 访问您的工作和审批列表
* 创建任务
* 创建问题
* 订阅与您共享的链接中的任意项目到该项目
* 通过与您共享的链接将任务和问题分配给他们
* 批准您的工作
* 访问“收藏夹”和“最近项目”列表

有关从Slack访问Workfront的更多信息，请参阅[将Workfront与Slack结合使用。](https://support.workfront.com/hc/en-us/sections/115000458033)

## Outlook 365改进 {#outlook-365-improvements}

我们已对的Workfront加载项进行了以下改进  Outlook 365：

* 在Workfront中将任务或问题添加到项目：您现在可以使用Outlook 365加载项在Workfront中将电子邮件转换为任务或问题。 在此流程中，您可以指定要将任务或问题添加到的项目，以及被分派人和到期日期。 在此增强功能之前，您只能向请求队列提交请求，或向Outlook 365中的“正在处理”列表添加个人任务。 
* 保留原始电子邮件中转换为任务、问题或请求的Workfront对象的链接：将来自Outlook 365的电子邮件转换为任务、问题或请求时，Outlook 365会保留原始电子邮件中从该电子邮件转换的任务或问题的链接。 在此更改之前，Outlook中没有任何指示电子邮件是否已转换为任务或作为请求提交。 

## API更改 {#api-changes}

* [API 8现已可用](#api-8-now-available)
* [已移除和已弃用的API版本](#removed-and-deprecated-versions-of-the-api)
* [2017.3 Beta最终发行版活动](#updated-message-format-for-event-subscriptions)
* [无法投放消息的事件订阅重试](#event-subscription-retries-for-undeliverable-messages)

### API 8现已可用 {#api-8-now-available}

Workfront API版本8现已可用，并且可为您的Workfront集成为您提供新的和更新的资源。

有关Workfront API更改列表，请参阅[API版本8](../../../../wf-api/api/new-api-version-8-updates.md)的更新。

### 已移除和已弃用的API版本 {#removed-and-deprecated-versions-of-the-api}

### 更新了活动订阅的消息格式

为了向包含Workfront事件订阅API的集成提供更多有用信息，我们通过包含与这些资源关联的旧值和新值，更改了支持资源的出站消息格式。 为避免失败，您需要将使用Workfront事件订阅API的任何集成更新为新格式，如[事件订阅API](../../../../wf-api/general/event-subs-api.md)中所述。

### 无法投放消息的事件订阅重试 {#event-subscription-retries-for-undeliverable-messages}

Workfront事件订阅框架现在提供了一种机制，用于处理无法交付到客户端点的事件触发出站消息。 为确保报文持续投放，客户应确保正确设置任何使用事件订阅出站报文的端点。 有关详细信息，请参阅[事件订阅重试次数](../../../../wf-api/api/event-sub-retries.md)。

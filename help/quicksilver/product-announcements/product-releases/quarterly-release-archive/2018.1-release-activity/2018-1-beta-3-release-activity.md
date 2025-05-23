---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 Beta 3发行版活动
description: 本页介绍了2018.1 Beta 3版本在“预览”环境中最近提供的所有更改。 该功能已于2018年1月7日在预览环境中提供。 它将于2018年初在“生产”环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 26bbc4a0-e5ed-4b5f-bfc2-f888362c1d22
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 0%

---

# 2018.1 Beta 3发行版活动

本页介绍了2018.1 Beta 3版本在“预览”环境中最近提供的所有更改。 该功能已于2018年1月7日在预览环境中提供。 它将于2018年初在“生产”环境中提供。

>[!IMPORTANT]
>
> 此页面上描述的功能在生产环境中可用之前可能会发生更改。

有关2018.1版中所做所有更改的列表，请参阅  [2018.1版本活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md)。

2018.1 Beta 3版本包含面向Workfront管理员和其他用户的增强功能：

管理员的&#x200B;**&#x200B;**

* [组管理员改进](#group-administrator-improvements)

所有用户&#x200B;**&#x200B;**

* [HTML5验证查看器改进](#html5-proofing-viewer-improvements)
* Workfront中的[验证改进](#proofing-improvements-within-workfront)
* [主页区域改进](#home-area-improvements) 
* [Agile改进](#agile-improvements)
* [甘特图改进](#gantt-chart-improvements)
* [资源规划者改进](#resource-planner-improvements)

## 组管理员改进 {#group-administrator-improvements}

* [重置组管理员的密码UI已更新](#reset-password-ui-updated-for-group-administrators)
* [组管理员的访问级别设置选项](#access-level-setup-options-for-group-administrators)
* [为组创建时间表配置文件](#create-timesheet-profiles-for-groups)
* [以组管理员身份恢复用户的已删除项目](#recover-deleted-items-for-users-as-a-group-administrator)

### 为组管理员更新了重置密码UI {#reset-password-ui-updated-for-group-administrators}

作为组管理员，当您为其他用户重置密码时，系统会提示您输入自己的密码，然后才能更改他们的密码。 更新了UI以反映此功能。 在此更改之前，UI显示需要Workfront管理员密码。

有关为其他用户重置密码的详细信息，请参阅[编辑用户的配置文件](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

有关组管理员的权能的详细信息，请参阅[创建组](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的“组管理员的权能”部分。

### 组管理员的访问级别设置选项 {#access-level-setup-options-for-group-administrators}

作为Workfront管理员，您现在可以控制组管理员是否可以作为其他用户登录，或者他们是否可以重置其他用户的密码。 我们已在访问级别中添加了新设置，以启用或禁用此访问。 在此更改之前，所有组管理员都可以作为其他用户登录，并默认重置其他用户的密码。 此更改仅影响Planner访问级别。

有关为用户配置访问级别的详细信息，请参阅[向用户授予访问权限](../../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

有关组管理员的权能的详细信息，请参阅[创建组](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的“组管理员的权能”部分。

### 为组创建周期性工时表 {#create-timesheet-profiles-for-groups}

作为组管理员，您现在可以为您管理的组创建时间表配置文件，并将其与您管理的组或这些组中的用户相关联。 时间表配置文件确保自动为与其关联的用户创建时间表。

在此更改之前，只有Workfront管理员可以创建时间表配置文件。

有关创建时间表配置文件的详细信息，请参阅[创建、编辑和分配时间表配置文件](../../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)。

有关组管理员的权能的详细信息，请参阅[创建组](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的“组管理员的权能”部分。

### 以组管理员身份恢复用户的已删除项目 {#recover-deleted-items-for-users-as-a-group-administrator}

如果项目与您作为组管理员的组相关联，则可以从回收站中恢复该项目或其任何已删除的任务、问题或文档。 在此更改之前，只有Workfront管理员才能从回收站中恢复项目。

有关在Workfront中恢复已删除项目的详细信息，请参阅[恢复已删除的项目](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)。

有关组管理员的权能的详细信息，请参阅[创建组](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)中的“组管理员的权能”部分。 

## HTML5验证查看器改进  {#html5-proofing-viewer-improvements}

* [比较模式](#compare-mode)
* [筛选评论列表](#filter-the-comment-list)
* [在输入第一个字符后搜索注释列表](#comment-list-is-searched-after-the-first-character-is-entered)

### 比较模式 {#compare-mode}

现在，您可以在查看HTML5校对查看器中查看静态和视频校对时使用比较模式。 

HTML5验证查看器中的比较模式与旧版验证查看器在以下方面不同：

* 在启动比较模式时，较新版本将移动到右侧，而您正在比较的版本将在左侧打开。

  以前，较新的版本移至左侧，而您要比较的版本在右侧打开。

* 您可以直接从验证查看器中选择要比较的验证版本。 
* 当进入同时导航时，保持校样查看器中校样的当前缩放级别和位置。
* 使用同步导航时新增重置选项。
* 退出比较模式时，可以选择要关闭的校样。 

  以前，旧版本始终处于关闭状态。

* 各种外观和感觉以及可用性改进。

有关详细信息，请参阅[在验证查看器中比较验证](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/compare-proofs.md)。

### 筛选评论列表 {#filter-the-comment-list}

您现在可以在注释列表中过滤注释。 您可以按用户、操作、未读内容等进行过滤。

### 在输入第一个字符后搜索注释列表 {#comment-list-is-searched-after-the-first-character-is-entered}

现在，搜索注释列表时，在您键入第一个字符后，将自动过滤列表。

在此更改之前，您必须在搜索字段中至少键入3个字符，然后才能过滤评论列表。

有关更多信息，请参阅中的。

## Workfront中的验证改进 {#proofing-improvements-within-workfront}

* [将校样从Workfront Proof链接到Workfront](#link-proofs-from-workfront-proof-to-workfront)
* [无法再从文档中删除校对](#can-no-longer-remove-a-proof-from-a-document)
* [生成和打开验证时的外观更新](#updated-look-and-feel-when-generating-and-opening-proofs)

### 将校样从Workfront Proof链接到Workfront {#link-proofs-from-workfront-proof-to-workfront}

现在，您可以将Workfront Proof帐户中已存在的文档校对关联到Workfront。

在此更改之前，您无法访问Workfront中Workfront Proof中已存在的验证。 

有关详细信息，请参阅[链接外部应用程序的文档](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)中的[链接外部应用程序的文档](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

### 无法再从文档中删除验证 {#can-no-longer-remove-a-proof-from-a-document}

您无法再从文档中删除验证。 相反，要删除验证，您必须删除整个文档。

此增强功能降低了用户意外删除校对文档所有版本的风险。 

有关删除文档的信息，请参阅[删除验证](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md)中的[删除验证](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md)。

### 生成和打开验证时的外观更新 {#updated-look-and-feel-when-generating-and-opening-proofs}

现在，当生成验证时，有一个更新的动画旋转器。

## 主页区域改进 {#home-area-improvements}

对“主页”区域进行了以下增强：

* [从主页区域查看校对审批](#view-proof-approvals-from-the-home-area)
* [为主页区域中的项目配置布局模板时，显示默认字段](#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area)

### 从主页区域查看验证审批 {#view-proof-approvals-from-the-home-area}

除了标准审批之外，您现在还可以在主页区域查看验证审批。

以前，您可以查看Workfront审批，但无法查看验证的审批。  

有关详细信息，请参阅[使用主页区域](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)。

### 为主页区域中的项目配置布局模板时，显示默认字段 {#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area}

以前，默认字段在布局模板中不可见。

有关详细信息，请参阅创建和管理布局模板。

## Agile改进 {#agile-improvements}

* [直接从任务或问题详细信息页面将任务和问题添加到迭代](#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page)
* [包含敏捷团队的Scrum积压和故事板上的问题](#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team)
* [将分组和筛选器应用于Agile团队的积压工作](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [创建空白迭代并稍后更新](#create-a-blank-iteration-and-update-it-later)
* [创建迭代时会预填充“焦点”和“容量”字段](#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration)

### 直接从任务或问题详细信息页面将任务和问题添加到迭代 {#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page}

您现在可以直接从任务或问题将当前分配给Agile团队的任务和问题添加到开发周期。

以前，您只能从积压工作中将任务添加到迭代。 

有关详细信息，请参阅[创建迭代](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)中的[创建迭代](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)。

### 包括有关Agile团队的Scrum积压和故事板的问题 {#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team}

在使用Scrum敏捷方法时，问题现在默认包含在敏捷团队的积压中（在使用Kanban方法时，问题未显示在敏捷团队的积压中）。

在此更改之前，只能将任务添加到积压。 如果要添加问题，必须先将问题转化为任务，然后才能添加问题。

有关在积压中使用问题的信息，请参阅  [管理Agile积压](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)。

### 将分组和筛选器应用于Agile团队的积压 {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

分组和筛选选项现在适用于Agile积压，允许您按分组组织积压，并筛选特定任务和问题。

在此更改之前，您可以将视图应用于Agile积压。

有关更多信息，请参阅  [管理Agile积压工作](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)，位于  [管理Agile积压](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)。

### 创建空白迭代并稍后更新 {#create-a-blank-iteration-and-update-it-later}

您不再需要将任务或问题添加到开发周期中来创建它。 您可以创建一个空白迭代，并在以后添加任务和问题。

有关详细信息，请参阅[创建迭代](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)。

### 创建迭代时会预填充“焦点”和“容量”字段 {#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration}

现在，在创建迭代时，“焦点”和“容量”字段会预填充您的团队已创建的所有过去迭代的平均值。 如果您的团队尚未创建任何过去的小版本，则这些字段将显示为0。

以前，这些字段始终设置为0。

有关详细信息，请参阅[创建迭代](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)。

## 甘特图改进 {#gantt-chart-improvements}

* [在甘特图中启用编辑模式](#enable-edit-mode-in-the-gantt-chart)
* [编辑甘特图时删除前置任务](#remove-predecessors-when-editing-the-gantt-chart)

### 在甘特图中启用编辑模式 {#enable-edit-mode-in-the-gantt-chart}

在甘特图中启用编辑模式时，可以更改图表中的信息。 在此更改之前，您无法编辑甘特图中的信息。 您只能在任务列表中编辑任务信息。

有关编辑甘特图的详细信息，请参阅任务列表甘特图中的[更新信息](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)。

### 编辑甘特图时删除前置任务 {#remove-predecessors-when-editing-the-gantt-chart}

使用甘特图的编辑模式，您现在可以删除项目甘特图中任务之间的前置任务关系。 在此增强功能之前，您只能在任务列表或任务级别删除前置任务关系。

有关编辑甘特图的详细信息，请参阅任务列表甘特图中的[更新信息](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)。

## 资源规划者改进 {#resource-planner-improvements}

* 资源规划者中的持续时间为零的[预算](#budget-with-zero-duration-in-the-resource-planner)

* [在资源规划程序中按成本显示数据](#show-data-by-cost-in-the-resource-planner)

### 资源规划者中的持续时间为零的预算 {#budget-with-zero-duration-in-the-resource-planner}

>[!NOTE]
>
>此功能已从预览环境中移除，将在18.1版本中发布。

您现在可以在资源规划者中为项目时间范围内的任何日期预算资源。 在此增强功能之前，您只能为项目时间范围内的日期预算资源。

有关资源规划者中预算资源的详细信息，请参阅[资源规划者概述](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)中的“资源规划者中的预算资源”部分。

### 在资源规划程序中按成本显示数据 {#show-data-by-cost-in-the-resource-planner}

除了小时和FTE值之外，您现在还可以按成本在资源计划程序中显示信息。 在“按项目查看”或“按角色查看”视图中查看资源计划器时，您可以在资源计划器中显示成本。 在“按用户查看”视图中查看资源规划者时无法显示成本。

有关按小时、FTE或成本值查看资源规划者的详细信息，请参阅[资源规划者导航概述](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)。

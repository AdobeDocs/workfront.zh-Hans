---
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3项目增强功能
description: 此页面介绍了在2019.3版本中进行的项目增强功能的所有更改。 该版本在2019年8月19日当周的生产环境中提供。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 127d695c-74e4-45f9-b5f6-55c1d05935cf
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1369'
ht-degree: 0%

---

# 2019.3项目增强功能

此页面介绍了在2019.3版本中进行的项目增强功能的所有更改。 该版本在2019年8月19日当周的生产环境中提供。

有关2019.3版中所做所有更改的列表，请参阅 [2019.3发布活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## 更改自定义表单中字段的显示类型

现在，您可以更改自定义表单中字段的显示类型。

例如，如果您已创建复选框字段，则可以将其更改为下拉列表字段或单选按钮字段。 这三种字段显示类型可以互换。

或者，如果您已创建单行文本字段，则可以将其更改为段落文本字段。 这两种字段显示类型可以互换。

以前，要更改自定义字段的显示类型，您必须创建新字段并删除旧字段。 这需要传输数据，而这通常非常耗时。

有关更多信息，请参阅 [创建或编辑自定义表单](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) 在文章中 [创建或编辑自定义表单](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

>[!NOTE]
>
>预览可用性： 2019年8月9日
>
>生产可用性：2019年8月30日

## 创建休息时间日历和报告

您现在可以看到用户的休息时间，以便更好地规划和执行。 您还可以将新的休息时间报告和日历添加到功能板，以便实时查看用户可用性。

>[!NOTE]
>
>预览可用性： 2019年8月9日
>
>生产可用性：2019年8月30日

## “打开”筛选器现在在问题列表中显示更多结果

将开放过滤器应用于问题列表时，该列表包含以下问题：

* 处于“已关闭 — 未决批准”状态
* 与解析对象相关联

在此更改之前，在应用“打开”筛选器时，这些问题未包含在列表中。

## 在列表中内联编辑信息时的新体验

当在新列表中内联编辑信息时，已编辑的行将变暗，但信息将保持可见。 在此更改之前，编辑的行显示为灰色，并且信息不可见。

您可以在Workfront的以下区域找到新列表：

* 项目和任务列表
* 项目、任务和问题的“小时”选项卡

## 项目、任务和问题小时选项卡的更新列表

项目、任务和问题的小时选项卡中现在提供了改进的列表视图。

在此增强功能之前，新列表仅应用于以下内容：

* 任务列表
* 项目列表

有关查看列表中的项目的信息，请参见 [开始使用Adobe Workfront中的列表](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## 在不启用特殊编辑模式的情况下编辑甘特图

现在可以编辑任务列表甘特图（无论是否启用了自动保存）。 切换打开时无法撤消更改。 在这种情况下，将自动保存您对项目所做的更改。

有关编辑任务列表甘特图的信息，请参阅 [更新任务列表甘特图中的信息](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## 从Kanban展示板中删除“问题”选项卡

我们正在从19.3生产版本中的Kanban展示板中删除“问题”选项卡。 您仍然可以从Kanban展示板上的积压工作中访问“问题”子选项卡。

## 从迭代详细信息页面中删除“文档”和“问题”选项卡

>[!NOTE]
>
>此更改将在2019.3版本的生产中进行。 它不会在生产版本发布之前的“预览”环境中进行。

我们将从Agile迭代详细信息页面中删除“文档”和“问题”选项卡：

* **文档：** 必须在生产版本之前移动存储在文档选项卡中的所有文档。 如果无法移动文档，您将无法再访问它们。
* **问题：** 此选项卡通常位于更多下拉菜单下。 您仍然可以从开发周期的工作项选项卡访问“问题”子选项卡。

## 考虑或忽略任务日期中的用户休息时间

您现在可以决定是否允许任务的主要被分配人的休息时间计划以调整计划日期。

您可以在系统级别(作为Workfront管理员)或项目级别（作为项目经理）做出此决策。

在此更改之前，如果任务限制允许修改日期，则主要被分配人的空闲时间始终调整任务的计划日期。

有关系统级别的用户休息时间设置的信息，请参阅 [配置系统范围的项目首选项](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

有关项目级别的用户休息时间设置的信息，请参阅 [编辑项目](../../../../manage-work/projects/manage-projects/edit-projects.md).

>[!NOTE]
>
>预览可用性： 2019年7月22日
>
>生产可用性：2019年8月9日

## 自定义完成情况

现在，您可以执行以下操作以自定义用于项目、任务和问题的条件，并更好地满足组织的需求：

* 使用您自己的标签和颜色创建自定义条件。
* 更改条件在下拉列表中的顺序，用户可在其中选择条件。
* 使用您创建的自定义条件来取代Workfront自动分配给工作项的内置默认条件。
* 更改项目、任务和问题的内置默认条件的名称和颜色。

此外，如果您有权编辑任务或问题，但您未获得分配（可能是因为您正在监督该任务或问题），则您现在可以使用列表视图中的条件列更改其条件。

以前，无法自定义或更改条件，并且只有分配了任务的用户，才能更改该任务或问题的条件。

有关更多信息，请参阅 [自定义完成情况](../../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

>[!NOTE]
>
>预览可用性： 2019年7月4日
>
>生产可用性： 9月底或10月初

## 团队的新电子邮件通知

为团队提供了新的电子邮件事件通知。 当具有分配给团队的任务的项目变为活动状态时，团队成员会收到电子邮件通知。 默认情况下，此设置处于关闭状态。

以前，当团队成员所在的项目处于活动状态时，无法通知他们。

有关更多信息，请参阅通知：关于我参与的项目的信息。

>[!NOTE]
>
>预览可用性： 2019年7月4日
>
>可用生产：2019年7月18日

## 文档更新现在显示在关联的对象和项目中

在文档上添加注释时，更新现在会显示在文档以及附加该文档的对象的“更新”选项卡上。

如果对象是项目的一部分，则文档上的注释也会出现在项目的“更新”选项卡上。

以前，更新注释仅出现在文档的“更新”选项卡上。

有关更多信息，请参阅部分 [更新工作](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#updates) 在文章中 [更新工作](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>预览可用性： 2019年6月6日
>
>可用生产：2019年6月20日

## 了解将用户分配给任务和问题时的用户休息时间计划

当您将用户分配给任务或问题时，如果所选用户在任务或问题的计划日期之间计划了任意时间的休息时间，您现在可以看到内联警告。

有关分配任务的信息，请参见 [分配任务](../../../../manage-work/tasks/assign-tasks/assign-tasks-1.md)

有关休息时间的信息，请参阅 [配置个人休息时间](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

>[!NOTE]
>
>预览可用性： 2019年5月30日
>
>可用生产：2019年6月13日

## 添加表示自定义Forms中对象的字段

我们在自定义表单生成器中创建了一种名为Typeahead的新字段类型。 此字段允许您向自定义表单添加表示对象的字段。 目前，User对象已启用Typeahead，而其他对象将在未来启用。

以前，管理员必须在自定义表单下拉菜单中手动将用户作为单个选项进行维护。

有关更多信息，请参阅 [创建或编辑自定义表单](../../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>预览可用性： 2019年5月30日
>
>可用生产：2019年6月13日
>
>在生产版本发布日期之前，新的自定义字段在Mobile、Outlook、MS Teams和本机Salesforce集成上不受支持。
>
>在生产环境中，现在支持Outlook和MS团队。 自6月底或7月初起，Mobile已受支持；自6月起，Salesforce集成已受支持。

## 新请求“主题”字段已重命名为“名称”

>[!NOTE]
>
>此功能已被删除，不会包含在2019.3版本中。

现在，当您向请求队列提交新请求时，在新请求表单的“名称”字段中输入请求名称。

在此更改之前，您需要在“主题”字段中输入请求的名称。

有关创建请求的信息，请参阅 [创建和提交Workfront请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).


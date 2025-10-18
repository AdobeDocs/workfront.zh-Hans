---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Kanban概述
description: 请参阅本文，以更好地了解Kanban展示板的运行方式。
author: Jenny
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Kanban概述

<!-- Audited: 01/2024 -->

您可以通过以下部分更好地了解[!UICONTROL Kanban]展示板的运行方式。

有关K[!UICONTROL anban]方法的说明，请参阅[创建Agile团队](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md)。

如果您有兴趣从敏捷团队[!UICONTROL Kanban]展示板迁移到[!DNL Workfront] [!UICONTROL 展示板]，请参阅[将敏捷团队[!UICONTROL Kanban]展示板迁移到 [!DNL Workfront] 展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md)。

## [!UICONTROL Kanban]展示板布局和功能

[!UICONTROL Kanban]展示板由以下元素组成：

**积压工作列**：显示积压工作中的当前所有任务。 默认情况下，此列不显示。 有关积压工作的更多信息，包括如何在[!UICONTROL Kanban]展示板上显示积压工作，请参阅[管理Agile积压工作](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)。

**故事状态**：根据故事所处的状态列指示故事的进度。

有关详细信息，请参阅[在[!UICONTROL Kanban]展示板](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)上更新故事的状态。

通过修改Agile视图，可以为项目自定义故事状态，如[[!UICONTROL 在]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view)中创建或编辑视图中的[创建或自定义Agile视图 [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md)部分所述。

>[!NOTE]
>
>默认情况下，Kanban展示板上最多可显示50张信息卡，但您可以单击&#x200B;**[!UICONTROL 显示更多]**&#x200B;来显示其他信息卡。

## 子任务和故事之间的关系

如果文章包含子任务，则无法更新有关父文章本身的任何信息（例如点/小时或完成百分比）。 此外，您无法跨[!UICONTROL Kanban]展示板移动故事以更新其状态。 相反，您对文章子任务所做的任何更改都会反映在文章中。 所有子任务的合并故事点或小时数决定了父故事的点或小时数。

例如，如果一个故事只有一个子任务被赋值为4点，则该故事本身也有4点。 如果将子任务点值更改为3，则父故事的点值将更改为3。 如果在同一内文中创建另一个子任务，并将该子任务的点值设置为4，则内文的点值将更改为7，以反映两个子任务的组合点值。

此逻辑同样适用于第二级子任务（子任务的子任务）。 如果子任务具有一个或多个第二级子任务，则根据第二级子任务计算子任务。

## 支持的功能

使用Kanban展示板时，您可以执行以下操作：

* [将子任务添加到[!UICONTROL Kanban]展示板上的现有故事中](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [将现有任务或问题添加到[!UICONTROL Kanban]展示板](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [将用户分配给[!UICONTROL Kanban]展示板上的故事](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [从[!UICONTROL Kanban]展示板添加故事和问题](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [从[!UICONTROL Kanban]展示板中删除故事或问题](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [编辑故事信息](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [在[!UICONTROL Kanban]展示板上按用户筛选](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [管理[!UICONTROL Kanban]展示板上的正在进行的工作(WIP)限制](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [重新排序[!UICONTROL Kanban]展示板上的故事](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [更新[!UICONTROL Kanban]展示板上故事的状态](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [在[!UICONTROL Kanban]展示板上的故事上使用标志](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [将积压工作添加到[!UICONTROL Kanban]展示板](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)

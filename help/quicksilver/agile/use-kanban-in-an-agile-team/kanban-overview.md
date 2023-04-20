---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: 看板概述
description: 查看本文，以更好地了解看板板的功能。
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: 2c6a828d95df1229780803a173d5013f5b1eb215
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# 看板概述

通过以下部分，您可以更好地了解 [!UICONTROL 看板] 董事会功能。

如果您有兴趣从敏捷的团队迁移 [!UICONTROL 看板] 展示到 [!DNL Workfront] [!UICONTROL 展示板]，请参阅 [迁移敏捷团队 [!UICONTROL 看板] 信息卡 [!DNL Workfront] 展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## [!UICONTROL 看板] 板布局和功能

的 [!UICONTROL 看板] 展示板包含以下元素：

**积压工作列**:显示当前处于积压工作中的所有任务。 默认情况下，此列不显示。 有关积压的详细信息，包括如何在 [!UICONTROL 看板] 展示板，请参阅 [管理敏捷积压](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**文章状态**:根据文章所在的状态列指示文章的进展情况。

有关更多信息，请参阅 [更新 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

可以通过修改灵活视图为项目自定义文章状态，如一节中所述 [[!UICONTROL 创建或自定义敏捷视图]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [视图概述 [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>默认情况下，看板板上最多显示50张卡，但您可以单击 **[!UICONTROL 显示更多]** 来显示其他卡片。

## 子任务与文章之间的关系

如果文章包含子任务，则无法更新有关父文章本身的任何信息（如点/小时或完成百分比）。 此外，您无法将故事在 [!UICONTROL 看板] 更新其状态。 相反，您对文章子任务所做的任何更改都会反映在文章中。 所有子任务的合并文章点或小时决定父文章的点或小时。

例如，如果一个故事只有一个子任务值为4分，则该故事本身也有4分。 如果将子任务点值更改为3，则父文章的点值将更改为3。 如果在同一文章上创建另一个子任务，并将该子任务的点值设置为4，则文章的点值将更改为7，以便反映两个子任务的合并点值。

同样的逻辑适用于二级子任务（子任务的子任务）。 如果子任务具有一个或多个二级子任务，则子任务基于二级子任务计算。

## 支持的功能

使用看板板时，您可以执行以下操作：

* [将子任务添加到 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [将现有任务或问题添加到 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [将用户分配到 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [添加 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [从 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [编辑文章信息](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [在 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [在 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [重新排序 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [更新 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [在 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [将积压工作添加到 [!UICONTROL 看板] 展示板](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)

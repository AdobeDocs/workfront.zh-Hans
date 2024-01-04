---
content-type: overview
product-area: agile-and-teams
navigation-topic: use-kanban-in-an-agile-team
title: Kanban概述
description: 请参阅本文，以更好地了解Kanban展示板的运行方式。
author: Lisa
feature: Agile
exl-id: d7daa6c1-dae2-4e5c-a765-6a6ebdfaa331
source-git-commit: fa499d74df891441e729c32188e9b2f74e4ef5c0
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Kanban概述

<!-- Audited: 01/2024 -->

通过下列部分，您可以更好地了解 [!UICONTROL Kanban] 董事会职能。

有关K的说明[!UICONTROL anban] 方法，请参见 [创建Agile团队](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

如果您有兴趣从Agile团队进行迁移 [!UICONTROL Kanban] 展示板目标位置 [!DNL Workfront] [!UICONTROL 讨论区]，请参见 [迁移敏捷团队 [!UICONTROL Kanban] 卡到 [!DNL Workfront] 展示板](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

## [!UICONTROL Kanban] 展示板布局和功能

此 [!UICONTROL Kanban] 板由下列元素组成：

**积压工作列**：显示当前积压中的所有任务。 默认情况下，此列不显示。 有关积压工作的更多信息，包括如何在 [!UICONTROL Kanban] 展示板，请参阅 [管理Agile积压](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

**故事状态**：根据故事所处的状态列指示故事的进度。

有关更多信息，请参阅 [在上更新文章的状态 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md).

通过修改敏捷视图，可以为项目自定义故事状态，如一节中所述 [[!UICONTROL 创建或自定义敏捷视图]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) 在 [在中创建或编辑视图 [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

>[!NOTE]
>
>默认情况下，Kanban展示板上最多显示50张信息卡，但您可以单击 **[!UICONTROL 显示更多]** 来显示其他信息卡。

## 子任务和故事之间的关系

如果文章包含子任务，则无法更新有关父文章本身的任何信息（例如点/小时或完成百分比）。 此外，您无法移动故事跨越 [!UICONTROL Kanban] 板以更新其状态。 相反，您对文章子任务所做的任何更改都会反映在文章中。 所有子任务的合并故事点或小时数决定了父故事的点或小时数。

例如，如果一个故事只有一个子任务被赋值为4点，则该故事本身也有4点。 如果将子任务点值更改为3，则父故事的点值将更改为3。 如果在同一内文中创建另一个子任务，并将该子任务的点值设置为4，则内文的点值将更改为7，以反映两个子任务的组合点值。

此逻辑同样适用于第二级子任务（子任务的子任务）。 如果子任务具有一个或多个第二级子任务，则根据第二级子任务计算子任务。

## 支持的功能

使用Kanban展示板时，您可以执行以下操作：

* [将子任务添加到上的现有故事 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/add-a-subtask-to-an-existing-story.md)
* [将现有任务或问题添加到 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/add-existing-tasks-or-issues-to-the-kanban-board.md)
* [将用户分配到上的故事 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/assign-users-to-a-story.md)
* [从添加故事和问题 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/add-story-from-kanban-board.md)
* [从中删除故事或问题 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/delete-story-from-kanban-board.md)
* [编辑故事信息](../../agile/use-kanban-in-an-agile-team/edit-story-information.md)
* [在上按用户筛选 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/filter-by-user.md)
* [管理上的正在进行的工作(WIP)限制 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md)
* [重新排序故事于 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/reorder-stories-on-the-kanban-board.md)
* [在上更新文章的状态 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/update-the-status-of-stories.md)
* [对上的故事使用标志 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/use-flags-on-stories.md)
* [将积压添加到 [!UICONTROL Kanban] 展示板](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md)

---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: 主板概述
description: Scrum敏捷故事板与完成状态和燃尽图一起显示。
author: Lisa
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '867'
ht-degree: 0%

---

# [!UICONTROL Scrum] 展示板概述

的 [!UICONTROL Scrum] 敏捷故事板与完成状态和燃尽图一起显示。 这些敏捷组件在以下情况下可用： [!UICONTROL Adobe Workfront]:

* 在灵活迭代中。 有关在纯敏捷环境（具有积压和迭代）中使用敏捷故事板、燃尽图和完成状态的更多详细信息，请参阅 [在灵活的环境中工作](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).
* 在敏捷视图中查看项目时。 有关如何利用现有项目中的敏捷故事板、燃尽图和完成状态的信息，请参阅 [在敏捷视图中管理项目](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

![敏捷迭代](assets/agile-iteration-with-callouts.png)

## 文章板布局和功能

![敏捷故事板](assets/agile-storyboard-callouts.png)

文章板包含以下元素：

* **[!UICONTROL 父文章] 列：** 与文章栏的其他栏目不同，  [!UICONTROL 父文章]  列不是任务状态，而是存在于小版本或项目中，用于存放包含子任务的任何文章。 只有文章板上至少有一个子任务的父文章才能驻留在此列中。 父文章本身不会在文章展示板中从状态移动到状态。

   在小版本中，仅当文章板上的一个或多个文章包含至少一个满足以下要求的子任务时，此列才会显示在文章板上：

   * 分配给与父任务相同的敏捷团队
   * 属于迭代

      在项目中，当任务至少具有一个子任务时，此列即会显示。

      ![父文章列](assets/agile-parentstory-swimlane.png)

* **任务状态：** 指示文章在小版本或项目中的进展情况，具体取决于文章所在的状态列。

   可以通过修改敏捷视图为项目自定义任务状态，如 [创建或自定义敏捷视图](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [视图概述 [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

* **游泳巷：** 当父文章及其子任务显示在文章板上时，将专门为文章及其子任务创建一条游泳道。 这提供了视觉上的区别，以便更好地查看故事的子任务在整个故事板上的进展情况。

   在迭代中，仅当文章板上的文章包含至少一个满足以下要求的子任务时，泳道才会出现在文章板上：

   * 分配给与父任务相同的敏捷团队
   * 属于迭代

   在项目中，每当任务至少具有一个子任务或一个父任务时，都会显示泳道。

* **个人文章：** 故事板上的任何泳道下方都会显示个别故事和问题。 这与泳道中的故事有视觉区别。

## 子任务与文章之间的关系

如果文章包含子任务，则无法更新有关父文章本身的任何信息（如点/小时或完成百分比）。 此外，您无法在文章展示板中移动文章以更新其状态。 相反，您对文章子任务所做的任何更改都会反映在文章中。 所有子任务的合并文章点或小时决定父文章的点或小时。

例如，如果一个故事只有一个子任务值为4分，则该故事本身也有4分。 如果将子任务点值更改为3，则父文章的点值将更改为3。 如果在同一文章上创建另一个子任务，并将该子任务的点值设置为4，则文章的点值将更改为7，以便反映两个子任务的合并点值。

同样的逻辑适用于二级子任务（子任务的子任务）。 如果子任务具有一个或多个二级子任务，则子任务基于二级子任务计算。

## 故事板与积压的关系

>[!NOTE]
>
>本节中的信息仅适用于迭代的敏捷视图；项目的敏捷视图不使用积压工作。 (有关小版本上的敏捷视图与项目之间差异的详细信息，请参阅使用 [!UICONTROL 敏捷] &quot;关于一个项目的逆&quot;，在 [在敏捷视图中管理项目](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).)

迭代积压仅显示可在其中设置估计的文章或子任务。 如果父文章的子任务显示在文章展示板上（因为它们被分配给同一敏捷团队并且属于小版本），则父任务不会显示在积压工作中。 在这种情况下，只在积压工作中显示子任务，而子任务和父文章则显示在文章展示板上。

例如，假设文章A包含子任务1和子任务2（两个子任务都分配给同一个敏捷团队）。 在这种情况下，文章A显示在具有子任务1和子任务2的游泳道的文章板上。 但是，在积压工作中只显示子任务1和子任务2。

同样的逻辑适用于二级子任务（子任务的子任务）。 如果子任务具有一个或多个分配给同一敏捷团队且属于迭代的二级子任务，则只会在积压工作中显示二级子任务。

有关积压工作的详细信息，请参阅 [管理敏捷积压](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

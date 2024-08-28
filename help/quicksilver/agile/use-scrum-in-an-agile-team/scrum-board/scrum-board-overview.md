---
content-type: overview
product-area: agile-and-teams
navigation-topic: scrum-board
title: Scrum展示板概述
description: Scrum敏捷故事板与完成状态和燃尽图一起显示。
author: Lisa
feature: Agile
exl-id: 584288bb-2d98-4b69-8deb-d3b8e54d328c
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# [!UICONTROL Scrum]展示板概述

[!UICONTROL Scrum]敏捷故事板与完成状态和燃尽图一起显示。 这些Agile组件在[!UICONTROL Adobe Workfront]的以下情况下可用：

* 在敏捷迭代中。 有关在纯Agile环境（包含积压和迭代）中使用Agile故事板、燃尽图和完成状态的更多详细信息，请参阅[在Agile环境中工作](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md)。
* 在Agile视图中查看项目时。 有关如何在现有项目中利用Agile故事板、燃尽图和完成状态的信息，请参阅[在Agile视图中管理项目](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md)。

![Agile迭代](assets/agile-iteration-with-callouts.png)

## 故事板布局和功能

![敏捷故事板](assets/agile-storyboard-callouts.png)

故事板由以下元素组成：

* **[!UICONTROL 父故事]列：**&#x200B;与故事板上的其他列不同，[!UICONTROL 父故事]列不是任务状态，而是为了容纳迭代或项目中包含子任务的任何故事而存在的。 只有故事板上至少有一个子任务的父故事才能位于此列中。 父故事本身不会在故事板中从状态移动到状态。

  在迭代中，仅当故事板上的一个或多个故事包含至少一个满足以下要求的子任务时，此列才会出现在故事板上：

   * 分配给与父任务相同的Agile团队
   * 属于迭代

     在项目中，每当任务至少有一个子任务时，就会显示此列。

     ![父故事列](assets/agile-parentstory-swimlane.png)

* **任务状态：**&#x200B;根据文章所处的状态列，指示文章在迭代或项目中的进度。

  通过修改Agile视图，可以为项目自定义任务状态，如[!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)的[视图概述中的[创建或自定义Agile视图](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view)中所述。

* **泳道：**&#x200B;当父故事及其子任务显示在故事板上时，将专门为故事及其子任务创建泳道。 这提供了一种视觉区别，以便更好地查看故事的子任务在整个故事板中的进度。

  在迭代中，仅当故事板上的故事至少包含一个满足以下要求的子任务时，泳道才会出现在故事板上：

   * 分配给与父任务相同的Agile团队
   * 属于迭代

  在项目中，每当任务至少有一个子任务或一个父任务时，泳道就会出现。

* **个人故事：**&#x200B;个人故事和问题显示在故事板上的任何游泳路线下方。 这与泳道中的故事有视觉上的区别。

## 子任务和故事之间的关系

如果文章包含子任务，则无法更新有关父文章本身的任何信息（例如点/小时或完成百分比）。 此外，您无法在故事板中移动故事以更新其状态。 相反，您对文章子任务所做的任何更改都会反映在文章中。 所有子任务的合并故事点或小时数决定了父故事的点或小时数。

例如，如果一个故事只有一个子任务被赋值为4点，则该故事本身也有4点。 如果将子任务点值更改为3，则父故事的点值将更改为3。 如果在同一内文中创建另一个子任务，并将该子任务的点值设置为4，则内文的点值将更改为7，以反映两个子任务的组合点值。

此逻辑同样适用于第二级子任务（子任务的子任务）。 如果子任务具有一个或多个第二级子任务，则根据第二级子任务计算子任务。

## 故事板和积压之间的关系

>[!NOTE]
>
>此部分中的信息仅适用于开发周期上的Agile视图；项目上的Agile视图不使用积压。 （有关开发周期上的Agile视图与项目之间的差异的更多信息，请参阅[在Agile视图下管理项目](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md)中的“在项目上使用[!UICONTROL Agile]视图与开发周期上的差异”。）

迭代积压事项仅显示可设置估算的故事或子任务。 如果父故事具有显示在故事板上的子任务（因为它们被分配到同一敏捷团队并属于迭代），则父任务不会显示在积压中。 在这种情况下，积压中仅显示子任务，而子任务和父故事显示在故事板上。

例如，假设故事A包含子任务1和子任务2（这两个子任务均分配给同一敏捷团队）。 在这种情况下，故事A显示在包含子任务1和子任务2的泳道中的故事板上。 但是，积压中只显示子任务1和子任务2。

此逻辑同样适用于第二级子任务（子任务的子任务）。 如果子任务具有分配给同一敏捷团队的一个或多个第二级子任务且属于迭代，则积压中仅显示第二级子任务。

有关积压工作的详细信息，请参阅[管理Agile积压工作](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)。

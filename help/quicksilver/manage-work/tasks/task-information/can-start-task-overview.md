---
content-type: overview
product-area: projects
navigation-topic: task-information
title: 任务的“可以开始”概述
description: 当任务准备就绪后，Adobe Workfront会向该任务中添加“可以启动”指示器，以便轻松确定开始处理该任务是否安全。 您可以在任务列表或报告的视图中查看此指示器。
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 任务的“可以开始”概述

当任务准备就绪后，Adobe Workfront会向该任务中添加“可以启动”指示器，以便轻松确定开始处理该任务是否安全。 您可以在任务列表或报告的视图中查看此指示器。

任务准备就绪后，任务上的“可以启动”字段将设置为True。

## Workfront如何将任务标记为“可以开始”

Workfront在将任务标记为True（可以开始）字段之前，会检查以下事项：

* 如果任务具有父项，则它会检查该任务的父项是否设置为True的“可以开始”值。 如果父项的值为False，则所有子任务的值都将“可以开始”设置为False。 
* 它还会检查任务的前任和父代的前任是否完成。 如果任务已完成，则任务的“可以启动”值将设置为True。 如果任务前置任务或其父任务的前置任务未完成，或者状态为“完成 — 待批准”，则任务的“可以开始”值将设置为“False”。 

   有关任务前置任务的信息，请参阅 [任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 有关确定已准备好开始的任务的注意事项

* 如果任务与其前置任务之间的依赖关系类型为“开始 — 开始”，则前置任务必须先启动，然后才能考虑解决前置任务关系并启动后续任务。 有关依赖关系类型的信息，请参阅 [任务依赖关系类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* 如果任务具有跨项目前置项，则前置项的完成不会触发“可以开始”指示符以自动应用于后继项。 您必须人工重新计算继任者项目的时间表，或者Workfront必须自动重新计算时间表，之后继任务才能显示为“可以启动”任务。 有关重新计算项目时间轴的更多信息，请参阅 [重新计算项目时间表](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

   有关跨项目前置项的信息，请参阅 [创建跨项目前置项](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

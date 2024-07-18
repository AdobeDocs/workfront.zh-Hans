---
content-type: overview
product-area: projects
navigation-topic: task-information
title: “可以开始”任务概述
description: 当任务准备开始时，Adobe Workfront会向任务添加一个“可以开始”指示器，以便轻松识别开始处理任务是否安全。 您可以在任务列表或报告的视图中查看此指示器。
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 任务的“可以开始”概述

当任务准备开始时，Adobe Workfront会向任务添加一个“可以开始”指示器，以便轻松识别开始处理任务是否安全。 您可以在任务列表或报告的视图中查看此指示器。

当任务准备就绪以进行处理时，任务的“可以开始”字段将设置为“True”。

## Workfront如何将任务标记为“可以开始”

Workfront会先检查以下内容，然后再在“可以开始”字段中将任务标记为“真”：

* 如果任务有父任务，它会检查父任务的“可以启动”值是否设置为True。 如果父任务的值为False，则所有子任务的值为Can Start也会设置为False。 
* 它还会检查任务的前置任务及其父项的前置任务是否完整。 如果任务完成，任务的“可以开始”值将设置为True。 如果任何任务前置任务或其父项的前置任务未完成，或状态为“完成 — 未决批准”，则任务的“可以开始”值将设置为False。 

  有关前置任务的信息，请参阅[前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

## 关于识别准备开始任务的注意事项

* 如果任务与其前置任务之间的依赖关系类型为“开始 — 开始”，则前置任务必须在前置任务关系被视为已解决并且后续任务可以开始之前开始。 有关依赖关系类型的信息，请参阅[任务依赖关系类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。
* 如果任务具有跨项目前置任务，则前置任务的完成不会触发可以开始指示符自动应用于前置任务。 您必须手动重新计算后续任务项目的时间线，或者Workfront必须先自动重新计算该时间线，然后后续任务才会显示为“可以开始”任务。 有关重新计算项目时间线的详细信息，请参阅[重新计算项目时间线](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)。

  有关跨项目前置任务的信息，请参阅[创建跨项目前置任务](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md)。

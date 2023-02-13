---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 任务依赖关系循环概述
description: 在向任务添加前置关系时，您可能会遇到依赖关系循环。 有关前置任务的信息，请参阅前置任务的概述。
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# 任务依赖关系循环概述

在向任务添加前置关系时，您可能会遇到依赖关系循环。 有关前置任务的信息，请参阅 [任务前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## 依赖关系循环概述

当您有两个或多个相互依赖的任务要完成时，会发生依赖关系循环。 Adobe Workfront不允许在任务之间创建前置关系（如果它创建依赖关系循环）。

**示例：** 任务2是任务1的前身，这意味着您必须先完成任务2，然后才能开始处理任务1。

如果尝试将任务1设为任务2的前置任务，则会出现依赖关系循环错误，因为在任务2完成之前，不能启动任务1，但任务2只有在任务1完成之后才能启动。

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## 有关依赖关系循环的注意事项

* 依赖关系循环可能涉及两个以上的任务。 有时，您与前置关系连接的任务的任何父级都是创建依赖关系循环的任务。
* 如果尝试将父项设为子项的前身，则也会发生依赖关系循环。
* 在依赖关系循环中，无法保存任务或项目。 要修复依赖关系循环，您必须重新评估错误消息中所列任务之间的前置任务关系，并删除冲突，然后才能保存任务或项目。

 

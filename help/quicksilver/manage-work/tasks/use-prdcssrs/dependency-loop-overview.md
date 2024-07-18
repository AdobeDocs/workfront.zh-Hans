---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: 任务依赖性循环概述
description: 将前置任务关系添加到任务时，您可能会遇到依赖关系循环。 有关前置任务的信息，请参阅任务前置任务概述。
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# 任务依赖性循环概述

将前置任务关系添加到任务时，您可能会遇到依赖关系循环。 有关前置任务的信息，请参阅[前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

## 依赖性循环概述

当有两个或多个任务相互依赖而需要完成时，就会发生依赖性循环。 如果Adobe Workfront创建依赖性循环，则不允许您在任务之间创建前置任务关系。

**示例：**&#x200B;任务2是任务1的前置任务，这意味着您必须先完成任务2，然后才能开始处理任务1。

如果尝试将任务1设置为任务2的前置任务，则会出现依赖关系循环错误，因为只有在任务2完成之后才能启动任务1，但在任务1完成之前无法启动任务2。

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## 关于依赖性循环的注意事项

* 依赖性循环可能涉及两个以上的任务。 有时，与前置任务关系连接的任务的任意数量的父项是创建依赖关系循环的父项。
* 如果您尝试将父项设置为子项的前置项，则也会发生依赖关系循环。
* 如果存在依赖性循环，则无法保存任务或项目。 为了修复依赖性循环，您必须重新评估错误消息中列出的任务之间的前置任务关系，并在保存任务或项目之前删除冲突。

 

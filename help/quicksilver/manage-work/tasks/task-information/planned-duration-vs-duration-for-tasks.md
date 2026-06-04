---
content-type: reference
product-area: projects
navigation-topic: task-information
title: 计划持续时间和任务持续时间之间的差异
description: 持续时间是工作项的计划开始日期和计划完成日期之间的时间量。 任务在Adobe Workfront中具有持续时间和已计划持续时间，具体取决于任务的持续时间类型。
author: Alina
feature: Work Management
exl-id: 183a3334-b4af-4f45-8e72-9e82ff3862a0
TQID: https://experienceleague.adobe.com/tVh55DKoBvOUZdq9lZ6y72rxZQ1WOoAYL-Pz8nlU588
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 272
ht-degree: 0%

---

# 任务计划持续时间和持续时间之间的差异

持续时间是工作项的计划开始日期和计划完成日期之间的时间量。 任务在Adobe Workfront中具有持续时间和已计划持续时间，具体取决于任务的持续时间类型。

问题和项目不能与持续时间类型关联，它们只有持续时间。

## 任务持续时间

对于任务，“持续时间”和“已计划持续时间”通常显示相同的值：任务的已计划开始日期与已计划完成日期之间的时间长度。

当任务的持续时间类型为投入比导向时，计划的持续时间会随着您向任务添加资源而减少。

**示例：**&#x200B;如果一项任务的工期类型为投入比导向，该任务的工期为3天，而您为该任务分配了一个具有全职计划的资源，则计划工期也为3天。

如果将具有全职计划的三个资源分配给同一任务，则持续时间将保留3天，但计划持续时间将变为1天。计划持续时间还会更改任务的计划开始日期和计划完成日期，以反映新的计划持续时间。因此，项目的时间表也会受到影响。
将任务分配给多个资源时，可以使用投入比导向的持续时间类型。这减少了完成任务工作所需的时间。

有关投入比驱动的持续时间类型的详细信息，请参阅[持续时间类型概述：投入比驱动](../../../manage-work/tasks/taskdurtn/effort-driven.md)。

## 问题和项目持续时间

问题和项目只有一个“持续时间”值，该值分别为问题和项目的计划开始日期和计划完成日期之间的差值。

---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: 迭代完成状态概述
description: 本文描述的完成信息显示在燃耗图上方。
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: 373f2522b85196d6395f189ae6cfe03449cac61a
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# 迭代完成状态概述

本文描述的完成信息显示在燃耗图上方。

迭代的完成百分比：

![](assets/burndown-percentcomplete-350x47.png)

此信息指示在燃耗图中当前选定的日期的迭代完成状态。 默认情况下，会根据当天的日期显示完成状态。

以下信息可供使用：

* **[!UICONTROL 完成百分比]:** 迭代的总体进度

   [!UICONTROL 完成百分比] 根据迭代中每个文章或任务的完成百分比进行调整，包括仅部分完成的文章或任务。

   的颜色 [!UICONTROL 完成百分比] 状态栏显示为红色或绿色，以匹配实际燃耗率的颜色。 当燃耗率小于理想值时，它以红色显示（每天剩余的点数或小时数多于理想值）；当燃耗率等于或优于理想值时，它以绿色显示（每天剩余的点数等于或少于理想值计算）。

* **[!UICONTROL 已完成的文章]:** （仅在小版本中可用）标记的文章数 [!UICONTROL 完成]. 这与小版本中的文章总数有关。 例如，“6的3个”表示小版本中6个文章中的3个已标记 [!UICONTROL 完成].
* **[!UICONTROL 完成的点数/小时]:** （仅在迭代中可用）标记的点数或小时数 [!UICONTROL 完成]. 与小版本中的总点数或小时数有关。 例如，“11的5篇”表示小版本中11篇文章中的5篇已标记 [!UICONTROL 完成]. 此数字与 [!UICONTROL 完成百分比] 计算，并会同时更新 [!UICONTROL 完成百分比] 更新。

   点数和小时数与文章相关。 当文章被标记时 [!UICONTROL 完成]，则与该文章关联的点数或小时数将标记为完成。

   默认情况下，会使用点。 您可以通过修改团队的设置来更改此设置，如 [创建敏捷的团队](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL 每日点数/小时数]:** （仅在迭代中可用）标记的平均点数或小时数 [!UICONTROL 完成] 从迭代开始到当天的每一天。

   此值由完成的总点数或小时数除以当天的总天数计算。 （部分天数将记录为整天。）

   此信息在规划将来的迭代时很有用。

* **[!UICONTROL 估计完成]:** 预计完成迭代的日期，基于每天点数/小时数中的当前比率（对于迭代）。

   当 [!UICONTROL 估计完成] 日期晚于为小版本定义的结束日期，剩余的工作天数将在小版本的 [!UICONTROL 估计完成] 日期。

   当 [!UICONTROL 估计完成] 日期早于小版本的计划结束日期，剩余工作天数将以绿色显示。 (计划小版本时指定小版本的结束日期，如 [创建迭代](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md);项目的结束日期是 [!UICONTROL 计划完成日期]，或者如果 [!UICONTROL 计划完成日期] 是过去。 的 [!UICONTROL 计划完成日期] )。 在计划小版本时，如果为非工作日设置小版本结束日期，并且小版本正在跟踪以按时完成，则在您设置的小版本结束日期之前的最后一个工作日设置“估计完成日期”（因为工作未计划在非工作日烧录）。

   例如，“（+9天）”表示预计完成日期比小版本的计划结束日期晚9个工作日。

   有关更多信息，请参阅 [迭代完成状态概述](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).

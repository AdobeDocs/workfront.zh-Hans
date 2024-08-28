---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: 迭代完成状态概述
description: 本文中描述的完成信息显示在燃尽图的上方。
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---

# 迭代完成状态概述

本文中描述的完成信息显示在燃尽图的上方。

迭代的完成百分比：

![](assets/burndown-percentcomplete-350x47.png)

此信息指示当前在燃尽图中选择的日期的迭代的完成状态。 默认情况下，会根据当天的日期显示完成状态。

以下信息可供使用：

* **[!UICONTROL 完成百分比]：**&#x200B;迭代的整体进度

  [!UICONTROL 完成百分比]根据迭代中每个文章或任务的完成百分比进行调整，包括仅部分完成的文章或任务。

  [!UICONTROL 完成百分比]状态栏的颜色显示为红色或绿色，以匹配实际燃尽率的颜色。 当燃尽率小于理想值（比理想燃尽计算每天剩余的点数或小时数多）时，它以红色显示；当燃尽率等于或大于理想值（等于或小于理想燃尽计算每天剩余的点数）时，它以绿色显示。

* **[!UICONTROL 已完成的故事]：** （仅在迭代中可用）标记为[!UICONTROL 完成]的故事数。 这相对于迭代中的文章总数显示。 例如，“第3个（共6个）”表示迭代中6个故事中有3个已被标记为[!UICONTROL 完成]。
* **[!UICONTROL 已完成点数/小时数]：** （仅在迭代中可用）标记为[!UICONTROL 完成]的点数或小时数。 与迭代中的总点数或小时数相关的显示。 例如，“5 / 11”表示迭代中11个故事中有5个已被标记为[!UICONTROL 完成]。 此数字与[!UICONTROL 完成百分比]计算直接相关，并且会在更新[!UICONTROL 完成百分比]的同时更新。

  点数和小时数与故事关联。 当故事标记为[!UICONTROL 完成]时，与该故事关联的点数或小时数将标记为“完成”。

  缺省情况下，使用点。 您可以修改团队的设置来更改此设置，如[创建Agile团队](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md)中所述。

* 每天&#x200B;**[!UICONTROL 点/小时]：** （仅在迭代中可用）自迭代开始到当前日期期间每天标记为[!UICONTROL 完成]的平均点数或小时数。

  此值通过总完成点数或小时数除以当天的总天数来计算。 （部分天数会记录为全天。）

  此信息在规划未来迭代时可能很有用。

* **[!UICONTROL 预计完成时间]：**&#x200B;预计完成迭代的日期，基于每天点/小时数的当前比率（对于迭代）。

  当[!UICONTROL 预计完成]日期晚于为迭代定义的结束日期时，剩余的工作日数将在[!UICONTROL 预计完成]日期旁边的括号中显示为红色。

  当[!UICONTROL 预计完成]日期早于迭代的计划结束日期时，剩余工作天数以绿色显示。 (在计划迭代时指定迭代的结束日期，如[创建迭代](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)中所述；项目的结束日期为[!UICONTROL 计划完成日期]，如果[!UICONTROL 计划完成日期]是过去的日期，则为当前日期。 项目的计划完成日期[!UICONTROL 是根据项目中任务的持续时间计算的。) ]在计划迭代时，如果您为非工作日设置迭代结束日期，并且迭代正在跟踪按时完成，则预计完成日期将为您设置的迭代结束日期之前的最后一个工作日设置（因为不计划在非工作日烧掉工作）。

  例如，“（+9天）”表示预计完成日期比迭代的计划结束日期晚9个工作日。

  有关详细信息，请参阅[迭代完成状态概述](#Understanding-How-Days-Off-Affect-the-Burndown-Chart)。

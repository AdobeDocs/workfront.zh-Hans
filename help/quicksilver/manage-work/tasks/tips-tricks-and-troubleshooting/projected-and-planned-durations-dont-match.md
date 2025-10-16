---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-tasks
title: 预计持续时间与计划持续时间不匹配
description: 本文介绍了当您可能收到以下消息时，Adobe Workfront中的疑难解答：“任务/问题的预计持续时间已变为0，与计划持续时间不匹配。”
author: Alina
feature: Work Management
exl-id: ef135d44-3138-457d-b54a-3f1102ce3116
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# 预计持续时间与计划持续时间不匹配

## 问题

您会收到以下错误消息：“任务/问题的预计持续时间已变为0，与计划持续时间不匹配。”

## 原因

当预计开始日期与预计完成日期匹配时，会导致这种情况。

## 解决方案

有许多因素可导致预计起始日期和完成日期匹配。 这个问题在很大程度上与相关任务或问题的时间分配有关。

在大多数情况下，根据任务的工期类型和任务限制，分配应将预计完成日期延长得比预期更久。 但是，在某些情况下，根据持续时间类型和任务限制的配置方式，该值可能会为零。

以下是通过其支持文章的链接来检查这些案例的最佳方法：

* 预计完成日期：[项目、任务和问题的预计完成日期概览](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)
* 任务限制：[任务限制概述](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)
* 持续时间类型： [任务持续时间和持续时间类型概述](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)

如果“预计完成日期”、“任务限制”或“持续时间”类型按预期工作，请联系支持人员以进行更深入的故障诊断。

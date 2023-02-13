---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算计划人工成本
description: 在您计划项目上的工作时，Adobe Workfront会根据职责和分配给此工作的用户的每小时成本值来计算计划人工成本。
author: Alina
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 计算计划人工成本

在您计划项目上的工作时，Adobe Workfront会根据职责和分配给此工作的用户的每小时成本值来计算计划人工成本。

项目的计划人工成本是与任务职责相关的成本或分配用于完成项目工作的用户与每个角色或用户完成该工作的计划小时数（计划小时数）之间的计算。

## 计划人工成本概览

的 **计划人工成本** 通过添加项目上所有任务的所有计划人工成本来计算项目的所有计划人工成本。

>[!TIP]
>
>没有与问题或项目本身相关的计划人工成本。

Workfront使用以下公式计算项目的计划人工成本：

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

任务计划人工成本的计算依据如下：

* 任务上的资源数量及其对任务的单独分配
* 任务的成本类型。

任务计划人工成本使用以下公式计算：

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

有关Workfront如何根据任务分配和成本类型计算任务的计划人工成本的详细信息，请参阅文章中的“修改单个任务的成本类型”部分 [跟踪成本](../../../manage-work/projects/project-finances/track-costs.md).

## 查找计划人工成本

您可以在Workfront的以下区域找到项目的计划人工成本：

* 项目报表
* 项目列表
* 一个基线报表，您可以在其中跟踪一段时间内的流量
* 通过API

有关创建报表和使用Workfront API的信息，请参阅以下文章：

* [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [API 基础知识](../../../wf-api/general/api-basics.md)

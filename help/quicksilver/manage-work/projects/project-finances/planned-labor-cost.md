---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算计划劳力成本
description: 在计划项目工作时，Adobe Workfront会根据角色和用户的每小时成本值计算分配给此工作的角色和用户的计划劳力成本。
author: Lisa
feature: Work Management
exl-id: af053e9a-09dc-4b4d-8ed4-f681ed611a59
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# 计算计划劳力成本

在计划项目工作时，Adobe Workfront会根据角色和用户的每小时成本值计算分配给此工作的角色和用户的计划劳力成本。

项目的计划劳力成本是在与工作角色或分配用于完成项目工作的用户关联的成本与每个角色或用户完成该工作的计划小时数（计划小时数）之间的计算。

## 计划劳力成本概览

通过添加项目上所有任务的所有计划劳力成本来计算项目的&#x200B;**计划劳力成本**。

>[!TIP]
>
>没有与问题或项目本身相关的计划劳力成本。

Workfront使用以下公式计算项目的计划劳力成本：

```
Project Planned Labor Cost= SUM(Tasks Planned Labor Cost)
```

任务计划劳力成本按以下方式计算：

* 任务的资源数及其分配给任务的各个资源
* 任务的成本类型。

任务计划人工成本使用以下公式计算：

```
Task Planned Cost = Planned Hours x User or Job Role Cost Per Hour
```

有关Workfront如何根据任务分配和成本类型计算任务计划劳力成本的更多信息，请参阅[跟踪成本](../../../manage-work/projects/project-finances/track-costs.md)一文中的“修改单个任务的成本类型”一节。

## 查找计划劳力成本

您可以在Workfront的以下区域中找到项目的计划劳力成本：

* 项目报告
* 项目列表
* 您可以随时间跟踪它的基线报告
* 通过API

有关创建报告和使用Workfront API的信息，请参阅以下文章：

* [创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
* [API 基础知识](../../../wf-api/general/api-basics.md)

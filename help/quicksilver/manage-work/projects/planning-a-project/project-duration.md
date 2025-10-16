---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 项目持续时间概述
description: Adobe Workfront计算项目的持续时间时，会考虑最早任务的开始日期和最晚任务的完成日期，并计算两个日期之间的天数。
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# 项目持续时间概述

Adobe Workfront计算项目的持续时间时，会考虑最早任务的开始日期和最晚任务的完成日期，并计算两个日期之间的天数。

## 项目持续时间

项目持续时间按以下公式计算：

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>项目上问题的持续时间不会影响项目的持续时间。

项目持续时间根据与项目关联的计划或分配给任务的用户的计划计算两个任务日期之间的天数。 有关Workfront使用哪个计划来计算持续时间的信息，请参阅[计划概述](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md)。

## 项目持续时间类型

有两种类型的项目持续时间以及Workfront计算项目持续时间的公式：

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **计划持续时间**： 

  ```
  Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
  ```

* **实际持续时间**： 

  ```
  Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
  ```

## 找到项目持续时间

您可以在Workfront的以下区域中找到项目计划和实际持续时间：

* 。在项目详细信息区域的概述部分。

  有关项目的概述子选项卡的详细信息，请参阅文章[在项目概述区域管理信息](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)。

* 在项目报告中，通过包含报告中的持续时间或实际持续时间字段。

  有关创建报告的详细信息，请参阅文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

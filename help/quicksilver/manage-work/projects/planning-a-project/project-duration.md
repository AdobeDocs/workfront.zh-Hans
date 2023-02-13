---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: 项目持续时间概述
description: Adobe Workfront通过考虑最早任务的开始日期和最新任务的完成日期来计算项目的持续时间，并计算两个日期之间的天数。
author: Alina
feature: Work Management
exl-id: b558eaad-669b-4079-b61a-07df227edfa2
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 2%

---

# 项目持续时间概述

Adobe Workfront通过考虑最早任务的开始日期和最新任务的完成日期来计算项目的持续时间，并计算两个日期之间的天数。

## 项目持续时间

项目持续时间通过以下公式计算：

```
Project Duration = Completion Date of the latest task - Start Date of the earliest task
```

>[!NOTE]
>
>项目问题的持续时间不会影响项目的持续时间。

项目持续时间根据与项目关联的计划或分配给任务的用户计算两个任务日期之间的天数。 有关Workfront用于计算持续时间的计划的信息，请参阅 [计划概述](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md).

## 项目持续时间的类型

项目持续时间有两种类型，而Workfront通过这两种类型的公式来计算：

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Check these formulas? Should they be divided by the hours per day?!) </p>
-->

* **计划持续时间**: 

   ```
   Project Planned Duration = Planned Completion Date of the latest task - Planned Start Date of the earliest task / Typical hour per day
   ```

* **实际持续时间**: 

   ```
   Project Actual Duration = Actual Completion Date of the latest task - Actual Start Date of the earliest task / Typical hour per day
   ```

## 找到项目持续时间

您可以在Workfront的以下区域找到项目计划持续时间和实际持续时间：

* . 在项目详细信息区域的概述部分。

   有关项目的“概述”子选项卡的更多信息，请参阅文章 [在项目概述区域中管理信息](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* 在项目报表中，通过在报表中包含持续时间或实际持续时间字段。

   有关创建报告的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

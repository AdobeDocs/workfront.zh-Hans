---
product-area: reports and dashboards
navigation-topic: data-connect
title: 在Data Connect中使用“作业历史记录”视图
description: 借助Data Connect，Workfront管理员可以在“作业历史记录”视图中访问每个数据刷新作业的详细记录。
author: Jenny
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
source-git-commit: 05cf34fe6659c50da76d2478c6e79352346dc9a5
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# 在Data Connect中使用“作业历史记录”视图

在“作业历史记录”视图中，Workfront管理员可以访问每个数据刷新作业的详细记录。 这些记录为让您的数据保持最新的作业提供了宝贵的insight，并帮助您确定理想的时间范围（确定何时执行流程和刷新业务可视化图表）。

![作业历史记录视图](assets/job-history-overview.png)

“作业历史记录”视图列包含以下信息：

* **OBJECT_NAME**：显示与作业关联的对象的名称。
* **SCHEDULED_TIME**：显示作业的开始时间。
* **COMPLETED_TIME**：显示作业的完成时间。
* **LATEST_FLAG**：指示作业是否为最近刷新的一部分。
* **状态**：显示作业状态。 有关详细信息，请参阅本文中的以下部分：[可用作业状态](#available-job-statuses)。
* **上次更新时间**：作业的上次更新时间戳。

>[!NOTE]
>
>“作业历史记录”视图包含过去72小时计划作业的详细信息。


## 可用作业状态

每个Data Connect作业都会分配一个状态，指示其是成功、跳过还是失败。

<table>
    <tr>
        <td><b>作业状态</b></td>
        <td><b>定义</b></td>
    </tr>
    <tr>
        <td>已成功</td>
        <td>作业已成功处理每个可用更新，并且该记录类型的所有更新现在都反映在数据湖中。</td>
    </tr>
    <tr>
        <td>已跳过</td>
        <td>已跳过该作业，因为队列中没有要处理的记录类型更新。</td>
    </tr>
    <tr>
        <td>失败</td>
        <td>作业无法执行。 在这些情况下，队列中可能没有任何数据被提交到数据湖。 保留在队列中的记录将在针对该记录类型的下一个计划作业中进行处理。 </td>
    </tr>
   </table>


## 有关作业执行和日志记录行为的注意事项

Snowflake使用作业计划程序优化工具，该工具可能会影响如何处理作业执行并将其记录在“作业历史记录”视图中。 此日志记录行为会因是否有要处理的数据而有所不同。

例如，当给定对象没有任何要处理的新行时，可能会出现以下结果之一：

* **作业执行并标记为“已跳过”**： Snowflake检测到没有要处理的行，执行作业并在表中将其记录为“已跳过”状态。

* **作业未执行**： Snowflake确定没有要处理的行，不执行作业，并在表中将其记录为“已跳过”状态。

  >[!NOTE]
  >
  >在作业未执行的第二种方案中，该对象的最新记录可能反映与预期计划不符的时间戳。

换言之，即使未处理任何行，作业也可以被视为已执行，并且根据作业调度程序对该特定作业的行为，可能会记录也可能不记录该作业。
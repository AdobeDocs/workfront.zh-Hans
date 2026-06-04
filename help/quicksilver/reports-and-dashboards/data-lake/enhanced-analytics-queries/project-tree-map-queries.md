---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 项目树状图查询
description: 增强的Analytics查询
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 3943703a-0d0b-46d3-a708-52987d330523
TQID: https://experienceleague.adobe.com/tukTMDDsdNPEaS5mPafVJ0ajIVQFQ7sLs9xBQ04uQ2w
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 110
ht-degree: 0%

---

# 项目树状图查询

您可以使用本文中的查询来创建类似于增强型分析中的数据可视化图表。

>[!IMPORTANT]
>
>查询将产生与增强型分析中所示类似的结果，但它们可能不完全匹配。


## 先决条件

在开始之前，您必须

1. 与Business Intelligence (BI)工具建立连接：
   1. [为Snowflake创建Reader帐户或连接](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [建立与Workfront数据连接的连接](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

建立连接后，您可以使用本文中的查询来提取和可视化数据。

## 已弃用项目计划小时数

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### 已弃用项目计划小时数：燃尽

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        workrequired, 
        percentcomplete, 
        calendardate, 
        (workrequired - (workrequired * percentcomplete)) as remainingMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.workrequired) as projectTotalWork, 
    sum(tdw.remainingMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

## 已弃用项目计划持续时间 

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

### 项目计划持续时间已停用：燃尽

```
WITH task_daily_work as ( 
    SELECT 
        taskid, 
        projectid, 
        planneddurationminutes, 
        percentcomplete, 
        calendardate, 
        (planneddurationminutes - (planneddurationminutes * percentcomplete)) as remainingDurationMinutes 
    FROM tasks_daily_history 
) 
 
SELECT 
    p.name, 
    p.projectid, 
    sum(tdw.planneddurationminutes) as projectTotalWork, 
    sum(tdw.remainingDurationMinutes) as projectRemainingWork, 
    tdw.calendardate 
FROM projects_current p 
    JOIN task_daily_work tdw ON p.projectid = tdw.projectid 
GROUP BY p.projectid, p.name, tdw.calendardate
```

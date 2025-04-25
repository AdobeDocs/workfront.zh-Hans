---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 项目活动查询
description: 增强的Analytics查询
author: Courtney
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: b7155160-4537-4919-bebf-72056b181bb6
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# 项目活动查询

您可以使用本文中的查询来创建类似于增强型分析中的数据可视化图表。

>[!IMPORTANT]
>
>查询将产生与增强型分析中所示类似的结果，但它们可能不完全匹配。


## 先决条件

在开始之前，您必须

1. 与Business Intelligence (BI)工具建立连接：
   1. [为Snowflake创建Reader帐户或连接](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)
   1. [建立与Workfront数据连接的连接](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)

建立连接后，即可使用本文档中的查询提取和可视化数据。

## 项目用户的登录事件

显示分配给项目、在给定日期登录的人员数量。

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 
 
SELECT 
    tds.projectid, 
    ads.calendardate, 
    count(1) 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN userlogins ul ON ads.assignedtoid = ul.userid and TO_DATE(ul.lastlogindate) = ads.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### Projects用户的登录事件：深入分析

```
WITH userlogins as ( 
    SELECT 
        userid, 
        lastlogindate 
    FROM ( 
        SELECT 
            userid, 
            lastlogindate, 
            lag(lastlogindate, 1, '1990-01-01') OVER (PARTITION BY userid ORDER BY begin_effective_timestamp) as previous_login 
        FROM users_event 
    ) 
    WHERE lastlogindate != previous_login 
) 

SELECT 
    tds.projectid, 
    ul.userid, 
    ads.calendardate, 
    count(1) 
FROM assignments_daily_history ads 
INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
INNER JOIN userlogins ul ON ads.assignedtoid = ul.userid AND TO_DATE(ul.lastlogindate) = ads.calendardate 
group by tds.projectid, ul.userid, ads.calendardate
 
```

## 项目用户的任务状态更改事件

显示在给定日期更改项目任务状态的人员数。

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status 
        FROM tasks_event 
        WHERE status != 'CPL' 
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    count(tds.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid and TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### 项目用户的任务状态更改事件：深入分析

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        lastupdatedbyid, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lastupdatedbyid, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status != 'CPL'  
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    tsc.lastupdatedbyid, 
    count(tsc.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid AND TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, tsc.lastupdatedbyid, ads.calendardate
```

## 项目用户的任务完成事件

显示在给定日期完成项目任务的人员数。

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status = 'CPL'  
    )  
    WHERE status != previous_status  
) 
 
SELECT 
    tds.projectid, 
    count(tds.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid and tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid and tsc.taskid = tds.taskid and TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, ads.calendardate
```

### 项目用户的任务完成事件：深入分析

```
WITH task_status_changes as (  
    SELECT 
        taskid, 
        status, 
        lastupdatedbyid, 
        begin_effective_timestamp  
    FROM (  
        SELECT 
            taskid, 
            status, 
            begin_effective_timestamp, 
            lastupdatedbyid, 
            lag(status, 1, 'NOSTATUS') OVER (PARTITION BY taskid ORDER BY begin_effective_timestamp) as previous_status  
        FROM tasks_event  
        WHERE status = 'CPL'  
    )  
    WHERE status != previous_status  
)  
 
SELECT 
    tds.projectid, 
    tsc.lastupdatedbyid, 
    count(tsc.status), 
    ads.calendardate 
FROM assignments_daily_history ads 
    INNER JOIN tasks_daily_history tds ON ads.taskid = tds.taskid AND tds.calendardate = ads.calendardate 
    INNER JOIN task_status_changes tsc ON tsc.taskid = ads.taskid AND tsc.taskid = tds.taskid AND TO_DATE(tsc.begin_effective_timestamp) = tds.calendardate 
GROUP BY tds.projectid, tsc.lastupdatedbyid, ads.calendardate
```

---
content-type: api
navigation-topic: wf-api
title: 获取用户可用时间API
description: 获取用户可用时间API
author: Becky
feature: Workfront API
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 7%

---

# 用户可用时间API

**URI:attask/api/v15.0/user/getUsersAvailableTime**

用户可用时间端点会检索有关用户可用时间的数据。 这允许根据用户属性和时间间隔进行数据聚合的集成。

## 示例请求

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## 请求参数

* **userIDs**:字符串数组。 必填. 示例: `"61a9cc0500002f9fdaa7a6f824f557e1"`.

* **fromDate**:datetime。 字符串。 必填. 示例:  `"2022-07-10T00:00:00"`.

* **toDate**:datetime。 字符串。 必填. 示例 `"2022-07-20T23:59:59"`.

## 示例响应：

```
{
    "data": {
        "result": {
            "PAVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            },
            "AVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    480.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            }
        }
    }
}
```

## 响应参数

* **AVL**:实际可用小时数。 数组。
* **巴甫勒**:用于计划的纯可用小时数，其中不包括非工作日或用户休息时间。 字符串.

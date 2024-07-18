---
content-type: api
navigation-topic: wf-api
title: 获取用户可用时间API
description: 获取用户可用时间API
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '94'
ht-degree: 0%

---

# 用户可用时间API

**URI： attask/api/v15.0/user/getUsersAvailableTime**

用户可用时间端点检索有关用户可用时间的数据。 这允许根据用户属性和时间间隔集成数据。

## 示例请求

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## 请求参数

* **userIDs**：字符串数组。 必需。 示例： `"61a9cc0500002f9fdaa7a6f824f557e1"`。

* **fromDate**： datetime。 字符串。 必需。 示例： `"2022-07-10T00:00:00"`。

* **toDate**： datetime。 字符串。 必需。 示例`"2022-07-20T23:59:59"`。

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

* **AVL**：实际可用小时数。 数字数组。
* **PAVL**：用于计划的纯可用小时数，不包含非工作日或用户休息时间。 字符串。

---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 当货币为null时，检索项目的货币信息
description: 当货币为null时，检索项目的货币信息
author: Becky
feature: Workfront API
source-git-commit: a9af457793e123a60172fe4baf5ae5def472b026
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# 当货币为null（未分配）时，检索项目的货币信息

可使用以下请求检索具有货币字段的项目对象：

```
GET /attask/api-internal/project/{{projectID}}?fields=currency
```

这将返回以下响应正文：

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": "EUR"
}
}
}
```

如果未为项目设置货币，则此响应将包含值为的货币 `null`:

```
{
{
"data": {
"ID": "some_project_id",
"name": "some_project_name",
"objCode": "PROJ",
"currency": null
}
}
}
```

如果需要项目使用货币（例如计算），则可以检索客户的默认货币：

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

响应包括用户设置为默认的货币，该货币将用于未设置该货币的客户的任何项目：

```
{
"data": [
{
"ID": "some_customer_id,
"name": "some_customer_name",
"objCode": "CUST",
"currency": "USD"
}
]
}
```

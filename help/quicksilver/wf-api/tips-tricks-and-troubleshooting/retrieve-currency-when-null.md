---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 在货币为null时检索项目的货币信息
description: 在货币为null时检索项目的货币信息
author: Becky
feature: Workfront API
role: Developer
exl-id: 31ed533b-be19-4ccb-aad4-7c78e008b3e9
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---

# 在货币为null（未分配）时检索项目的货币信息

使用以下请求可检索包含货币字段的项目对象：

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

如果未为项目设置货币，则此响应将包含值为`null`的货币：

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

如果您需要项目的币种（如用于计算的币种），则可以检索客户的默认币种：

`GET /attask/api-internal/CUST/currentCustomer?fields=currency`

此响应包括用户设置为默认值的货币，没有该货币设置的任何项目都将使用此货币：

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

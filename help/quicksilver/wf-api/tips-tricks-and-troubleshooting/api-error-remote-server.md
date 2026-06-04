---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API错误消息400错误请求
description: API错误消息400错误请求
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
TQID: https://experienceleague.adobe.com/19PIdv4u8de0BlasXD0Yy6GssO3vv6Jt8BzcljB-m1w
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 93
ht-degree: 2%

---

# API错误：“远程服务器返回错误(400)错误请求”

## 问题

尝试使用API将自定义字段导入问题时，出现以下错误：

`The remote server returned an error: (400) Bad Request`

## 原因

当您尝试通过API导入项目中的自定义字段时，出现此错误，该项目没有与队列主题关联的自定义表单。

## 解决方案

将正确的自定义表单添加到队列主题。

要了解有关队列主题的更多信息，请参阅[创建队列主题](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

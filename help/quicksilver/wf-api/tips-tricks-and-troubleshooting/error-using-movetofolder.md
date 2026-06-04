---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 文档moveToFolder操作无效
description: 使用Document moveToFolder操作时，返回422错误。
author: Becky
feature: Workfront API
role: Developer
exl-id: 811efabc-e101-4de5-a800-a1447654dc3e
TQID: https://experienceleague.adobe.com/UV4VnQEs-jGJau1UqXTLnp7Ak-cmKRpjuJqxgNTF5z8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 121
ht-degree: 1%

---

# 文档moveToFolder操作无效

## 问题

使用文档对象的`moveToFolder`操作时，返回422错误。

或

如果通过Workfront Fusion中的Adobe Authenticator模块使用此操作，则不会移动文档，但不会指示出现错误。 错误相同，但Adobe Authenticator模块不显示该错误。

## 解决方案

此操作出现422错误的一个可能原因是该操作正在尝试将一个链接文件夹中的文档移动到另一个链接文件夹中。

选中以确保要移动的文档不在链接文件夹中。

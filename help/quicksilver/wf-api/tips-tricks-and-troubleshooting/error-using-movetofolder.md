---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 文档moveToFolder操作无效
description: 使用Document moveToFolder操作时，返回422错误。
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 86c0517443537ec5af640036c290b3a495825fdc
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---


# 文档moveToFolder操作无效

## 问题

使用Document对象的 `moveToFolder` 操作，将返回422错误。

或

如果通过Workfront Fusion中的Adobe Authenticator模块使用此操作，则不会移动文档，但不会指示出现错误。 错误相同，但Adobe Authenticator模块不显示该错误。

## 解决方案

此操作出现422错误的一个可能原因是该操作正在尝试将一个链接文件夹中的文档移动到另一个链接文件夹中。

选中以确保要移动的文档不在链接文件夹中。

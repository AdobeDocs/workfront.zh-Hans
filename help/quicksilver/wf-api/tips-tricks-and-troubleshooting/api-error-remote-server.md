---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API错误消息400错误请求
description: API错误消息400错误请求
author: Becky
feature: Workfront API
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# API错误：&quot;远程服务器返回错误(400)错误请求&quot;

## 问题

尝试使用API将自定义字段导入问题时出现以下错误：

`The remote server returned an error: (400) Bad Request`

## 原因

当您尝试通过API从没有与队列主题关联的自定义表单的项目导入自定义字段时，会发生此错误。

## 解决方案

将正确的自定义表单添加到队列主题。

要了解有关队列主题的更多信息，请参阅 [创建队列主题](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

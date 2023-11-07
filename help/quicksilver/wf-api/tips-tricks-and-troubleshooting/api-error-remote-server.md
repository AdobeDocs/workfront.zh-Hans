---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API错误消息400错误请求
description: API错误消息400错误请求
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '90'
ht-degree: 0%

---


# API错误：“远程服务器返回错误(400)错误请求”

## 问题

尝试使用API将自定义字段导入问题时，出现以下错误：

`The remote server returned an error: (400) Bad Request`

## 原因

当您尝试通过API导入项目中的自定义字段时，出现此错误，该项目没有与队列主题关联的自定义表单。

## 解决方案

将正确的自定义表单添加到队列主题。

要了解有关队列主题的更多信息，请参阅 [创建队列主题](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

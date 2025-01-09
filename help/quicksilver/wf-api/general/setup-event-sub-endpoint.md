---
content-type: api
navigation-topic: general-api
title: 事件订阅提交要求
description: 事件订阅提交要求
author: Becky
feature: Workfront API
role: Developer
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: 77c07c7c7104d37360cc7630a89dd72836da477c
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---


# 事件订阅提交要求

事件订阅消息是可设置为在发生某些事件时通知用户的通知。 若要了解有关什么是事件订阅的详细信息，请参阅[常见问题解答 — 事件订阅](../../wf-api/general/event-subs-faq.md)。

## 事件订阅报文交付标准

使用Adobe Workfront事件订阅消息的服务端点必须满足以下基本要求，以确保正确发送和接收消息：

* 服务终结点必须接受HTTPPOST请求。 HTTPPOST是在所有事件订阅消息（包括验证消息）投放中使用的请求方法。

* 为了让事件订阅投放系统确认消息已成功接收，端点必须返回所有传入消息的200级HTTP状态（例如，200 OK或202）。

* 如果未返回200级状态，则事件订阅系统会假定消息未成功传递，并开始应用相应的重试策略。 要了解有关Workfront重试策略的更多信息，请参阅[事件订阅重试](../../wf-api/api/event-sub-retries.md)。

* 在将200级状态作为响应状态返回的同时，必须在投放尝试开始后的五秒内收到HTTP响应。此约束确保消费者业务流程或基础架构限制不会延迟其他待投放消息的投放。

* 如果从事件订阅消息触发长时间运行的业务流程，Workfront建议  该

   1. 端点在收到消息时保存消息信息，并立即以200级状态响应。
   1. 在端点响应事件订阅投放请求后，即可处理保存的消息。

* 事件订阅消息或对象不能大于1 MB。
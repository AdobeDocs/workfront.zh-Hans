---
content-type: api
navigation-topic: general-api
title: 事件订阅提交要求
description: 事件订阅提交要求
author: Becky
feature: Workfront API
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# 事件订阅提交要求

事件订阅消息是可设置为在发生某些事件时通知用户的通知。 要详细了解事件订阅，请参阅 [常见问题解答 — 事件订阅](../../wf-api/general/event-subs-faq.md).

## 事件订阅消息投放标准

使用Adobe Workfront事件订阅消息的服务端点必须满足以下基本要求，才能确保正确发送和接收消息：

* 服务端点必须接受HTTPPOST请求。 HTTPPOST是用于事件订阅消息（包括验证消息）所有投放的请求方法。

* 为了事件订阅投放系统确认消息已成功接收，端点必须为所有传入消息返回200级HTTP状态（例如，200 OK或202）。

* 如果未返回200级状态，则事件订阅系统会假定消息未成功发送，并开始应用相应的重试策略。 要了解有关Workfront重试策略的更多信息，请参阅 [事件订阅重试](../../wf-api/api/event-sub-retries.md).

* 在返回200级状态作为响应状态的同时，必须在投放尝试开始后的5秒内接收HTTP响应。此约束可确保消费者业务流程或基础架构限制不会延迟其他消息的投放，以等待投放。

* 如果长时间运行的业务流程从事件订阅消息触发，Workfront建议

   1. 端点在收到消息时保存消息信息，并立即以200级状态进行响应。
   1. 端点响应事件订阅投放请求后，可以处理保存的消息。

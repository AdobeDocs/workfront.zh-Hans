---
content-type: api
navigation-topic: api-navigation-topic
title: 事件订阅重试
description: 事件订阅重试
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# 事件订阅重试

在实施消息投放系统时，必须解决一些注意事项，以确保稳定性、一致性和良好的用户体验。 消息投放系统的缺点之一是确保消息成功到达目的地，并了解消息未到达时应该怎么做。

某些集成可以接受投放失败，然后丢弃消息并转到下一个消息。  在其他集成中，无法忽略无法投放消息的情况。 例如，金融集成可能尝试传递消息，但接收的HTTP状态代码为404，这表示服务器找不到要向其传递消息的端点。 在这种情况下，缺少消息可能意味着某人没有获得时间报酬，或者组织超过合同资源的预算。

## Adobe Workfront的事件订阅重试策略

由于客户将Workfront平台用作其日常知识工作的核心部分，因此Workfront事件订阅框架提供了一种机制，可确保尽可能全面地尝试投放每条消息。

无法投放到客户端点的事件触发出站消息会重新发送，直到投放成功持续长达48小时。 在此期间，重试的频率会递增直至投放成功或进行11次尝试。

这些重试尝试的公式为：

`((2^attempt) - 1) * 84800ms`

第一次重试在1.5分钟后进行，第二次重试在大约5分钟后进行，第11次重试在大约48小时后进行。

客户需要确保将任何使用来自Workfront事件订阅的出站消息的端点设置为在投放成功时返回Workfront的200级响应消息。

## 已禁用和冻结的订阅规则

* 如果订阅URL的失败率超过70%且尝试次数超过100，或者如果连续失败2,000，则订阅URL为&#x200B;**已禁用**
* 如果订阅URL连续失败超过2,000次，并且上次成功是在72小时之前，或者在任何时间范围内连续失败超过50,000次，则订阅URL为&#x200B;**冻结**。
* **已禁用**&#x200B;订阅URL将继续每10分钟尝试一次传递，并在成功传递后重新启用。
* **冻结**&#x200B;订阅URL将永远不会尝试投放，除非通过发出API请求手动启用它。




<!--

## Handling Failed Event-Triggered Outbound Messages

The following flowchart shows the strategy for reattempting message deliveries with Workfront Event Subscriptions:

![Event sub retries](assets/event-subscription-circuit-breaker-retries-350x234.png)

The following explanations correspond with the steps depicted in the flowchart:

1. Message fails to be delivered. 
1. Message delivery failure information is logged.

   All failed attempts to deliver a message are logged so that debugging may be performed to determine the root cause of a given failure or series of failures. 

1. URL failures incremented. 
1. Message attempt count is incremented. 
1. Calculate the delay until this message's delivery will be attempted again. 
1. Message is placed onto the message retry queue.

   As shown in the preceding flowchart, the message queue used for processing message delivery retries is a separate queue from the one that processes the initial delivery attempt for each message. This allows the near real-time flow of messages to continue unimpeded by the failure of any subset of messages. 

1. URL circuit status is evaluated. One of the following occurs:

   * If the circuit is open and not allowing deliveries at this time, restart the process at step 5.
   * If the circuit is half-open, this implies that our circuit is currently open, but enough time has passed to allow testing of the URL to see if the problem with delivering to it has been resolved.
   * If the message delivery attempt limits have been reached (48 hours of retrying) then the message is dropped

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1 

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1.
   -->

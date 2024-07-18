---
content-type: api
navigation-topic: api-navigation-topic
title: 事件订阅重试
description: 事件订阅重试
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# 事件订阅重试

在实施消息投放系统时，必须解决一些注意事项，以确保稳定性、一致性和良好的用户体验。 消息投放系统的缺点之一是确保消息成功到达目的地，并了解消息未到达时应该怎么做。

某些集成可以接受投放失败，然后丢弃消息并转到下一个消息。  在其他集成中，无法忽略无法投放消息的情况。 例如，金融集成可能尝试传递消息，但接收的HTTP状态代码为404，这表示服务器找不到要向其传递消息的端点。 在这种情况下，缺少消息可能意味着某人没有获得时间报酬，或者组织超过合同资源的预算。

## Adobe Workfront的事件订阅重试策略

由于客户将Workfront平台用作其日常知识工作的核心部分，因此Workfront事件订阅框架提供了一种机制，可确保尽可能全面地尝试投放每条消息。

无法投放到客户端点的事件触发出站消息会重新发送，直到投放成功持续长达48小时。 在此期间，重试次数会递减直至投放成功或经过48小时。

客户需要确保将任何使用来自Workfront事件订阅的出站消息的端点设置为在投放成功时返回Workfront的200级响应消息。

## 处理失败的事件触发出站消息

以下流程图显示了使用Workfront事件订阅重新尝试消息投放的策略：

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

以下说明与流程图中描述的步骤相对应：

1. 消息无法投放。
1. 将记录消息投放失败信息。

   所有尝试传递消息的失败都将被记录，以便执行调试以确定给定失败或一系列失败的根本原因。

1. URL失败次数会增加。
1. 消息尝试计数会增加。
1. 计算再次尝试投放此消息之前的延迟。
1. 消息将置于消息重试队列中。

   如前面的流程图所示，用于处理消息投放重试的消息队列与处理每个消息的初始投放尝试的消息队列是一个单独的队列。 这样，几乎实时的消息流就可以不受任何消息子集失败的阻碍。

1. 评估URL电路状态。 出现以下情况之一：

   * 如果电路已打开且此时不允许投放，请在步骤5中重新启动该过程。
   * 如果电路是半开的，这意味着我们的电路当前是开的，但已经过了足够的时间来允许测试URL，以查看向它交付内容的问题是否已解决。
   * 如果已达到消息投放尝试限制（重试时间为48小时），则将丢弃消息

1. 如果URL回路关闭并允许投放，则尝试投放消息。 如果此投放失败，则消息将在步骤1重新启动

1. 如果URL回路关闭并允许投放，则尝试投放消息。 如果此投放失败，则消息将在步骤1重新启动。

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront disables Event Subscriptions when both of the following criteria are met:
   <ul>
   <!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Event Subscription has failed 1000 delivery attempts consecutively</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">48 hours have passed since the last successful delivery</li>
   </ul></li>
   -->

---
content-type: api
navigation-topic: api-navigation-topic
title: 事件订阅重试
description: 事件订阅重试
author: John
feature: Workfront API
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# 事件订阅重试

在实施消息投放系统时，必须注意一些注意事项，以确保稳定性、一致性和良好的用户体验。 消息投放系统的一个缺点是确保消息成功到达其目的地，并知道当消息未到达时应该怎么做。

某些集成可以接受投放失败，然后删除消息并移至下一条消息。  在其他集成中，无法传递消息的问题不容忽视。 例如，金融集成可能会尝试发送消息，但却收到HTTP状态代码为404，这表示服务器找不到要将消息发送到的端点。 在这种情况下，信息缺失可能意味着某人没有按期领取报酬，或某组织在合同资源上超出预算。

## Adobe Workfront重试事件订阅策略

由于客户将Workfront平台作为其日常知识工作的核心内容，因此Workfront事件订阅框架提供了一种机制，可确保尽可能地尝试交付每条消息。

在48小时内成功交付之前，会重新发送未能发送到客户端点的事件触发的出站消息。 在此期间，重试将以递送成功或48小时之前的递增减少频率进行。

客户需要确保将使用Workfront事件订阅中出站消息的任何端点设置为，以在成功交付时将200级响应消息返回Workfront。

## 处理失败的事件触发的出站消息

以下流程图显示了重新尝试通过Workfront事件订阅发送消息的策略：

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

以下说明与流程图中描述的步骤相对应：

1. 消息传送失败。
1. 消息投放失败信息已记录。

   所有传递消息的失败尝试均被记录，以便执行调试以确定给定失败或一系列失败的根本原因。

1. URL失败次数增加。
1. 消息尝试计数增加。
1. 计算延迟，直到再次尝试发送此消息为止。
1. 消息被置于消息重试队列中。

   如上一流程图所示，用于处理消息投放重试的消息队列是一个与处理每个消息的初始投放尝试的队列不同的队列。 这允许消息的近乎实时的流继续不受任何消息子集故障的阻碍。

1. 评估URL电路状态。 出现以下情况之一：

   * 如果此时电路已打开且不允许投放，请在步骤5中重新启动该进程。
   * 如果电路半开，则意味着我们的电路当前处于打开状态，但已经过了足够的时间来测试URL，以查看传送到它的问题是否已解决。
   * 如果达到消息投放尝试限制（重试48小时），则将丢弃消息

1. 如果URL电路已关闭并允许投放，请尝试投放消息。 如果此投放失败，消息将在步骤1重新启动

1. 如果URL电路已关闭并允许投放，请尝试投放消息。 如果此投放失败，消息将在步骤1重新启动。

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront disables Event Subscriptions when both of the following criteria are met:
   <ul>
   <!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Event Subscription has failed 1000 delivery attempts consecutively</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">48 hours have passed since the last successful delivery</li>
   </ul></li>
   -->

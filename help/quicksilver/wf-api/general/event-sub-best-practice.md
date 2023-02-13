---
content-type: api
navigation-topic: general-api
title: 事件订阅最佳实践
description: 事件订阅最佳实践
author: John
feature: Workfront API
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 50675b7af3fcd2188a18391732a93a7b67454db9
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# 事件订阅最佳实践

Adobe Workfront事件订阅消息在您正确配置服务并创建事件订阅以触发这些消息投放后，会自动从Workfront发送。 要了解有关正确设置事件订阅的更多信息，请参阅 [事件订阅提交要求](../../wf-api/general/setup-event-sub-endpoint.md).


下面列出了一些可帮助您有效创建事件订阅的最佳实践。

## 提供所有必需的请求正文字段

确保向API提供所有必需的请求正文字段。 有关所有必需的请求属性的信息，请参阅 [事件订阅API](../../wf-api/general/event-subs-api.md).

## 避免包含额外的正文字段

请求中不要包含额外的正文字段，因为这将导致API无法创建订阅。

## 在宽限期内完成测试

尝试在100条消息的宽限期内完成所有订阅测试。 要了解有关此宽限期的更多信息，请参阅 [常见问题解答 — 事件订阅](../../wf-api/general/event-subs-faq.md).

## 满足标准事件订阅消息投放要求

确保您的订阅端点符合标准事件订阅消息传递要求。 要了解这些要求，请参阅 [事件订阅提交要求](../../wf-api/general/setup-event-sub-endpoint.md).

## 按全允许列表局区域IP地址

要通过防火墙接收事件订阅负载，您必须按全局区域将IP地址添允许列表加到中。 要了解更多信息，请参阅 [事件订阅API](../../wf-api/general/event-subs-api.md).

## 具有正确的访问级别和API密钥

要创建、查询或删除事件订阅，您的Workfront用户需要：

* 访问级别 **系统管理员**
要了解更多信息，请参阅 [授予用户完全管理访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) 或 [授予用户对特定区域的管理访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* API密钥

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->

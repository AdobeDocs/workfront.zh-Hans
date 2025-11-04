---
content-type: api
navigation-topic: general-api
title: 事件订阅最佳实践
description: 事件订阅最佳实践
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 3a538a15daad5fa0dced8d45bb260d6087be81ff
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# 事件订阅最佳实践

正确配置服务并创建事件订阅以触发这些消息投放后，Adobe Workfront事件订阅消息将自动从Workfront发送。 要了解有关正确设置事件订阅的更多信息，请参阅[事件订阅交付要求](../../wf-api/general/setup-event-sub-endpoint.md)。


下面列出了一些最佳实践，可帮助您有效创建活动订阅。

## 提供所有必需的请求正文字段

确保所有必需的请求正文字段均已提供给API。 有关所有必需请求属性的信息，请参阅[事件订阅API](../../wf-api/general/event-subs-api.md)。

## 避免包含额外的正文字段

请勿在请求中包含额外的正文字段，因为这将导致API创建订阅失败。

## 避免使事件订阅过载

事件订阅服务旨在为所有用户提供可靠的事件交付。 为确保这一点，已实施保护措施以防止单个用户产生过多事件，这可能会对所有用户造成潜在服务质量问题。 因此，在短时间内以高速率生成过多事件的用户可能会遇到沙箱处理和事件投放延迟的情况。

## 在宽限期内完成测试

尝试在100条报文的宽限期内完成所有订阅测试。 若要了解有关此宽限期的更多信息，请参阅[常见问题解答 — 活动订阅](../../wf-api/general/event-subs-faq.md)。

## 满足标准事件订阅消息投放要求

确保您的订阅端点符合标准事件订阅消息投放要求。 若要了解这些要求，请参阅[事件订阅提交要求](../../wf-api/general/setup-event-sub-endpoint.md)。

## 按全球地区允许列表IP地址

列入允许列表要通过防火墙接收事件订阅负载，必须将IP地址添加到按全局区域进行的IP地址。 若要了解详细信息，请参阅[事件订阅API](../../wf-api/general/event-subs-api.md)。

## 拥有正确的访问级别和身份验证

要创建、查询或删除事件订阅，您的Workfront用户需要：

* **系统管理员**的访问级别
要了解更多信息，请参阅[授予用户完全管理访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)或[授予用户对特定区域的管理访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

* 如果您的组织使用Adobe IMS (Identity Management System)，请包含在`X-User-Token`标头中传递的IMS用户令牌。

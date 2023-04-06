---
content-type: api
navigation-topic: api-navigation-topic
title: 更新使用默认API版本控制的集成
description: 更新使用默认API版本控制的集成
author: Becky
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 2b9eacc9b2c8f499cdd1794a55879a56224051c8
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# 更新使用默认API版本控制的集成

我们每两年发布一次Adobe Workfront API的新版本。 每个版本在发布后三年内都受支持，在已弃用状态下再受一年支持，即版本可用但不受支持。

在URI中未指定API版本的集成将自动路由到默认。 如果您希望API调用使用特定版本的API，则必须在Workfront API请求中指定该版本。

>[!NOTE]
>
>如果贵组织当前使用默认API，则Workfront管理员已收到公告中心消息，其中包含有关默认API的进一步说明。

要了解有关在API请求中指定版本的信息，请参阅 [在集成中指定API版本](../../wf-api/api/specify-api-version-integrations.md).

## 使用默认API时的注意事项

使用Workfront默认API时，请考虑以下事项：

* API的默认版本为最新版本。 任何未指定版本的API调用都将使用默认版本。 每次Workfront发布新版API时，默认版本都将更新至最新版本。 **因此，在发布新版Workfront API后，应检查使用默认版本的任何API调用，以确保仍支持该功能**.
* 如果贵组织当前使用的是以前已弃用的默认API，则Workfront管理员已收到公告中心消息，其中包含有关默认API的进一步说明。

要查看API的最新版本，请参阅 [API版本控制和支持计划](../../wf-api/api/api-version-support-schedule.md).

## 将集成更新到支持的API版本

如果您的Workfront API请求未指定版本，则它们使用默认版本。 我们建议您的API请求指定受支持的API版本，最好是最新受支持的API版本。

例如，以下Workfront API请求未指定API版本：

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

发出此请求后，您将收到一个响应，其中包含JSON编码文本，用于指定来自Workfront实例的数据。 由于此URI中未指定API版本，因此调用将转为默认。

要将默认API请求转换为版本控制的API请求，只需调用支持的API版本。 例如，以下URI请求版本15:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

在更新Workfront API请求时，您可以指定我们API的任何受支持版本。 要了解有关引用特定API的更多信息，请参阅 [在集成中指定API版本](../../wf-api/api/specify-api-version-integrations.md).

要确保最大支持窗口，您应调用最新版本。 您可以在 [API版本控制和支持计划](../../wf-api/api/api-version-support-schedule.md).

## API默认版本的历史记录

“默认API”（或“默认API”）的原始意图是将其映射到最新版本的Workfront API。 这样，具有称为“默认”的基本集成的客户就永远无需更新其API请求。

2011年，Workfront发布了版本3.0的API。 默认值已自动移至版本3.0，这会破坏许多过于复杂且无法在不更新的情况下利用版本3.0的客户集成。 因此，Workfront回滚了此更改，并将默认版本保留为版本2。

自2011年以来，Workfront显着增强了API功能。 因此，我们弃用了旧版本的API。 2017年，我们完全删除了默认版本的概念，而不是更新默认版本。 这是为了鼓励我们的客户使用我们的API的稳定版本，并在最多三年的周期内维护他们的集成。

Workfront现在正在恢复默认API版本。 默认API设置为Workfront API的最新版本，并在每次发布新版本时都会更新为最新版本。


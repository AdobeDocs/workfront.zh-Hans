---
content-type: api
navigation-topic: api-navigation-topic
title: 更新使用默认API版本控制的集成
description: 更新使用默认API版本控制的集成
author: Becky
feature: Workfront API
role: Developer
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# 更新使用默认API版本控制的集成

我们每半年发布一个新版本的Adobe Workfront API。 每个版本在发布后三年内均受支持，另外还有一年处于已弃用状态，该状态表示版本可用但不受支持。

未在URI中指定API版本的集成会自动路由到默认设置。 如果您希望API调用使用特定版本的API，则必须在Workfront API请求中指定该版本。

>[!NOTE]
>
>如果您的组织当前正在使用默认API，则Workfront管理员已收到Announcement Center消息，该消息包含有关默认API的更多说明。

要了解如何在API请求中指定版本，请参阅[在集成中指定API版本](../../wf-api/api/specify-api-version-integrations.md)。

## 使用默认API时的注意事项

使用Workfront默认API时，请考虑以下事项：

* API的默认版本为最新版本。 任何未指定版本的API调用都将使用默认版本。 每当Workfront发布API的新版本时，默认版本都将更新为最新版本。 **因此，在发布Workfront API的新版本后，应检查任何使用默认版本的API调用，以确保仍然支持该功能**。
* 如果您的组织当前正在使用以前弃用的默认API，则Workfront管理员已收到一条公告中心消息，其中包含有关默认API的更多说明。

若要查看API的最新版本，请参阅[API版本控制和支持计划](../../wf-api/api/api-version-support-schedule.md)。

## 将集成更新到支持的API版本

如果您的Workfront API请求未指定版本，则它们将使用“默认”请求。 我们建议您的API请求指定支持的API版本，最好是到最新支持的API。

例如，以下Workfront API请求未指定API版本：

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

发出此请求后，您将收到一个包含JSON编码文本的响应，该文本指定来自Workfront实例的数据。 由于此URI中未指定API版本，因此调用将转至“默认”。

要将默认API请求转换为版本化API请求，只需调用支持的API版本即可。 例如，以下URI请求版本15：

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

在更新Workfront API请求时，您可以指定我们的API的任何受支持版本。 要了解有关引用特定API的更多信息，请参阅[在您的集成中指定API版本](../../wf-api/api/specify-api-version-integrations.md)。

要确保获得最大的支持窗口，应调用最新版本。 您可以在[API版本控制和支持计划](../../wf-api/api/api-version-support-schedule.md)中找到支持的API列表。

## API默认版本的历史记录

“默认API”（或默认API）的原始目的是将其映射到Workfront API的最新版本。 这将允许具有称为“默认”的基本集成的客户永远不必更新其API请求。

2011年，Workfront发布了API 3.0版。 默认版本已自动移至版本3.0，这中断了许多客户集成，这些集成过于复杂，以至于无法在不更新版本的情况下使用版本3.0。 因此，Workfront回滚了此更改，并将默认版本保留为版本2。

自2011年以来，Workfront大幅提升了API功能。 因此，我们已弃用旧版本的API。 2017年，我们完全删除了默认版本的概念，而不是更新Default。 这是为了鼓励我们的客户使用我们的API的稳定版本，并在最多三年的周期内维护他们的集成。

Workfront现在正在恢复默认API版本。 默认API设置为Workfront API的最新版本，并且会在每次发布新版本时更新到最新版本。


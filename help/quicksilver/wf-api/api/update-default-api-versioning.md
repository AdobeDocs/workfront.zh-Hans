---
content-type: api
navigation-topic: api-navigation-topic
title: 更新使用默认API版本控制的集成
description: 更新使用默认API版本控制的集成
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# 更新使用默认API版本控制的集成

我们每两年发布一次Adobe Workfront API的新版本。 每个版本在发布后三年内都受支持，在已弃用状态下再受一年支持，即版本可用但不受支持。

在URI中未指定API版本的集成将自动路由到默认，该默认已弃用。 要使您的Workfront集成有效，您必须在Workfront API请求中指定受支持的API版本。

要了解有关在API请求中指定版本的信息，请参阅 [在集成中指定API版本](../../wf-api/api/specify-api-version-integrations.md).

## 了解API的默认版本

“默认API”（或“默认API”）的原始意图是将其映射到最新版本的Workfront API。 这样，具有称为“默认”的基本集成的客户就永远无需更新其API请求。

2011年，Workfront发布了版本3.0的API。 默认值已自动移至版本3.0，这会破坏许多过于复杂且无法在不更新的情况下利用版本3.0的客户集成。 因此，Workfront回滚了此更改，并将默认版本保留为版本2。

遗憾的是，此主题从未再次讨论过，现在，当我们计划大幅增加API功能时，我们被迫放弃旧版本的API，包括默认API。 我们并没有更新默认版本（这无疑会破坏更多集成），而是完全删除默认版本的概念。 这是为了鼓励我们的客户使用我们的API的稳定版本，并在最多三年的周期内维护他们的集成。

## 弃用默认值

为了改进Workfront API，我们正在删除超过我们三年支持期限的旧版API。 其中一个版本是版本2，默认值会映射到该版本。 此版本于2010年发布，Attask/Workfront应用程序当时支持的大部分逻辑已不复存在或已发生重大更改。

我们于2017年7月弃用了默认版本，将不再将特定版本的API指定为默认版本。 相反，所有Workfront API请求必须指定特定的API版本。

>[!IMPORTANT]
>
> 到2018年7月1日，您所有使用默认值的Workfront集成都必须更新，才能调用特定的受支持API版本。 在该日期之后，由未指定版本的集成使用的所有Workfront API请求都将失败。

要了解Workfront的弃用频率，请参阅 [API版本控制和支持计划](../../wf-api/api/api-version-support-schedule.md).

## 将集成更新到支持的API版本

如果您的Workfront API请求未指定版本，则它们使用默认版本。 您必须更新API请求，以指定受支持的API版本，最好是最新受支持的API。

例如，以下Workfront API请求未指定API版本：

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

发出此请求后，您将收到一个响应，其中包含JSON编码文本，用于指定来自Workfront实例的数据。 由于此URI中未指定API版本，因此调用将转为默认。

要将默认API请求转换为版本控制的API请求，只需调用支持的API版本。 例如，以下URI请求版本9:

`https://davidwhite.my.workfront.com/attask/api/`**v9.0**`/project/metadata`

在更新Workfront API请求时，您可以指定我们API的任何受支持版本。 要了解有关引用特定API的更多信息，请参阅 [在集成中指定API版本](../../wf-api/api/specify-api-version-integrations.md).

要确保最大支持窗口，您应调用最新版本（版本9）。 您可以在 [API版本控制和支持计划](../../wf-api/api/api-version-support-schedule.md).

您必须更新您拥有且使用默认值的集成。 如果您当前的集成没有指定版本，则可能会收到Workfront销售人员、客户成功经理或支持代表的通知，或公告中心消息。

请尽快确保您的集成已更新，以调用我们的API的受支持版本。

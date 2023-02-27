---
content-type: api
navigation-topic: api-navigation-topic
title: 更新使用默认API版本控制的集成
description: 更新使用默认API版本控制的集成
author: Becky
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# 更新使用默认API版本控制的集成

<!-- This article is going to need a complete revamp or to be removed-->

<span class="preview">此页面上突出显示的信息是指目前尚不普遍可用的功能。 它仅在“预览沙盒”环境中可用。</span>

我们每两年发布一次Adobe Workfront API的新版本。 每个版本在发布后三年内都受支持，在已弃用状态下再受一年支持，即版本可用但不受支持。

在URI中未指定API版本的集成将自动路由到默认。 如果您希望API调用使用特定版本的API，则必须在Workfront API请求中指定该版本。

>[!NOTE]
>
>如果贵组织当前使用默认API，则Workfront管理员已收到公告中心消息，其中包含有关默认API的进一步说明。


<!--
Integrations that do not specify a version of the API in the URI are automatically routed to Default, which has been deprecated. In order for your Workfront integrations to be valid, you must specify a supported API version in your Workfront API requests.
-->

要了解有关在API请求中指定版本的信息，请参阅 [在集成中指定API版本](../../wf-api/api/specify-api-version-integrations.md).

## 使用默认API时的注意事项

使用Workfront默认API时，请考虑以下事项：

* 在23.2版本发布后，API的默认版本将设置为最新版本。 任何未指定版本的API调用都将使用默认版本。 每次Workfront发布新版API时，默认版本都将更新至最新版本。 **因此，在发布新版Workfront API后，应检查使用默认版本的任何API调用，以确保仍支持该功能**.
* 如果贵组织当前使用的是已弃用的默认API，则Workfront管理员已收到公告中心消息，其中包含有关默认API的进一步说明。
* <span class="preview">预览环境中的默认API当前设置为最新版本。 在23.2版本发布后，生产环境中的默认API将设置为最新版本。</span>

要查看API的最新版本，请参阅 [API版本控制和支持计划](../../wf-api/api/api-version-support-schedule.md).

<!--

## Deprecating Default

In an effort to improve the Workfront API, we are in the process of removing older API versions that have exceeded our support window of three years. One of these versions is Version 2, to which Default is mapped. This version was released in 2010, and much of the logic supported in the Attask/Workfront application at that time either no longer exists or has substantially changed.

We deprecated Default in July 2017, and we will no longer designate a specific version of the API to be the default version. Instead, all Workfront API requests must specify a specific API version.

>[!IMPORTANT]
>
> By July 1, 2018 all of your Workfront integrations that use Default must be updated to call a specific supported API version. After that date, all of your Workfront API requests used by integrations that do not specify a version will fail.

To learn about the Workfront deprecation cadence, see [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md).

-->

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


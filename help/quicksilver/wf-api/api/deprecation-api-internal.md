---
content-type: api
navigation-topic: api-navigation-topic
title: 弃用API-Internal
description: 弃用API-Internal
author: Becky
feature: Workfront API
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 弃用API-Internal

API-Internal是Adobe Workfront API的一个版本，由于其设计和用途而不受支持。 尽管其中包含Workfront API的最新更新，但是更改后可能会恕不另行通知，因此在生产集成中应务必谨慎使用。 Workfront强烈建议将所有API内部集成更新到版本控制的API。

要了解有关受支持版本的Workfront API的更多信息，请参阅 [API版本控制和支持计划](../../wf-api/api/api-version-support-schedule.md).

**使用不支持的API**

如果您的集成需要版本控制API中不可用的功能，则Workfront建议使用不支持的API。 与API内部类似，不支持API不支持。 不支持的API还包括对Workfront API的最新更改，如有更改，恕不另行通知。 Workfront鼓励您使用测试环境中不受支持的API，在该环境中，您可以探索新功能并确保API不会出现错误。

**确定您使用的API版本**

您可以通过使用REST来构建URI，该URI通过HTTPS发送调用到Workfront，然后返回JSON响应，从而确定集成使用的API的版本。

以下示例显示了一个调用API-Internal的URI:

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

以下示例显示了调用API不受支持的URI:

```
https://<domainname>.my.workfront.com/attask/api/api-unsupported/proj/4c70...
```

以下示例显示了一个调用API版本15.0的URI:

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```

---
content-type: api
navigation-topic: api-navigation-topic
title: 弃用API — 内部
description: 弃用API — 内部
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: acc7414a9c6eef838147aee675603b6cc2566fb9
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# 弃用API — 内部

API-Internal是Adobe Workfront API的一个版本，由于其设计和用途不受支持。 尽管它包含Workfront API的最新更新，但如有更改，恕不另行通知，因此在生产集成中应谨慎使用。 Workfront强烈建议将所有API内部集成更新到受版本控制的API。

要了解有关Workfront API受支持版本的更多信息，请参阅[API版本控制和支持计划](../../wf-api/api/api-version-support-schedule.md)。

**使用不支持的API**

如果您的集成需要版本控制API中不提供的功能，Workfront建议使用不支持API的功能。 与API内部类似，不支持API不受支持。 “不支持的API”还包括对Workfront API的最新更改，如有更改，恕不另行通知。 Workfront建议您使用测试环境中不支持的API，以便探索新功能并确保API无错误。

**确定您正在使用的API版本**

您可以使用REST构建一个URI，确定集成使用的API的版本，该URI通过HTTPS向Workfront发送调用，然后返回JSON响应。

以下示例显示了一个调用API-Internal的URI：

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

以下示例显示了调用API-Unsupported的URI：

```
https://<domainname>.my.workfront.com/attask/api-unsupported/proj/4c70...
```

>[!NOTE]
>
>不支持API的调用忽略了URL的`/api`部分。

以下示例显示了一个调用API版本15.0的URI：

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```

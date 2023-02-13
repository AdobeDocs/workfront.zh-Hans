---
content-type: api
keywords: API，数据，同步，日志，条目，对象
navigation-topic: general-api
title: 使用API同步程序和服务的数据
description: 使用API同步程序和服务的数据
author: John
feature: Workfront API
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: e6bad8cbe84d0f116e9679ecaba5178973a2604f
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# 使用API同步程序和服务的数据

这些是您使用API同步程序和服务数据的一些常用方法。

## 近乎实时的更新

Adobe Workfront使用“事件订阅”（通常称为Webhook）通过API将有关受支持对象和操作的近乎实时更新发送到所需的端点。 您可能会在5秒内收到有关新对象和操作的更新，但平均大约1秒后才会收到更新。 有关如何设置事件订阅的其他信息、支持的操作类型、技术详细信息和示例，请参阅 [事件订阅API](../../wf-api/general/event-subs-api.md) 和 [事件订阅提交要求](../../wf-api/general/setup-event-sub-endpoint.md).

## 批量更新

批量更新是一种通过定期向Workfront服务器发出请求来配置系统以进行更新的方法。 可以使用多种方法来实现此目的，但通常此过程包括让您的服务向Workfront API服务器提出请求，并搜索自上次请求调用以来创建或修改的对象。 有关潜在请求调用和有用参数的信息，请参阅 [GET行为](../../wf-api/general/api-basics.md#get-behavior) 部分 [API基础知识](../../wf-api/general/api-basics.md) 文章。

在设置批量更新服务时，请牢记以下几点重要事项：

### 登录日期

使用ISO 8601格式存储登录日期。 此标准包括日期、时间和时区信息。

**示例：** ISO 8601日期格式

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

创建对象的日期和修改对象的最后日期分别存储为“entryDate”和“lastUpdateDate”。 有关Workfront对象、其关联字段和字段名称的详细信息，请参阅 [API Explorer](../../wf-api/general/api-explorer.md). 请注意，任何给定Workfront对象的entryDate不会发生更改，每次修改对象时，lastUpdatedDate都会发生更改。

**示例：** GET请求问题对象，利用 **lastUpdateDate** 字段。 此请求将返回自指定日期以来更新的所有问题。

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v11.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### 日记帐分录对象

如果您有兴趣获取对象上特定字段的更改，则可以查询“日记帐分录”对象。 可以设置“Workfront日记帐条目”对象，以便在修改特定对象字段时记录有关这些字段的信息，请参阅 [配置系统更新](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) 以了解更多详细信息。

如果将字段设置为作为“日记帐分录”对象的一部分进行记录，则每次修改该字段时都会创建相应的“日记帐分录”。 然后，您可以使用与以下类似的API调用查询“日志条目”对象：

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v11.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>“entryDate”用于查看更改的日志条目，而不是查看更改的对象本身。
